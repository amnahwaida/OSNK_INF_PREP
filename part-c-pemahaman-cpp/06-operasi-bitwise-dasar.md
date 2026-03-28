# 6. Operasi Bitwise Tingkat Lanjut (Menekan Saklar Alam Biner)

Level tertinggi yang biasanya dihindari oleh mayoritas peserta OSN-K amatiran adalah soal baris array yang menggunakan lambang alien: `&, |, ^, <<, >>`.
Lambang-lambang tersebut bukan mencari sisa bagi (Modulo) atau mengecek kesamaan Boolean ganda (`&&`). Mereka adalah penguasa tergelap hardware asli: **Operator Bitwise (Manipulasi Bilangan Basis 2)**.

Dalam Bitwise, komputer mencopot topeng angka Desimal harianmu (angka $5, 12, 18$, dll), menyulap mereka menjadi sejajar bohlam **Biner 0 dan 1**, dan menekan saklarnya satu persatu vertikal menembus ke bawah.

---

## 💡 A. Bohlam AND (`&`) dan OR (`|`) Vertikal

Ingat, ini cuma pakai SATU karater, BUKAN dua karakter logika sirkuit (`&&`).
Setiap kali OSN-K menyuruhmu menghitung `12 & 10`, kamu JANGAN MALAS mengubahnya jadi biner!

*(Biner: Angka pecahan basis dua murni. Susunannya $8, 4, 2, 1$)*.
- Angka `12` (Ingin menyala $8 + 4$) $\rightarrow$ Biner isinya `1 1 0 0`
- Angka `10` (Ingin menyala $8 + 2$) $\rightarrow$ Biner isinya `1 0 1 0`

Sekarang tarungkan dua pasukan saklar itu secara vertikal menukik ke bawah.
**1. Operator AND (`&`)**: "Wajib Dua-duanya Menyala (1)". Kalau ada satu bohlam redup (0), matikan semua ke bawah! Serigala Kejam!
```text
  1 1 0 0  (Ini 12)
  1 0 1 0  (Ini 10)
  ↓ ↓ ↓ ↓
  1 0 0 0  (Hasil Tembak AND ke bawah)
```
Tembakan akhirnya hanya menyisakan `1000`. Desimal kembalian juri dari `1000` biner adalah **8**.

**2. Operator OR (`|`)**: "Cukup Satu Bohlam Saja Udah Terselamatkan!". Baik budi super dermawan!
```text
  1 1 0 0  (Ini 12)
  1 0 1 0  (Ini 10)
  ↓ ↓ ↓ ↓
  1 1 1 0  (Hasil Tembak OR ke bawah)
```
Menyala pada saklar bernilai $8, 4,$ dan $2$. Jika ditambahkan $8+4+2 = 14$. Hasil juri adalah mutlak **14**.

---

## 🎭 B. Ilmu Paling Sakti Se-OSNK: `XOR` (`^`)

Sang Penakluk Array kembar, **XOR (Exclusive-OR)!**
**Aturan Main Tombol Gaib:**
- Kalau kamu menyentuhnya 1 kali (Ganjil): "Togel Berbalik Arah! Nyala jadi mati, mati jadi nyala." 
- Kalau kamu menyentuhnya 2 kali atau berapapun jumlah GENAP: "Sihir Luntur Penuh! Balik ke sifat perawan aslinya!". 
Itulah kenapa `1 ^ 1` (Sama Jenis) hasilnya `0` (Mati/Hilang lebur). `1 ^ 0` (Beda Jenis) hasilnya `1` (Nyala/Membelot).

**Fungsi Rahasia Juri OSN (Menghapus Angka Kembar Pasangan):**
Jika ada operasi beruntun `A ^ B ^ A`. Kita bongkar paksa:
Karena ada si `A` muncul DUA kali genap kembar siam, secara gaib mereka akan MELEDAKKAN DIRINYA SENDIRI MENJADI 0 dan Lenyap Tak Bersisa! Rumus mutarnya seketika tuntas tersisa huruf `B` telanjang sendiri. BUM! 
Inilah alasan mengapa kodingan deteksi Array Mencari Angka Tunggal di Padang Kembar paling cepat dieksekusi pakai `XOR`.

