🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Dynamic Programming Dasar (Part 6 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Dynamic Programming Dasar**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 5 | 2 |
| 1 | 3 | 1 |
| 5 | 2 | 2 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 13 Poin Karung
B. 10 Poin Karung
C. 14 Poin Karung
D. 11 Poin Karung
E. 12 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: A (13 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 5 = 6
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 6 + 2 = 8
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 1 = 2
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 5 = 7
- DP[1][1]: Dilema rakus. Datang dari Kiri(2) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 9.
- DP[1][2]: Dilema rakus. Datang dari Kiri(9) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 10.
- DP[2][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 11.
- DP[2][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 13.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **13**. 

Opsi yang sangat sah adalah **A**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 3 | 3 |
| 4 | 1 | 1 |
| 4 | 2 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 12 Poin Karung
B. 16 Poin Karung
C. 13 Poin Karung
D. 14 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (15 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 3 = 4
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 3 = 7
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 4 = 5
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 4 = 9
- DP[1][1]: Dilema rakus. Datang dari Kiri(5) atau Atas(4)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 6.
- DP[1][2]: Dilema rakus. Datang dari Kiri(6) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 8.
- DP[2][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 11.
- DP[2][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 15.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **15**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 253**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 90 macam kombinasi rute
B. 91 macam kombinasi rute
C. 89 macam kombinasi rute
D. 88 macam kombinasi rute
E. 92 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: C (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **C**.
</details>

---
**Soal 254**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 54 macam kombinasi rute
B. 58 macam kombinasi rute
C. 57 macam kombinasi rute
D. 55 macam kombinasi rute
E. 56 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: D (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **D**.
</details>

---
**Soal 255**
Pak Dengklek harus mendaki Kuil Kematian setinggi **7 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-7?

A. 20 macam kombinasi rute
B. 22 macam kombinasi rute
C. 21 macam kombinasi rute
D. 24 macam kombinasi rute
E. 23 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: C (21 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`


Tembus mutlak! Di tangga puncak 7, tercetak ada **21 kombinasi jalur mutlak**. Opsi dewa presisi adalah **C**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 5 | 2 | 3 |
| 5 | 2 | 3 |
| 4 | 4 | 3 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 22 Poin Karung
B. 21 Poin Karung
C. 20 Poin Karung
D. 18 Poin Karung
E. 19 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (21 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 5 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 2 = 7
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 7 + 3 = 10
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 5 = 10
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 10 + 4 = 14
- DP[1][1]: Dilema rakus. Datang dari Kiri(10) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 12.
- DP[1][2]: Dilema rakus. Datang dari Kiri(12) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(14) atau Atas(12)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 18.
- DP[2][2]: Dilema rakus. Datang dari Kiri(18) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 21.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **21**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 5 | 1 | 4 |
| 1 | 1 | 5 |
| 4 | 3 | 2 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 15 Poin Karung
B. 16 Poin Karung
C. 18 Poin Karung
D. 17 Poin Karung
E. 14 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: D (17 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 5 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 1 = 6
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 6 + 4 = 10
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 1 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 4 = 10
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 7.
- DP[1][2]: Dilema rakus. Datang dari Kiri(7) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(10) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 13.
- DP[2][2]: Dilema rakus. Datang dari Kiri(13) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 17.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **17**. 

Opsi yang sangat sah adalah **D**.
</details>

---
**Soal 258**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 88 macam kombinasi rute
B. 89 macam kombinasi rute
C. 92 macam kombinasi rute
D. 91 macam kombinasi rute
E. 90 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 4 | 4 | 5 |
| 5 | 1 | 3 |
| 4 | 4 | 5 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 21 Poin Karung
B. 23 Poin Karung
C. 22 Poin Karung
D. 19 Poin Karung
E. 20 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: C (22 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 4 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 4 = 8
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 8 + 5 = 13
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 4 + 5 = 9
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 9 + 4 = 13
- DP[1][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 10.
- DP[1][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(13)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 16.
- DP[2][1]: Dilema rakus. Datang dari Kiri(13) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 17.
- DP[2][2]: Dilema rakus. Datang dari Kiri(17) atau Atas(16)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 22.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **22**. 

Opsi yang sangat sah adalah **C**.
</details>

---
**Soal 260**
Pak Dengklek harus mendaki Kuil Kematian setinggi **5 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-5?

A. 10 macam kombinasi rute
B. 8 macam kombinasi rute
C. 11 macam kombinasi rute
D. 9 macam kombinasi rute
E. 7 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (8 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`


Tembus mutlak! Di tangga puncak 5, tercetak ada **8 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 261**
Pak Dengklek harus mendaki Kuil Kematian setinggi **5 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-5?

A. 9 macam kombinasi rute
B. 11 macam kombinasi rute
C. 8 macam kombinasi rute
D. 10 macam kombinasi rute
E. 7 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: C (8 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`


Tembus mutlak! Di tangga puncak 5, tercetak ada **8 kombinasi jalur mutlak**. Opsi dewa presisi adalah **C**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 2 | 1 |
| 4 | 3 | 1 |
| 3 | 1 | 1 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 12 Poin Karung
B. 11 Poin Karung
C. 9 Poin Karung
D. 10 Poin Karung
E. 8 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (11 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 2 = 4
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 1 = 5
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 4 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 3 = 9
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(4)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 9.
- DP[1][2]: Dilema rakus. Datang dari Kiri(9) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 10.
- DP[2][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 10.
- DP[2][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 11.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **11**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 263**
Pak Dengklek harus mendaki Kuil Kematian setinggi **5 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-5?

A. 10 macam kombinasi rute
B. 8 macam kombinasi rute
C. 11 macam kombinasi rute
D. 7 macam kombinasi rute
E. 9 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (8 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`


Tembus mutlak! Di tangga puncak 5, tercetak ada **8 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 4 | 4 |
| 3 | 5 | 3 |
| 2 | 2 | 1 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 12 Poin Karung
B. 11 Poin Karung
C. 13 Poin Karung
D. 14 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: D (14 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 4 = 5
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 4 = 9
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 3 = 4
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 4 + 2 = 6
- DP[1][1]: Dilema rakus. Datang dari Kiri(4) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 10.
- DP[1][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 13.
- DP[2][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 12.
- DP[2][2]: Dilema rakus. Datang dari Kiri(12) atau Atas(13)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 14.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **14**. 

Opsi yang sangat sah adalah **D**.
</details>

---
**Soal 265**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 55 macam kombinasi rute
B. 54 macam kombinasi rute
C. 57 macam kombinasi rute
D. 56 macam kombinasi rute
E. 58 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: A (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **A**.
</details>

---
**Soal 266**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 55 macam kombinasi rute
B. 54 macam kombinasi rute
C. 56 macam kombinasi rute
D. 58 macam kombinasi rute
E. 57 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: A (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **A**.
</details>

---
**Soal 267**
Pak Dengklek harus mendaki Kuil Kematian setinggi **8 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-8?

A. 37 macam kombinasi rute
B. 36 macam kombinasi rute
C. 33 macam kombinasi rute
D. 35 macam kombinasi rute
E. 34 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (34 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`


Tembus mutlak! Di tangga puncak 8, tercetak ada **34 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 2 | 3 |
| 5 | 2 | 2 |
| 1 | 1 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 14 Poin Karung
B. 15 Poin Karung
C. 13 Poin Karung
D. 12 Poin Karung
E. 11 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: A (14 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 2 = 3
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 3 = 6
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 5 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 1 = 7
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(3)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 8.
- DP[1][2]: Dilema rakus. Datang dari Kiri(8) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 10.
- DP[2][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 9.
- DP[2][2]: Dilema rakus. Datang dari Kiri(9) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 14.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **14**. 

Opsi yang sangat sah adalah **A**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 5 | 5 |
| 3 | 1 | 3 |
| 4 | 5 | 2 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 18 Poin Karung
B. 15 Poin Karung
C. 17 Poin Karung
D. 14 Poin Karung
E. 16 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: C (17 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 5 = 7
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 7 + 5 = 12
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 3 = 5
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 4 = 9
- DP[1][1]: Dilema rakus. Datang dari Kiri(5) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 8.
- DP[1][2]: Dilema rakus. Datang dari Kiri(8) atau Atas(12)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 14.
- DP[2][2]: Dilema rakus. Datang dari Kiri(14) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 17.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **17**. 

Opsi yang sangat sah adalah **C**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 5 | 5 |
| 4 | 5 | 5 |
| 1 | 1 | 3 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 20 Poin Karung
B. 19 Poin Karung
C. 18 Poin Karung
D. 16 Poin Karung
E. 17 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (19 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 5 = 6
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 6 + 5 = 11
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 4 = 5
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 1 = 6
- DP[1][1]: Dilema rakus. Datang dari Kiri(5) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 11.
- DP[1][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 16.
- DP[2][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 12.
- DP[2][2]: Dilema rakus. Datang dari Kiri(12) atau Atas(16)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 19.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **19**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 1 | 5 |
| 5 | 4 | 3 |
| 3 | 2 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 16 Poin Karung
B. 18 Poin Karung
C. 17 Poin Karung
D. 19 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 1 = 3
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 5 = 8
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 5 = 7
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 7 + 3 = 10
- DP[1][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(3)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 11.
- DP[1][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 14.
- DP[2][1]: Dilema rakus. Datang dari Kiri(10) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 13.
- DP[2][2]: Dilema rakus. Datang dari Kiri(13) atau Atas(14)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 3 | 2 | 1 |
| 2 | 1 | 1 |
| 2 | 4 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 12 Poin Karung
B. 13 Poin Karung
C. 16 Poin Karung
D. 14 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (15 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 3 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 2 = 5
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 1 = 6
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 3 + 2 = 5
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 2 = 7
- DP[1][1]: Dilema rakus. Datang dari Kiri(5) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 6.
- DP[1][2]: Dilema rakus. Datang dari Kiri(6) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 7.
- DP[2][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 11.
- DP[2][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 15.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **15**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 1 | 5 | 2 |
| 2 | 2 | 5 |
| 5 | 3 | 5 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 16 Poin Karung
B. 17 Poin Karung
C. 15 Poin Karung
D. 19 Poin Karung
E. 18 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 1 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 1 + 5 = 6
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 6 + 2 = 8
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 1 + 2 = 3
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 3 + 5 = 8
- DP[1][1]: Dilema rakus. Datang dari Kiri(3) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 8.
- DP[1][2]: Dilema rakus. Datang dari Kiri(8) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 13.
- DP[2][1]: Dilema rakus. Datang dari Kiri(8) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 11.
- DP[2][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(13)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 274**
Pak Dengklek harus mendaki Kuil Kematian setinggi **8 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-8?

A. 33 macam kombinasi rute
B. 34 macam kombinasi rute
C. 37 macam kombinasi rute
D. 35 macam kombinasi rute
E. 36 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (34 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`


Tembus mutlak! Di tangga puncak 8, tercetak ada **34 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 275**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 91 macam kombinasi rute
B. 90 macam kombinasi rute
C. 88 macam kombinasi rute
D. 89 macam kombinasi rute
E. 92 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: D (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **D**.
</details>

---
**Soal 276**
Pak Dengklek harus mendaki Kuil Kematian setinggi **7 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-7?

A. 20 macam kombinasi rute
B. 24 macam kombinasi rute
C. 23 macam kombinasi rute
D. 21 macam kombinasi rute
E. 22 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: D (21 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`


Tembus mutlak! Di tangga puncak 7, tercetak ada **21 kombinasi jalur mutlak**. Opsi dewa presisi adalah **D**.
</details>

---
**Soal 277**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 89 macam kombinasi rute
B. 92 macam kombinasi rute
C. 91 macam kombinasi rute
D. 90 macam kombinasi rute
E. 88 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: A (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **A**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 5 | 4 | 5 |
| 3 | 4 | 1 |
| 3 | 1 | 3 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 15 Poin Karung
B. 18 Poin Karung
C. 16 Poin Karung
D. 17 Poin Karung
E. 19 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 5 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 4 = 9
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 9 + 5 = 14
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 3 = 8
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 8 + 3 = 11
- DP[1][1]: Dilema rakus. Datang dari Kiri(8) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 13.
- DP[1][2]: Dilema rakus. Datang dari Kiri(13) atau Atas(14)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(11) atau Atas(13)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 14.
- DP[2][2]: Dilema rakus. Datang dari Kiri(14) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 2 | 1 |
| 5 | 3 | 1 |
| 5 | 1 | 3 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 14 Poin Karung
B. 13 Poin Karung
C. 15 Poin Karung
D. 16 Poin Karung
E. 17 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: D (16 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 2 = 4
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 1 = 5
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 5 = 7
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 7 + 5 = 12
- DP[1][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(4)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 10.
- DP[1][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 11.
- DP[2][1]: Dilema rakus. Datang dari Kiri(12) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 13.
- DP[2][2]: Dilema rakus. Datang dari Kiri(13) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 16.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **16**. 

Opsi yang sangat sah adalah **D**.
</details>

---
**Soal 280**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 55 macam kombinasi rute
B. 57 macam kombinasi rute
C. 54 macam kombinasi rute
D. 58 macam kombinasi rute
E. 56 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: A (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **A**.
</details>

---
**Soal 281**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 91 macam kombinasi rute
B. 92 macam kombinasi rute
C. 90 macam kombinasi rute
D. 88 macam kombinasi rute
E. 89 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 282**
Pak Dengklek harus mendaki Kuil Kematian setinggi **7 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-7?

A. 24 macam kombinasi rute
B. 20 macam kombinasi rute
C. 23 macam kombinasi rute
D. 21 macam kombinasi rute
E. 22 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: D (21 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`


Tembus mutlak! Di tangga puncak 7, tercetak ada **21 kombinasi jalur mutlak**. Opsi dewa presisi adalah **D**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 5 | 2 | 1 |
| 4 | 2 | 5 |
| 1 | 5 | 2 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 17 Poin Karung
B. 16 Poin Karung
C. 18 Poin Karung
D. 15 Poin Karung
E. 19 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: C (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 5 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 2 = 7
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 7 + 1 = 8
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 5 + 4 = 9
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 9 + 1 = 10
- DP[1][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 11.
- DP[1][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 16.
- DP[2][1]: Dilema rakus. Datang dari Kiri(10) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 16.
- DP[2][2]: Dilema rakus. Datang dari Kiri(16) atau Atas(16)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **C**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 3 | 2 | 2 |
| 4 | 3 | 5 |
| 1 | 3 | 3 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 16 Poin Karung
B. 19 Poin Karung
C. 18 Poin Karung
D. 17 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: C (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 3 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 2 = 5
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 2 = 7
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 3 + 4 = 7
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 7 + 1 = 8
- DP[1][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 10.
- DP[1][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(8) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 13.
- DP[2][2]: Dilema rakus. Datang dari Kiri(13) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **C**.
</details>

---
**Soal 285**
Pak Dengklek harus mendaki Kuil Kematian setinggi **5 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-5?

A. 10 macam kombinasi rute
B. 9 macam kombinasi rute
C. 11 macam kombinasi rute
D. 7 macam kombinasi rute
E. 8 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (8 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`


Tembus mutlak! Di tangga puncak 5, tercetak ada **8 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 4 | 1 | 3 |
| 2 | 2 | 2 |
| 1 | 4 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 15 Poin Karung
B. 14 Poin Karung
C. 17 Poin Karung
D. 13 Poin Karung
E. 16 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (16 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 4 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 1 = 5
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 5 + 3 = 8
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 4 + 2 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 1 = 7
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(5)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 8.
- DP[1][2]: Dilema rakus. Datang dari Kiri(8) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 10.
- DP[2][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 12.
- DP[2][2]: Dilema rakus. Datang dari Kiri(12) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 16.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **16**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 287**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 91 macam kombinasi rute
B. 90 macam kombinasi rute
C. 92 macam kombinasi rute
D. 88 macam kombinasi rute
E. 89 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 4 | 5 |
| 4 | 4 | 4 |
| 3 | 1 | 2 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 14 Poin Karung
B. 15 Poin Karung
C. 18 Poin Karung
D. 16 Poin Karung
E. 17 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (17 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 4 = 6
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 6 + 5 = 11
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 4 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 3 = 9
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 10.
- DP[1][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(10)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 11.
- DP[2][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(2). Maksimum Tabungan Di Area Ini = 17.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **17**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 289**
Pak Dengklek harus mendaki Kuil Kematian setinggi **6 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-6?

A. 15 macam kombinasi rute
B. 14 macam kombinasi rute
C. 12 macam kombinasi rute
D. 16 macam kombinasi rute
E. 13 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (13 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`


Tembus mutlak! Di tangga puncak 6, tercetak ada **13 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 290**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 56 macam kombinasi rute
B. 55 macam kombinasi rute
C. 58 macam kombinasi rute
D. 57 macam kombinasi rute
E. 54 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 291**
Pak Dengklek harus mendaki Kuil Kematian setinggi **6 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-6?

A. 12 macam kombinasi rute
B. 15 macam kombinasi rute
C. 13 macam kombinasi rute
D. 16 macam kombinasi rute
E. 14 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: C (13 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`


Tembus mutlak! Di tangga puncak 6, tercetak ada **13 kombinasi jalur mutlak**. Opsi dewa presisi adalah **C**.
</details>

---
**Soal 292**
Pak Dengklek harus mendaki Kuil Kematian setinggi **6 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-6?

A. 12 macam kombinasi rute
B. 14 macam kombinasi rute
C. 13 macam kombinasi rute
D. 16 macam kombinasi rute
E. 15 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: C (13 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`


Tembus mutlak! Di tangga puncak 6, tercetak ada **13 kombinasi jalur mutlak**. Opsi dewa presisi adalah **C**.
</details>

---
**Soal 293**
Pak Dengklek harus mendaki Kuil Kematian setinggi **10 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-10?

A. 89 macam kombinasi rute
B. 91 macam kombinasi rute
C. 90 macam kombinasi rute
D. 88 macam kombinasi rute
E. 92 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: A (89 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`
- Lantai 10: Dicapai dari gabungan rute L9 dan L8 $\rightarrow$ `55 + 34 = 89`


Tembus mutlak! Di tangga puncak 10, tercetak ada **89 kombinasi jalur mutlak**. Opsi dewa presisi adalah **A**.
</details>

---
**Soal 294**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 57 macam kombinasi rute
B. 56 macam kombinasi rute
C. 54 macam kombinasi rute
D. 58 macam kombinasi rute
E. 55 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: E (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 4 | 3 | 2 |
| 2 | 4 | 4 |
| 3 | 3 | 5 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 19 Poin Karung
B. 21 Poin Karung
C. 18 Poin Karung
D. 17 Poin Karung
E. 20 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: E (20 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 4 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 4 + 3 = 7
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 7 + 2 = 9
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 4 + 2 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 3 = 9
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(7)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 11.
- DP[1][2]: Dilema rakus. Datang dari Kiri(11) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 15.
- DP[2][1]: Dilema rakus. Datang dari Kiri(9) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(3). Maksimum Tabungan Di Area Ini = 14.
- DP[2][2]: Dilema rakus. Datang dari Kiri(14) atau Atas(15)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 20.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **20**. 

Opsi yang sangat sah adalah **E**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 3 | 5 | 3 |
| 3 | 1 | 5 |
| 1 | 1 | 1 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 17 Poin Karung
B. 14 Poin Karung
C. 18 Poin Karung
D. 16 Poin Karung
E. 15 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: A (17 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 3 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 5 = 8
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 8 + 3 = 11
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 3 + 3 = 6
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 6 + 1 = 7
- DP[1][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(8)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 9.
- DP[1][2]: Dilema rakus. Datang dari Kiri(9) atau Atas(11)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 16.
- DP[2][1]: Dilema rakus. Datang dari Kiri(7) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 10.
- DP[2][2]: Dilema rakus. Datang dari Kiri(10) atau Atas(16)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(1). Maksimum Tabungan Di Area Ini = 17.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **17**. 

Opsi yang sangat sah adalah **A**.
</details>

---
**Soal 3**
Robot Pak Dengklek diletakkan di **pojok kiri atas (Indeks [0][0])** pada peta harta karun berukuran 3x3 yang wujud nilai kotak emas-emasnya berwujud berikut:
| 2 | 1 | 3 |
| 2 | 5 | 4 |
| 2 | 5 | 4 |


Robot hanya diizinkan bergerak **KE KANAN** atau **KE BAWAH** satu langkah satu kotak. Setiap menginjak kotak, robot mengambil total emas disitu.
Pakai perhitungan kacamata *Dynamic Programming Peta 2D*, berapa Total Maksimum poin Murni yang bisa dikarungi Robot saat tancap gas finish berhenti di lubang **pojok kanan bawah (Indeks [2][2])**?

A. 15 Poin Karung
B. 18 Poin Karung
C. 19 Poin Karung
D. 16 Poin Karung
E. 17 Poin Karung

<details>
<summary><b>Klik untuk melihat kunci jawaban & Simulasi Memori Peta Titisan Dewa Masa Depan</b></summary>

**Jawaban: B (18 Poin Karung)**

**Pembahasan (Matrix Tabulasi Bottom-Up DP):**
Otak DP tidak mikir langsung serakah panjang. DP mengecek **Tiap 1 Kotak yang dia singgahi, dia selalu bertanya**: *"Siapa yang bisa mewariskan harta lebih tinggi kepadaku untuk masuk ke ranah kotakku ini? Saudaraku si Kiri atau si Atas?"*

Bongkar isi warisannya sel / koordinat persel:
- DP[0][0]: Kantongi 2 start.
- DP[0][1] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 2 + 1 = 3
- DP[0][2] (Ujung Kanan Pinggir): Ambil sisa masa lalu kiri + balok saat ini -> 3 + 3 = 6
- DP[1][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 2 + 2 = 4
- DP[2][0] (Jurang Bawah Kiri): Ambil sisa masa lalu Atas + balok -> 4 + 2 = 6
- DP[1][1]: Dilema rakus. Datang dari Kiri(4) atau Atas(3)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 9.
- DP[1][2]: Dilema rakus. Datang dari Kiri(9) atau Atas(6)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 13.
- DP[2][1]: Dilema rakus. Datang dari Kiri(6) atau Atas(9)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(5). Maksimum Tabungan Di Area Ini = 14.
- DP[2][2]: Dilema rakus. Datang dari Kiri(14) atau Atas(13)? Si dewa DP pilih yang maksimal!. Ambil yg gede + nilainya(4). Maksimum Tabungan Di Area Ini = 18.

Finish! Saldo akhir saat kakinya mijak kotak Pojok Kanan Bawah bernilai klimaks pada mutlak angka **18**. 

Opsi yang sangat sah adalah **B**.
</details>

---
**Soal 298**
Pak Dengklek harus mendaki Kuil Kematian setinggi **8 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-8?

A. 36 macam kombinasi rute
B. 34 macam kombinasi rute
C. 35 macam kombinasi rute
D. 37 macam kombinasi rute
E. 33 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (34 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`


Tembus mutlak! Di tangga puncak 8, tercetak ada **34 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 299**
Pak Dengklek harus mendaki Kuil Kematian setinggi **9 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-9?

A. 58 macam kombinasi rute
B. 55 macam kombinasi rute
C. 54 macam kombinasi rute
D. 57 macam kombinasi rute
E. 56 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: B (55 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`
- Lantai 8: Dicapai dari gabungan rute L7 dan L6 $\rightarrow$ `21 + 13 = 34`
- Lantai 9: Dicapai dari gabungan rute L8 dan L7 $\rightarrow$ `34 + 21 = 55`


Tembus mutlak! Di tangga puncak 9, tercetak ada **55 kombinasi jalur mutlak**. Opsi dewa presisi adalah **B**.
</details>

---
**Soal 300**
Pak Dengklek harus mendaki Kuil Kematian setinggi **7 anak tangga**. 
Fisik Pak Dengklek mengizinkannya untuk *hanya* bisa memanjat maju **1 anak tangga** ATAU **2 anak tangga** secara langsung sekaligus dalam satu hentakan langkah.

Lakukan memoisasi tabel perhitungan mundur (Dynamic Programming)! Ada berapa total BANYAKNYA VARIASI KOMBINASI rute langkah sah yang bisa membawa Pak Dengklek sampai tepat memijak anak tangga ke-7?

A. 22 macam kombinasi rute
B. 23 macam kombinasi rute
C. 24 macam kombinasi rute
D. 21 macam kombinasi rute
E. 20 macam kombinasi rute

<details>
<summary><b>Klik untuk melihat kunci jawaban & Buku Tabungan Rute DP</b></summary>

**Jawaban: D (21 macam rute)**

**Pembahasan (Menguapkan Cabang Pohon dengan Tabel):**
Kalau dieksekusi manual kuli Brute Force gambar pohon rute (`1-1-1...` atau `2-1-2...`), dijamin mati kelelahan di OSN-K. 
Kita pakai ilmu **DP Memoization 1+1 (Memasukkan pengalaman Masa Lalu)**.

Syaratnya gampang: 
Berapapun jalan untuk nyampai ke Lantai N = Total Rute nyampai ke L(N-1) DIGABUNG dengan Rute ke L(N-2). Kok bisa? Karena pijakan harfiah terakhir lu sebelum lantai-N mutlak pasti lu jongkok di Lantai-1 di bawahnya atau Lantai-2 di bawahnya. Logika siluman Fibonacci pecah.

Buka buku catatan Memo Array nya:
- Lantai 0: `1` Cara (Diam Start)
- Lantai 1: `1` Cara (Loncat 1x daridarat)
- Lantai 2: Dicapai dari gabungan rute L1 dan L0 $\rightarrow$ `1 + 1 = 2`
- Lantai 3: Dicapai dari gabungan rute L2 dan L1 $\rightarrow$ `2 + 1 = 3`
- Lantai 4: Dicapai dari gabungan rute L3 dan L2 $\rightarrow$ `3 + 2 = 5`
- Lantai 5: Dicapai dari gabungan rute L4 dan L3 $\rightarrow$ `5 + 3 = 8`
- Lantai 6: Dicapai dari gabungan rute L5 dan L4 $\rightarrow$ `8 + 5 = 13`
- Lantai 7: Dicapai dari gabungan rute L6 dan L5 $\rightarrow$ `13 + 8 = 21`


Tembus mutlak! Di tangga puncak 7, tercetak ada **21 kombinasi jalur mutlak**. Opsi dewa presisi adalah **D**.
</details>

---
