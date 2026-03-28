# 1. Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)

Selamat datang di markas besar *Compiler Manusia*! 
Di sini, mesin Juri OSN-K akan melempar sebaris dua baris kode berbahasa **C++** yang memanipulasi rentetan angka. Sebagai *Compiler Manusia*, kamu wajib tahu sifat-sifat kejam kodingan C++ yang sering kali **berlawanan dengan hukum matematika di sekolah**.

Mari kita bedah dua konsep penjebak massal: **Sifat Kejam Kotak Integer** dan **Sihir Modulo (`%`)**.

---

## 📦 A. Aturan Main Kotak (Tipe Data `int`)

Di bahasa C++, kamu tidak bisa sembarangan menaruh barang ke udara kosong. Kamu butuh **"Kotak Loker"** (Variabel). Kotak ini ada label nama tipe datanya, yang paling sering memakan korban adalah:

- `int` (Kotak Semen): Cuma bisa diisi **Bilangan Bulat** antara minus 2 miliar sampai plus 2 miliar.
- `long long` (Peti Kemas): Sama kayak `int`, cuma kapsitasnya raksasa (sampai triliunan `10^18`).

### ⚠️ Jebakan Batman #1: Integer Division (Membagi Tanpa Ampun)

Guru Matematika di sekolah mengajarkan: $5 \div 2 = 2.5$. Benar kan?
**Di dunia C++, `5 / 2` HASILNYA ADALAH `2`!** Lho kok bisa? Kemana sisa $0.5$ nya?

**Analogi Loker & Pembagian Permen Mentah:**
Bayangkan tipe `int` itu adalah **Laci Semen keras tanpa celah karet (desimal)**.
Kalau Pak Dengklek menyuruh mesin C++ membagi 5 biji permen mentah ke 2 anak (Budi dan Wati). 
- Budi dapat 2 biji.
- Wati dapat 2 biji.
Sisa 1 biji lagi gak bisa dibelah pisau karena kodratnya di kodingan variabel `int` (Bilangan Bulat) melarang keras adanya "serpihan desimal"!!
Karena komputer itu robot bodoh, dia cuma nanya: *"Eh satu anak dapet utuh berapa bulatnya?"* Jawabnya 2. Sisa serpihannya? **DIBUANG KE TONG SAMPAH, DIABAIKAN, DIBAKAR!**

Jadi jangan heran kalau disodorkan kode begini di kertas OSN-K:
```cpp
int a = 20;
int b = 3;
int hasil = a / b;
// Hasil yang tercetak BUKAN 6.666, TAPI MURNI 6!
```
*Aturan Emas Tracing C++:* Kalau tipe datanya `int`, setiap ada rumus Pembagian `/`, **potong buang semua angka koma di belakangnya tanpa pembulatan ke atas**.

---

## 🔮 B. Sihir Sisa Bagi (Modulo `%`)

Nah, tadi kan sisa 1 permennya dibuang tuh sama operator pembagi `/`. Terus kalau kita mau cari tahu permen sisa yang gak bisa dibagi rata itu berapa, ke mana kita mencarinya?
Jawabannya adalah **Operator Modulo (Simbolnya `%`)**.

Modulo artinya: **"Cari Sisa Baginya!"**

**Analogi Kelereng Harian:**
Kamu punya 14 kelereng. Kamu ingin membagikannya adil ke 4 temanmu.
- Bagi Rata ($14 \div 4$): Setiap anak dapet 3 biji utuh (`14 / 4 = 3`).
- Sisa Kelereng ($14 \pmod 4$): Total yang dibagikan $3 \times 4 = 12$ biji. Tanganmu sisa $14 - 12 = 2$ biji kelereng yang gak bisa dibagi. Inilah hasil Modulonya! (`14 % 4 = 2`).

### ⚠️ Jebakan Batman #2: Sifat Modulo Bikin Pusing
**1. Modulo Angka Kecil terhadap Angka Besar**
Coba jawab cepat! Berapa hasil `3 % 7` (3 sisa bagi 7)?
- Insting salah: `4` (Dikurangin aja $7-3$). Ini jelas Sesat!
- **Analogi Logis:** Pak Dengklek punya 3 kelereng. Disuruh membagikan merata ke 7 anak. Apa yang terjadi? Ya nggak mungkin! Kelerengnya kurang dari jumlah anak, nggak bisa dibagi satu pun ke siapa-siapa. Kesimpulannya: Kelereng di tangan Pak Dengklek utuh tidak berkurang. 
- Hasilnya: **`3 % 7 = 3`**.
*Aturan Emas Modulo OSN-K:* Jika angka kiri *lebih kecil* dari angka kanan ($A \pmod B$ dimana $A < B$), **jawabannya adalah Angka Kiri itu sendiri ($A$)**.

**2. Pendeteksi Genap-Ganjil Instant**
Di soal operasi *looping* array panjang, Modulo `2` seringkali nongol mendadak.
```cpp
if (x % 2 == 0) { ... }
```
Jangan panik ngitung sisa bagi angka gila! `% 2 == 0` terjemahan bahasa Indonesianya murni satu kalimat: **"Apakah `x` ini genap?"**.
Dan jika `x % 2 != 0`, artinya variabel itu sedang memegang angka saklek **Ganjil**.

---

## 🔤 C. Rahasia Tipe Data Lainnya (Karakter, Pecahan, & Saklar)

Selain kotak semen (`int`), kamu akan sering diteriaki oleh jenis kotak aneh lainnya di OSN-K:

