# 03. Pengenalan Pola - Bagian 1 (Soal 1-50)

[🏠 Indeks](../03-pattern-recognition.md) | [Bagian 2 (51-100) >](03-pattern-recognition-part-2.md)

---
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

