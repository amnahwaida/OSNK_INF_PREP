# 03. Pengenalan Pola (Pattern Recognition)

> "Jika kamu melihat sesuatu terjadi berulang kali, itu bukan kebetulan. Itu adalah pola."

---

## Apa itu Pengenalan Pola?

Setelah kita berhasil memecah masalah besar menjadi bagian-bagian kecil (Dekomposisi), langkah selanjutnya adalah mencari **kemiripan** atau **karakteristik berulang** di antara masalah-masalah kecil tersebut.

**Pengenalan Pola** adalah kemampuan untuk menemukan kesamaan, tren, atau keteraturan dalam suatu data atau masalah. Dengan mengenali pola, kita bisa membuat prediksi dan mencari solusi yang lebih efisien karena kita tidak perlu "menemukan roda baru" setiap kali menghadapi masalah yang mirip.

---

## Analogi di Kehidupan Nyata

Agar lebih mudah dipahami, mari kita lihat bagaimana otak kita bekerja secara alami dalam mengenali pola:

### 1. Prediksi Cuaca (The "Mendung" Pattern)
Pernahkah kamu melihat langit gelap, udara terasa lembap, dan angin berhembus kencang? Secara otomatis kamu akan berpikir: *"Wah, mau hujan nih, lebih baik bawa payung."*
*   **Polanya:** Langit gelap + Udara lembap + Angin kencang = Hujan.
*   Kamu tahu ini karena kamu sudah melihat pola yang sama berkali-kali di masa lalu.

### 2. Belajar Musik
Saat kamu belajar bermain gitar atau piano, kamu tidak menghafal setiap nada satu per satu untuk ribuan lagu. Kamu mengenali **pola kunci (Chord)**. 
*   Misalnya, lagu-lagu Pop seringkali menggunakan pola progresi yang sama (seperti I - V - vi - IV). Sekali kamu tahu polanya, kamu bisa memainkan ratusan lagu dengan mudah!

### 3. Lalu Lintas Kota
Seorang pengemudi ojek online tahu bahwa di Jakarta, jalanan menuju pusat perkantoran akan macet total pada jam 07.00 - 09.00 pagi.
*   **Polanya:** Hari kerja + Pagi hari + Jalur kantor = Macet.
*   Dengan pola ini, dia bisa memilih rute tikus yang lebih cepat.

---

## Mengapa Pengenalan Pola Sangat Penting di Informatika?

Dalam dunia komputer dan pemrograman, pengenalan pola adalah "bahan bakar" bagi teknologi canggih masa kini:

1.  **Machine Learning & AI**: Inilah cara ChatGPT atau Google Lens bekerja. Mereka dilatih dengan jutaan data untuk mengenali pola bahasa atau pola gambar.
2.  **Efisiensi Algoritma**: Seorang programmer tidak menulis kode yang sama berulang kali. Jika ada fungsi yang sering dipakai, dia akan membuat **fungsi (Function)** atau **looping**.
3.  **Deteksi Penyakit**: Komputer bisa menganali pola pada foto Rontgen untuk mendeteksi kanker dengan akurasi yang terkadang melebihi dokter karena kemampuannya memproses pola ribuan data medis sebelumnya.

---

## Relevansi dalam OSN-K Informatika

Di olimpiade, soal-soal seringkali terlihat sangat rumit dan membutuhkan waktu lama jika dikerjakan secara manual. Namun, biasanya ada **pola tersembunyi** yang jika ditemukan, soal tersebut bisa selesai dalam hitungan detik!

**Contoh Kasus:**
Diberikan barisan angka: 3, 6, 12, 24, 48, ... Berapakah angka ke-100?
*   **Tanpa Pengenalan Pola:** Kamu akan mengalikan 2 terus menerus sampai 100 kali (lelah dan rawan salah!).
*   **Dengan Pengenalan Pola:** Kamu sadar ini adalah barisan geometri dengan rasio 2. Rumusnya adalah $U_n = a \cdot r^{n-1}$. Jadi $U_{100} = 3 \cdot 2^{99}$. Selesai!

---

## Langkah-Langkah Mengenali Pola

Jika kamu menghadapi masalah, gunakan "kacamata" pengenalan pola dengan langkah berikut:

1.  **Amati (Observe)**: Lihat data atau sub-masalah yang sudah ada. Adakah yang terlihat mirip?
2.  **Bandingkan (Compare)**: Apa yang sama? Apa yang berbeda? Catat perubahannya (misal: "setiap langkah, angkanya bertambah 5").
3.  **Uji (Test)**: Cobalah pola yang kamu temukan pada data baru. Jika cocok terus, berarti pola tersebut valid.
4.  **Simpulkan (Finalize)**: Jadikan pola tersebut sebagai aturan umum (kita akan bahas ini di materi **Abstraksi** nanti).

---

## Latihan Soal Pengenalan Pola (Tahap 1)

Uji kemampuan detektif polamu di sini!

### Soal #1: Barisan Binatang
Seorang peternak mengatur urutan hewannya: Sapi, Kambing, Ayam, Sapi, Kambing, Ayam, Sapi, ...
Hewan apakah yang berada pada urutan ke-20?
A. Sapi
B. Kambing
C. Ayam
D. Bebek

<details>
<summary>💡 Hint</summary>
Polanya berulang setiap 3 hewan. Gunakan sisa bagi (modulus). 20 dibagi 3 sisanya berapa?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kambing.**
Pola berulang: 1=Sapi, 2=Kambing, 3=Ayam.
$20 \div 3 = 6$ sisa **2**. Urutan ke-2 adalah Kambing.
</details>

### Soal #2: Lampu Lalu Lintas Pintar
Sebuah lampu lalu lintas diatur dengan pola waktu: Hijau (30 detik), Kuning (5 detik), Merah (60 detik). Pola ini terus berulang. Jika sekarang lampu baru saja berubah menjadi Merah, warna apakah yang muncul tepat setelah 200 detik kemudian?
A. Merah
B. Kuning
C. Hijau
D. Mati

<details>
<summary>💡 Hint</summary>
Total satu siklus adalah $30 + 5 + 60 = 95$ detik. Hitung berapa siklus yang terjadi dalam 200 detik.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Hijau.**
Total siklus = 95 detik.
200 detik = 2 kali siklus penuh ($95 \times 2 = 190$ detik) + sisa **10 detik**.
Karena kita mulai dari awal Merah, setelah 190 detik ia kembali ke awal Merah. Detik ke-1 sampai ke-60 adalah Merah. Tunggu, soal ini menjebak.
Mari hitung ulang:
Merah (0-60s) -> Hijau (60-90s) -> Kuning (90-95s).
Sisa 10 detik setelah 2 siklus penuh (190s) berarti kita berada di detik ke-10 dari siklus ke-3.
Detik 0-60 di siklus baru adalah Merah. (Jawaban seharusnya A).
*Revisi Logika:* Jika start dari Merah, maka 10 detik kemudian masih Merah.
</details>

### Soal #3: Deteksi Serangga
Peneliti mengamati jumlah serangga: Hari ke-1 (5 ekor), Hari ke-2 (10 ekor), Hari ke-3 (20 ekor), Hari ke-4 (40 ekor).
Berdasarkan pola ini, berapa jumlah serangga di Hari ke-7?
A. 80 ekor
B. 160 ekor
C. 320 ekor
D. 640 ekor

<details>
<summary>💡 Hint</summary>
Cek rasio kenaikannya. Apakah ditambah atau dikali?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 320 ekor.**
Polanya adalah dikali 2 (eksponensial).
H1=5, H2=10, H3=20, H4=40, H5=80, H6=160, H7=320.
</details>

### Soal #4: Pola Lantai (Tesselation)
Seorang tukang bangunan memasang ubin: Hijau, Putih, Hijau, Putih, Hijau, Putih.
Manakah pernyataan yang sesuai dengan pola tersebut?
A. Semua ubin ganjil berwarna Hijau.
B. Semua ubin ganjil berwarna Putih.
C. Warna ubin ditentukan oleh ukuran ruangan.
D. Ubin ke-10 akan berwarna Hijau.

<details>
<summary>💡 Hint</summary>
Nomor ubin 1=H, 2=P, 3=H, 4=P... perhatikan angka ganjilnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Semua ubin ganjil berwarna Hijau.**
Ganjil (1, 3, 5...) adalah Hijau. Genap (2, 4, 6...) adalah Putih.
</details>

### Soal #5: Password Rahasia
Seseorang menggunakan pola untuk password-nya: `A1B2C3D4...`. Jika password-nya berlanjut sampai huruf `J`, angka berapakah yang mengikuti huruf `J`?
A. 8
B. 9
C. 10
D. 11

<details>
<summary>💡 Hint</summary>
A adalah huruf ke-1, B ke-2, C ke-3. J adalah huruf ke-berapa?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 10.**
Pola: Huruf ke-$n$ diikuti oleh angka $n$. Karena J adalah huruf ke-10, maka diikuti angka 10.
</details>

### Soal #6: Barisan Kursi Bioskop
Nomor kursi diatur: A1, A2, A3, ..., A10, B1, B2, ..., B10, C1, dst.
Kursi ke-25 dalam urutan ini adalah...
A. B5
B. C5
C. C10
D. D5

<details>
<summary>💡 Hint</summary>
Setiap baris (A, B, C...) punya 10 kursi.
Baris A: 1-10
Baris B: 11-20
Baris C: 21-30
</details>

<details>
<summary>✅ Jawaban</summary>
**B. C5.**
Kursi 1-10 di A, 11-20 di B. Maka nomor 21-30 ada di baris C. Kursi ke-25 adalah kursi ke-5 di baris C.
</details>

### Soal #7: Pola Chatting
Di aplikasi chat, status "Typing..." muncul setiap 2 detik, hilang selama 1 detik, lalu muncul lagi.
Dalam waktu 10 detik, berapa kali status "Typing..." muncul secara total?
A. 3 kali
B. 4 kali
C. 5 kali
D. 10 kali

<details>
<summary>💡 Hint</summary>
Satu siklus = 2s (muncul) + 1s (hilang) = 3 detik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 4 kali.**
- Detik 1-2: Muncul (1)
- Detik 3: Hilang
- Detik 4-5: Muncul (2)
- Detik 6: Hilang
- Detik 7-8: Muncul (3)
- Detik 9: Hilang
- Detik 10: Muncul (4)
</details>

### Soal #8: Menabung Harian
Budi menabung: Senin Rp1.000, Selasa Rp2.000, Rabu Rp3.000, dst.
Berapa total uang Budi setelah menabung selama 10 hari?
A. Rp10.000
B. Rp45.000
C. Rp55.000
D. Rp100.000

<details>
<summary>💡 Hint</summary>
Ini adalah Deret Aritmatika: $1 + 2 + 3 + ... + 10$.
Rumus: $\frac{n(n+1)}{2} \times 1.000$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Rp55.000.**
$1.000 + 2.000 + ... + 10.000 = 55.000$.
</details>

### Soal #9: Kuman di Laboratorium
Satu kuman membelah diri menjadi 3 setiap jam. Jika jam 08.00 ada 1 kuman, pukul berapa jumlah kuman menjadi minimal 81?
A. 11.00
B. 12.00
C. 13.00
D. 14.00

<details>
<summary>💡 Hint</summary>
Pola perpangkatan 3: $3^1, 3^2, 3^3, 3^4...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 12.00.**
- 08.00: 1
- 09.00: 3
- 10.00: 9
- 11.00: 27
- 12.00: 81
Dibutuhkan 4 jam dari pukul 08.00.
</details>

### Soal #10: Sudut Jarum Jam
Setiap jam, jarum panjang berputar 360 derajat. Berapa total putaran jarum panjang dalam 2 hari?
A. 24 putaran
B. 36 putaran
C. 48 putaran
D. 60 putaran

<details>
<summary>💡 Hint</summary>
1 hari = 24 jam. Jangan lupa ada 2 hari.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 48 putaran.**
1 jam = 1 putaran. 2 hari = 48 jam = 48 putaran.
</details>

### Soal #11: Barisan Fibonanci (Versi Newbie)
Urutan angka: 1, 1, 2, 3, 5, 8, ...
Berapakah angka berikutnya?
A. 10
B. 11
C. 13
D. 15

<details>
<summary>💡 Hint</summary>
Lihat dua angka sebelumnya. Apa yang terjadi jika mereka dijumlahkan?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 13.**
Polalanya: Angka saat ini = jumlah 2 angka sebelumnya. $5 + 8 = 13$.
</details>

### Soal #12: Warna Kabel Network
Urutan standar kabel LAN: Putih-Oren, Oren, Putih-Hijau, Biru, Putih-Biru, Hijau, Putih-Cokelat, Cokelat.
Kabel ke-6 dalam urutan ini berwarna?
A. Biru
B. Hijau
C. Putih-Biru
D. Oren

<details>
<summary>💡 Hint</summary>
Hitung saja urutan katanya dengan teliti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hijau.**
1.P-O, 2.O, 3.P-H, 4.B, 5.P-B, **6.Hijau**.
</details>

### Soal #13: Pola Huruf Terbalik
Pola: ABC, ZYX, DEF, WVU, ...
Tiga huruf berikutnya adalah?
A. GHI
B. JKL
C. TSR
D. RST

<details>
<summary>💡 Hint</summary>
Perhatikan ada dua barisan yang bergantian: Maju alfabet dan Mundur alfabet.
Barisan 1: ABC, DEF, ...
Barisan 2: ZYX, WVU, ...
</details>

<details>
<summary>✅ Jawaban</summary>
**A. GHI.**
Barisan ganjil (1, 3...) maju alfabet per 3 huruf. Barisan genap (2, 4...) mundur alfabet. Karena setelah urutan ke-4 (WVU), maka urutan ke-5 adalah lanjutan dari ABC dan DEF, yaitu GHI.
</details>

### Soal #14: Deteksi Serangan Cyber
Sistem keamanan mencatat login gagal: Menit 1 (1 kali), Menit 2 (3 kali), Menit 3 (5 kali), Menit 4 (7 kali).
Berapa jumlah login gagal pada menit ke-10 jika polanya tetap?
A. 15 kali
B. 17 kali
C. 19 kali
D. 20 kali

<details>
<summary>💡 Hint</summary>
Ini pola bilangan ganjil: $2n - 1$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 19 kali.**
$2(10) - 1 = 19$.
</details>

### Soal #15: Penomoran Halaman
Sebuah buku tebal memiliki pola nomor halaman di pojok kanan bawah jika genap, dan pojok kiri bawah jika ganjil. Halaman 256 akan berada di?
A. Pojok Kanan Bawah
B. Pojok Kiri Bawah
C. Tengah Bawah
D. Tidak ada nomor

<details>
<summary>💡 Hint</summary>
256 adalah bilangan genap atau ganjil?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pojok Kanan Bawah.**
Karena 256 adalah bilangan genap.
</details>

---
### Soal #16: Barisan Bilangan Kuadrat
Urutan angka: 1, 4, 9, 16, 25, ...
Berapakah angka ke-10 dalam urutan ini?
A. 81
B. 100
C. 121
D. 144

<details>
<summary>💡 Hint</summary>
Pikirkan hubungan antara posisi ($n$) dengan angka tersebut. $1=1^2, 2=4^2$ (salah), coba $1=1 \times 1, 2=2 \times 2$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 100.**
Polanya adalah $n^2$. Maka urutan ke-10 adalah $10^2 = 100$.
</details>

### Soal #17: Bilangan Prima
Barisan: 2, 3, 5, 7, 11, 13, ...
Berapakah dua angka berikutnya?
A. 15, 17
B. 17, 19
C. 17, 21
D. 19, 23

<details>
<summary>💡 Hint</summary>
Cari angka yang hanya bisa dibagi 1 dan dirinya sendiri.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 17, 19.**
15 bukan prima (bisa dibagi 3 dan 5). 21 bukan prima (bisa dibagi 3 dan 7).
</details>

### Soal #18: Pergeseran Keyboard (QWERTY)
Pola: Q, W, E, R, T, ...
Jika kita mengikuti baris kedua keyboard (Home Row), urutan apa yang setara dengan pola di atas?
A. A, S, D, F, G
B. Z, X, C, V, B
C. P, O, I, U, Y
D. L, K, J, H, G

<details>
<summary>💡 Hint</summary>
Lihat susunan keyboard fisik atau bayangkan baris tengah (A, S, D...).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. A, S, D, F, G.**
QWERTY adalah baris atas. ASDFG adalah baris tengah (Home Row).
</details>

### Soal #19: Sandi Geser (Caesar Cipher)
Pola sandi: `HELLO` menjadi `IFMMP`.
Berdasarkan pola tersebut, kata `WORLD` akan menjadi...
A. XPSME
B. VNSKC
C. XPMRE
D. YPSME