### 1. `char` (Kartu Pelajar & Rahasia Sandi ASCII)
`char` hanya bisa menyimpan **Satu Huruf Tunggal** (misal `'A'`, `'x'`, `'9'`). Tapi hati-hati! Di dunia C++, huruf itu sebenarnya **Hanyalah Angka Berbaju Kostum**!
Komputer menggunakan tabel *ASCII* (American Standard Code).
- `'A'` itu secara batin setara dengan angka **65**.
- `'a'` bernilai **97**.
- Huruf `'0'` (sebagai teks) BUKANLAH bernilai nol mutlak! Dia bernilai **48** di batinnya.

Karena huruf sejatinya adalah angka, Juri C++ bisa seenaknya menyuruhmu **Menambah/Mengurang Huruf layaknya Matematika!!**
```cpp
char huruf = 'C';
char huruf_baru = huruf + 2; 
```
*Tracing Logika (Maju Alfabet):* `'C'` ditambah 2 langkah ke depan? Murni melompat abjad $\rightarrow$ `'C' \rightarrow 'D' \rightarrow 'E'`. Hasil akhirnya mutlak mencetak huruf **`E`**. (Inilah jantung dari kode pertahanan Sandi Caesar Chiper di OSN-K!).

### 2. `bool` (Saklar Lampu: Hidup/Mati)
`bool` (Boolean) cuma bisa nampung 2 takdir: **`true` (1)** atau **`false` (0)**.
- **Jebakan Batman OSN-K:** Di dunia C++, **SEMUA ANGKA SELAIN `0` DIANGGAP `TRUE`!**
```cpp
int nyawa = -15;
if (nyawa) {
   // Blok ini AKAN DIJALANKAN! Kenapa? 
   // Karena -15 itu BUKAN 0! Selain 0, maka saklar otomatis bernilai TRUE!
}
```

### 3. `double` / `float` (Gelas Air Minum Berkomah)
Kalau kamu paksa menyiram pecahan ke kotak `int`, komanya dibakar. Nah, kalau kamu butuh komonya diselamatkan, pakailah `double`. Dia kayak Gelas Air Minum yang rela meneteskan nol koma sisa debunya.
- **Syarat Mutlak Pak Dengklek:** Pembagian koma *hanya* akan muncul jika ADA SALAH SATU elemen di rumusnya yang memang pakai koma.
```cpp
double hasil1 = 5 / 2;     // Hasilnya 2.0 (Karena 5 dan 2 diotak int, komanya keburu dibakar sebelum masuk gelas).
double hasil2 = 5.0 / 2;   // Hasilnya 2.5 (Aman! Ada pengawal '5.0' menjaga takdir pecahannya).
```

---

## 🌍 D. Wilayah Kekuasaan Variabel (Scope Global vs Lokal)

Di kodingan OSN-K, juri sangat benci melihatmu bahagia. Mereka suka menamai **Dua Variabel Berbeda dengan NAMA YANG SAMA PERSIS** untuk mengecoh otakmu!

**Analogi Ketua OSIS (Global) vs Ketua Kelas (Lokal):**
```cpp
int uang = 100; // GLOBAL (Ketua OSIS, semua murid kenal dia)

void cek_dompet() {
    int uang = 5; // LOKAL (Ketua Kelas 12A)
    printf("%d", uang);
}
```
**Hukum Kesopanan C++:** "Orang Dalam Lebih Berkuasa".
Saat mesin berada di dalam kamar fungsi `cek_dompet()`, ia melihat ada ketua OSIS (`100`) dan ada ketua kelasnya sendiri (`5`). Siapa yang lebih ia taati? Tentu saja yang terdekat! Fungsi itu akan mencetak mutlak **`5`**. Uang `100` di luar sana sama sekali tak dianggap (Tertimpa bayangan/ *Shadowing*).
*Aturan Emas Tracing:* Selalu lirik letak kurung kurawal `{ }` saat mencatat variabel. Jangan sampai nilai variabel tetangga kecoret!

---

### Siap Di Uji Tracing?
Diberikan kutipan variabel *Compiler Manusia* berikut ini:
```cpp
int uang_jajan = 15;
int teman_nabrak = 6;

int disita_guru = uang_jajan % teman_nabrak;
int jatah_nongkrong = uang_jajan / teman_nabrak;
int hasil_akhir = (disita_guru + jatah_nongkrong) * (uang_jajan % 2);
```
**Berapakah nilai `hasil_akhir` yang ada di otak program?**

**Diagnosis Logika Papan Tulis:**
- `uang_jajan % teman_nabrak` $\rightarrow 15 \pmod 6$. Sisa bagi kelereng. $15$ dibagi $6$ dapat $2 (12)$. Sisanya $15-12 = 3$. Makmurnya, `disita_guru = 3`.
- `uang_jajan / teman_nabrak` $\rightarrow 15 \div 6$. Pembagian kejam *Integer*! $15/6$ hasilnya $2.5$. Karena `int`, komanya dibakar abadi. `jatah_nongkrong = 2`.
- `uang_jajan % 2` $\rightarrow$ Apakah 15 ganjil? Angka Ganjil kalau di-modulo 2 Sisa `1`. 
- `hasil_akhir = (3 + 2) * 1 = 5 * 1 = 5`.

Gampang dan cantik bukan? Ingat selalu permen dan sisa kelereng di kepala saat mencoret soal ini!

⏩ **Lanjut ke Modul Kedua:** [Logika Percabangan (Razia BP)](./02-percabangan-dan-boolean-logika.md)
