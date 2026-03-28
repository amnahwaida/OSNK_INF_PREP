# 09. Kombinatorika (Art of Counting)

> "Berapa banyak password yang bisa kamu buat dari namamu? Berapa cara memilih ketua kelas dan wakil? Di sinilah Kombinatorika, 'Seni Menghitung Tanpa Perlu Mendaftar Satu-Satu', menjadi penyelamatmu!"

Kalau Graf adalah "Tamu MVP", di OSN-K, **Kombinatorika** adalah rajanya! Teori ini adalah tentang berhitung *kemungkinan* dan cara menyusun sesuatu. Modul ini dijamin bikin kamu jago berhitung.

---

## 🎲 1. Aturan Dasar Menghitung (Penjumlahan vs Perkalian)

Kapan harus ditambah? Kapan harus dikali? Ini adalah kesalahan terbesar peserta OSN yang baru belajar.

### A. Aturan Penjumlahan (Atau / OR)
Kamu pakai ini saat **hanya SATU kegiatan yang dipilih** dari dua pilihan yang **terpisah (tidak bisa dilakukan bersamaan)**.

**Contoh (Sangat Gampang):**
Kamu mau makan siang. Di kantin ada **3 jenis nasi** dan **4 jenis mie**. Kamu punya uang terbatas, kamu HANYA BISA BELI SATU MAKANAN (mau nasi ATAU mie).
Berapa pilihan makananmu?
> **Jawab:** $3 + 4 = 7$ pilihan makanan.
> **Logika:** Kejadian A (makan nasi) dan Kejadian B (makan mie) tidak terjadi bersamaan.

### B. Aturan Perkalian (Dan / AND)
Kamu pakai ini saat kegiatan dilakukan secara **berturut-turut** atau **bersamaan** (paket komplit). Kejadian A DILANJUTKAN Kejadian B.

**Contoh (Sangat Gampang):**
Kamu mau beli paket makan siang. Kamu HARUS MEMILIH **1 Makanan (dari 3 jenis nasi)** DAN **1 Minuman (dari 4 jenis es)**.
Berapa kemungkinan paket makan siangmu?
> **Jawab:** $3 \times 4 = 12$ paket makan siang.
> **Logika:** "Nasi Goreng + Es Teh", "Nasi Goreng + Es Jeruk", dsb. (Pilih Makanan **DAN** Minuman).

---

## 🔄 2. Permutasi (Urutan Sangat Penting!)

**Permutasi** adalah cara menyusun *n* benda ke dalam *r* tempat, di mana **URUTAN MEMPENGARUHI HASIL**.

> **Kata Kunci Permutasi:**
> Jabatan (Ketua, Wakil), Password, Kartu ATM, Nomor Antrian, Plat Nomor Motor.
> **(Budi jadi Ketua, Anton jadi Wakil)** BEDA dengan **(Anton jadi Ketua, Budi jadi Wakil)**.

### A. Permutasi Biasa (Tanpa Pengembalian)
**Kasus:** Ada 5 orang kandidat mau dipilih jadi Ketua, Wakil, dan Bendahara (3 jabatan). Berapa cara?
Pikirkan pakai **Slot Kosong**:
- Jabatan 1 (Ketua): Ada 5 orang yang bisa dipilih. (Masuk 1 orang, sisa 4)
- Jabatan 2 (Wakil): Tinggal 4 orang yang bisa dipilih. (Masuk 1 orang, sisa 3)
- Jabatan 3 (Bendahara): Tinggal 3 orang.
> **Total Cara:** $5 \times 4 \times 3 = 60$ cara.

**Rumus Permutasi dari Benda Beda (P):**
$$P(n, r) = \frac{n!}{(n - r)!}$$
*Catatan: FAKTORIAL (`!`) artinya $n \times (n-1) \times (n-2) ... \times 1$. Contoh $5! = 5 \times 4 \times 3 \times 2 \times 1 = 120$.*

### B. Permutasi Unsur Sama (Anagram)
**Kasus:** Berapa banyak susunan kata unik yang bisa dibuat dari kata **"KATAK"**?
Huruf "K" pertama dan huruf "K" kedua bentuknya persis! Jadi kalau ditukar posisinya tidak ada yang sadar. Jadi harus dibagi kembarannya.

**Rumus:**
$$P = \frac{n!}{k_1! \times k_2! \times ...}$$
*(Total Huruf dibagikan semua huruf kembar)*

**Cara Jawab ("KATAK"):**
- Total huruf (n) = 5
- Huruf kembar: K ada 2. A ada 2. T ada 1.
- Total kemungkinan = $\frac{5!}{2! \times 2!} = \frac{120}{2 \times 2} = \frac{120}{4} = 30$ kata.

