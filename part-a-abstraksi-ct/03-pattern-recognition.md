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

[< Materi Sebelumnya: Decomposition](./02-decomposition.md) | [Materi Selanjutnya: Abstraction](./04-abstraction.md)
[< Kembali ke Beranda Materi](../README.md)