---

## ⏩ C. SHIFT Kanan Kiri (Membelai Kekuatan Perkalian dan Penebasan)

Daripada CPU pusing berlama-lama menghitung Matematika bagi (/) atau kali (*) dasar, mereka punya gigi mesin sakti *Shifting* yang hanya merembet menggeser gerbong kereta biner.

- **Shift Kiri (`<<`)**: Membuang kotak terdepan, menyuntik masuk `0` gaib di ekor saklar belakang. Sangat jenius! Menggeser satu langkah `<< 1` sama wujudnya dengan **Mengalikan angka murni itu dengan kelipatan stabil 2**. 
Jika juri iseng naruh `5 << 2`, artinya $5$ dikali $2^2$ (yaitu 4) = **20**.

- **Shift Kanan (`>>`)**: Memotong abadi buntut biner di ujung pedang. Sama bentuknya dengan **Membagi Integer angka tersebut dengan kelipatan stabil 2**. (Ingat hukum Laci Bulat Tipe Data Int: buang semua koma pecahannya!).
Jika juri usil nebar kode `13 >> 1`, artinya $13$ dibagi $2^1$ ($2$) = hasilnya $6.5$. Komanya dibakar kiamat! Angka final jawaban adalah mutlak **6**.

---

### Siap Di Uji Tracing Tingkat Emas?

Coret dan temukan takdir `hasil_akhir` dari sintaksis kompilasi ini:
```cpp
int a = 15;
int b = (a >> 1) ^ a;
int c = a & b;
int hasil_akhir = (c << 2) | 1;
```

**Diagnosis Papan Tulis Matrix (Membongkar Biner 8-4-2-1):**
- Biner `a = 15` $\rightarrow$ Menyala semua rentang: `1111`.
- Berapa nilai kemurnian `b`? `(15 >> 1) ^ 15`
  - Langkah 1: Pangkas buntu `15 >> 1` (Dipotong ekornya 1) $\rightarrow 15 \div 2 = 7$ bulat mentah (Biner $4-2-1$: `0111`).
  - Langkah 2: Adu beda `(0111) ^ (1111)`. Pasukan mana yang saling beda ganjil? Angka paling kiri (angka $8$). Biner hasilnya mutlak `1000` (atau sama dengan $8$ angka desimalnya). (Sejarah mencatat mutlak: `b = 8`).
- Berapa saklar `c`? `15 & 8` $\rightarrow$ `(1111) & (1000)`. AND wajib sejalan ganda. Yang sejalan murni cuma digit 8 paling depan. Sisa mati kelam. Hasil saklar `c = 8`.
- Hitung final `hasil_akhir`: `(8 << 2) | 1`.
  - Langkah 1: Genjot gas dorong `8 << 2`. Angka $8$ dikali takdir $2^2 \rightarrow 8 \times 4 = 32$. Biner $32$ itu wujudnya `100000`.
  - Langkah 2: Sambung paku OR `32 | 1` $\rightarrow$ `(100000) | (000001)` $\rightarrow$ Menyala bareng `100001`. 
  - Desimal Final mendarat stabil di angka mutlak = **33**.

Keringat dingin membedah bitwise 4 level berantai... terselesaikan jernih dengan pensil *Compiler Manusia*! 

---
**🏆 SELAMAT!**
Kamu telah menyuntikkan serum utuh ke dalam otakmu meresap ketiga babak Olimpiade Silabus Besar 2025: **Matematika Logika (Part A)**, **Jejak Pola Algoritmik Abstrak (Part B)**, dan **Bedah Jantung Sintaks Mesin C++ Murni (Part C)**.

Silabus Teori Selesai. Saatnya menerjunkan diri berenang ke lautan samudera merah Beribu-Ordo Kompilasi Bank Soal sesungguhnya! Semoga medali emas OSN-K Provinsi mengalungi dada kalian kelak.

[< Kembali ke Indeks Pembuka Kurikulum Besar OSNK](/README.md)