<details>
<summary>💡 Hint</summary>
Cek pergeseran setiap huruf. H ke I (+1), E ke F (+1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. XPSME.**
W+1=X, O+1=P, R+1=S, L+1=M, D+1=E.
</details>

### Soal #20: Menghitung Biner
Pola angka biner: 0, 1, 10, 11, ...
Berapakah angka berikutnya?
A. 12
B. 100
C. 111
D. 101

<details>
<summary>💡 Hint</summary>
Dalam biner, angka maksimal adalah 1. Jika sudah 11, kita butuh kolom baru di kiri.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 100.**
Urutan desimalnya: 0, 1, 2, 3. Maka berikutnya adalah 4 desimal, yang dalam biner adalah 100.
</details>

### Soal #21: Pergeseran Hari
Jika hari ini adalah Senin, dan kita mengikuti pola "Lompat 2 hari", urutannya adalah: Senin, Kamis, Minggu, ...
Hari apakah yang muncul setelah Minggu?
A. Selasa
B. Rabu
C. Kamis
D. Jumat

<details>
<summary>💡 Hint</summary>
Senin (+2 hari kosong: Selasa, Rabu) -> Kamis.
Kamis (+2 hari kosong: Jumat, Sabtu) -> Minggu.
Minggu (+2 hari kosong: ...) -> ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rabu.**
Setelah Minggu adalah Senin dan Selasa (lompat), maka hari berikutnya adalah Rabu.
</details>

### Soal #22: Jam Digital (Format 12 Jam)
Pola waktu: 10.00 AM, 11.00 AM, 12.00 PM, ...
Waktu apakah yang muncul setelah 12.00 PM?
A. 13.00 PM
B. 01.00 AM
C. 01.00 PM
D. 12.00 AM

<details>
<summary>💡 Hint</summary>
Setelah jam 12 siang, angka kembali ke 1 dan status AM/PM tetap PM sampai tengah malam.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 01.00 PM.**
Dalam format 12 jam, setelah 12.00 PM adalah 01.00 PM.
</details>

### Soal #23: Fase Bulan
Urutan: Bulan Baru, Hilal (Bulan Sabit Muda), Perbani Awal (Setengah), ...
Manakah fase berikutnya yang paling tepat?
A. Bulan Mati
B. Bulan Purnama
C. Bulan Cembung (Waxing Gibbous)
D. Gerhana Matahari

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana bulan perlahan-lahan "membesar" dari sabit ke setengah, lalu menuju penuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Bulan Cembung (Waxing Gibbous).**
Pola pertumbuhan penampakan bulan adalah: Baru -> Sabit -> Setengah -> Cembung -> Purnama.
</details>

### Soal #24: Pola Lampu Hias
Lampu hias berkedip: Merah (2x), Biru (1x), Merah (2x), Biru (1x).
Jika lampu sudah berkedip total 20 kali, berapa kali warna Biru muncul?
A. 6 kali
B. 7 kali
C. 10 kali
D. 20 kali

<details>
<summary>💡 Hint</summary>
Satu paket pola = M, M, B (3 kedipan).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 6 kali.**
$20 \div 3 = 6$ siklus (sisa 2). Satu siklus ada 1 Biru. $6 \times 1 = 6$. Sisa 2 kedipan adalah Merah, Merah. Total Biru tetap 6.
</details>

### Soal #25: Pergerakan Lift
Lift bergerak dari lantai: 1 -> 4 -> 7 -> 10.
Lantai berapakah berikutnya jika polanya tetap?
A. 11
B. 12
C. 13
D. 14

<details>
<summary>💡 Hint</summary>
Berapa jarak antar lantai yang dikunjungi?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 13.**
Polanya adalah $+3$. $10 + 3 = 13$.
</details>

### Soal #26: Layout Ikon Smartphone
Ikon diatur dalam grid 3x3 (3 kolom, 3 baris). Ikon nomor 1 (Pojok Kiri Atas), nomor 3 (Pojok Kanan Atas).
Di manakah letak ikon nomor 5?
A. Pojok Kiri Bawah
B. Tengah-Tengah
C. Pojok Kanan Bawah
D. Tengah Atas

<details>
<summary>💡 Hint</summary>
1 2 3
4 5 6
7 8 9
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tengah-Tengah.**
Dalam grid 3x3, angka 5 berada tepat di pusat (baris 2, kolom 2).
</details>

### Soal #27: Refresh News Feed
Sebuah aplikasi menampilkan 5 berita baru setiap kali layar di-swipe bawah. Jika saat ini ada 15 berita, dan kamu swipe 4 kali lagi, total berita menjadi...
A. 20
B. 30
C. 35
D. 40

<details>
<summary>💡 Hint</summary>
Hitung penambahan dasarnya: $15 + (4 \times 5)$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 35.**
$15 + 20 = 35$.
</details>

### Soal #28: Navigasi Halaman (Pagination)
Tombol halaman: `1 2 3 [Next]`. Jika kamu klik Next, muncul `2 3 4 [Next]`. Klik Next lagi muncul `3 4 5 [Next]`.
Setelah total 10 kali klik Next dari posisi awal, angka pertama yang muncul adalah...
A. 10
B. 11
C. 12
D. 13

<details>
<summary>💡 Hint</summary>
Klik 1: Awalnya 1.
Klik 1: Muncul 2 di awal.
Klik 2: Muncul 3 di awal.
Pola: Angka awal = 1 + (jumlah klik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 11.**
$1 + 10 = 11$.
</details>

### Soal #29: Penurunan Baterai
Baterai HP: 100% (Jam 12.00), 95% (Jam 12.30), 90% (Jam 13.00).
Jam berapakah baterai akan menyentuh 50% jika penggunaan tetap sama?
A. 15.00
B. 16.00
C. 17.00
D. 18.00

<details>
<summary>💡 Hint</summary>
Baterai turun 5% setiap 30 menit (10% per jam).
Total penurunan yang dicari: $100\% - 50\% = 50\%$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 17.00.**
Turun 50% butuh waktu $50\% \div 10\%/\text{jam} = 5$ jam.
12.00 + 5 jam = 17.00.
</details>

### Soal #30: Pola Kecepatan Mengetik (WPM)
Menit 1: 20 WPM, Menit 2: 25 WPM, Menit 3: 30 WPM.
Pada menit ke-berapa kamu mencapai kecepatan 60 WPM?
A. Menit 8
B. Menit 9
C. Menit 10
D. Menit 11

<details>
<summary>💡 Hint</summary>
Kenaikan $5$ WPM per menit.
Berapa kenaikan total dari 20 ke 60?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menit 9.**
Selisih = 40 WPM. $40 \div 5 = 8$ langkah tambahan setelah menit ke-1.
$1 + 8 = 9$.
</details>

### Soal #31: Pola Pakaian Musim
Urutan: Jaket Tebal (Dingin), Kaos (Panas), Jas Hujan (Hujan), Jaket Tebal, Kaos, Jas Hujan.
Jika sekarang musim ke-100, pakaian apa yang dipakai?
A. Jaket Tebal
B. Kaos
C. Jas Hujan
D. Baju Renang

<details>
<summary>💡 Hint</summary>
Pola berulang 3. $100 \div 3$ sisanya berapa?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Jaket Tebal.**
$100 \div 3 = 33$ sisa **1**. Urutan ke-1 adalah Jaket Tebal.
</details>

### Soal #32: Metamorfosis Kupu-Kupu
Urutan: Telur, Ulat, Kepompong, Kupu-Kupu, Telur, ...
Jika kita anggap ini siklus 4 tahap, tahap ke-15 adalah...
A. Telur
B. Ulat
C. Kepompong
D. Kupu-Kupu

<details>
<summary>💡 Hint</summary>
$15 \div 4$ sisanya berapa?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kepompong.**
$15 \div 4 = 3$ sisa **3**. Urutan ke-3 adalah Kepompong.
</details>

### Soal #33: Pola Rantai Makanan
Pola: Rumput -> Belalang -> Katak -> Ular -> Elang.
Jika populasi Katak menurun drastis, manakah pola perubahan yang logis?
A. Populasi Belalang bertambah, Populasi Ular berkurang.
B. Populasi Rumput bertambah, Populasi Elang bertambah.
C. Populasi Belalang berkurang, Populasi Ular bertambah.
D. Semua populasi punah seketika.

<details>
<summary>💡 Hint</summary>
Katak memakan Belalang (jika Katak sedikit, Belalang senang).
Ular memakan Katak (jika Katak sedikit, Ular lapar).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Belalang bertambah, Ular berkurang.**
Ketidakhadiran predator (Katak) membuat mangsa (Belalang) melonjak, dan pemangsa atas (Ular) kelaparan.
</details>

### Soal #34: Tabel Periodik Sederhana
Unsur: H (1), He (2), Li (3), Be (4), ...
Unsur nomor atom 10 (Neon) mengikuti pola gas mulia yang sama dengan He (2). Berapa selisih nomor atomnya?
A. 2
B. 8
C. 10
D. 18

<details>
<summary>💡 Hint</summary>
$10 - 2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 8.**
Pola periodik seringkali memiliki selisih 8 (oktet) untuk unsur-unsur yang sifatnya mirip di awal tabel.
</details>

### Soal #35: Pola Hex Warna
Warna: `#FF0000` (Merah), `#00FF00` (Hijau), `#0000FF` (Biru).
Berdasarkan pola posisi `FF` (nilai maksimal), manakah kode untuk warna Kuning (campuran Merah dan Hijau)?
A. `#FFFF00`
B. `#00FFFF`
C. `#FF00FF`
D. `#FFFFFF`

<details>
<summary>💡 Hint</summary>
Merah di posisi 1-2, Hijau di 3-4, Biru di 5-6.
Kuning = Merah + Hijau. Gabungkan posisi `FF`-nya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. #FFFF00.**
Posisi Merah dan Hijau diisi `FF`, Biru diisi `00`.
</details>

### Soal #36: Angka Romawi
Urutan: I (1), II (2), III (3), IV (4), V (5), VI (6).
Berapakah angka Romawi untuk 9?
A. VIIII
B. IX
C. XI
D. VX

<details>
<summary>💡 Hint</summary>
Polanya menggunakan pengurangan dari 10 (X) jika angkanya tepat di bawah 5 atau 10.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. IX.**
I (1) diletakkan di kiri X (10) berarti $10 - 1 = 9$.
</details>

### Soal #37: Pola Koordinat Mobil
Mobil bergerak: (0,0) -> (0,2) -> (0,4) -> (0,6).
Manakah arah gerak mobil tersebut?
A. Ke kanan (Sumbu X positif)
B. Ke atas (Sumbu Y positif)
C. Diagonal
D. Berputar di tempat

<details>
<summary>💡 Hint</summary>
Lihat angka mana yang berubah. X (depan) atau Y (belakang)?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ke atas (Sumbu Y positif).**
Nilai Y bertambah secara konsisten sementara X tetap 0.
</details>

### Soal #38: Baris Sudoku
Sebuah baris Sudoku berisi: 1, 2, 3, 4, 5, 6, 7, 8, ...
Angka berapakah yang wajib ada di kotak terakhir?
A. 0
B. 9
C. 10
D. Berapa saja bebas

<details>
<summary>💡 Hint</summary>
Pola Sudoku menggunakan angka 1 sampai 9 tanpa pengulangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 9.**
Setiap baris/kolom Sudoku harus berisi pola unik 1-9.
</details>

### Soal #39: Kemenangan Tic-Tac-Toe
Simbol `X` berada di grid (1,1) dan (2,2). Untuk pola menang diagonal, di manakah `X` selanjutnya harus diletakkan?
A. (3,1)
B. (3,3)
C. (1,3)
D. (2,1)

<details>
<summary>💡 Hint</summary>
Diagonal berarti x dan y bertambah/berkurang bersamaan: (1,1), (2,2), ...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. (3,3).**
Mengikuti garis lurus diagonal dari kiri atas ke kanan bawah.
</details>

### Soal #40: Langkah Kuda Catur
Kuda bergerak dalam pola "L" (2 langkah lurus, 1 samping). Jika kuda di (0,0) bergerak ke depan, posisi mana yang **MUNGKIN**?
A. (1,1)
B. (2,1)
C. (2,2)
D. (3,0)

<details>
<summary>💡 Hint</summary>
2 langkah di sumbu X dan 1 di sumbu Y, atau sebaliknya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. (2,1).**
Dua langkah horizontal dan satu vertikal membentuk huruf L.
</details>

### Soal #41: Durasi Nada Musik
Pola: Whole Note (4 ketuk), Half Note (2 ketuk), Quarter Note (1 ketuk), ...
Berapa ketuk untuk nada berikutnya (Eighth Note)?
A. 0,5 ketuk
B. 0,25 ketuk
C. 2 ketuk
D. 0 ketuk

<details>
<summary>💡 Hint</summary>
Lihat rasionya. Dari 4 ke 2, dari 2 ke 1. Apakah dibagi 2?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 0,5 ketuk.**
Setiap langkah, durasi nada didekomposisi menjadi setengahnya.
</details>

### Soal #42: Lapisan Melukis
Urutan: Gesso (Primer), Sketsa, Warna Dasar, Detail, Pernis.
Jika kamu sedang memberikan bayangan halus pada karakter, di posisi manakah kamu berada?
A. Sketsa
B. Detail
C. Pernis
D. Gesso

<details>
<summary>💡 Hint</summary>
Bayangan halus biasanya diberikan setelah warna dasar selesai tapi sebelum lapisan pelindung (pernis).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Detail.**
Bekerja pada aspek halus seperti bayangan masuk dalam kategori pengerjaan detail.
</details>

### Soal #43: Resep Kue
Langkah: 1. Campur Adonan, 2. Masukkan Oven, 3. Dinginkan, 4. Beri Topping.
Jika kamu melihat seseorang sedang mengoleskan krim cokelat di atas kue yang sudah matang, ia ada di tahap...
A. 1
B. 2
C. 3
D. 4

<details>
<summary>💡 Hint</summary>
Topping adalah bagian paling akhir untuk dekorasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. 4.**
Pemberian krim/cokelat adalah bagian dari topping.
</details>

### Soal #44: Stacking Balok
Balok disusun: Bawah (3 balok), Tengah (2 balok), Atas (1 balok).
Jika kita ingin membuat piramida 5 tingkat, berapa balok di tingkat paling bawah?
A. 4
B. 5
C. 6
D. 10

<details>
<summary>💡 Hint</summary>
Pola: Tingkat 1 (Atas) = 1.
Tingkat 2 = 2.
Tingkat 3 = 3.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 5.**
Mengikuti pola linear sederhana dimana jumlah balok = nomor tingkat dari atas.
</details>

### Soal #45: Refleksi Cermin
Di depan cermin, kamu mengangkat tangan kanan. Di dalam cermin, posisi bayangan tanganmu terlihat di sebelah...
A. Kanan bayangan
B. Kiri bayangan
C. Atas bayangan
D. Bawah bayangan

<details>
<summary>💡 Hint</summary>
Cermin membalikkan pola horizontal (Kanan-Kiri) tapi tidak vertikal (Atas-Bawah).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kiri bayangan.**
Simetri cermin membalikkan orientasi sisi.
</details>

### Soal #46: Panjang Bayangan Matahari
Panjang bayangan: Jam 07.00 (Panjang), Jam 10.00 (Sedang), Jam 12.00 (Pendek).
Pola yang terjadi setelah jam 12.00 adalah...
A. Bayangan makin pendek
B. Bayangan menghilang selamanya
C. Bayangan kembali memanjang
D. Bayangan berputar-putar

<details>
<summary>💡 Hint</summary>
Bayangan terpendek saat matahari tepat di atas. Setelah itu, matahari mulai condong ke barat.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Bayangan kembali memanjang.**
Matahari yang menjauh dari posisi tegak lurus (Zenit) akan memperpanjang bayangan lagi.
</details>

### Soal #47: Pasang Surut Air Laut
Jika air laut tertinggi (pasang) jam 06.00 dan terendah (surut) jam 12.00, kapan pasang berikutnya terjadi?
A. 14.00
B. 16.00
C. 18.00
D. 24.00

<details>
<summary>💡 Hint</summary>
Satu siklus Pasang -> Surut butuh 6 jam. Berapa lama untuk Surut -> Pasang?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 18.00.**
Siklus biasanya berulang setiap 12 jam untuk pasang yang sama (semidiurnal). $6 + 12 = 18$.
</details>

### Soal #48: Pertumbuhan Penduduk
Penduduk desa: Tahun 1 (100 orang), Tahun 2 (200), Tahun 3 (400).
Jika pertumbuhan ini adalah pola "Lipat Dua", berapa penduduk di Tahun 5?
A. 800
B. 1.200
C. 1.600
D. 2.000

<details>
<summary>💡 Hint</summary>
T1=100, T2=200, T3=400, T4=..., T5=...
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 1.600.**
T4 = 800, T5 = 1.600.
</details>

### Soal #49: Peluruhan Zat Radioaktif
Zat X seberat 100 gram memiliki waktu paruh (half-life) 1 jam. Artinya setiap 1 jam beratnya berkurang setengah.
Berapa gram sisa zat setelah 3 jam?
A. 50 gram
B. 25 gram
C. 12,5 gram
D. 0 gram

<details>
<summary>💡 Hint</summary>
Jam 1: 100 -> 50.
Jam 2: 50 -> 25.
Jam 3: 25 -> ...
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 12,5 gram.**
Pembagian 2 berulang adalah pola peluruhan alami.
</details>

### Soal #50: Pasangan Basa DNA
Pola DNA: Adenin (A) selalu dengan Timin (T), Sitosin (C) selalu dengan Guanin (G).
Jika urutan di satu sisi adalah `A-C-G-T`, urutan pasangannya adalah...
A. `T-G-C-A`
B. `G-A-T-C`
C. `A-C-G-T`
D. `U-A-C-G`

<details>
<summary>💡 Hint</summary>
A-T, C-G. Tukarkan saja setiap hurufnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. T-G-C-A.**
A dipasangkan dengan T, C dengan G, G dengan C, T dengan A.
</details>

### Soal #51: Siklus Lampu Lalu Lintas Kota
Pola lampu: Hijau (40 detik), Kuning (5 detik), Merah (55 detik).
Jika sekarang baru saja berubah menjadi Hijau, warna apa yang menyala tepat pada detik ke-101?
A. Hijau
B. Kuning
C. Merah
D. Padam

<details>
<summary>💡 Hint</summary>
Total satu siklus = $40 + 5 + 55 = 100$ detik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hijau.**
Setelah 100 detik, lampu kembali ke awal siklus (Hijau). Detik ke-101 adalah detik ke-1 dari siklus kedua.
</details>

### Soal #52: Pola Buka Kunci (Pattern Unlock)
Seseorang membuat pola buka kunci HP berbentuk huruf "L" terbalik pada grid 3x3. Ia menyentuh titik: 1, 4, 7, 8, 9.
Jika ia ingin membuat pola "U" yang dimulai dari titik 1, urutan titik manakah yang paling logis?
A. 1, 4, 7, 8, 9, 6, 3
B. 1, 2, 3, 6, 9, 8, 7
C. 1, 5, 9
D. 7, 4, 1, 2, 3, 6, 9

<details>
<summary>💡 Hint</summary>
Grid 3x3:
1 2 3
4 5 6
7 8 9
Pola "U" turun, mendatar, lalu naik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 1, 4, 7, 8, 9, 6, 3.**
1-4-7 (turun kiri), 7-8-9 (dasar), 9-6-3 (naik kanan).
</details>

### Soal #53: Sandi Morse Sederhana
Pola: Titik (pendek), Strip (panjang). Huruf `S` adalah `...` dan huruf `O` adalah `---`.
Bagaimana pola untuk kata `SOS`?
A. `... --- ...`
B. `--- ... ---`
C. `... ... ...`
D. `--- --- ---`

<details>
<summary>💡 Hint</summary>
Gabungkan saja pola S, O, dan S.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. ... --- ...**
Pola internasional yang sangat mudah dikenali.
</details>

### Soal #54: Pola Barcode
Sebuah barcode terdiri dari garis hitam tebal dan tipis. Jika pola garisnya adalah: Tipis, Tebal, Tipis, Tebal.
Manakah yang merupakan representasi angka jika angka tersebut selalu dimulai dengan garis Tipis?
A. Angka Ganjil
B. Angka Genap
C. Tergantung panjang barcode
D. Pola garis tidak berhubungan dengan angka

<details>
<summary>💡 Hint</summary>
Barcode menggunakan ketebalan garis sebagai "kode" untuk dibaca sensor.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Angka Ganjil (Dalam sistem kode tertentu).**
Meskipun sistem barcode asli rumit, dalam dekomposisi sederhana, variasi ketebalan adalah cara mengenali identitas data.
</details>

### Soal #55: Kotak Sudut QR Code
Perhatikan gambar QR Code (bayangkan). Di 3 sudutnya selalu ada kotak besar dengan kotak kecil di dalamnya. Apa fungsinya berdasarkan pengenalan pola?
A. Agar terlihat bagus saja.
B. Sebagai titik acuan (pola posisi) agar kamera tahu orientasi dan batas kode.
C. Untuk menyimpan data nama pemilik QR.
D. Sebagai hiasan pelengkap.

<details>
<summary>💡 Hint</summary>
Gunakan logika: Mengapa posisinya selalu di sudut yang sama (kiri atas, kanan atas, kiri bawah)?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sebagai titik acuan posisinya.**
Pola kotak sudut membantu scanner mengenali QR Code meskipun posisinya miring atau terbalik.
</details>

### Soal #56: Pola Membersihkan Jendela
Seorang pembersih kaca menyeka jendela dengan pola "S" atau "Zig-zag" dari atas ke bawah. Mengapa ia tidak melakukannya secara acak?
A. Agar air sabun tidak menetes ke bagian yang sudah bersih.
B. Agar pekerjaannya terlihat seperti sedang menari.
C. Karena aturan dari pabrik pembersih kaca.
D. Karena dia takut ketinggian.

<details>
<summary>💡 Hint</summary>
Dekomposisi tugas membersihkan: Area atas dibersihkan dulu agar tetesan air tidak mengotori area bawah yang sudah bersih.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Agar air tidak menetes ke bagian bersih.**
Efisiensi gerak dan hasil akhir yang maksimal ditentukan oleh pola kerja yang konsisten.
</details>

### Soal #57: Memotong Rumput Stadion
Petugas memotong rumput stadion sepak bola dengan pola lingkaran konsentris dari tengah ke luar. Manakah pernyataan yang benar?
A. Pola ini lebih cepat selesai daripada pola lurus.
B. Pola ini menciptakan estetika visual garis-garis melingkar karena arah rebah rumput.
C. Petugas tersebut sedang pusing sehingga jalannya berputar.
D. Memotong rumput harus selalu melingkar menurut hukum fisika.

<details>
<summary>💡 Hint</summary>
Pola pengerjaan fisik seringkali ditujukan untuk hasil visual atau kemudahan navigasi alat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan estetika visual.**
Pola yang rapi memberikan identitas visual pada stadion profesional.
</details>

### Soal #58: Pola Susunan Bata (Stretcher Bond)
Dinding bata disusun: Baris 1 (Utuh, Utuh...), Baris 2 (Setengah, Utuh, Utuh..., Setengah).
Mengapa bata baris kedua digeser setengah panjang bata?
A. Agar tukangnya tidak bosan.
B. Agar celah antar bata tidak sejajar lurus dari atas ke bawah (menambah kekuatan struktur).
C. Karena kekurangan jumlah bata utuh.
D. Agar dinding terlihat bergerigi di sampingnya.

<details>
<summary>💡 Hint</summary>
Pola selang-seling bertujuan untuk mengunci beban antar balok bata.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Agar celah tidak sejajar (Memperkuat struktur).**
Ini adalah pola rekayasa sipil klasik untuk stabilitas bangunan.
</details>

### Soal #59: Bagan Turnamen (Bracket)
Dalam turnamen sistem gugur dengan 16 tim, berapa banyak pertandingan di babak pertama?
A. 4
B. 8
C. 16
D. 32

<details>
<summary>💡 Hint</summary>
Pola sistem gugur: 2 tim bertanding menghasilkan 1 pemenang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 8.**
$16 \text{ tim} \div 2 = 8 \text{ pertandingan}$. Polanya adalah jumlah pertandingan = setengah dari jumlah tim di babak tersebut.
</details>

### Soal #60: Warna Papan Catur
Kotak papan catur di posisi (1,1) berwarna Hitam. Kotak (1,2) berwarna Putih.
Warna kotak di posisi (8,8) adalah?
A. Hitam
B. Putih
C. Merah
D. Hijau

<details>
<summary>💡 Hint</summary>
Jika jumlah koordinat ($x+y$) genap, warnanya Hitam. Jika ganjil, warnanya Putih.
$(1,1) \rightarrow 1+1=2$ (Hitam).
$(1,2) \rightarrow 1+2=3$ (Putih).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hitam.**
$8 + 8 = 16$. Karena 16 adalah genap, maka warnanya Hitam.
</details>

### Soal #61: Pola Tuts Piano
Tuts hitam pada piano diatur dalam kelompok: 2 tuts, 3 tuts, 2 tuts, 3 tuts.
Berapa jumlah total tuts hitam dalam satu oktaf (dari C ke B)?
A. 2
B. 3
C. 5
D. 7

<details>
<summary>💡 Hint</summary>
Satu oktaf berisi satu kelompok "2" dan satu kelompok "3".
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 5.**
$2 + 3 = 5$ tuts hitam.
</details>

### Soal #62: Stem Gitar (Standard Tuning)
Urutan nada senar dari yang paling tebal (atas) ke paling tipis (bawah): E, A, D, G, B, E.
Senar nomor berapa yang memiliki nada paling tinggi?
A. Senar 1 (paling bawah)
B. Senar 6 (paling atas)
C. Senar 3
D. Senar 4

<details>
<summary>💡 Hint</summary>
Semakin tipis senar, getarannya semakin cepat (nada tinggi).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Senar 1 (paling bawah).**
Pola urutan ini dirancang agar jari manusia mudah menjangkau harmoni nada.
</details>

### Soal #63: Ikon Indikator Baterai
Indikator baterai berubah warna: Hijau (100-21%), Kuning (20-11%), Merah (10-0%).
Jika bateraimu 15%, warna apa yang terlihat?
A. Hijau
B. Kuning
C. Merah
D. Biru

<details>
<summary>💡 Hint</summary>
Cek range angkanya. 15 berada di antara 11 dan 20.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kuning.**
Warna kuning menunjukkan peringatan (Warning) sebelum benar-benar habis.
</details>

### Soal #64: Progress Bar Download
Sebuah file 100MB didownload. Progress bar menunjukkan: 25% (25MB), 50% (50MB).
Manakah yang benar tentang pola progress bar linear?
A. Panjang bar berbanding lurus dengan jumlah data yang sudah masuk.
B. Bar akan langsung penuh meskipun baru 1%.
C. Bar tidak bergerak sampai download selesai.
D. Bar bergerak mundur jika internet lambat.

<details>
<summary>💡 Hint</summary>
Linear berarti tetap/sejajar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Panjang bar berbanding lurus dengan data.**
Inilah dekomposisi visual dari status proses digital.
</details>

### Soal #65: Bar Sinyal Wi-Fi
Ikon Wi-Fi menunjukkan 4 bar saat kamu di samping router, dan 1 bar saat kamu di luar rumah. Apa polanya?
A. Jumlah bar mewakili kekuatan sinyal (dBm).
B. Jumlah bar mewakili jumlah orang yang pakai Wi-Fi.
C. Jumlah bar menunjukkan harga routernya.
D. Bar akan penuh jika kamu berteriak kencang ke HP.

<details>
<summary>💡 Hint</summary>
Pola visual ini membantu pengguna mendeteksi "masalah jarak" dengan sumber internet.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mewakili kekuatan sinyal.**
Semakin banyak bar, semakin kuat penerimaan gelombang radio.
</details>

### Soal #66: Posisi Scroll Bar
Jika kamu berada di bagian paling bawah sebuah artikel yang sangat panjang, di manakah posisi kotak scroll bar di sisi kanan layar?
A. Di paling atas
B. Di paling bawah
C. Di tengah-tengah
D. Menghilang

<details>
<summary>💡 Hint</summary>
Scroll bar adalah pola penunjuk lokasi relatif terhadap total konten.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di paling bawah.**
Posisi fisik scroll bar mencerminkan posisi pandanganmu di dokumen.
</details>

### Soal #67: Notifikasi Badge (Angka di Ikon App)
Di ikon WhatsApp tertulis angka "5". Setelah kamu membaca 2 chat baru, angka tersebut menjadi "3". Apa polanya?
A. Angka tersebut adalah jumlah chat yang belum dibaca.
B. Angka tersebut adalah tanggal hari ini.
C. Angka tersebut acak agar pengguna penasaran.
D. Angka tersebut menunjukkan sisa memori HP.

<details>
<summary>💡 Hint</summary>
Pola counter (penghitung) akan berkurang sesuai aksi pengguna (membaca).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Jumlah chat yang belum dibaca.**
Sederhananya: $5 - 2 = 3$.
</details>

### Soal #68: Warning Cloud Storage
Google Drive memberimu peringatan warna merah pada bar penyimpanan jika penggunaan mencapai 14.5GB dari 15GB. Mengapa warnanya berubah merah?
A. Karena Google suka warna merah.
B. Pola peringatan ambang batas (threshold) untuk memberitahu kapasitas hampir penuh.
C. Karena ada virus di dalam file.
D. Karena filenya terbakar.

<details>
<summary>💡 Hint</summary>
Warna merah secara universal digunakan untuk status "Bahaya" atau "Kritis".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola peringatan ambang batas (Threshold).**
Sistem mengenali pola data $> 90\%$ sebagai kondisi kritis yang butuh perhatian pengguna.
</details>

### Soal #69: Auto-Brightness
Layar HP redup saat kamu masuk ke bioskop yang gelap, dan menjadi sangat terang saat kamu keluar ke terik matahari. Sensor apa yang mengenali pola cahaya ini?
A. Sensor Suhu
B. Sensor Cahaya (Ambient Light Sensor)
C. Sensor Sentuh
D. Sensor Suara

<details>
<summary>💡 Hint</summary>
Output (terang layar) mengikuti Input (cahaya sekitar).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor Cahaya.**
Algoritma menyesuaikan level kecerahan berdasarkan pola intensitas cahaya ruangan.
</details>

### Soal #70: Landskap Wajah (FaceID)
Teknologi FaceID mengenali wajahmu meskipun kamu memakai kacamata, tapi sering gagal jika kamu memakai masker medis yang menutupi hidung dan mulut. Mengapa?
A. Karena kacamata tidak banyak mengubah pola bentuk mata dan dahi yang unik.
B. Karena HP tidak suka orang memakai masker.
C. Karena masker membuat wajahmu menjadi terlalu cantik/tampan.
D. Karena masker merusak kamera depan.

<details>
<summary>💡 Hint</summary>
Sistem memecah wajah menjadi ribuan titik (titik-titik pola). Jika terlalu banyak titik yang hilang (tertutup), pola tidak terbaca.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kacamata tidak banyak mengubah pola mata/dahi.**
Mata, dahi, dan tulang pipi seringkali cukup untuk identifikasi jika polanya masih konsisten dengan data tersimpan.
</details>

### Soal #71: Pola Sidik Jari
Tiga pola dasar sidik jari manusia adalah: Loop (Melengkung), Whorl (Lingkaran), dan Arch (Busur). Manakah pernyataan yang benar?
A. Semua orang di dunia memiliki pola yang persis sama.
B. Pola tetap sama sepanjang hidup, tapi detail kecilnya (minutiae) unik untuk setiap orang.
C. Sidik jari bisa berubah jika kita sering mencuci piring.
D. Sidik jari hanya untuk membuka pintu kantor.

<details>
<summary>💡 Hint</summary>
Meskipun polanya mirip (seperti pola garis-garis), setiap pola punya rincian pengulangan yang berbeda.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola tetap sama, detailnya unik.**
Pengenalan pola sidik jari adalah dasar keamanan biometrik modern.
</details>

### Soal #72: Pola Iris Mata
Mengapa Iris mata lebih akurat daripada sidik jari untuk keamanan?
A. Karena mata tidak pernah kotor.
B. Karena pola tekstur iris sangat kompleks dan hampir tidak mungkin dipalsukan atau berubah karena luka fisik.
C. Karena mata adalah jendela hati.
D. Karena scan mata terlihat lebih keren seperti di film fiksi ilmiah.

<details>
<summary>💡 Hint</summary>
Kerumitan pola menentukan tingkat keamanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tekstur iris sangat kompleks.**
Dekomposisi tekstur mata menghasilkan ribuan variabel data unik.
</details>

### Soal #73: Irama Jantung (EKG)
Dokter melihat grafik "P-Q-R-S-T" yang berulang teratur pada layar monitor. Jika jarak antar puncak grafik (R-R) semakin pendek, apa yang terjadi?
A. Detak jantung melambat.
B. Detak jantung lebih cepat (misal: saat olahraga).
C. Pasien tertidur lelap.
D. Alatnya rusak.

<details>
<summary>💡 Hint</summary>
Laju (Rate) berhubungan dengan frekuensi pengulangan pola.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Detak jantung lebih cepat.**
Semakin sering pola muncul dalam satu waktu, semakin tinggi frekuensinya.
</details>

### Soal #74: Pola Pernapasan
Pola napas normal manusia dewasa adalah 12-20 kali per menit. Jika seseorang bernapas 40 kali per menit, pola ini menunjukkan kondisi...
A. Sangat santai.
B. Hiperventilasi atau sesak napas (butuh penanganan medis).
C. Sedang bermeditasi.
D. Tubuh sedang membutuhkan karbon dioksida tinggi.

<details>
<summary>💡 Hint</summary>
Mengenali pola "Normal" membantu mendeteksi pola "Anomali" (Kejanggalan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hiperventilasi (Sesak napas).**
Anomali pada pola biologis adalah cara tubuh memberi sinyal adanya masalah.
</details>

### Soal #75: Ritme Sirkadian
Tubuh manusia memproses pola: Jam 21.00 Produksi Melatonin (Ngantuk), Jam 06.00 Produksi Kortisol (Bangun).
Apa yang terjadi jika kamu begadang sampai pagi?
A. Ritme tubuhmu tetap normal.
B. Terjadi kekacauan pola internal (Jet lag sosial) yang membuat tubuh tetap merasa lelah.
C. Tubuh akan berubah menjadi robot.
D. Mata menjadi hijau.

<details>
<summary>💡 Hint</summary>
Pola alami yang terganggu membutuhkan waktu untuk sinkronisasi ulang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terjadi kekacauan pola internal.**
Gaya hidup yang berlawanan dengan pola biologis (Circadian Rhythm) berdampak buruk pada kesehatan jangka panjang.
</details>

### Soal #76: Migrasi Burung
Kelompok burung terbang membentuk formasi huruf "V". Apa pola fungsional di baliknya?
A. Menghemat energi dengan memanfaatkan pusaran udara dari kepakan burung di depannya.
B. Agar terlihat seperti panah penunjuk jalan.
C. Karena leader burungnya suka huruf V.
D. Agar burung di belakang tidak bisa melihat pemandangan.

<details>
<summary>💡 Hint</summary>
Pola di alam hampir selalu memiliki tujuan efisiensi bertahan hidup.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menghemat energi.**
Dekomposisi aerodinamika menunjukkan bahwa pola "V" sangat efisien untuk perjalanan jarak jauh.
</details>

### Soal #77: Jadwal Pelajaran Sekolah
Senin (Matematika, Fisika), Selasa (Bahasa Indonesia, Sejarah), Senin depan muncul (Matematika, Fisika).
Mata pelajaran apa yang kemungkinan besar muncul di Selasa depan?
A. Olahraga
B. Bahasa Indonesia
C. Seni Budaya
D. Libur

<details>
<summary>💡 Hint</summary>
Jadwal sekolah biasanya menggunakan pola pengulangan mingguan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bahasa Indonesia.**
Mengikuti pola rutin yang sama dari minggu sebelumnya.
</details>

### Soal #78: Kesulitan Soal Ujian
Sebuah ujian dikomposisi menjadi 40 soal. Polanya: 10 soal awal (Mudah), 20 soal tengah (Sedang), 10 soal akhir (Sulit).
Jika kamu sedang mengerjakan soal nomor 35, tingkat kesulitannya kemungkinan besar adalah...
A. Sangat Mudah
B. Sedang
C. Sulit
D. Bonus

<details>
<summary>💡 Hint</summary>
Nomor 35 berada di rentang 10 soal terakhir (31-40).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Sulit.**
Pola ini umum digunakan dalam perancangan tes standar (seperti TOEP atau SAT).
</details>

### Soal #79: Penilaian Nilai (Rubrik)
Pola Nilai: A (90-100), B (80-89), C (70-79).
Jika nilaimu 85, huruf apa yang kamu dapatkan?
A. A
B. B
C. C
D. D

<details>
<summary>💡 Hint</summary>
85 masuk ke range yang mana?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
Dekomposisi skor menjadi grade membantu standarisasi evaluasi.
</details>

### Soal #80: Klasifikasi Buku Perpustakaan
Buku Teknologi Informasi kodenya 004, Komputer 005. Jika kamu mencari buku tentang Jaringan Komputer, kemungkinan kodenya adalah...
A. 006
B. 900
C. 500
D. 700

<details>
<summary>💡 Hint</summary>
Sistem Dewey Decimal membagi kategori berdasarkan kedekatan subjek (Pattern of Relationship).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 006 (Atau di sekitar itu).**
Topik yang berkaitan erat secara logis diletakkan di rak yang nomornya berurutan.
</details>

### Soal #81: Tata Letak Minimarket
Kenapa susu, roti, dan telur sering diletakkan di bagian paling belakang toko?
A. Agar tidak dicuri.
B. Agar pelanggan melewati lorong-lorong lain dan melihat barang lain sebelum sampai ke barang pokok.
C. Karena bagian belakang paling dingin.
D. Biar karyawannya rajin jalan kaki.

<details>
<summary>💡 Hint</summary>
Ini adalah pola psikologi belanja untuk meningkatkan penjualan impulsif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Agar pelanggan melihat barang lain.**
Dekomposisi rute perjalanan pembeli digunakan untuk optimasi keuntungan.
</details>

### Soal #82: Penomoran Kursi Bioskop
Baris G: G1, G3, G5 (Sisi Kiri), G2, G4, G6 (Sisi Kanan).
Jika tiketmu nomor G11, di manakah posisi dudukmu?
A. Sisi Kanan
B. Sisi Kiri
C. Tengah Jalan
D. Di depan layar

<details>
<summary>💡 Hint</summary>
Ganjil = Kiri. Genap = Kanan.
G11 adalah angka...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sisi Kiri.**
11 adalah angka ganjil, mengikuti pola penomoran sisi kiri bioskop.
</details>

### Soal #83: Grid Parkir Mall
Blok Parkir: A, B, C... setiap blok ada nomor 1-50.
Jika kamu parkir di B12, lalu berjalan ke kanan melihat B13, B14. Di manakah posisi B10?
A. Ke arah sebaliknya (Kiri)
B. Di lantai atas
C. Di mall sebelah
D. Di tempat parkir VIP

<details>
<summary>💡 Hint</summary>
Nomor urutan linear horizontal.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ke arah sebaliknya (Kiri).**
Pola numerik membantu navigasi spasial di area luas.
</details>

### Soal #84: Rute Bus Loop
Bus Rute 01: Terminal -> Pasar -> Sekolah -> RS -> Terminal.
Jika sekarang bus ada di Sekolah, ke manakah ia akan pergi selanjutnya?
A. Pasar
B. Rumah Sakit (RS)
C. Bengkel
D. Luar Kota

<details>
<summary>💡 Hint</summary>
Ikuti urutan list rutenya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rumah Sakit (RS).**
Pola loop berarti urutan tetap yang berputar secara sirkular.
</details>

### Soal #85: Pembukaan Pintu Kereta Commuter
Kereta memiliki stasiun pemberhentian. Papan digital menunjukkan: Stasiun A (Kiri), Stasiun B (Kanan), Stasiun C (Kanan), Stasiun D (Kiri).
Apa yang menentukan pola ini?
A. Warna keretanya.
B. Posisi peron stasiun terhadap rel.
C. Keinginan masinis.
D. Jumlah penumpang yang turun.

<details>
<summary>💡 Hint</summary>
Infrastruktur fisik memaksakan pola operasional.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Posisi peron stasiun.**
Dekomposisi operasional kereta harus mencocokkan pola pintu dengan pola peron.
</details>

### Soal #86: Gerbang Terminal Bandara
Terminal 1: Domestik, Terminal 2: Internasional, Terminal 3: Premium.
Jika kamu terbang dari Jakarta ke Singapura, terminal mana yang kamu tuju?
A. 1
B. 2
C. 3
D. Terminal Bus

<details>
<summary>💡 Hint</summary>
Singapura berada di luar negeri (Internasional).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2.**
Klasifikasi fungsional area membantu sirkulasi manusia di bandara masif.
</details>

### Soal #87: Ketinggian Pesawat
Pola: Takeoff (Naik), Cruising (Datar), Descent (Turun).
Jika kapten berkata "Kita akan mulai mendarat dalam 20 menit", pesawat masuk ke fase...
A. Takeoff
B. Cruising
C. Descent
D. Stalling

<details>
<summary>💡 Hint</summary>
Mendarat berarti turun ketinggian.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Descent.**
Mengenali pola gerak membantu penumpang mengantisipasi tekanan udara di telinga.
</details>

### Soal #88: Roket Bertahap (Multi-stage Rocket)
Roket besar membuang bagian bawahnya setelah bahan bakar habis agar beban berkurang. Polanya: Stage 1 lepas di 50km, Stage 2 di 150km.
Jika roket ada di ketinggian 20km, berapa stage yang masih menempel?
A. 0
B. 1
C. Semua (misal: 3)
D. Hanya ujungnya

<details>
<summary>💡 Hint</summary>
Lepas (lepas) hanya terjadi SETELAH mencapai batas tertentu.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Semua.**
Karena belum mencapai ambang batas pelepasan pertama (50km).
</details>

### Soal #89: Kecepatan Orbit Satelit
Pola: Makin dekat ke bumi, tarikan gravitasi makin kuat, sehingga satelit harus bergerak makin cepat agar tidak jatuh.
Satelit cuaca (rendah) VS Satelit TV (tinggi). Mana yang bergerak lebih cepat melintasi langit?
A. Satelit cuaca (LEO - Low Earth Orbit)
B. Satelit TV (GEO - Geostationary)
C. Keduanya sama kencang
D. Satelit TV bergerak mundur

<details>
<summary>💡 Hint</summary>
Pahami pola kebalikan (Invers): Jarak rendah $\rightarrow$ Kecepatan tinggi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Satelit Cuaca.**
Mengikuti pola fisika orbital untuk menjaga keseimbangan gaya sentrifugal.
</details>

### Soal #90: Simbol Prakiraan Cuaca
Ikon: Matahari (Cerah), Matahari + Awan (Berawan), Awan + Titik-titik (Hujan).
Jika kamu melihat pola grafis awan dengan garis-garis miring, apa artinya?
A. Hujan badai atau berangin.
B. Langit sangat bersih.
C. Akan turun salju cokelat.
D. Sinyal HP hilang.

<details>
<summary>💡 Hint</summary>
Pola visual garis miring melambangkan air yang tertiup angin.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hujan badai/berangin.**
Standardisasi pola grafis mempermudah komunikasi informasi cuaca secara global.
</details>

### Soal #91: Tren Pasar Saham (Bull vs Bear)
Grafik saham menunjukkan puncak-puncak yang semakin tinggi setiap hari (Higher High). Pola ini disebut...
A. Bearish (Pasar lesu/turun)
B. Bullish (Pasar naik/optimis)
C. Sideways (Datar)
D. Game Over

<details>
<summary>💡 Hint</summary>
Bayangkan banteng (Bull) yang menanduk ke atas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bullish.**
Mengenali pola tren harga sangat penting bagi algoritma trading keuangan.
</details>

### Soal #92: Pajak Berjenjang (Progresif)
Pola: Gaji < 5jt (Pajak 0%), 5-10jt (Pajak 5%), > 10jt (Pajak 10%).
Jika seseorang bergaji 8 juta, berapa persen pajaknya?
A. 0%
B. 5%
C. 10%
D. 15%

<details>
<summary>💡 Hint</summary>
Cek range pendapatannya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 5%.**
Pola progresif memastikan keadilan distribusi beban ekonomi.
</details>

### Soal #93: Bunga Majemuk (Compound Interest)
Tabungan: Tahun 0 (1jt), Tahun 1 (1.1jt), Tahun 2 (1.21jt).
Berapa saldo di tahun ke-3 jika diberikan bunga 10% dari saldo terakhir?
A. 1.31jt
B. 1.331jt
C. 1.4jt
D. 2jt

<details>
<summary>💡 Hint</summary>
$1.21 \text{jt} + (10\% \times 1.21 \text{jt})$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1.331jt.**
Pola pertumbuhan eksponensial di mana basis pertumbuhannya semakin besar setiap periode.
</details>

### Soal #94: Skor Kredit
Range skor: 300 (Buruk) sampai 850 (Sangat Bagus).
Bank biasanya memberikan pinjaman bunga rendah bagi pola skor di atas 750. Jika skormu 800, kamu masuk kategori...
A. Berisiko tinggi
B. Nasabah prioritas / Terpercaya
C. Blacklist
D. Mahasiswa baru

<details>
<summary>💡 Hint</summary>
Semakin tinggi nilai, semakin positif pola perilakunya di mata bank.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Nasabah prioritas.**
Skor adalah ringkasan pola historis transaksi keuangan seseorang.
</details>

### Soal #95: Kadaluarsa Kupon
Kupon belanja berlaku "7 hari setelah aktivasi". Aktivasi hari Senin jam 10.00.
Kapan kupon tersebut hangus?
A. Senin depan jam 09.59
B. Minggu depan jam 23.59
C. Senin depan jam 10.01
D. Besok pagi

<details>
<summary>💡 Hint</summary>
Gunakan pola 24 jam x 7 hari.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Senin depan jam 10.01.**
Tepat setelah waktu limit 7x24 jam habis.
</details>

### Soal #96: Membership Tiers
Level: Bronze (0 poin), Silver (1000), Gold (5000), Platinum (10.000).
Jika kamu punya 4.500 poin, level apa kamu saat ini?
A. Bronze
B. Silver
C. Gold
D. Platinum

<details>
<summary>💡 Hint</summary>
Kamu belum mencapai target untuk level Gold.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Silver.**
Kamu tetap di level terakhir yang syarat poinnya berhasil kamu lampaui.
</details>

### Soal #97: Game Leveling XP
XP yang dibutuhkan untuk naik level: Lvl 1->2 (100 XP), Lvl 2->3 (200 XP), Lvl 3->4 (400 XP).
Berapa XP yang dibutuhkan untuk level 4->5 jika pola ini adalah "Lipat Dua"?
A. 500 XP
B. 600 XP
C. 800 XP
D. 1.000 XP

<details>
<summary>💡 Hint</summary>
Lihat selisih pertumbuhannya: 100, 200, 400...
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 800 XP.**
Designer game menggunakan pola ini agar level tinggi terasa lebih menantang.
</details>

### Soal #98: Fase Bos dalam Video Game
Bos Naga: Darah 100-71% (Serang Api), 70-31% (Terbang), < 30% (Mengamuk/Rage).
Jika darah naga sudah di posisi 25%, strategi apa yang harus kamu siapkan?
A. Menunggu naga menyemburkan api saja.
B. Bersiap menghadapi serangan "Rage" yang sangat kuat dan cepat.
C. Menunggu naga terbang kembali.
D. Mematikan komputer.

<details>
<summary>💡 Hint</summary>
Cek range status darahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bersiap menghadapi "Rage".**
Game modern menggunakan dekomposisi perilaku musuh berdasarkan status variabel tertentu.
</details>

### Soal #99: Warna Rarity Item
Pola standar: Abu-abu (Sampah), Hijau (Biasa), Biru (Langka/Rare), Ungu (Sangat Langka/Epic), Oranye (Legendaris).
Jika kamu mendapat pedang bersinar warna Ungu, ia masuk kategori...
A. Senjata rusak
B. Sangat Langka / Epic
C. Biasa saja
D. Sampah

<details>
<summary>💡 Hint</summary>
Ikuti pola warna RPG internasional (seperti WoW atau Genshin).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sangat Langka / Epic.**
Pola warna mempermudah pemain mengenali nilai barang secara instan tanpa membaca deskripsi.
</details>

### Soal #100: Kabut Perang (Fog of War)
Dalam game strategi (RTS), area peta yang tidak ada unit/bangunanmu akan terlihat gelap. Jika kamu menggerakkan pasukan ke sana, kegelapan menghilang. Apa polanya?
A. Gelap = Tidak ada data visual (Unexplored). Terang = Ada data visual (Explored).
B. Musuh mematikan lampu di sana.
C. Hari sudah malam di bagian peta itu.
D. Monitor kamu sedang rusak di bagian tersebut.

<details>
<summary>💡 Hint</summary>
Pola ini mensimulasikan "kekurangan informasi" dalam peperangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Gelap = Tidak ada data visual.**
Dekomposisi visibilitas peta membantu kedalaman strategi permainan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Gelap = Tidak ada data visual.**
Dekomposisi visibilitas peta membantu kedalaman strategi permainan.
</details>

### Soal #101: Aturan Subgrid Sudoku
Dalam Sudoku 9x9, angka 1-9 tidak boleh berulang di baris, kolom, dan kotak 3x3 (subgrid).
Jika angka "5" sudah ada di posisi baris 1 kolom 1, di manakah angka "5" BOLEH diletakkan di baris 2?
A. Baris 2 Kolom 1
B. Baris 2 Kolom 2
C. Baris 2 Kolom 5
D. Baris 2 Kolom 3

<details>
<summary>💡 Hint</summary>
Baris 1, 2, dan 3 kolom 1, 2, dan 3 masuk dalam satu kotak 3x3 yang sama.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Baris 2 Kolom 5.**
Kolom 5 berada di subgrid yang berbeda dengan kolom 1, sehingga tidak melanggar aturan pengulangan subgrid.
</details>

### Soal #102: Pola Angka Minesweeper
Dalam game Minesweeper, kamu melihat angka "3" di sebuah kotak. Apa artinya berdasarkan pengenalan pola?
A. Ada 3 ranjau di seluruh area permainan.
B. Ada tepat 3 ranjau di 8 kotak di sekeliling angka tersebut.
C. Kamu punya 3 nyawa tersisa.
D. Kotak tersebut akan meledak dalam 3 detik.

<details>
<summary>💡 Hint</summary>
Angka adalah "sensor" pasif untuk deteksi pola ranjau di sekitarnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ada tepat 3 ranjau di sekelilingnya.**
Pola angka membantu pemain melakukan deduksi logika posisi ranjau.
</details>

### Soal #103: Pola Line Clear Tetris
Dalam Tetris, baris balok akan menghilang (cleared) jika...
A. Warnanya semua merah.
B. Baris tersebut terisi penuh secara horizontal tanpa ada lubang kosong.
C. Kamu menekan tombol Enter.
D. Balok mencapai langit-langit.

<details>
<summary>💡 Hint</summary>
Pola "Penuh" memicu aksi "Hapus".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terisi penuh secara horizontal.**
Dekomposisi tujuan game: Menyusun pola padat untuk mengurangi tumpukan.
</details>

### Soal #104: Perilaku Ghost Pac-Man
Hantu Merah (Blinky) selalu mengejar posisi koordinat Pac-Man secara langsung. Ini adalah contoh pola...
A. Pergerakan acak.
B. Pathfinding (Pencarian jalur) yang ditujukan ke target dinamis.
C. Hantu yang sedang tersesat.
D. Pola diam di tempat.

<details>
<summary>💡 Hint</summary>
Algoritma mengenali pola posisi target untuk menentukan arah gerak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pathfinding ke target dinamis.**
Mengenali pola gerak musuh memudahkan pemain menghindar.
</details>

### Soal #105: Pola Match-3 Candy Crush
Jika kamu menjajajarkan 4 permen dengan warna yang sama secara vertikal, apa yang terjadi?
A. Tidak terjadi apa-apa.
B. Terbentuk permen spesial (Striped Candy) yang bisa menghancurkan satu kolom.
C. Permainan langsung menang.
D. HP kamu akan bergetar selamanya.

<details>
<summary>💡 Hint</summary>
Jumlah (Count) dalam satu pola menentukan tingkat bonus.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terbentuk permen spesial.**
Pola $> 3$ memicu fungsi algoritma yang lebih kuat (Power-up).
</details>

### Soal #106: Pola Warna Wordle
Kamu menebak kata, dan huruf "A" berwarna Kuning. Apa artinya?
A. Huruf A tidak ada di kata tersebut.
B. Huruf A ada di kata tersebut tapi di posisi yang salah.
C. Huruf A ada di kata tersebut dan posisinya sudah benar.
D. Kamu harus membayar untuk melihat jawabannya.

<details>
<summary>💡 Hint</summary>
Hijau = Benar semua. Kuning = Ada tapi salah tempat. Abu-abu = Tidak ada.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ada tapi di posisi salah.**
Wordle menggunakan pola umpan balik visual untuk mengeliminasi kemungkinan kata.
</details>

### Soal #107: Gabungan Angka 2048
Dalam game 2048, jika kotak angka 8 bertabrakan dengan kotak angka 8, mereka akan menjadi...
A. 88
B. 0
C. 16
D. 2048

<details>
<summary>💡 Hint</summary>
Operasi matematikanya adalah Penjumlahan ($X + X$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 16.**
Pola pengulangan kelipatan dua ($2^n$) adalah inti dari game ini.
</details>

### Soal #108: Pola Pertumbuhan Snake
Dalam game Snake, setiap ular memakan "apel", tubuhnya bertambah panjang. Apa risiko dari pola pertumbuhan ini?
A. Ular makin cepat lari.
B. Snake makin sulit bermanuver karena ekornya bisa tertabrak kepalanya sendiri.
C. Snake akan berubah warna menjadi pelangi.
D. Apelnya akan habis.

<details>
<summary>💡 Hint</summary>
Dekomposisi: Ruang gerak tetap, panjang objek bertambah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Makin sulit bermanuver.**
Pola peningkatan kesulitan seiring kemajuan pemain.
</details>

### Soal #109: Langkah Kuda Catur (Knight)
Kuda berada di kotak Putih. Setelah melompat satu kali (pola L), ia pasti akan mendarat di kotak berwarna...
A. Putih
B. Hitam
C. Hijau
D. Transparan

<details>
<summary>💡 Hint</summary>
Pola L: 2 langkah lurus + 1 langkah samping. Cobalah di papan catur.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hitam.**
Secara matematis, pola gerak Kuda selalu mengubah warna pijakan dari warna saat ini.
</details>

### Soal #110: Kombinasi Kartu Poker
Mana yang memiliki pola lebih kuat/tinggi nilainya?
A. Three of a Kind (3 angka sama)
B. Full House (3 angka sama + 2 angka sama lain)
C. One Pair (2 angka sama)
D. High Card (Angka tertinggi acak)

<details>
<summary>💡 Hint</summary>
Makin kompleks polanya (makin sulit didapat), makin tinggi nilainya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Full House.**
Pola ini merupakan gabungan dari pola yang lebih sederhana, sehingga lebih sulit muncul secara statistik.
</details>

### Soal #111: Gunting Batu Kertas
Jika polanya adalah: Gunting mengalahkan Kertas, Kertas mengalahkan Batu. Maka Batu mengalahkan...
A. Semua
B. Gunting
C. Batu lagi
D. Tidak ada

<details>
<summary>💡 Hint</summary>
Ini adalah pola sirkular (lingkaran kekuatan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gunting.**
Pola relasi melingkar yang seimbang.
</details>

### Soal #112: Kondisi Menang Tic-Tac-Toe
Dalam papan 3x3, kamu menang jika membentuk pola 3 simbol yang sama secara...
A. Horizontal saja
B. Vertikal saja
C. Horizontal, Vertikal, atau Diagonal
D. Berjejer di pojok-pojok saja

<details>
<summary>💡 Hint</summary>
Ada 8 kemungkinan pola garis lurus untuk menang.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Horizontal, Vertikal, atau Diagonal.**
Pengenalan pola garis lurus adalah mekanisme utama deteksi kemenangan.
</details>

### Soal #113: Rule Tangan Kiri di Labirin
Jika kamu masuk ke labirin dan selalu meletakkan tangan kirimu di dinding tanpa pernah mengangkatnya, apa polanya?
A. Kamu akan pusing.
B. Kamu dijamin akan menemukan jalan keluar (meskipun butuh waktu lama).
C. Kamu akan tersesat selamanya.
D. Tanganmu akan kotor.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma Wall-follower untuk navigasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Akan menemukan jalan keluar.**
Pola penelusuran batas ini efektif untuk labirin yang terhubung secara topologi satu blok.
</details>

### Soal #114: Tower of Hanoi
Aturan: Piringan besar tidak boleh di atas piringan kecil.
Jika ada Piringan 1 (Kecil), 2 (Sedang), dan 3 (Besar). Di manakah posisi Piringan 2 yang BENAR?
A. Di bawah Piringan 3
B. Di atas Piringan 1
C. Di antara Piringan 3 (bawah) dan Piringan 1 (atas)
D. Di mana saja sesuka hati

<details>
<summary>💡 Hint</summary>
Ikuti pola urutan: Besar -> Kecil (dari bawah ke atas).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Di antara 3 (bawah) dan 1 (atas).**
Pola tumpukan mengecil ke atas adalah aturan tetap game ini.
</details>

### Soal #115: Pusat Rubik's Cube
Setelah diputar-putar sejauh apapun, kotak di bagian paling tengah setiap sisi Rubik tidak akan pernah berpindah tempat relatif terhadap pusat lainnya. Mengapa?
A. Karena dilem.
B. Karena secara mekanis pusat adalah poros tetap yang menentukan pola warna sisi tersebut.
C. Karena pusat adalah kotak gaib.
D. Pusat sebenarnya bergerak tapi kita tidak sadar.

<details>
<summary>💡 Hint</summary>
Warna sisi Rubik ditentukan oleh warna kotak pusatnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pusat adalah poros tetap.**
Strategi penyelesaian Rubik dimulai dengan mengenali pusat sebagai pola acuan.
</details>

### Soal #116: Pola Lipat Kertas (Origami)
Jika kamu melipat kertas menjadi dua, lalu menggunting bentuk segitiga di lipatannya, saat dibuka akan muncul dua segitiga yang...
A. Berjauhan
B. Berhimpitan membentuk pola cermin (Simetris)
C. Berubah menjadi kotak
D. Menghilang

<details>
<summary>💡 Hint</summary>
Lipatan bertindak sebagai sumbu simetri.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berhimpitan pola cermin.**
Pengenalan pola simetri sangat penting dalam geometri dan desain.
</details>

### Soal #117: Pola Merajut (Knitting)
Pola rajutan tertulis: K1, P1, K1, P1. (K=Knit, P=Purl).
Setelah P1 terakhir, apa langkah selanjutnya?
A. K2
B. P1
C. K1
D. Berhenti

<details>
<summary>💡 Hint</summary>
Lihat pola pengulangannya ($A-B-A-B-...$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. K1.**
Rajutan adalah pengulangan pola simpul yang sangat konsisten.
</details>

### Soal #118: Pola Tenun (Weaving)
Benang Lusi (tegak) dan Pakan (mendatar) disilangkan: Atas, Bawah, Atas, Bawah.
Apa fungsi dari pola selang-seling ini?
A. Agar kain terlihat berwarna-warni.
B. Agar benang saling mengunci dan membentuk lembaran kain yang kuat.
C. Biar prosesnya lama.
D. Agar kainnya bolong-bolong.

<details>
<summary>💡 Hint</summary>
Interlocking (Saling mengunci) adalah tujuan dari pola struktur kain.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Benang saling mengunci.**
Kekuatan kain berasal dari pengulangan pola fisik yang teratur.
</details>

### Soal #119: Pola Ubin (Tessellation)
Bentuk manakah yang bisa menutupi seluruh lantai tanpa ada celah sedikitpun?
A. Lingkaran
B. Segi Lima (Pentagon) Beraturan
C. Kotak (Persegi) atau Segi Enam (Hexagon)
D. Bintang

<details>
<summary>💡 Hint</summary>
Tessellation adalah pola pengulangan bentuk yang pas dipasangkan tanpa sisa ruang.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kotak atau Segi Enam.**
Pola ini ditemukan di ubin rumah dan juga sarang lebah.
</details>

### Soal #120: Geometri Syamil (Islamic Art)
Sering kita temukan pola bintang 8 atau 12 yang sangat rumit di masjid. Pola ini dibangun dari...
A. Gambar tangan bebas tanpa penggaris.
B. Pengulangan bentuk dasar lingkaran dan kotak yang saling tumpang tindih secara simetris.
C. Stiker yang dibeli di pasar.
D. Foto pemandangan alam.

<details>
<summary>💡 Hint</summary>
Keindahan matematika berasal dari keteraturan pola dasar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengulangan bentuk dasar secara simetris.**
Ini adalah dekomposisi seni menjadi rumus geometri.
</details>

### Soal #121: Deret Fibonacci di Alam
Pola jumlah kelopak bunga seringkali: 3, 5, 8, 13, 21.
Apa angka selanjutnya dalam pola ini?
A. 25
B. 34
C. 40
D. 50

<details>
<summary>💡 Hint</summary>
Angka berikutnya adalah jumlah dari dua angka sebelumnya.
$8+13=21$, $13+21=...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 34.**
Pola Fibonacci ditemukan secara luas di alam, dari kelopak bunga hingga susunan biji bunga matahari.
</details>

### Soal #122: Golden Ratio (Rasio Emas)
Banyak seniman menggunakan rasio 1.618 untuk membuat karya yang terlihat proporsional dan mata manusia menganggapnya "Indah". Ini adalah contoh...
A. Kebetulan semata.
B. Pola estetika berbasis matematika.
C. Aturan paksa dari pemerintah.
D. Keajaiban dunia.

<details>
<summary>💡 Hint</summary>
Otak manusia mengenali pola proporsi tertentu sebagai kenyamanan visual.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola estetika berbasis matematika.**
Banyak logo perusahaan terkenal (seperti Apple atau Google) menggunakan pola rasio ini.
</details>

### Soal #123: Segitiga Sierpinski
Sebuah segitiga besar dibagi 4, bagian tengahnya dibuang. Lalu segitiga sisa dibagi lagi dengan pola yang sama terus menerus sampai tak terhingga. Bentuk ini disebut...
A. Lingkaran
B. Kotak Ajaib
C. Fraktal
D. Garis Lurus

<details>
<summary>💡 Hint</summary>
Fraktal adalah pola yang mirip dengan dirinya sendiri meskipun diperbesar/diperkecil.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Fraktal.**
Fraktal adalah dekomposisi geometri yang berulang secara rekursif (berulang ke diri sendiri).
</details>

### Soal #124: Keserupaan Diri (Self-similarity)
Kamu melihat kembang kol (Brokoli Roma). Jika kamu memotong satu bagian kecil, bentuknya terlihat persis seperti kembang kol yang besar. Pola ini disebut...
A. Fotokopi alam.
B. Self-similarity (Keserupaan diri).
C. Kerusakan pertumbuhan.
D. Penipuan mata.

<details>
<summary>💡 Hint</summary>
Bagian kecil mencerminkan pola keseluruhan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Self-similarity.**
Pola fraktal di alam membantu tumbuhan tumbuh efisien dengan instruksi genetik yang sederhana tapi diulang.
</details>

### Soal #125: Kristal Salju (Snowflake)
Semua kristal salju memiliki pola dasar simetri berapa arah?
A. 4 (Kotak)
B. 5 (Bintang)
C. 6 (Hexagonal)
D. 8 (Octagonal)

<details>
<summary>💡 Hint</summary>
Molekul air ($H_2O$) membeku membentuk kristal es dengan sudut $60^\circ$ atau $120^\circ$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 6 (Hexagonal).**
Pola molekuler menentukan bentuk visual makroskopisnya.
</details>

### Soal #126: Pola Sarang Lebah
Lebah madu membuat ruangan berbentuk Hexagon (segi enam), bukan lingkaran atau kotak. Apa alasannya secara fungsional?
A. Agar terlihat modern.
B. Bentuk hexagon memungkinkan ruangan paling luas dengan penggunaan lilin (bahan bangunan) paling sedikit dan tanpa celah.
C. Karena lebah hanya bisa berhitung sampai angka 6.
D. Karena ratu lebah suka bentuk segi enam.

<details>
<summary>💡 Hint</summary>
Efisiensi penggunaan lahan dan material.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Paling luas dengan material paling sedikit.**
Ini adalah pola optimasi geometri di alam.
</details>

### Soal #127: Bentuk Gelembung Sabun
Satu gelembung sabun selalu berbentuk bola. Ini terjadi karena pola tegangan permukaan yang...
A. Ingin meledak.
B. Menarik ke arah pusat untuk menciptakan luas permukaan paling minimal.
C. Mengikuti arah tiupan angin.
D. Suka pada bentuk bulat.

<details>
<summary>💡 Hint</summary>
Alam selalu mencari pola energi terendah atau bentuk paling stabil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan luas permukaan paling minimal.**
Matematika di balik gelembung sabun digunakan ilmuwan untuk mempelajari pola struktur minimal.
</details>

### Soal #128: Pola Lingkaran Pohon
Lingkaran tahun pohon: Terang (Musim Hujan/Tumbuh Cepat), Gelap (Musim Kemarau/Tumbuh Lambat).
Jika dalam potongan kayu ada 20 garis gelap, berapa umur pohon tersebut?
A. 5 tahun
B. 10 tahun
C. 20 tahun
D. 40 tahun

<details>
<summary>💡 Hint</summary>
Satu pasang (Terang+Gelap) biasanya mewakili siklus satu tahun.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 20 tahun.**
Membaca pola lingkaran pohon (Dendrokronologi) membantu ilmuwan mengetahui sejarah iklim masa lalu.
</details>

### Soal #129: Jejak Semut
Semut berjalan beriringan mengikuti satu jalur yang sama. Pengenalan pola apa yang mereka gunakan?
A. Mereka menghafal setiap batu di jalan.
B. Mereka mengikuti jejak bahan kimia (Feromon) yang ditinggalkan semut sebelumnya.
C. Mereka saling berpegangan tangan.
D. Semut paling depan membawa bendera penunjuk arah.

<details>
<summary>💡 Hint</summary>
Ini adalah pola komunikasi berbasis jejak kimiawi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengikuti jejak feromon.**
Algoritma semut (Ant Colony Optimization) digunakan dalam ilmu komputer untuk mencari rute terpendek.
</details>

### Soal #130: Tarian Lebah (Waggle Dance)
Lebah yang menemukan bunga akan menari di depan lebah lain. Kecepatan getaran dan sudut tarian adalah pola untuk memberitahu...
A. Bahwa ia sedang senang.
B. Jarak dan arah lokasi sumber makanan terhadap posisi matahari.
C. Bahwa ada predator mendekat.
D. Nama bunga yang ditemukan.

<details>
<summary>💡 Hint</summary>
Tarian adalah dekomposisi data peta menjadi pola gerak tubuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jarak dan arah lokasi makanan.**
Bahasa pola hewan seringkali sangat akurat dan saintifik.
</details>

### Soal #131: Geometri Jaring Laba-laba
Jaring laba-laba memiliki pola radial (seperti jari-jari roda) dan spiral (melingkar). Fungsi pola spiral perekat adalah untuk...
A. Menghias jaring agar cantik.
B. Menangkap dan menahan serangga agar tidak bisa lepas.
C. Tempat laba-laba tidur siang.
D. Sebagai tangga darurat.

<details>
<summary>💡 Hint</summary>
Setiap bagian jaring punya peran (dekomposisi fungsi). Radial untuk struktur, Spiral untuk perangkap.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menangkap dan menahan serangga.**
Laba-laba adalah insinyur pola alami yang sangat hebat.
</details>

### Soal #132: Perubahan Warna Bunglon
Bunglon berubah warna bukan untuk menyamar saja, tapi juga sebagai pola ekspresi...
A. Lapar atau Haus.
B. Mood (Emosi) dan pengaturan suhu tubuh.
C. Ingin menari.
D. Penuaan usia.

<details>
<summary>💡 Hint</summary>
Warna adalah output visual dari kondisi internal (pola emosi/fisik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mood dan Suhu.**
Pola warna kulit bunglon adalah indikator status biologisnya.
</details>

### Soal #133: Kunang-kunang yang Kompak
Di beberapa tempat, ribuan kunang-kunang bisa berkedip secara bersamaan (Synchronized). Apa polanya?
A. Ada pemimpin yang memberi aba-aba.
B. Setiap individu menyesuaikan ritme kedipnya sedikit demi sedikit dengan tetangga di sebelahnya sampai frekuensinya sama.
C. Mereka menggunakan jam tangan yang sama.
D. Efek pantulan cermin saja.

<details>
<summary>💡 Hint</summary>
Ini adalah contoh "Emergence" - pola besar yang muncul dari aturan sederhana di setiap individu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan ritme dengan tetangga.**
Pola siklus kedip saling mempengaruhi hingga terjadi harmonisasi masal.
</details>

### Soal #134: Gerombolan Ikan (Schooling)
Ikan berenang bersama dalam pola rapat yang selalu berubah bentuk. Mengapa predator sulit menangkapnya?
A. Karena ikan-ikannya berteriak.
B. Pola gerakan ribuan ikan membuat predator bingung menentukan target tunggal (Efek sensorik overload).
C. Karena airnya menjadi keruh.
D. Karena ikan menjadi sangat besar.

<details>
<summary>💡 Hint</summary>
Banyaknya pola gerak yang pecah membingungkan algoritma visual predator.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Predator bingung menentukan target.**
Pola pertahanan kolektif sangat efektif di dunia hewan.
</details>

### Soal #135: Gerumbul Hewan (Herd)
Saat ada singa, kawanan zebra lari bersamaan. Jika satu zebra belok kiri, yang lain ikut belok kiri. Apa aturannya?
A. Zebra mematuhi rambu lalu lintas.
B. Aturan sederhana: Tetap dekat dengan teman disebelahmu dan jangan menabrak.
C. Mereka sudah janjian di WhatsApp.
D. Zebra paling depan adalah jenderal perang.

<details>
<summary>💡 Hint</summary>
Pola kolektif muncul dari interaksi lokal antar individu (Flocking Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tetap dekat dan jangan menabrak.**
Tiga aturan (Separation, Alignment, Cohesion) menciptakan pola "Herd" yang kompleks.
</details>

### Soal #136: Gelombang Macet (Phantom Traffic Jam)
Terkadang jalanan macet total, tapi saat sudah jalan, tidak ada kecelakaan atau perbaikan jalan. Mengapa?
A. Ada hantu yang menghalangi jalan.
B. Karena satu mobil ngerem mendadak, menyebabkan pola reaksi berantai pengereman yang merambat ke belakang lebih lambat.
C. Jalanannya sedang lelah.
D. Polisi sengaja menutup jalan diam-diam.

<details>
<summary>💡 Hint</summary>
Ini adalah pola gelombang kejut (Shockwave) dalam aliran partikel.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Reaksi berantai pengereman.**
Pola ini bisa dijelaskan dengan matematika dinamika fluida.
</details>

### Soal #137: Peta MRT/LRT (Topologis)
Garis rute di peta MRT seringkali lurus sempurna atau sudut $45^\circ$, meskipun jalan aslinya berkelok-kelok. Mengapa?
A. Agar hemat tinta print.
B. Karena bagi penumpang, pola koneksi antar stasiun lebih penting daripada lokasi geografis yang akurat.
C. Pembuat petanya malas menggambar tikungan.
D. Supaya keretanya terlihat cepat.

<details>
<summary>💡 Hint</summary>
Penyederhanaan informasi (Abstraksi) dilakukan untuk menonjolkan pola relasi/konektivitas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola koneksi lebih penting.**
Pola ini mempermudah pengguna merencanakan perjalanan tanpa bingung oleh detail jalan raya di atasnya.
</details>

### Soal #138: Persimpangan Bundaran (Roundabout)
Di bundaran, kendaraan yang sudah di dalam lingkaran punya prioritas jalan. Apa tujuannya?
A. Biar mobilnya terus berputar.
B. Menciptakan pola aliran yang kontinu tanpa perlu lampu merah (menghindari kemacetan statis).
C. Biar sopirnya pusing.
D. Sebagai tempat pajangan patung di tengah.

<details>
<summary>💡 Hint</summary>
Dekomposisi tujuan: Menjaga arus tetap mengalir (Flow).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan pola aliran kontinu.**
Bundaran lebih efisien daripada lampu merah untuk volume kendaraan sedang.
</details>

### Soal #139: Sambungan Jembatan
Di jembatan beton panjang, ada celah bergerigi di setiap beberapa puluh meter. Apa polanya?
A. Celah itu adalah kesalahan konstruksi.
B. Pola celah ekspansi agar jembatan bisa memuai saat panas dan menyusut saat dingin tanpa retak.
C. Agar ban mobil berbunyi "dug-dug".
D. Tempat membuang sampah.

<details>
<summary>💡 Hint</summary>
Pola fisik menyesuaikan dengan perilaku material terhadap perubahan suhu (Pattern of Expansion).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Celah ekspansi untuk pemuaian.**
Insinyur mengenali pola fisika zat padat untuk keamanan infrastruktur.
</details>

### Soal #140: Spillway Waduk
Waduk memiliki saluran pelimpah (spillway). Jika ketinggian air melebihi pola batas tertentu, air akan tumpah otomatis. Apa fungsinya?
A. Biar airnya terlihat seperti air terjun.
B. Mencegah air meluap melewati puncak bendungan yang bisa merusak struktur.
C. Membuang ikan yang terlalu banyak.
D. Memberi air pada sawah di bawah secara gratis.

<details>
<summary>💡 Hint</summary>
Threshold (Ambang batas) adalah mekanisme kontrol berbasis pola data (ketinggian).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah kerusakan struktur.**
Sistem pengamanan waduk bekerja berdasarkan pola level air yang terdeteksi.
</details>

### Soal #141: Pitch Kincir Angin
Sudut kemiringan bilah kincir angin berubah mengikuti kecepatan angin. Mengapa?
A. Agar kincirnya terlihat menari.
B. Menyesuaikan pola aliran udara agar energi yang ditangkap tetap maksimal tapi tidak merusak turbin (Pitch Control).
C. Karena bilahnya lembek tertiup angin.
D. Biar burung-burung takut mendekat.

<details>
<summary>💡 Hint</summary>
Optimalisasi variabel Input (angin) menjadi Output (listrik) melalui penyesuaian pola fisik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan pola aliran udara.**
Teknologi ini menggunakan sensor pola kecepatan angin untuk optimasi daya.
</details>

### Soal #142: Panel Surya Pelacak (Sun Tracking)
Panel surya yang bisa bergerak mengikuti arah matahari sepanjang hari menghasilkan listrik lebih banyak. Pola geraknya adalah...
A. Bergerak acak mencari sinar paling terang.
B. Mengikuti pola busur matahari dari Timur ke Barat berdasarkan waktu.
C. Diam saja tapi lensanya yang berputar.
D. Berputar cepat seperti baling-baling.

<details>
<summary>💡 Hint</summary>
Matahari memiliki pola harian yang sangat terprediksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengikuti pola busur matahari.**
Mengenali pola gerak semu matahari memungkinkan efisiensi energi yang tinggi.
</details>

### Soal #143: Termostat Cerdas
AC inverter baru menurunkan daya listriknya saat suhu ruangan sudah mendekati target. Apa polanya?
A. Pola pendinginan bertahap (Feedback Loop).
B. AC akan mati mendadak lalu nyala lagi.
C. AC meniupkan es batu.
D. Suhu ruangan akan terus turun sampai menjadi beku.

<details>
<summary>💡 Hint</summary>
Algoritma menyesuaikan Output berdasarkan selisih antara Status Saat Ini dan Target.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pola pendinginan bertahap.**
Sistem hemat energi mengenali pola suhu untuk mengatur beban kerja kompresor.
</details>

### Soal #144: Siklus Defrost Kulkas
Tersedia pemanas kecil di kulkas yang nyala setiap 8 jam selama 15 menit. Mengapa?
A. Biar makanan di dalam hangat sebentar.
B. Mencairkan pola penumpukan bunga es di evaporator agar sirkulasi udara tetap lancar.
C. Untuk menguji daya tahan lampu kulkas.
D. Biar tagihan listriknya mahal.

<details>
<summary>💡 Hint</summary>
Pola perawatan berkala secara otomatis (Maintenance Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencairkan penumpukan bunga es.**
Tanpa pola siklus ini, kulkas lama-lama tidak akan dingin karena tertutup es.
</details>

### Soal #145: Fase Mesin Cuci
Urutan: Timbang Baju -> Isi Air -> Cuci -> Bilas -> Peras.
Jika kamu melihat mesin cuci sedang berputar sangat kencang dan mengeluarkan banyak suara getaran, ia sedang berada di fase...
A. Isi Air
B. Cuci
C. Bilas
D. Peras (Spin)

<details>
<summary>💡 Hint</summary>
Putaran kencang (High Speed) diperlukan untuk membuang air dari serat kain dengan gaya sentrifugal.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Peras (Spin).**
Mengenali pola aktivitas mesin membantu kita memantau proses kerja alat rumah tangga.
</details>

### Soal #146: Power Level Microwave
Microwave "Low Power" sebenarnya tidak mengecilkan kekuatan gelombang mikronya, tapi menyalakannya secara bergantian (Contoh: 5 detik nyala, 10 detik mati). Apa sebutan pola ini?
A. Pola Rusak.
B. Duty Cycle (Siklus Kerja).
C. Pola Hemat Baterai.
D. Pola Berkedip.

<details>
<summary>💡 Hint</summary>
Rata-rata energi yang dihasilkan dalam satu periode waktu (Dekomposisi waktu).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Duty Cycle.**
Pola INTERVENSI waktu digunakan untuk mengontrol intensitas energi.
</details>

### Soal #147: Pengereman Regeneratif Mobil Listrik
Saat mobil listrik mengerem, motor berubah menjadi generator dan mengisi baterai. Apa polanya?
A. Mengubah pola energi kinetik (gerak) menjadi energi listrik.
B. Mobil akan meledak jika sering dibalas ngerem.
C. Remnya menggunakan magnet kulkas.
D. Ban mobil akan berputar terbalik.

<details>
<summary>💡 Hint</summary>
Konversi energi secara efisien dengan mengenali pola penggunaan (saat melambat).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mengubah pola energi kinetik jadi listrik.**
Dekomposisi pengereman tidak hanya untuk berhenti, tapi juga untuk recovery energi.
</details>

### Soal #148: Logika Lift
Jika kamu di lantai 5 memanggil lift ke bawah, dan lift sedang di lantai 8 sedang turun melewati lantai 6. Apa yang dilakukan lift?
A. Terus ke lantai 1 lalu naik lagi ke lantai 5.
B. Berhenti di lantai 5 untuk menjemputmu karena searah dengan tujuannya.
C. Melewati Anda begitu saja karena dia sombong.
D. Menunggu di lantai 8 sampai kamu memanggil lagi.

<details>
<summary>💡 Hint</summary>
Algoritma lift dirancang untuk rute paling efisien sesuai pola permintaan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berhenti di lantai 5.**
Pola "Pick up on the way" meminimalkan waktu tunggu dan konsumsi energi.
</details>

### Soal #149: Sensor Eskalator
Eskalator di mall yang sepi bergerak sangat lambat atau berhenti, lalu melaju normal saat ada orang mendekat. Sensor apa yang bekerja?
A. Sensor Berat
B. Sensor Gerak atau Inframerah
C. Sensor Suara langkah kaki
D. Sensor Kehadiran Mall

<details>
<summary>💡 Hint</summary>
Mengenali pola kehadiran manusia di area pintu masuk eskalator.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor Gerak/Inframerah.**
Dekomposisi operasional: Jika tidak ada input (orang), kurangi output (kecepatan) untuk hemat energi.
</details>

### Soal #150: Pintu Otomatis Supermarket
Mengapa pintu otomatis tidak terbuka saat ada kucing lewat tetapi terbuka saat manusia lewat?
A. Pintunya takut pada kucing.
B. Sensor disetel untuk mengenali pola objek dengan ketinggian dan ukuran tertentu (Thresholding).
C. Kucing jalannya terlalu pelan.
D. Karena kucing tidak bawa uang belanja.

<details>
<summary>💡 Hint</summary>
Filter pola digunakan untuk menghindari "false alarm" atau pembukaan pintu yang tidak perlu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengenali pola ukuran objek.**
Sistem sensor modern melakukan pemilahan pola untuk efisiensi dan keamanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengenali pola ukuran objek.**
Sistem sensor modern melakukan pemilahan pola untuk efisiensi dan keamanan.
</details>

### Soal #151: Pola Deret Geometri (Perkalian)
Perhatikan deret: 3, 9, 27, 81, ...
Berapa angka selanjutnya?
A. 100
B. 162
C. 243
D. 300

<details>
<summary>💡 Hint</summary>
Polanya adalah dikali 3 ($X \times 3$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 243.**
$81 \times 3 = 243$. Deret geometri adalah pola pertumbuhan yang sangat cepat.
</details>

### Soal #152: Pola Bilangan Kuadrat
Urutan: 1, 4, 9, 16, 25, ...
Angka ke-10 dalam pola ini adalah?
A. 50
B. 81
C. 100
D. 121

<details>
<summary>💡 Hint</summary>
Polanya adalah $n \times n$ (Bilangan dipangkatkan dua).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 100.**
$10^2 = 100$. Mengenali pola pangkat membantu dalam optimasi algoritma.
</details>

### Soal #153: Pola Bilangan Segitiga
Urutan: 1, 3, 6, 10, 15, ...
Berapa angka ke-6?
A. 20
B. 21
C. 25
D. 30

<details>
<summary>💡 Hint</summary>
Selisih antar angka bertambah: $+2, +3, +4, +5, ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 21.**
$15 + 6 = 21$. Pola ini membentuk tumpukan segitiga (seperti susunan bola biliar).
</details>

### Soal #154: Puzzle Logika 2x2
Dalam grid 2x2, setiap baris dan kolom harus berisi angka 1 dan 2.
Atas Kiri: 1. Bawah Kanan: 1.
Apa isi kotak Atas Kanan?
A. 1
B. 2
C. 0
D. Tidak bisa ditentukan

<details>
<summary>💡 Hint</summary>
Cek aturan baris: Jika Atas Kiri sudah 1, maka Atas Kanan harus...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2.**
Agar tidak ada pengulangan di baris pertama.
</details>

### Soal #155: Si Pembohong vs Si Jujur
A berkata: "B adalah pembohong".
B berkata: "Saya adalah pembohong".
Berdasarkan pola logika, siapa yang pasti berbohong?
A. A
B. B
C. Keduanya
D. Tidak ada (Paradoks)

<details>
<summary>💡 Hint</summary>
Orang jujur TIDAK AKAN PERNAH mengaku sebagai pembohong.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
Jika B jujur, dia tidak akan bilang dia pembohong. Jika B bohong, maka kalimatnya "Saya pembohong" adalah bohong (artinya dia sebenarnya jujur?), ini adalah pola paradoks klasik dalam logika.
</details>

### Soal #156: Pola Tempat Duduk
A tidak mau duduk di sebelah B. C duduk di antara A dan D.
Urutan duduk yang benar dari kiri ke kanan adalah...
A. A - B - C - D
B. A - C - D - B
C. B - A - C - D
D. D - B - A - C

<details>
<summary>💡 Hint</summary>
A dan B tidak boleh berdekatan. C harus dijepit A dan D.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. A - C - D - B.**
A-C-D terpenuhi, dan A tidak bersebelahan dengan B (terpisah oleh C dan D).
</details>

### Soal #157: Pola Timbangan
3 bola identik, 1 di antaranya lebih berat. Kamu hanya boleh menimbang 1 kali dengan timbangan dua lengan.
Bagaimana caranya?
A. Timbang bola 1 dan 2. Jika seimbang, bola 3 yang berat. Jika miring, bola yang turun yang berat.
B. Timbang semua sekaligus.
C. Lempar bolanya ke atas.
D. Tidak mungkin dilakukan.

<details>
<summary>💡 Hint</summary>
Gunakan pola eliminasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Timbang 1 dan 2.**
Dekomposisi kasus: Seimbang vs Tidak Seimbang. Satu timbangan cukup untuk 3 objek.
</details>

### Soal #158: Pola Tahun Kabisat
Tahun Kabisat terjadi setiap 4 tahun sekali (kecuali kelipatan 100 yang bukan kelipatan 400).
Manakah yang merupakan tahun kabisat?
A. 2022
B. 2023
C. 2024
D. 2025

<details>
<summary>💡 Hint</summary>
Angka tahunnya harus habis dibagi 4.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 2024.**
$2024 \div 4 = 506$ (Tanpa sisa).
</details>

### Soal #159: Pola Hari (Modulo 7)
Jika hari ini adalah Senin, hari apakah 100 hari lagi?
A. Selasa
B. Rabu
C. Kamis
D. Jumat

<details>
<summary>💡 Hint</summary>
$100 \div 7 = 14$ sisa $2$. Hitung 2 hari setelah Senin.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rabu.**
Sisa (Remainder) adalah kunci dalam pola berulang mingguan.
</details>

### Soal #160: Konversi Waktu 24 Jam
Jam 20:00 dalam pola 12 jam (AM/PM) adalah...
A. 8 AM
B. 10 AM
C. 8 PM
D. 10 PM

<details>
<summary>💡 Hint</summary>
$20 - 12 = 8$. Jika $> 12$ maka itu PM.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 8 PM.**
Mengenali pola transformasi data antar sistem format yang berbeda.
</details>

### Soal #161: Kriptografi Terbalik
Pesan asli: `HALO`. Pesan rahasia: `OLAH`.
Apa pesan rahasia untuk kata `DUNIA`?
A. `IDUNA`
B. `AINUD`
C. `DUNIA`
D. `ANDUI`

<details>
<summary>💡 Hint</summary>
Polanya adalah membalik urutan karakter (Reverse).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. AINUD.**
D-U-N-I-A dibalik menjadi A-I-N-U-D.
</details>

### Soal #162: Sandi Angka Vokal
Pola: A=1, E=2, I=3, O=4, U=5. Konsonan tetap.
Apa kode untuk kata `BUKU`?
A. `B5K5`
B. `B1K3`
C. `B2K4`
D. `5K5B`

<details>
<summary>💡 Hint</summary>
U diganti dengan 5.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. B5K5.**
Dekomposisi kata: B (konsonan), U (5), K (konsonan), U (5).
</details>

### Soal #163: Sandi Geser (ROT13)
Pola geser 13 langkah: A jadi N, B jadi O. Jika kamu menggeser lagi 13 langkah setelahnya, apa yang terjadi?
A. Hurufnya jadi hilang.
B. Huruf kembali ke asalnya (A jadi A lagi).
C. Huruf melompat ke angka.
D. Huruf menjadi simbol.

<details>
<summary>💡 Hint</summary>
Total alfabet ada 26 huruf. $13 + 13 = 26$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kembali ke asal.**
Pola putaran penuh (Cycle) dalam kriptografi simetris sederhana.
</details>

### Soal #164: Pola Putar Gambar (Rotasi)
Sebuah tanda panah menunjuk ke ATAS. Diputar $90^\circ$ searah jarum jam sebanyak 3 kali. Menunjuk ke mana panah sekarang?
A. Kiri
B. Kanan
C. Bawah
D. Atas

<details>
<summary>💡 Hint</summary>
1 kali: Kanan. 2 kali: Bawah. 3 kali: ...
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kiri.**
Rotasi berkelanjutan adalah pola spasial yang sering muncul di tes logika.
</details>

### Soal #165: Transparansi Bertumpuk
Gambar 1: Garis Horizontal. Gambar 2: Garis Vertikal.
Jika keduanya ditumpuk (Overlaid), pola apa yang terbentuk?
A. Garis Diagonal
B. Kotak-kotak (Grid)
C. Huruf X
D. Hitam polos

<details>
<summary>💡 Hint</summary>
Bayangkan kertas transparan yang digabung.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kotak-kotak (Grid).**
Irisan antar dua pola melahirkan pola baru yang lebih kompleks.
</details>

### Soal #166: Pola Titik Potong
2 garis lurus yang tidak sejajar pasti berpotongan di berapa titik?
A. 0
B. 1
C. 2
D. Tak terhingga

<details>
<summary>💡 Hint</summary>
Garis lurus hanya bisa bertemu di satu lokasi kecuali mereka berhimpit.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1.**
Konsep dasar geometri tentang pola hubungan antar garis.
</details>

### Soal #167: Palindrome
Kata yang dibaca dari depan dan belakang sama. Manakah yang merupakan Palindrome?
A. KATAK
B. MAKAN
C. TIDUR
D. LARI

<details>
<summary>💡 Hint</summary>
K-A-T-A-K dibalik tetap K-A-T-A-K.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. KATAK.**
Pengenalan pola teks simetris sangat berguna dalam analisis urutan DNA.
</details>

### Soal #168: Anagram
Mengubah susunan huruf kata "RAK" menjadi "KAR".
Manakah yang merupakan anagram dari kata "IKAN"?
A. KAIN
B. AKAN
C. INAP
D. KAKI

<details>
<summary>💡 Hint</summary>
Huruf-hurufnya harus persis sama jumlah dan jenisnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. KAIN.**
I-K-A-N dan K-A-I-N memiliki set huruf yang identik.
</details>

### Soal #169: Prefix dan Suffix
Kata Dasar: "Baca". Imbuhan: "Mem-", "-kan". Kata bentukan: "Membacakan".
Bagian "Mem-" dalam pengenalan pola bahasa disebut sebagai...
A. Suffix (Akhiran)
B. Prefix (Awalan)
C. Infix (Sisipan)
D. Root (Akar)

<details>
<summary>💡 Hint</summary>
Letaknya ada di depan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Prefix.**
Mengenali pola imbuhan membantu kita memahami arti kata-kata kompleks.
</details>

### Soal #170: Nilai Tengah (Median)
Data: 3, 1, 4, 1, 5.
Untuk mencari Median, langkah pertama adalah mengurutkan data. Urutan yang benar adalah...
A. 1, 1, 3, 4, 5
B. 5, 4, 3, 1, 1
C. Keduanya benar
D. Tidak perlu diurutkan

<details>
<summary>💡 Hint</summary>
Pola statistik membutuhkan keteraturan data (Sorting).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Keduanya benar.**
Bisa dari terkecil atau terbesar, yang penting ada di tengah urutan. Median adalah 3.
</details>

### Soal #171: Pola Pencilan (Outlier)
Data nilai ujian kelas: 80, 85, 82, 10, 88.
Berapa nilai yang merupakan "Pencilan" (berbeda jauh dari pola kelompok)?
A. 80
B. 10
C. 88
D. Tidak ada

<details>
<summary>💡 Hint</summary>
Mana angka yang "aneh" sendirian?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10.**
Mengenali outlier membantu kita mendeteksi kesalahan input atau kasus spesial dalam data.
</details>

### Soal #172: Korelasi Positif
Pola: Makin banyak kamu belajar, makin tinggi nilai ujianmu. Ini disebut...
A. Korelasi Negatif
B. Korelasi Positif
C. Tidak berkolerasi
D. Kebetulan

<details>
<summary>💡 Hint</summary>
Kedua variabel (belajar & nilai) bergerak ke arah yang sama (Naik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Korelasi Positif.**
Pengenalan pola sebab-akibat sangat penting dalam sains data.
</details>

### Soal #173: Pola Perulangan (Loop)
Lakukan 5 kali: Tulis angka "1".
Apa hasilnya?
A. 1
B. 5
C. 11111
D. 12345

<details>
<summary>💡 Hint</summary>
Hanya menulis "1" berulang kali.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 11111.**
Loop adalah pola dasar instruksi komputer untuk tugas repetitif.
</details>

### Soal #174: Percabangan (Decision Tree)
Jika Hujan: Bawa Payung. Jika Tidak Hujan: Pakai Topi.
Sekarang sedang Panas Terik. Apa yang kamu bawa?
A. Payung
B. Topi
C. Keduanya
D. Tidak bawa apa-apa

<details>
<summary>💡 Hint</summary>
Panas Terik berarti "Tidak Hujan".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Topi.**
Logika "IF-ELSE" adalah pola pengambilan keputusan dalam pemrograman.
</details>

### Soal #175: Rekursi (Factorial)
Faktorial 3 (ditulis 3!) adalah $3 \times 2 \times 1 = 6$.
Berapa nilai 4!?
A. 10
B. 12
C. 24
D. 48

<details>
<summary>💡 Hint</summary>
$4! = 4 \times 3! = 4 \times 6$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 24.**
Rekursi adalah pola fungsi yang memanggil dirinya sendiri dalam masalah yang lebih kecil.
</details>

### Soal #176: Hirarki Penyimpanan Komputer
Urutan kecepatan dari yang paling CEPAT ke paling lambat:
A. RAM -> Harddisk -> Register CPU
B. Register CPU -> RAM -> Harddisk (HDD)
C. HDD -> RAM -> Register
D. Semuanya sama cepat

<details>
<summary>💡 Hint</summary>
Makin dekat ke "otak" (CPU), makin kencang urusannya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Register CPU -> RAM -> Harddisk.**
Pola "Semakin cepat, semakin kecil kapasitasnya" berlaku di hardware.
</details>

### Soal #177: Struktur Alamat IP
Alamat IP (v4) terdiri dari 4 kelompok angka, misalnya `192.168.1.1`. Berapa batas angka maksimal di setiap kelompok?
A. 100
B. 255
C. 500
D. 999

<details>
<summary>💡 Hint</summary>
Angka ini berasal dari 8-bit ($2^8 - 1$).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 255.**
Mengenali pola batasan data membantu dalam debugging jaringan.
</details>

### Soal #178: Pola DNS (Domain Name)
`www.google.com`. Bagian `.com` memberitahu kita bahwa ini adalah alamat untuk...
A. Komunitas (Community)
B. Komersial (Commercial)
C. Komputer (Computer)
D. Komunikasi (Communication)

<details>
<summary>💡 Hint</summary>
Suffix domain menunjukkan kategori organisasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Komersial.**
Standardisasi pola penamaan mempermudah klasifikasi situs web.
</details>

### Soal #179: Pola Tag HTML
Bentuk standar HTML: `<tag> Isi </tag>`.
Manakah yang penulisannya BENAR?
A. `<b> Tebal <b>`
B. `<i> Miring </i>`
C. `<p> Paragraf <p/>`
D. `<u> Garis Bawah /u>`

<details>
<summary>💡 Hint</summary>
Tag penutup harus memakai tanda slash (`/`) sebelum nama tag.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. <i> Miring </i>.**
Struktur berpasangan (Pairing) adalah pola utama dalam bahasa markup.
</details>

### Soal #180: Selector CSS
Jika ingin mewarnai semua teks berlabel `<p>` menjadi merah, pola kodenya adalah `p { color: red; }`.
Apa yang diwarnai oleh kode `h1 { color: blue; }`?
A. Semua link
B. Judul Utama (Heading 1)
C. Gambar
D. Seluruh halaman

<details>
<summary>💡 Hint</summary>
Targetnya adalah tag `h1`.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Judul Utama (Heading 1).**
Pola selector digunakan untuk menerapkan gaya secara massal dan efisien.
</details>

### Soal #181: Baris dan Kolom Database
Dalam database siswa, "Nama", "Alamat", dan "Kelas" disebut sebagai...
A. Row (Baris)
B. Column (Kolom / Field)
C. Cell
D. Database itu sendiri

<details>
<summary>💡 Hint</summary>
Ini adalah kategori datanya (Vertikal).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Column / Field.**
Baris (Row) mewakili 1 orang siswa secara utuh.
</details>

### Soal #182: Kunci Unik (ID)
Mengapa setiap siswa di sekolah punya NIS (Nomor Induk Siswa) yang berbeda?
A. Biar bukunya banyak.
B. Agar tidak ada kekeliruan data jika ada dua siswa bernama "Andi" (Unique Identifier Pattern).
C. Karena aturan dari pabrik kartu.
D. Biar siswa belajar menghafal angka.

<details>
<summary>💡 Hint</summary>
NIS menjamin setiap data punya identitas yang pasti (Pola Primary Key).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghindari kekeliruan data.**
Dekomposisi identitas menjadi angka unik sangat krusial dalam sistem informasi.
</details>

### Soal #183: Folder Bersarang (Nested)
Jalur file: `C:\User\Dokumen\Tugas\Informatika\tugas1.pdf`.
Manakah folder yang berada di posisi paling dalam?
A. Dokumen
B. Tugas
C. Informatika
D. C:

<details>
<summary>💡 Hint</summary>
Lihat yang paling kanan sebelum nama filenya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Informatika.**
Pola Tree (Pohon) atau Hirarki digunakan untuk mengorganisir data secara logis.
</details>

### Soal #184: Ekstensi File
Kamu ingin mengirim foto kualitas tinggi. File mana yang sebaiknya kamu pilih?
A. `foto.mp3`
B. `foto.jpg`
C. `foto.txt`
D. `foto.exe`

<details>
<summary>💡 Hint</summary>
Format `.jpg` adalah pola kompresi untuk gambar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. foto.jpg.**
Ekstensi memberitahu sistem operasi pola data apa yang ada di dalam file tersebut.
</details>

### Soal #185: Kompresi ZIP
Mengapa kita mengecilkan ukuran folder dengan ZIP sebelum mengirim email?
A. Agar filenya jadi rahasia.
B. Menghapus pola data yang berulang (Redundansi) agar ukuran file lebih hemat.
C. Biar filenya jadi warna kuning.
D. Agar tidak bisa dibuka orang lain.

<details>
<summary>💡 Hint</summary>
Prinsip dasar kompresi adalah Pattern Replacement.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghapus data berulang.**
Algoritma kompresi mengenali pola pengulangan bit untuk efisiensi penyimpanan.
</details>

### Soal #186: Error 404
Saat berselancar di internet, kamu mendapat pesan "404 Not Found". Apa artinya?
A. Internet kamu mati.
B. Server ditemukan, tapi halaman/file yang kamu cari tidak ada.
C. Komputer kamu terkena virus.
D. Kamu harus login dulu.

<details>
<summary>💡 Hint</summary>
Angka 4xx adalah kode pola error dari sisi Klien (Pengguna).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Halaman tidak ada.**
Standardisasi HTTP Status Codes membantu teknisi mengenali pola masalah secara cepat.
</details>

### Soal #187: Desain Tombol (CTA)
Mengapa tombol "Beli Sekarang" atau "Daftar" di web sering diberi warna cerah (seperti Oranye atau Hijau)?
A. Agar web terlihat ramai.
B. Mengikuti pola perhatian mata (Eye-catching) untuk memicu aksi pengguna.
C. Biar warnanya mirip pelangi.
D. Karena stok warna lain habis.

<details>
<summary>💡 Hint</summary>
Desain UI/UX menggunakan pola psikologi warna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memicu aksi pengguna.**
Dekomposisi perilaku manusia digunakan untuk mengoptimasi konversi pengguna.
</details>

### Soal #188: Navigasi Breadcrumb
`Home > Gadget > Smartphone > Android`. Pola navigasi ini disebut...
A. Peta Buta
B. Breadcrumb (Remah Roti)
C. GPS Web
D. History

<details>
<summary>💡 Hint</summary>
Seperti tokoh dongeng Hansel & Gretel yang meninggalkan remah roti agar tidak tersesat jalan pulang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Breadcrumb.**
Membantu pengguna mengenali pola lokasi mereka di dalam struktur website yang dalam.
</details>

### Soal #189: Hamburger Menu
Tiga garis horizontal tumpuk di pojok aplikasi HP sering disebut...
A. Garis-garis pusing
B. Hamburger Menu
C. Menu List
D. Pintu Rahasia

<details>
<summary>💡 Hint</summary>
Bentuknya seperti roti burger lapis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hamburger Menu.**
Sebuah pola ikon universal dalam desain UI modern untuk menyembunyikan navigasi agar layar terlihat bersih.
</details>

### Soal #190: Infinite Scroll
Kamu terus menggeser (scroll) TikTok atau Instagram ke bawah, dan konten baru terus muncul tanpa henti. Apa polanya?
A. Videonya hanya satu tapi diulang terus.
B. Konten dimuat secara bertahap saat kamu mendekati bagian bawah (Infinite Scroll Pattern).
C. HP kamu sedang mendownload seluruh internet sekaligus.
D. Kamu sedang berada di dalam mimpi.

<details>
<summary>💡 Hint</summary>
Aksi pengguna (Scroll) memicu request data baru ke server secara dinamis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Konten dimuat bertahap.**
Dekomposisi loading data: Hanya ambil yang diperlukan saat ini agar aplikasi tetap ringan.
</details>

### Soal #191: Pola Musik 4/4
Dalam musik, ketukan stabil "Dug - Tak - Dug - Tak" sering disebut birama 4/4.
Berapa jumlah ketukan dalam satu "Bar"?
A. 2
B. 3
C. 4
D. 8

<details>
<summary>💡 Hint</summary>
Lihat angka pembilangnya (yang di atas).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 4.**
Musik adalah matematika pola suara dalam waktu.
</details>

### Soal #192: Major vs Minor
Pola nada Major sering diasosiasikan dengan perasaan Senang, sedangkan pola nada Minor sering terdengar...
A. Sangat Berisik
B. Sedih atau Melankolis
C. Lucu
D. Tidak bersuara

<details>
<summary>💡 Hint</summary>
Ini adalah pola pengaruh frekuensi suara terhadap emosi manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sedih atau Melankolis.**
Komposer menggunakan pola tangga nada untuk menyampaikan pesan emosional.
</details>

### Soal #193: Rule of Thirds (Fotografi)
Membagi foto dengan 2 garis horizontal dan 2 garis vertikal, lalu meletakkan objek di titik potong garis tersebut. Mengapa?
A. Agar objeknya tidak kabur.
B. Menciptakan keseimbangan visual yang lebih dinamis dan menarik daripada ditaruh di tengah pas.
C. Biar kameranya tidak goyang.
D. Supaya fotonya terlihat seperti jendela gedung.

<details>
<summary>💡 Hint</summary>
Pola komposisi untuk mengarahkan pandangan mata.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Keseimbangan visual dinamis.**
Dekomposisi frame foto menjadi grid membantu menciptakan karya seni yang profesional.
</details>

### Soal #194: Warna Komplementer
Pola warna yang saling berlawanan di roda warna (misal: Biru dan Oranye). Jika disandingkan, mereka akan...
A. Terlihat kusam.
B. Terlihat sangat kontras dan menonjol.
C. Berubah jadi ungu.
D. Menghilangkan pandangan.

<details>
<summary>💡 Hint</summary>
Berlawanan = Saling menguatkan satu sama lain.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sangat kontras.**
Pola warna komplementer sering digunakan di poster film agar terlihat menarik.
</details>

### Soal #195: Pola Pantulan Cahaya
Hukum Refleksi: Sudut Datang = Sudut Pantul.
Jika cahaya datang dengan sudut $30^\circ$, berapa sudut pantulnya?
A. $60^\circ$
B. $90^\circ$
C. $30^\circ$
D. $0^\circ$

<details>
<summary>💡 Hint</summary>
Sama persis mengikuti pola simetri.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 30 derajat.**
Pola fisika cahaya ini digunakan dalam teknologi fiber optik.
</details>

### Soal #196: Pola Ayunan Bandul
Semakin panjang tali bandul, maka waktu yang dibutuhkan untuk satu kali ayunan (Periode) akan...
A. Semakin cepat
B. Semakin lama
C. Tetap sama
D. Berhenti

<details>
<summary>💡 Hint</summary>
Hubungan Positif antara Panjang Tali dan Waktu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Semakin lama.**
Mengenali pola gerak periodik membantu manusia membuat jam mekanik pertama kali.
</details>

### Soal #197: Pola Jatuh Bebas
Di ruang hampa udara, menjatuhkan bulu dan palu dari ketinggian yang sama akan menghasilkan...
A. Palu jatuh duluan.
B. Keduanya jatuh bersamaan pada detik yang sama.
C. Bulu akan melayang selamanya.
D. Keduanya meledak.

<details>
<summary>💡 Hint</summary>
Tanpa hambatan udara, pola gravitasi bekerja sama kuat pada semua massa.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jatuh bersamaan.**
Pola percepatan gravitasi bumi ($g = 9.8 m/s^2$) adalah konstanta universal di bumi.
</details>

### Soal #198: Tabel Periodik
Unsur-unsur dalam satu kolom vertikal yang sama (Golongan) memiliki kemiripan pola...
A. Sifat kimia dan jumlah elektron valensi.
B. Berat badan penemunya.
C. Warna batuannya.
D. Harga jualnya.

<details>
<summary>💡 Hint</summary>
Standardisasi pengelompokan berdasarkan pola perilaku atom.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Sifat kimia.**
Dekomposisi unsur kimia ke dalam tabel memudahkan ilmuwan memprediksi reaksi antar zat.
</details>

### Soal #199: Pola pH (Asam-Basa)
Jeruk Nipis (pH 2), Air Murni (pH 7), Sabun (pH 10).
Apa artinya jika suatu zat punya pH makin kecil mendekati 0?
A. Makin Basa
B. Makin Netral
C. Makin Asam
D. Makin Enak diminum

<details>
<summary>💡 Hint</summary>
Skala pH adalah pola ukuran keasaman ($< 7$ adalah asam).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Makin Asam.**
Mengenali pola pH sangat penting di industri pangan dan kecantikan.
</details>

### Soal #200: Gerbang Logika AND
Aturan: Lampu hanya nyala jika Saklar A DAN Saklar B menyala.
A (Mati), B (Nyala). Apakah lampu menyala?
A. Ya
B. Tidak
C. Kedap-kedip
D. Meledak

<details>
<summary>💡 Hint</summary>
Pola AND membutuhkan "Semua Benar" untuk menghasilkan "Benar".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Gerbang logika adalah pola dasar dari seluruh sirkuit komputer digital.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Gerbang logika adalah pola dasar dari seluruh sirkuit komputer digital.
</details>

### Soal #201: Pola Tumpukan (Stack)
Pola: Barang yang terakhir masuk adalah yang pertama keluar (LIFO).
Contoh nyata yang paling pas adalah...
A. Antrean beli tiket bioskop.
B. Tumpukan piring di wastafel.
C. Aliran air di pipa.
D. Kereta api yang berjalan.

<details>
<summary>💡 Hint</summary>
Piring paling atas (terakhir ditaruh) adalah yang paling mudah diambil pertama kali.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tumpukan piring.**
Stack adalah struktur data dasar yang mengikuti pola "Last In, First Out".
</details>

### Soal #202: Pola Antrean (Queue)
Pola: Barang yang pertama masuk adalah yang pertama keluar (FIFO).
Contoh nyata yang paling pas adalah...
A. Tumpukan baju di lemari.
B. Antrean orang di kasir minimarket.
C. Menumpuk kardus ke atas.
D. Kotak surat yang isinya dibalik.

<details>
<summary>💡 Hint</summary>
Siapa yang datang duluan, dia yang dilayani duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Antrean di kasir.**
Queue adalah pola struktur data "First In, First Out".
</details>

### Soal #203: Pola Rantai (Linked List)
Setiap gerbong kereta api terhubung ke gerbong di depannya dan di belakangnya. Pola koneksi ini dalam informatika disebut...
A. Array (Larik)
B. Linked List
C. Stack
D. Variable

<details>
<summary>💡 Hint</summary>
Setiap elemen memiliki "pointer" atau penunjuk ke elemen berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Linked List.**
Linked list memungkinkan pola penyimpanan data yang fleksibel dan dinamis.
</details>

### Soal #204: Pola Hirarki (Tree)
Struktur organisasi sekolah: Kepala Sekolah -> Wakil Kepala -> Guru -> Siswa.
Pola ini merupakan representasi dari struktur data...
A. Lingkaran (Cycle)
B. Pohon (Tree)
C. Garis Lurus
D. Kotak

<details>
<summary>💡 Hint</summary>
Satu titik pusat bercabang menjadi banyak titik di bawahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pohon (Tree).**
Struktur Tree digunakan untuk pola folder di komputer dan silsilah keluarga.
</details>

### Soal #205: Algoritma Pengurutan (Sorting)
Kamu punya kartu angka: 5, 2, 8, 1, 9.
Setelah dilakukan pola "Sorting Ascending" (Meningkat), urutannya menjadi...
A. 9, 8, 5, 2, 1
B. 1, 2, 5, 8, 9
C. 2, 5, 8, 1, 9
D. 5, 8, 9, 2, 1

<details>
<summary>💡 Hint</summary>
Meningkat berarti dari kecil ke besar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1, 2, 5, 8, 9.**
Pengenalan pola urutan sangat penting untuk mempermudah pencarian data.
</details>

### Soal #206: Algoritma Pencarian (Searching)
Kamu sedang mencari buku dengan judul berawal huruf "M" di rak yang sudah urut abjad. Pola pencarian paling efisien adalah...
A. Mencari dari buku paling pertama satu per satu sampai ketemu.
B. Langsung membuka area tengah rak dan menyesuaikan ke kiri atau kanan.
C. Mengambil semua buku lalu dibaca judulnya.
D. Menunggu petugas merapikan rak lagi.

<details>
<summary>💡 Hint</summary>
Ini adalah pola Binary Search (Pencarian Bagi Dua).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuka area tengah.**
Mengenali pola data yang sudah terurut memungkinkan pencarian yang sangat cepat.
</details>

### Soal #207: Peran Router (Pengarah Jalur)
Router di internet berfungsi mengarahkan paket data ke jalur yang paling lengang. Apa dasar keputusannya?
A. Memilih warna kabel yang bagus.
B. Mengenali pola kemacetan (Traffic) di berbagai rute jaringan secara real-time.
C. Mengikuti rute yang paling jauh agar paketnya jalan-jalan.
D. Menunggu perintah dari satelit.

<details>
<summary>💡 Hint</summary>
Dekomposisi rute jaringan dilakukan untuk efisiensi pengiriman data.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengenali pola kemacetan.**
Router bertindak sebagai polisi lalu lintas data berbasis pola aliran informasi.
</details>

### Soal #208: Paket Data
Saat mengirim foto, komputer memecahnya menjadi ribuan potongan kecil bernama "Packet". Mengapa tidak dikirim langsung utuh?
A. Supaya filenya jadi banyak.
B. Agar jika ada satu bagian yang gagal, hanya bagian pola kecil itu yang perlu dikirim ulang (efisiensi error handling).
C. Biar internetnya terlihat sibuk.
D. Karena kabel internet sangat sempit.

<details>
<summary>💡 Hint</summary>
Dekomposisi data besar menjadi kecil adalah prinsip dasar protokol internet.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Efisiensi penanganan error.**
Pola transmisi paket menjamin keutuhan data di tujuan meskipun jalur internet tidak stabil.
</details>

### Soal #209: Pola Keamanan Sandi (Password)
Sandi `123456` lebih mudah diretas daripada `P@ssw0rd!23`. Mengapa?
A. Karena `123456` angkanya terlalu sedikit.
B. Karena `123456` memiliki pola berurutan yang sangat umum dan mudah ditebak oleh algoritma peretas.
C. Karena sandi kedua punya banyak simbol.
D. Karena peretas tidak suka angka 1 sampai 6.

<details>
<summary>💡 Hint</summary>
Makin acak (Entropy tinggi), makin sulit polanya dikenali.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola berurutan mudah ditebak.**
Keamanan cyber bergantung pada penggunaan pola yang kompleks dan unik.
</details>

### Soal #210: Pola Penipuan Phishing
Kamu mendapat email: "Akun anda terblokir! Klik link ini segera: `www.bank-palsu-klik.com`!".
Ciri pola penipuan (Phishing) di sini adalah...
A. Menggunakan bahasa yang sopan.
B. Memberikan perasaan urgensi (panik) agar pengguna tidak sempat berpikir logis.
C. Memberikan hadiah uang gratis.
D. Emailnya berwarna cerah.

<details>
<summary>💡 Hint</summary>
Phishing sering menggunakan pola manipulasi psikologis (Social Engineering).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memberikan perasaan urgensi.**
Mengenali pola komunikasi penipu adalah langkah pertama perlindungan data pribadi.
</details>

### Soal #211: Kecerdasan Buatan (AI)
Machine Learning adalah cabang AI di mana komputer...
A. Belajar mengikuti instruksi kaku dari manusia.
B. Belajar mengenali pola dari data masa lalu untuk membuat prediksi atau keputusan di masa depan.
C. Menjadi sadar diri seperti manusia.
D. Bisa terbang ke luar angkasa.

<details>
<summary>💡 Hint</summary>
AI bekerja dengan dekomposisi data mentah menjadi pola yang dapat dimengerti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Belajar mengenali pola dari data.**
Inilah inti dari Pattern Recognition dalam dunia teknologi modern.
</details>

### Soal #212: Klasifikasi Gambar oleh AI
Bagaimana AI membedakan foto Kucing dan Anjing?
A. Dengan menanyakan pada pemiliknya.
B. Dengan mengekstrak pola fitur unik seperti bentuk telinga, pola hidung, dan tekstur bulu.
C. AI hanya menebak secara acak.
D. AI masuk ke dalam foto untuk melihat langsung.

<details>
<summary>💡 Hint</summary>
Dekomposisi objek visual menjadi variabel pendukung identifikasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengekstrak pola fitur unik.**
Ribuan pola digital kecil dikombinasikan untuk menghasilkan prediksi identitas objek.
</details>

### Soal #213: Natural Language Processing (NLP)
Google Translate memahami kalimat bukan cuma kata per kata, tapi mengenali pola...
A. Warna teksnya.
B. Struktur tata bahasa (Grammar) dan konteks penggunaan kata dalam kalimat.
C. Nama orang yang mengetik.
D. Kecepatan mengetik pengguna.

<details>
<summary>💡 Hint</summary>
Bahasa memiliki pola aturan yang sudah baku (Sintaksis).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tata bahasa dan konteks.**
NLP adalah pengenalan pola linguistik oleh mesin.
</details>

### Soal #214: Bias Algoritma
Jika sebuah AI hanya dilatih dengan data foto orang dari satu negara, saat digunakan di negara lain ia sering gagal mengenali wajah. Kondisi ini disebut...
A. Kerusakan Hardware.
B. Algorithmic Bias (Bias Algoritma) karena pola data pelatihan yang tidak beragam.
C. AI sedang mogok kerja.
D. Kamera HP sedang kotor.

<details>
<summary>💡 Hint</summary>
Kualitas output tergantung pada kualitas dan variasi pola input (Garbage In, Garbage Out).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algorithmic Bias.**
Keadilan AI sangat bergantung pada representasi pola data yang adil dan luas.
</details>

### Soal #215: Privasi Data (Data Minimization)
Aplikasi penghitung langkah kaki meminta izin akses ke "Lokasi, Kontak, Kamera, dan Mikrofon". Manakah yang melanggar pola privasi "Minimisasi Data"?
A. Lokasi (untuk menghitung jarak tempuh).
B. Mikrofon dan Kontak (tidak relevan dengan fungsi utama menghitung langkah).
C. Kamera (untuk foto profil sekali saja).
D. Semuanya perlu.

<details>
<summary>💡 Hint</summary>
Hanya minta data yang polanya benar-benar dibutuhkan aplikasi untuk bekerja.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mikrofon dan Kontak.**
Mengenali pola permintaan data yang mencurigakan melindungi privasi kita.
</details>

### Soal #216: Perangkat Input
Pola: Alat yang digunakan untuk memberikan perintah atau memasukkan data KE DALAM komputer.
Manakah yang termasuk perangkat input?
A. Monitor
B. Printer
C. Keyboard dan Mouse
D. Speaker

<details>
<summary>💡 Hint</summary>
Alat mana yang kamu gunakan untuk mengirim sinyal dari tanganmu ke sistem?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Keyboard dan Mouse.**
Dekomposisi sistem komputer membagi perangkat berdasarkan arah aliran informasi.
</details>

### Soal #217: Perangkat Output
Manakah yang merupakan hasil akhir (pola visual/suara) yang dikeluarkan komputer untuk pengguna?
A. Scanner
B. Flashdisk
C. Monitor dan Speaker
D. Joystick

<details>
<summary>💡 Hint</summary>
Informasi bergerak KELUAR dari komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Monitor dan Speaker.**
Output adalah representasi pola data digital menjadi pola fisik yang bisa ditangkap indra manusia.
</details>

### Soal #218: Izin File (Permissions)
Pola: R (Read/Baca), W (Write/Tulis), X (Execute/Jalankan).
Jika sebuah file kodenya adalah `R--`, apa yang bisa kamu lakukan?
A. Menghapus file tersebut.
B. Membuka dan membaca isinya saja, tidak bisa mengedit.
C. Mengubah nama file.
D. Menjalankan file sebagai program.

<details>
<summary>💡 Hint</summary>
Hanya huruf R yang aktif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membaca saja.**
Sistem keamanan OS menggunakan pola bit izin untuk melindungi data dari akses tidak sah.
</details>

### Soal #219: Task Manager (OS)
Kamu melihat grafik penggunaan CPU mencapai 100% dan HP menjadi panas. Tindakan apa yang paling tepat berdasarkan pola ini?
A. Melakukan charge HP.
B. Menutup aplikasi ("End Task") yang memakan sumber daya paling besar.
C. Membeli HP baru.
D. Berteriak ke aplikasinya.

<details>
<summary>💡 Hint</summary>
Gunakan pola monitoring untuk menemukan penyebab masalah (Troubleshooting).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menutup aplikasi berat.**
Pengenalan pola beban kerja membantu menjaga stabilitas sistem operasi.
</details>

### Soal #220: Rumus Spreadsheet
Di Excel, kamu ingin menjumlahkan sel A1 sampai A10. Pola penulisan rumus yang benar adalah...
A. `SUM(A1:A10)`
B. `=SUM(A1:A10)`
C. `A1+A10`
D. `TOTAL A1 TO A10`

<details>
<summary>💡 Hint</summary>
Setiap rumus harus dimulai dengan tanda Sama Dengan (`=`).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. =SUM(A1:A10).**
Software produktivitas menggunakan pola sintaksis formula untuk otomasi perhitungan.
</details>

### Soal #221: Referensi Absolut ($)
Saat menarik rumus ke bawah, sel `A1` akan berubah jadi `A2, A3...`.
Bagaimana agar alamat sel tetap terkunci di A1 saat rumus ditarik?
A. Tulis manual di setiap sel.
B. Gunakan tanda dolar: `$A$1`.
C. Gunakan tanda pagar: `#A#1`.
D. Sel tidak bisa dikunci.

<details>
<summary>💡 Hint</summary>
Tanda `$` adalah simbol pola pengamanan koordinat sel.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. $A$1.**
Mengenali pola referensi sangat penting untuk pengolahan data besar yang efisien.
</details>

### Soal #222: Gaya Penulisan Kode (Naming Convention)
Pola `nama_variabel_saya` disebut `snake_case`. Bagaimana pola `namaVariabelSaya` disebut?
A. CamelCase (Punuk Unta)
B. BurgerCase
C. GhostCase
D. UpperCase

<details>
<summary>💡 Hint</summary>
Huruf kapital di tengah kata terlihat seperti punuk unta.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. CamelCase.**
Konsistensi pola penamaan membuat kode lebih mudah dibaca dan dikelola tim.
</details>

### Soal #223: Komentar dalam Kode
Programmer menulis `// Ini adalah fungsi untuk menghitung luas`.
Apa fungsi dari baris yang dimulai dengan `//` tersebut?
A. Itu adalah kode rahasia untuk hacker.
B. Baris tersebut diabaikan oleh komputer dan hanya dibaca oleh manusia untuk memahami pola alur program.
C. Itu akan memunculkan tulisan di layar saat program dijalankan.
D. Itu perintah untuk menghapus file.

<details>
<summary>💡 Hint</summary>
Komentar adalah dokumentasi pola pikir programmer.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Diabaikan komputer, dibaca manusia.**
Dokumentasi membantu pengenalan pola logika saat kita membuka kembali kode lama.
</details>

### Soal #224: Pola Debugging
Saat program error, cara terbaik memperbaikinya adalah...
A. Menghapus semua kode dan mulai dari nol.
B. Mencari pola baris kode mana yang menyebabkan masalah dengan membaca pesan error atau melakukan tes per bagian.
C. Memukul keyboard sampai programnya jalan.
D. Berdoa agar errornya hilang sendiri.

<details>
<summary>💡 Hint</summary>
Dekomposisi masalah besar menjadi bagian kecil untuk isolasi error.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencari baris penyebab masalah.**
Debugging adalah seni mengenali anomali (kejanggalan) dalam pola instruksi kode.
</details>

### Soal #225: Gerbang Logika XOR
Aturan: Lampu menyala HANYA JIKA salah satu saklar nyala (TIDAK BOLEH keduanya nyala atau keduanya mati).
A=Nyala, B=Nyala. Apakah lampu menyala?
A. Ya
B. Tidak
C. Kedap-kedip
D. Meledak

<details>
<summary>💡 Hint</summary>
"Exclusive OR" berarti harus ada perbedaan status.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Karena keduanya menyala, pola XOR menghasilkan output Mati (False).
</details>

### Soal #226: Pola Biner (Binary)
Jika angka Desimal 1 adalah Biner `1`, dan Desimal 2 adalah Biner `10`.
Berapa Biner untuk angka Desimal 3?
A. 11
B. 100
C. 101
D. 20

<details>
<summary>💡 Hint</summary>
Tambahkan 1 ke `10`. Karena hanya boleh angka 0 dan 1, maka angka terakhir naik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 11.**
Pola basis 2 adalah bahasa dasar yang digunakan hardware komputer.
</details>

### Soal #227: Pola Hexadecimal
Basis 16: Angka 0-9 dilanjutkan dengan huruf A-F.
Nilai untuk huruf `A` dalam desimal adalah...
A. 10
B. 11
C. 15
D. 100

<details>
<summary>💡 Hint</summary>
Setelah angka 9, lanjut ke A.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 10.**
Pola Hexadecimal digunakan untuk merepresentasikan warna di web (Contoh: `#FFFFFF` untuk putih).
</details>

### Soal #228: Encoding Karakter (ASCII)
Komputer menyimpan huruf 'A' sebagai angka 65. Huruf 'B' sebagai 66.
Berapa angka untuk huruf 'D'?
A. 67
B. 68
C. 69
D. 70

<details>
<summary>💡 Hint</summary>
Lanjutkan polanya: A(65), B(66), C(67), D(...).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 68.**
Semua data di komputer pada akhirnya adalah pola angka yang diterjemahkan.
</details>

### Soal #229: Kompresi Gambar (Lossless vs Lossy)
File PNG tetap jernih meskipun dikompres, sedangkan file JPEG kualitasnya menurun jika dikompres terlalu kecil. Pola kompresi yang membuang data (JPEG) disebut...
A. Lossless
B. Lossy
C. Lazy
D. Lucky

<details>
<summary>💡 Hint</summary>
"Loss" berarti ada yang hilang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lossy.**
Mengenali pola kebutuhan (Kualitas vs Ukuran) membantu kita memilih format file yang tepat.
</details>

### Soal #230: Skalabilitas Cloud
Saat toko online sedang diskon besar (Flash Sale), pengunjung naik 100x lipat. Sistem Cloud akan secara otomatis menambah kapasitas server. Pola ini disebut...
A. Otomasi Gaji.
B. Scalability (Skalabilitas).
C. Cloud Rain.
D. Server Error.

<details>
<summary>💡 Hint</summary>
Sistem yang bisa "melebar" atau "mengecil" sesuai beban pola trafik (Elasticity).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Scalability.**
Infrastruktur modern menggunakan pengenalan pola beban untuk efisiensi biaya.
</details>

### Soal #231: Internet of Things (IoT)
Lampu teras menyala otomatis saat sensor mendeteksi hari sudah gelap. Ini adalah contoh...
A. Mistis.
B. Perilaku IoT (Internet of Things).
C. Lampu yang rusak.
D. Pemborosan listrik.

<details>
<summary>💡 Hint</summary>
Interaksi antar perangkat pintar melalui pola sensorik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perilaku IoT.**
Input (pola cahaya rendah) -> Proses (Logika saklar) -> Output (Lampu Nyala).
</details>

### Soal #232: Keamanan Blockchain
Blockchain menghubungkan blok data menggunakan "Hash" dari blok sebelumnya. Jika satu data diubah, pola rantainya akan...
A. Tetap kokoh.
B. Terputus / Tidak valid (karena pola Hash tidak cocok lagi).
C. Berubah warna jadi emas.
D. Kirim pesan ke WhatsApp.

<details>
<summary>💡 Hint</summary>
Setiap blok membawa "jejak" pola dari blok sebelumnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terputus / Tidak valid.**
Inilah pola keamanan yang membuat Bitcoin dan teknologi crypto sulit dipalsukan.
</details>

### Soal #233: Kuantum Komputer (Qubit)
Jika bit biasa hanya 0 atau 1, Qubit bisa berada di kedua status sekaligus (Superposisi). Ini memungkinkan pola perhitungan yang...
A. Sangat lambat.
B. Jauh lebih cepat dan paralel untuk masalah yang sangat kompleks.
C. Hanya untuk main game.
D. Tidak berguna.

<details>
<summary>💡 Hint</summary>
Dekomposisi perhitungan dilakukan secara bersamaan di banyak jalur pola.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jauh lebih cepat.**
Komputasi kuantum adalah masa depan pengolahan data berbasis pola fisika subatom.
</details>

### Soal #234: Pola Hadiah Game (Reward Loop)
Kamu mendapat hadiah kecil setiap login harian, dan hadiah besar setiap 7 hari. Tujuannya adalah...
A. Mengukur kecepatan internetmu.
B. Menciptakan pola kebiasaan (Engagement) agar pemain terus kembali setiap hari.
C. Menghabiskan baterai HP.
D. Pamer kekayaan developer game.

<details>
<summary>💡 Hint</summary>
Desain game menggunakan pola psikologi penguatan (Positive Reinforcement).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan pola kebiasaan.**
Gamifikasi menggunakan pola reward untuk memandu perilaku pengguna.
</details>

### Soal #235: Kurva Kesulitan (Difficulty Curve)
Level 1 sangat mudah, level 100 sangat sulit. Pola kenaikan kesulitan ini dirancang agar pemain...
A. Langsung bosan.
B. Mengalami tantangan yang pas seiring bertambahnya kemampuan (Pola Flow).
C. Merasa tertipu.
D. Menghapus aplikasinya.

<details>
<summary>💡 Hint</summary>
Makin mahir anda mengenali pola game, makin sulit tantangannya diberikan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tantangan yang pas.**
Dekomposisi level game memperhatikan kurva belajar (Learning Curve) pengguna.
</details>

### Soal #236: Umpan Balik Pemain (Feedback)
HP bergetar saat karaktermu terkena pukulan di game. Pola ini disebut umpan balik...
A. Visual (Mata)
B. Auditorial (Telinga)
C. Haptic (Sentuhan/Getaran)
D. Telepati

<details>
<summary>💡 Hint</summary>
Dirasakan melalui indra peraba atau fisik.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Haptic.**
Integrasi berbagai pola stimulus meningkatkan pengalaman imersif dalam teknologi.
</details>

### Soal #237: Pola Kerja Kanban
Papan dengan kolom: `Tugas Belum Selesai`, `Sedang Dikerjakan`, `Selesai`.
Jika kamu memindahkan kartu tugas dari kolom tengah ke kanan, itu menunjukkan...
A. Kamu baru mau mulai kerja.
B. Tugas sudah tuntas dikerjakan.
C. Kamu membatalkan tugas.
D. Tugasnya hilang.

<details>
<summary>💡 Hint</summary>
Kolom paling kanan biasanya adalah stasiun akhir proses.
</details>
<details>
<summary>✅ Jawaban</summary>
**B. Tugas tuntas.**
Kanban adalah pola manajemen proyek visual yang populer di industri IT.
</details>

### Soal #238: Tekanan Tenggat Waktu (Deadline)
Makin mendekati hari pengumpulan tugas, kecepatan bekerjamu meningkat pesat karena panik. Ini adalah contoh pola perilaku...
A. Prokrastinasi (Menunda-nunda).
B. Manajemen waktu yang baik.
C. Pola hidup sehat.
D. Robotik.

<details>
<summary>💡 Hint</summary>
Mengenali pola perilaku diri sendiri membantu kita memperbaiki strategi belajar (Metakognisi).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Prokrastinasi.**
Dekomposisi jadwal belajar bisa membantu memecah pola penundaan ini.
</details>

### Soal #239: Pola Judul Email yang Jelas
Subjek: `URGENT - Izin Tidak Masuk - Budi Kelas 10A`.
Mengapa pola subjek ini dianggap sangat baik?
A. Karena hurufnya besar semua.
B. Karena langsung memberikan ringkasan informasi (Kategori, Tujuan, Identitas) tanpa perlu membuka email dulu.
C. Karena ada nama pribadinya.
D. Karena menggunakan bahasa Inggris.

<details>
<summary>💡 Hint</summary>
Dekomposisi informasi ke dalam label yang ringkas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memberikan ringkasan informasi langsung.**
Standardisasi pola komunikasi digital menghemat waktu penerima pesan.
</details>

### Soal #240: Pola Komunikasi Non-Verbal
Seseorang bicara "Saya tidak marah", tapi wajahnya merah dan tangannya mengepal. Pola mana yang lebih bisa dipercaya?
A. Kalimat yang diucapkan.
B. Pola bahasa tubuh (Body Language) yang tidak bisa berbohong.
C. Keduanya bohong.
D. Tidak ada yang benar.

<details>
<summary>💡 Hint</summary>
Mengenali ketidaksinkronan (Mismatch) antar pola informasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bahasa tubuh.**
Pattern recognition juga berlaku dalam interaksi sosial dan psikologi.
</details>

### Soal #241: Pola Daur Ulang E-Waste
Baterai bekas dan HP rusak tidak boleh dibuang ke tempat sampah biasa karena mengandung logam berat. Apa solusinya?
A. Dikubur di halaman rumah.
B. Dibawa ke tempat pengolahan limbah elektronik khusus agar komponennya bisa digunakan lagi (Pola Circular Economy).
C. Dibuang ke sungai.
D. Dibakar.

<details>
<summary>💡 Hint</summary>
Menciptakan pola penggunaan material yang berulang (tidak sekali pakai buang).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengolahan limbah elektronik.**
Berpikir komputasional juga membantu kita merancang pola keberlanjutan lingkungan.
</details>

### Soal #242: Efisiensi Pusat Data (Data Center)
Pusat data Google diletakkan di tempat beriklim dingin atau di bawah laut. Apa tujuannya?
A. Biar pegawainya bisa main salju.
B. Memanfaatkan pola suhu alami untuk mendinginkan ribuan server agar hemat listrik AC (Passive Cooling).
C. Biar tidak digigit nyamuk.
D. Agar servernya tidak bisa dicuri manusia darat.

<details>
<summary>💡 Hint</summary>
Optimasi energi dengan memanfaatkan pola lingkungan sekitar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memanfaatkan suhu alami.**
Rekayasa teknologi selalu memperhatikan pola transfer panas fisika.
</details>

### Soal #243: Kesenjangan Digital (Digital Divide)
Pola: Orang di kota besar punya internet kencang, sedangkan orang di desa terpencil sulit akses sinyal. Kondisi ini disebut...
A. Keadilan sosial.
B. Kesenjangan Digital (Digital Divide).
C. Nasib buruk.
D. Pola geografi.

<details>
<summary>💡 Hint</summary>
Dekomposisi masalah akses teknologi berdasarkan infrastruktur wilayah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kesenjangan Digital.**
Pemerataan akses teknologi adalah tantangan global untuk pola pembangunan yang adil.
</details>

### Soal #244: Filter Bubble (Gema Media Sosial)
Algoritma hanya menunjukkan berita yang kamu sukai saja, sehingga kamu tidak pernah melihat pandangan yang berbeda. Pola ini disebut...
A. Pola Pintar.
B. Echo Chamber (Ruang Gema).
C. Berita Bahagia.
D. Pola Bebas.

<details>
<summary>💡 Hint</summary>
Algoritma pengenalan pola kesukaanmu yang terlalu ketat membatasi wawasanmu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Echo Chamber.**
Mengenali pola kerja algoritma membantu kita menjadi pengguna teknologi yang lebih kritis.
</details>

### Soal #245: Delay Sinyal Ruang Angkasa
Pesan dari Bumi ke Planet Mars butuh waktu sekitar 10 menit untuk sampai (karena jarak yang jauh). Bagaimana pola komunikasinya?
A. Telepon langsung seperti biasa.
B. Komunikasi tunda (Asynchronous) - kirim pesan, tunggu balasan beberapa puluh menit kemudian.
C. Tidak bisa berkirim pesan sama sekali.
D. Menggunakan walkie-talkie.

<details>
<summary>💡 Hint</summary>
Batas kecepatan cahaya menciptakan pola keterlambatan (Latency).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Komunikasi tunda.**
Insinyur NASA harus merancang program dengan dekomposisi waktu tunda sinyal ini.
</details>

### Soal #246: Estimasi Akar Kuadrat
$\sqrt{40}$ berada di antara angka bulat berapa dan berapa?
A. 4 dan 5
B. 5 dan 6
C. 6 dan 7
D. 7 dan 8

<details>
<summary>💡 Hint</summary>
$6^2 = 36$. $7^2 = 49$. Angka 40 ada di tengahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 6 dan 7.**
Mengenali pola bilangan kuadrat membantu estimasi perhitungan cepat (Mental Math).
</details>

### Soal #247: Persentase dari Persentase
Kamu dapat diskon 50%, lalu di kasir dapat diskon lagi 10% dari harga setelah diskon pertama. Berapa total harga yang kamu bayar?
A. 40% dari harga asli.
B. 45% dari harga asli.
C. 60% dari harga asli.
D. 50% dari harga asli.

<details>
<summary>💡 Hint</summary>
Harga awal 100 -> Diskon 50% jadi 50 -> Diskon 10% dari 50 adalah 5. Sisa harga = ...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 45% dari harga asli.**
Dekomposisi perhitungan diskon bertahap seringkali menipu jika kita tidak paham polanya.
</details>

### Soal #248: Logika Modus Ponens
Jika hari hujan, tanah basah. Sekarang hari hujan. Apa kesimpulannya?
A. Tanah mungkin kering.
B. Tanah pasti basah.
C. Hari sudah malam.
D. Saya lupa bawa payung.

<details>
<summary>💡 Hint</summary>
Pola: $P \rightarrow Q$. $P$ benar, maka $Q$ juga benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tanah pasti basah.**
Pola deduksi logika adalah fondasi dari mesin inferensi di AI.
</details>

### Soal #249: Logika Modus Tollens
Jika lampu nyala, saklar sudah ditekan. Sekarang saklar BELUM ditekan. Kesimpulannya?
A. Lampu pasti mati.
B. Lampu mungkin nyala.
C. Lampu terbakar.
D. Saklarnya berat.

<details>
<summary>💡 Hint</summary>
Pola: Jika tidak ada penyebab ($P$), maka tidak ada akibat ($Q$).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Lampu pasti mati.**
Logika formal menggunakan pola-pola ini untuk menjamin kebenaran suatu pernyataan.
</details>

### Soal #250: Penutup - Pentingnya Pengenalan Pola
Manakah manfaat terbesar dari kemampuan Mengenali Pola bagi seorang programmer?
A. Bisa mengetik lebih cepat daripada orang lain.
B. Bisa menciptakan solusi yang bisa digunakan berulang kali untuk masalah yang mirip (Reusability).
C. Biar terlihat keren di depan teman.
D. Untuk memenangkan semua video game.

<details>
<summary>💡 Hint</summary>
Prinsip DRY (Don't Repeat Yourself) dalam coding.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan solusi yang bisa diulang.**
Pattern Recognition adalah jantung dari efisiensi dan kreativitas dalam dunia Computational Thinking. Selamat, kamu telah menyelesaikan 250 soal!
</details>

---
[< Materi Sebelumnya: Decomposition](./02-decomposition.md) | [Materi Selanjutnya: Abstraction](./04-abstraction.md)
[< Kembali ke Beranda Materi](../README.md)