### C. Permutasi Siklis (Melingkar)
**Kasus:** 5 orang rapat duduk melingkar di meja bundar. Ada berapa formasi duduk?
Kalau di meja bundar, geser kursi searah jarum jam berarti formasinya **masih sama**! (Patokan sudut pandang hilang). Olek karena itu, kita "paku" 1 orang jadi patokan diam.

**Rumus:**
$$P_{siklis} = (n - 1)!$$
**Jawab:**
$(5 - 1)! = 4! = 4 \times 3 \times 2 \times 1 = 24$ cara duduk.

---

## 🤝 3. Kombinasi (Urutan Bodo Amat!)

**Kombinasi** adalah cara MEMILIH obyek dari sebuah grup, di mana **URUTAN TIDAK DIPEDULIKAN**.

> **Kata Kunci Kombinasi:**
> Tim Cerdas Cermat, Mewakili Sekolah (Delegasi), Mengambil Kelereng Acak, Berjabat Tangan, Segitiga dari titik, Campur Warna.
> **(Budi dan Anton masuk tim Olimpiade)** SAMA SAJA dengan **(Anton dan Budi masuk tim Olimpiade)**.

**Kasus:**
Dari 5 murid unggulan, Bapak Guru ingin memilih 3 anak untuk mewakili tim cerdas cermat. Budi, Andi, Cici ada di tim. Siapapun yang dipanggil duluan tidak masalah, yang penting bertiga.

Karena urutan tidak penting, jumlah pilihannya PASTI LEBIH SEDIKIT dari permutasi (karena yang dianggap beda-beda tadi, sekarang digabung/dikurangi).

**Rumus Kombinasi (C):**
$$C(n, r) = \frac{n!}{r! \times (n - r)!}$$

**Cara Jawab:**
- $n = 5$, $r = 3$
- $C(5, 3) = \frac{5!}{3! \times (5 - 3)!} = \frac{5!}{3! \times 2!}$
- $\frac{5 \times 4 \times 3!}{3! \times 2 \times 1}$ (Coret $3!$)
- $\frac{20}{2} = 10$ tim yang berbeda.

---

## 🕊️ 4. Pigeonhole Principle (Prinsip Sarang Merpati)

Ini adalah prinsip logika matematika yang super lucu tapi sangat sering keluar di soal "Keadaan terburuk" (Worst-case scenario).

**Teori Sederhananya:**
"Jika kamu punya 10 merpati, tapi kamu hanya punya 9 sarang. Cepat atau lambat, kalau semua burung pulang masuk ke sarang, HUKUM ALAM MENGATAKAN: PASTI ADA minimal 1 sarang yang kepenuhan (ditempati minimal oleh 2 ekor merpati)."

> Jika N obyek ditaruh di dalam M wadah (di mana N > M), pasti ada minimal 1 wadah yang berisi sekurang-kurangnya $ \lceil \frac{N}{M} \rceil $ obyek.

**Penerapan di OSN-K:**
Biasanya dipakai dalam soal "Berapa banyak X yang harus DIAMBIL ACAK agar KITA PASTI MENDAPATKAN..."

**Contoh Soal (Pengambilan Acak):**
Di laci gelap lemarimu terdapat:
- 10 kaos kaki hitam
- 8 kaos kaki putih
- 6 kaos kaki merah
Kamu ingin mengambil kaos kaki secara **acak berurutan dalam kegelapan**. Berapa jumlah kaos kaki MINIMAL yang harus kamu tarik agar **DIJAMIN (100% PASTI)** kamu mendapatkan SEPASANG (2 buah) kaos kaki berwarna HITAM?

**Analisa dengan PHP (Worst-Case / Nasib Paling Sial):**
- Bayangkan kamu adalah orang paling sial sedunia.
- Kamu pengen Hitam, eh yang keambil malah Putih. (Terambil: 8 Putih).
- Kamu ambil lagi, ya elah, malah Merah yang keluar semua. (Terambil: 6 Merah).
- Total kamu sudah mengambil $8 + 6 = 14$ kaos kaki. Di ranjangmu sekarang ada 8 Putih dan 6 Merah. Laci hanya sisa Hitam!
- Artinya, ambilan ke-15 *PASTI* Hitam (karena nggak ada warna lain).
- Ambilan ke-16 *PASTI* Hitam juga (dan kamu dapat sepasang!).

**Jawaban:** $8 + 6 + 2 = 16$ kaos kaki harus diambil.

---
[< Materi Sebelumnya: Teori Himpunan](./08-teori-himpunan.md) | [Materi Berikutnya: Deret & Pola Bilangan >](./10-deret-dan-pola-bilangan.md)
[< Kembali ke Beranda Materi](../README.md)
