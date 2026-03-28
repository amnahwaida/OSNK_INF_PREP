# 05. Algorithm Design (Perancangan Algoritma)

> "Algoritma bukan hanya tentang kode, tapi tentang cara kita memberikan instruksi yang presisi untuk menyelesaikan masalah."

Selamat! Kamu telah sampai di pilar terakhir dari Computational Thinking: **Algorithm Design** (Perancang Algoritma). Jika Decomposition memecah masalah, Pattern Recognition mencari kesamaan, dan Abstraction membuang detail, maka Algorithm Design adalah **penyusun langkah demi langkah** untuk mencapai solusi akhir.

---

## 🚀 Apa itu Algorithm Design?

**Algorithm Design** adalah kemampuan untuk menyusun langkah-langkah logis, terurut, dan detail untuk menyelesaikan sebuah masalah atau menjalankan sebuah tugas.

Bayangkan kamu adalah seorang arsitek yang memberikan instruksi kepada pekerja bangunan. Jika instruksimu tidak jelas, bangunan bisa rubuh. Begitu juga dengan komputer; ia hanya melakukan apa yang kamu perintahkan secara persis.

---

## 🍕 Analogi 1: Resep Membuat Pizza
Bayangkan kamu ingin mengajari adikmu membuat pizza. Kamu tidak bisa hanya bilang "buat pizza". Kamu harus memberikan algoritma:
1. Siapkan adonan roti.
2. Oleskan saus tomat di atas adonan.
3. Taburkan keju mozzarella dan topping lainnya.
4. Panggang di dalam oven pada suhu 200°C selama 15 menit.
5. Keluarkan dari oven dan potong menjadi 8 bagian.

Langkah-langkah di atas adalah sebuah **Algoritma**. Jika urutannya ditukar (misal: potong pizza dulu baru panggang), hasilnya akan kacau!

---

## 📦 Analogi 2: Rakit Lemari IKEA
Pernahkah kamu melihat buku instruksi merakit mainan atau lemari?
*   Ada daftar bahan (Input).
*   Ada langkah demi langkah gambar (Langkah Algoritma).
*   Ada hasil akhir lemari yang berdiri tegak (Output).

Buku instruksi tersebut adalah bentuk fisik dari sebuah desain algoritma.

---

## 💻 Kenapa Penting dalam Informatika?

Dalam dunia komputer, algoritma adalah "otak" dari setiap aplikasi.
*   **Google Maps**: Menggunakan algoritma untuk mencari rute tercepat (Dijkstra's Algorithm).
*   **Instagram**: Menggunakan algoritma untuk menentukan foto mana yang muncul paling atas di feed-mu.
*   **Sorting (Pengurutan)**: Algoritma untuk mengurutkan daftar nama dari A ke Z.

### 4 Syarat Algoritma yang Baik:
1.  **Finiteness (Terbatas)**: Harus ada titik berhenti. Jangan sampai komputer "hang" karena berputar selamanya.
2.  **Definiteness (Jelas)**: Setiap langkah tidak boleh bermakna ganda (ambigu).
3.  **Input & Output**: Harus jelas apa yang dimasukkan dan apa yang dihasilkan.
4.  **Effectiveness (Efektif)**: Langkahnya harus sederhana dan bisa dilakukan.

---

## 📝 Contoh di OSN-K Informatika

Di soal OSN-K, kamu sering diminta mengikuti jejak variabel dalam sebuah instruksi (Trace).
**Contoh sederhana:**
1. Mulai dengan angka $X = 5$.
2. Jika $X$ ganjil, tambahkan 1.
3. Jika $X$ genap, bagi dengan 2.
4. Ulangi langkah 2 & 3 sebanyak 3 kali. Berapa hasil akhirnya?

Kemampuan kamu mengikuti langkah di atas secara teliti adalah inti dari Algorithm Design.

---

## 🏗️ Latihan Soal Level: Newbie sampai Mahir

Berikut adalah bank soal latihan untuk mengasah logika algoritmamu.

### Soal #1: Algoritma Mencari Kaus Kaki
Kamu punya 5 pasang kaus kaki acak di lantai. Algoritma paling efisien untuk memasangkan mereka adalah...
A. Ambil satu, lalu cari pasangannya satu per satu sampai ketemu.
B. Buat tumpukan berdasarkan warna dulu (Sorting), lalu pasangkan di dalam tiap tumpukan.
C. Tutup mata dan ambil dua secara acak.
D. Biarkan saja sampai ada orang lain yang merapikan.

<details>
<summary>💡 Hint</summary>
Mengelompokkan benda yang mirip (Sorting/Categorizing) sebelum memprosesnya biasanya lebih cepat daripada mencari satu-satu secara acak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Buat tumpukan berdasarkan warna (Sorting).**
Metode ini mengurangi jumlah perbandingan yang perlu dilakukan mata kita.
</details>

### Soal #2: Algoritma "Lampu Sensor Gerak"
1. JIKA ada gerakan terdeteksi, MAKA nyalakan lampu selama 10 detik.
2. JIKA dalam 10 detik ada gerakan baru, MAKA reset hitungan jadi 10 detik lagi.
Jika kamu masuk ruangan pada detik ke-0 dan diam mematung pada detik ke-5, kapan lampu mati?
A. Detik ke-10
B. Detik ke-15
C. Detik ke-5
D. Tidak pernah mati

<details>
<summary>💡 Hint</summary>
Gerakan terakhir terjadi pada detik ke-0 (saat masuk). Hitungan 10 detik dimulai dari sana.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Detik ke-10**
Karena tidak ada gerakan baru setelah detik ke-0, lampu akan mati tepat 10 detik setelah aktivitas terakhir.
</details>

### Soal #3: Algoritma Menyeberang Jalan
Urutan yang paling aman dan benar:
1. Tengok kanan.
2. Jalan menyeberang.
3. Tengok kiri.
4. Berhenti di pinggir jalan.

A. 4-1-3-1-2
B. 4-2-1-3
C. 1-3-2-4
D. 4-1-3-2

<details>
<summary>💡 Hint</summary>
Prinsip "Tengok Kanan - Tengok Kiri - Tengok Kanan Lagi" sebelum melangkah.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4-1-3-1-2**
Berhenti (4) -> Kanan (1) -> Kiri (3) -> Kanan lagi (1) untuk memastikan -> Seberang (2).
</details>

### Soal #4: Algoritma "Matematika Cepat"
$X = 10$. Ulangi 5 kali: "Tambahkan $X$ dengan 2". Berapa nilai akhir $X$?
A. 12
B. 20
C. 15
D. 20

<details>
<summary>💡 Hint</summary>
$10 + (2 \times 5) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 20**
Penjumlahan berulang sebanyak 5 kali menghasilkan 10 + 10 = 20.
</details>

### Soal #5: Algoritma "Urutan Masak Nasi"
1. Masukkan panci ke magic com dan klik tombol "Cook".
2. Cuci beras sampai bersih.
3. Masukkan air secukupnya.
4. Masukkan beras ke dalam panci.

A. 2-4-3-1
B. 4-2-3-1
C. 2-3-4-1
D. 4-3-2-1

<details>
<summary>💡 Hint</summary>
Cuci dulu (2), masuk panci (4), beri air (3), masak (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 2-4-3-1**
Urutan standar menyiapkan nasi sebelum dimasak.
</details>

### Soal #6: Algoritma Penilaian (Nested If)
"Jika nilai > 90, predikat A. Jika nilai 80-90, predikat B. Jika < 80, predikat C."
Berapa predikat untuk nilai tepat **80**?
A. A
B. B
C. C
D. Tidak terdefinisi

<details>
<summary>💡 Hint</summary>
Perhatikan rentang "80-90". Biasanya angka batas bawah ikut masuk ke dalam kategori tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B**
Karena 80 masuk dalam rentang minimal predikat B.
</details>

### Soal #7: Algoritma Menghitung Keliling Persegi
Input: Sisi (S). Algoritma manakah yang **SALAH**?
A. S + S + S + S
B. S x 4
C. S x S
D. 2 x (S + S)

<details>
<summary>💡 Hint</summary>
Ingat rumus keliling adalah total semua tepian, panjang x lebar adalah luas.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. S x S**
S x S adalah algoritma untuk mencari Luas, bukan Keliling.
</details>

### Soal #8: Algoritma "Tangga Darurat"
"Turun 2 lantai, lalu naik 1 lantai". Kamu mulai di lantai 5. Setelah melakukan algoritma itu 3 kali, di lantai berapa kamu?
A. Lantai 2
B. Lantai 3
C. Lantai 4
D. Lantai 1

<details>
<summary>💡 Hint</summary>
Setiap satu siklus, kamu turun $(2 - 1) = 1$ lantai.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Lantai 2**
Mulai di 5. Siklus 1: $5 - 1 = 4$. Siklus 2: $4 - 1 = 3$. Siklus 3: $3 - 1 = 2$.
</details>

### Soal #9: Algoritma "Antrian Bank"
Siapa yang paling dulu dilayani dalam algoritma antrian standar (FIFO - First In First Out)?
A. Yang paling tua.
B. Yang datang paling awal.
C. Yang paling cantik/ganteng.
D. Yang saldonya paling banyak.

<details>
<summary>💡 Hint</summary>
FIFO berarti "Yang pertama masuk, yang pertama dilayani".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Yang datang paling awal.**
Sistem antrian adil mendasarkan pada urutan kehadiran.
</details>

### Soal #10: Algoritma "Cari Nama di Kontak HP"
Kamu mencari nama "Yadi". Manakah cara yang paling tidak efektif (paling lambat)?
A. Klik huruf 'Y' di samping layar.
B. Ketik "Yadi" di kolom search.
C. Scroll satu per satu mulai dari huruf 'A'.
D. Meminta asisten suara memanggil Yadi.

<details>
<summary>💡 Hint</summary>
Pikirkan cara yang membutuhkan langkah (step) paling banyak bagi manusia atau komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Scroll dari huruf 'A'.**
Ini setara dengan *Linear Search* pada daftar yang sangat panjang, sangat tidak efisien.
</details>

### Soal #11: Algoritma Pengisian Galon
"Isi galon sampai penuh". Algoritma yang presisi bagi robot adalah...
A. Tuang air selamanya.
B. Ulangi: Tuang 1 liter air, JIKA galon penuh MAKA berhenti.
C. Tuang air lalu berdoa agar tidak tumpah.
D. Tuang 19 liter air tanpa mengecek kondisi.

<details>
<summary>💡 Hint</summary>
Algoritma butuh "Feedback Loop" (pemeriksaan kondisi) agar tidak terjadi *Overflow*.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ulangi: Tuang 1 liter, cek apakah penuh.**
Ini adalah bentuk pengulangan (Looping) dengan syarat berhenti (Condition).
</details>

### Soal #12: Algoritma "Cek Angka Genap"
Manakah langkah algoritma yang paling tepat untuk menentukan angka $N$ adalah genap?
A. Cek apakah $N$ bisa dikurangi 2.
B. Cek apakah sisa bagi $N$ dengan 2 adalah 0.
C. Cek apakah $N$ lebih besar dari 2.
D. Cek apakah $N$ diakhiri dengan angka 1.

<details>
<summary>💡 Hint</summary>
Gunakan konsep matematika Modulo (sisa bagi).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sisa bagi N dengan 2 adalah 0.**
Definisi angka genap adalah angka yang habis dibagi 2.
</details>

### Soal #13: Algoritma Membuat Kopi
Jika langkah "Tuangkan gula" diletakkan setelah "Aduk kopi hingga rata", apa risikonya?
A. Kopi tidak akan manis.
B. Gula mungkin belum larut sempurna dan kopi perlu diaduk kembali.
C. Kopi akan tumpah.
D. Gelas akan pecah.

<details>
<summary>💡 Hint</summary>
Algoritma mementingkan urutan untuk efisiensi. Mengaduk dua kali lebih boros energi daripada mengaduk sekali di akhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perlu diaduk kembali.**
Urutan yang tidak tepat menambah langkah (step) dalam proses solusi.
</details>

### Soal #14: Efektivitas Langkah
Manakah instruksi yang paling "Definite" (Jelas) bagi komputer?
A. Gambarlah kotak yang indah.
B. Gambarlah kotak dengan sisi 5 cm dan warna merah.
C. Gambarlah kotak yang cukup besar.
D. Coba gambar sesuatu berbentuk kotak.

<details>
<summary>💡 Hint</summary>
Komputer butuh angka dan parameter pasti, bukan opini atau perasaan (seperti "indah" atau "cukup").
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampirkan ukuran (5 cm) dan warna (Merah).**
Presisi adalah kunci dalam desain algoritma informatika.
</details>

### Soal #15: Algoritma "Lift Penuh"
"Jika berat beban > 500kg, bunyi alarm dan jangan jalan."
Jika beban saat ini 501kg, apa yang dilakukan lift sesuai algoritma?
A. Jalan pelan-pelan.
B. Membunyikan alarm dan tidak bergerak.
C. Mengeluarkan satu orang secara acak.
D. Tetap jalan karena hanya beda 1kg.

<details>
<summary>💡 Hint</summary>
Komputer mematuhi angka secara mutlak. 501 sudah memenuhi syarat "> 500".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bunyi alarm dan tidak jalan.**
Aturan algoritma harus dipatuhi secara ketat demi keamanan.
</details>

### Soal #16: Algoritma "Saldo Minimal"
"Transfer bisa dilakukan jika sisa saldo setelah transfer minimal Rp 50.000."
Saldo awal Budi: Rp 100.000. Budi ingin transfer Rp 60.000. Apakah berhasil?
A. Berhasil, saldo sisa Rp 40.000.
B. Tidak, karena sisa saldo akan menjadi di bawah Rp 50.000.
C. Berhasil, karena Budi punya uang cukup.
D. Gagal, karena bank butuh admin.

<details>
<summary>💡 Hint</summary>
$\text{Saldo Akhir} = \text{Saldo Awal} - \text{Transfer}$. Cek apakah $\text{Saldo Akhir} \ge 50.000$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak berhasil.**
$100.000 - 60.000 = 40.000$. Syarat minimal 50.000 tidak terpenuhi.
</details>

### Soal #17: Algoritma "Alarm Pagi"
1. JIKA hari Senin-Jumat, set alarm jam 06:00.
2. JIKA hari Sabtu-Minggu, jangan set alarm.
Hari ini adalah **Sabtu**. Apa status alarm?
A. Bunyi jam 06:00.
B. Tidak berbunyi.
C. Bunyi jam 08:00.
D. Laptop menyala sendiri.

<details>
<summary>💡 Hint</summary>
Analisis kondisi (Condition) hari dalam seminggu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak berbunyi.**
Sabtu masuk kategori hari libur sesuai algoritma tersebut.
</details>

### Soal #18: Algoritma Game "Flappy Bird"
"JIKA layar diketuk, MAKA burung naik. JIKA TIDAK, MAKA burung jatuh."
Jika kamu tidak menyentuh layar selama 5 detik, apa yang terjadi pada burung?
A. Berhenti di udara.
B. Tetap terbang stabil.
C. Jatuh ke bawah.
D. Kecepatan bertambah.

<details>
<summary>💡 Hint</summary>
Ketiadaan input (Else condition) memicu aksi jatuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Jatuh ke bawah.**
Respon sistem terhadap tidak adanya aksi pengguna.
</details>

### Soal #19: Algoritma "Lampu Otomatis"
Mulai jam 18:00 lampu menyala, jam 06:00 lampu mati. Berapa lama lampu menyala dalam satu hari?
A. 6 jam
B. 12 jam
C. 18 jam
D. 24 jam

<details>
<summary>💡 Hint</summary>
Hitung selisih waktu dari jam 6 sore sampai jam 6 pagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 12 jam**
Durasi malam hari (dari angka 18 ke 06) adalah tepat setengah hari.
</details>

### Soal #20: Algoritma Sorting "Tinggi Badan"
Ada 3 anak: Ali (150cm), Budi (145cm), Cici (155cm). Urutkan dari yang **tertinggi**.
A. Budi - Ali - Cici
B. Cici - Ali - Budi
C. Ali - Budi - Cici
D. Cici - Budi - Ali

<details>
<summary>💡 Hint</summary>
Urutan *Descending* (Paling besar ke paling kecil).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Cici - Ali - Budi**
155 > 150 > 145.
</details>

### Soal #21: Algoritma Mencari Kaus Kaki
Kamu punya 5 pasang kaus kaki acak di lantai. Algoritma paling efisien untuk memasangkan mereka adalah...
A. Ambil satu, lalu cari pasangannya satu per satu sampai ketemu.
B. Buat tumpukan berdasarkan warna dulu (Sorting), lalu pasangkan di dalam tiap tumpukan.
C. Tutup mata dan ambil dua secara acak.
D. Biarkan saja sampai ada orang lain yang merapikan.

<details>
<summary>💡 Hint</summary>
Mengelompokkan benda yang mirip (Sorting/Categorizing) sebelum memprosesnya biasanya lebih cepat daripada mencari satu-satu secara acak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Buat tumpukan berdasarkan warna (Sorting).**
Metode ini mengurangi jumlah perbandingan yang perlu dilakukan mata kita.
</details>

### Soal #22: Algoritma "Lampu Sensor Gerak"
1. JIKA ada gerakan terdeteksi, MAKA nyalakan lampu selama 10 detik.
2. JIKA dalam 10 detik ada gerakan baru, MAKA reset hitungan jadi 10 detik lagi.
Jika kamu masuk ruangan pada detik ke-0 dan diam mematung pada detik ke-5, kapan lampu mati?
A. Detik ke-10
B. Detik ke-15
C. Detik ke-5
D. Tidak pernah mati

<details>
<summary>💡 Hint</summary>
Gerakan terakhir terjadi pada detik ke-0 (saat masuk). Hitungan 10 detik dimulai dari sana.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Detik ke-10**
Karena tidak ada gerakan baru setelah detik ke-0, lampu akan mati tepat 10 detik setelah aktivitas terakhir.
</details>

### Soal #23: Algoritma Menyeberang Jalan
Urutan yang paling aman dan benar:
1. Tengok kanan.
2. Jalan menyeberang.
3. Tengok kiri.
4. Berhenti di pinggir jalan.

A. 4-1-3-1-2
B. 4-2-1-3
C. 1-3-2-4
D. 4-1-3-2

<details>
<summary>💡 Hint</summary>
Prinsip "Tengok Kanan - Tengok Kiri - Tengok Kanan Lagi" sebelum melangkah.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4-1-3-1-2**
Berhenti (4) -> Kanan (1) -> Kiri (3) -> Kanan lagi (1) untuk memastikan -> Seberang (2).
</details>

### Soal #24: Algoritma "Matematika Cepat"
$X = 10$. Ulangi 5 kali: "Tambahkan $X$ dengan 2". Berapa nilai akhir $X$?
A. 12
B. 20
C. 15
D. 20

<details>
<summary>💡 Hint</summary>
$10 + (2 \times 5) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 20**
Penjumlahan berulang sebanyak 5 kali menghasilkan 10 + 10 = 20.
</details>

### Soal #25: Algoritma "Urutan Masak Nasi"
1. Masukkan panci ke magic com dan klik tombol "Cook".
2. Cuci beras sampai bersih.
3. Masukkan air secukupnya.
4. Masukkan beras ke dalam panci.

A. 2-4-3-1
B. 4-2-3-1
C. 2-3-4-1
D. 4-3-2-1

<details>
<summary>💡 Hint</summary>
Cuci dulu (2), masuk panci (4), beri air (3), masak (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 2-4-3-1**
Urutan standar menyiapkan nasi sebelum dimasak.
</details>

### Soal #26: Algoritma Penilaian (Nested If)
"Jika nilai > 90, predikat A. Jika nilai 80-90, predikat B. Jika < 80, predikat C."
Berapa predikat untuk nilai tepat **80**?
A. A
B. B
C. C
D. Tidak terdefinisi

<details>
<summary>💡 Hint</summary>
Perhatikan rentang "80-90". Biasanya angka batas bawah ikut masuk ke dalam kategori tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B**
Karena 80 masuk dalam rentang minimal predikat B.
</details>

### Soal #27: Algoritma Menghitung Keliling Persegi
Input: Sisi (S). Algoritma manakah yang **SALAH**?
A. S + S + S + S
B. S x 4
C. S x S
D. 2 x (S + S)

<details>
<summary>💡 Hint</summary>
Ingat rumus keliling adalah total semua tepian, panjang x lebar adalah luas.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. S x S**
S x S adalah algoritma untuk mencari Luas, bukan Keliling.
</details>

### Soal #28: Algoritma "Tangga Darurat"
"Turun 2 lantai, lalu naik 1 lantai". Kamu mulai di lantai 5. Setelah melakukan algoritma itu 3 kali, di lantai berapa kamu?
A. Lantai 2
B. Lantai 3
C. Lantai 4
D. Lantai 1

<details>
<summary>💡 Hint</summary>
Setiap satu siklus, kamu turun $(2 - 1) = 1$ lantai.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Lantai 2**
Mulai di 5. Siklus 1: $5 - 1 = 4$. Siklus 2: $4 - 1 = 3$. Siklus 3: $3 - 1 = 2$.
</details>

### Soal #29: Algoritma "Antrian Bank"
Siapa yang paling dulu dilayani dalam algoritma antrian standar (FIFO - First In First Out)?
A. Yang paling tua.
B. Yang datang paling awal.
C. Yang paling cantik/ganteng.
D. Yang saldonya paling banyak.

<details>
<summary>💡 Hint</summary>
FIFO berarti "Yang pertama masuk, yang pertama dilayani".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Yang datang paling awal.**
Sistem antrian adil mendasarkan pada urutan kehadiran.
</details>

### Soal #30: Algoritma "Cari Nama di Kontak HP"
Kamu mencari nama "Yadi". Manakah cara yang paling tidak efektif (paling lambat)?
A. Klik huruf 'Y' di samping layar.
B. Ketik "Yadi" di kolom search.
C. Scroll satu per satu mulai dari huruf 'A'.
D. Meminta asisten suara memanggil Yadi.

<details>
<summary>💡 Hint</summary>
Pikirkan cara yang membutuhkan langkah (step) paling banyak bagi manusia atau komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Scroll dari huruf 'A'.**
Ini setara dengan *Linear Search* pada daftar yang sangat panjang, sangat tidak efisien.
</details>

### Soal #31: Algoritma Pengisian Galon
"Isi galon sampai penuh". Algoritma yang presisi bagi robot adalah...
A. Tuang air selamanya.
B. Ulangi: Tuang 1 liter air, JIKA galon penuh MAKA berhenti.
C. Tuang air lalu berdoa agar tidak tumpah.
D. Tuang 19 liter air tanpa mengecek kondisi.

<details>
<summary>💡 Hint</summary>
Algoritma butuh "Feedback Loop" (pemeriksaan kondisi) agar tidak terjadi *Overflow*.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ulangi: Tuang 1 liter, cek apakah penuh.**
Ini adalah bentuk pengulangan (Looping) dengan syarat berhenti (Condition).
</details>

### Soal #32: Algoritma "Cek Angka Genap"
Manakah langkah algoritma yang paling tepat untuk menentukan angka $N$ adalah genap?
A. Cek apakah $N$ bisa dikurangi 2.
B. Cek apakah sisa bagi $N$ dengan 2 adalah 0.
C. Cek apakah $N$ lebih besar dari 2.
D. Cek apakah $N$ diakhiri dengan angka 1.

<details>
<summary>💡 Hint</summary>
Gunakan konsep matematika Modulo (sisa bagi).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sisa bagi N dengan 2 adalah 0.**
Definisi angka genap adalah angka yang habis dibagi 2.
</details>

### Soal #33: Algoritma Membuat Kopi
Jika langkah "Tuangkan gula" diletakkan setelah "Aduk kopi hingga rata", apa risikonya?
A. Kopi tidak akan manis.
B. Gula mungkin belum larut sempurna dan kopi perlu diaduk kembali.
C. Kopi akan tumpah.
D. Gelas akan pecah.

<details>
<summary>💡 Hint</summary>
Algoritma mementingkan urutan untuk efisiensi. Mengaduk dua kali lebih boros energi daripada mengaduk sekali di akhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perlu diaduk kembali.**
Urutan yang tidak tepat menambah langkah (step) dalam proses solusi.
</details>

### Soal #34: Efektivitas Langkah
Manakah instruksi yang paling "Definite" (Jelas) bagi komputer?
A. Gambarlah kotak yang indah.
B. Gambarlah kotak dengan sisi 5 cm dan warna merah.
C. Gambarlah kotak yang cukup besar.
D. Coba gambar sesuatu berbentuk kotak.

<details>
<summary>💡 Hint</summary>
Komputer butuh angka dan parameter pasti, bukan opini atau perasaan (seperti "indah" atau "cukup").
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampirkan ukuran (5 cm) dan warna (Merah).**
Presisi adalah kunci dalam desain algoritma informatika.
</details>

### Soal #35: Algoritma "Lift Penuh"
"Jika berat beban > 500kg, bunyi alarm dan jangan jalan."
Jika beban saat ini 501kg, apa yang dilakukan lift sesuai algoritma?
A. Jalan pelan-pelan.
B. Membunyikan alarm dan tidak bergerak.
C. Mengeluarkan satu orang secara acak.
D. Tetap jalan karena hanya beda 1kg.

<details>
<summary>💡 Hint</summary>
Komputer mematuhi angka secara mutlak. 501 sudah memenuhi syarat "> 500".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bunyi alarm dan tidak jalan.**
Aturan algoritma harus dipatuhi secara ketat demi keamanan.
</details>

### Soal #36: Algoritma "Saldo Minimal"
"Transfer bisa dilakukan jika sisa saldo setelah transfer minimal Rp 50.000."
Saldo awal Budi: Rp 100.000. Budi ingin transfer Rp 60.000. Apakah berhasil?
A. Berhasil, saldo sisa Rp 40.000.
B. Tidak, karena sisa saldo akan menjadi di bawah Rp 50.000.
C. Berhasil, karena Budi punya uang cukup.
D. Gagal, karena bank butuh admin.

<details>
<summary>💡 Hint</summary>
$\text{Saldo Akhir} = \text{Saldo Awal} - \text{Transfer}$. Cek apakah $\text{Saldo Akhir} \ge 50.000$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak berhasil.**
$100.000 - 60.000 = 40.000$. Syarat minimal 50.000 tidak terpenuhi.
</details>

### Soal #37: Algoritma "Alarm Pagi"
1. JIKA hari Senin-Jumat, set alarm jam 06:00.
2. JIKA hari Sabtu-Minggu, jangan set alarm.
Hari ini adalah **Sabtu**. Apa status alarm?
A. Bunyi jam 06:00.
B. Tidak berbunyi.
C. Bunyi jam 08:00.
D. Laptop menyala sendiri.

<details>
<summary>💡 Hint</summary>
Analisis kondisi (Condition) hari dalam seminggu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak berbunyi.**
Sabtu masuk kategori hari libur sesuai algoritma tersebut.
</details>

### Soal #38: Algoritma Game "Flappy Bird"
"JIKA layar diketuk, MAKA burung naik. JIKA TIDAK, MAKA burung jatuh."
Jika kamu tidak menyentuh layar selama 5 detik, apa yang terjadi pada burung?
A. Berhenti di udara.
B. Tetap terbang stabil.
C. Jatuh ke bawah.
D. Kecepatan bertambah.

<details>
<summary>💡 Hint</summary>
Ketiadaan input (Else condition) memicu aksi jatuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Jatuh ke bawah.**
Respon sistem terhadap tidak adanya aksi pengguna.
</details>

### Soal #39: Algoritma "Lampu Otomatis"
Mulai jam 18:00 lampu menyala, jam 06:00 lampu mati. Berapa lama lampu menyala dalam satu hari?
A. 6 jam
B. 12 jam
C. 18 jam
D. 24 jam

<details>
<summary>💡 Hint</summary>
Hitung selisih waktu dari jam 6 sore sampai jam 6 pagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 12 jam**
Durasi malam hari (dari angka 18 ke 06) adalah tepat setengah hari.
</details>

### Soal #40: Algoritma Sorting "Tinggi Badan"
Ada 3 anak: Ali (150cm), Budi (145cm), Cici (155cm). Urutkan dari yang **tertinggi**.
A. Budi - Ali - Cici
B. Cici - Ali - Budi
C. Ali - Budi - Cici
D. Cici - Budi - Ali

<details>
<summary>💡 Hint</summary>
Urutan *Descending* (Paling besar ke paling kecil).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Cici - Ali - Budi**
155 > 150 > 145.
</details>

### Soal #41: Algoritma "Kode Diskon"
"Gunakan kode 'HEMAT' untuk diskon 10%". Budi mengetik 'hemat'. Apakah diskon aktif?
A. Ya, karena katanya sama.
B. Tergantung apakah sistemnya *Case Sensitive* (membedakan huruf besar/kecil) atau tidak.
C. Pasti ya.
D. Pasti tidak.

<details>
<summary>💡 Hint</summary>
Dalam algoritma komputer, 'A' and 'a' dianggap karakter yang berbeda di tingkat kode biner.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tergantung sistem (Case Sensitivity).**
Abstraksi karakter mengharuskan kita tahu apakah kapitalisasi berpengaruh pada validitas data.
</details>

### Soal #42: Algoritma Mencari Buku di Perpustakaan
Buku disusun berdasarkan kode nomor: 100-200-300 dst. Kamu mencari buku kode 250. Dimanakah lokasinya?
A. Di antara rak 100 dan 200.
B. Di antara rak 200 dan 300.
C. Di paling depan.
D. Di paling belakang.

<details>
<summary>💡 Hint</summary>
Gunakan konsep pengurutan angka untuk mempersempit area pencarian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Antara rak 200 dan 300.**
Prinsip dasar pengarsipan data yang terurut.
</details>

### Soal #43: Algoritma "Uang Pas"
Harga barang: Rp 7.500. Kamu bayar dengan Rp 10.000. Algoritma kasir untuk kembalian adalah...
A. $10.000 + 7.500$
B. $10.000 - 7.500$
C. $7.500 - 10.000$
D. $10.000 \div 7.500$

<details>
<summary>💡 Hint</summary>
Kembalian adalah selisih antara uang bayar dan harga.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10.000 - 7.500**
Operasi matematika dasar dalam algoritma transaksi.
</details>

### Soal #44: Langkah Keamanan (Firewall)
"Jika alamat IP ada di daftar hitam, tolak koneksi."
Alamat 1.2.3.4 ada di daftar hitam. Apa yang terjadi saat ia mencoba masuk?
A. Diizinkan karena hanya satu IP.
B. Akses ditolak (Block).
C. Diminta password baru.
D. Kecepatan internetnya dikurangi.

<details>
<summary>💡 Hint</summary>
Filtrasi data berdasarkan aturan (Rule-based Filter).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Akses ditolak.**
Implementasi aturan keamanan yang tegas dalam jaringan.
</details>

### Soal #45: Algoritma "Resep Kue" (Parallelism)
"Sambil menunggu oven panas (10 menit), kocoklah telur dan gula."
Keuntungan dari algoritma ini adalah...
A. Kue jadi lebih enak.
B. Menghemat waktu secara keseluruhan (Efisien).
C. Telur jadi lebih mengembang.
D. Oven tidak cepat rusak.

<details>
<summary>💡 Hint</summary>
Melakukan dua pekerjaan dalam satu rentang waktu disebut *Concurrency* atau tugas paralel.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghemat waktu (Efisien).**
Algoritma yang baik mengoptimalkan penggunaan sumber daya (dalam hal ini, waktu).
</details>

### Soal #46: Algoritma Penentuan Tahun Kabisat
Sebuah tahun adalah kabisat jika habis dibagi 4. Manakah tahun kabisat?
A. 2021
B. 2022
C. 2023
D. 2024

<details>
<summary>💡 Hint</summary>
Cek apakah dua angka terakhir tahun tersebut habis dibagi 4.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. 2024**
$24 \div 4 = 6$ (tanpa sisa).
</details>

### Soal #47: Algoritma "Password Strength"
"Password minimal 8 karakter". Kamu mengetik "1234567". Apakah diterima?
A. Ya, karena angka semua.
B. Tidak, karena baru 7 karakter.
C. Ya, karena mudah diingat.
D. Tidak, karena tidak ada huruf besar.

<details>
<summary>💡 Hint</summary>
Algoritma validasi panjang string (Length validation).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak, baru 7 karakter.**
Password harus memenuhi syarat minimal yang ditetapkan algoritma keamanan.
</details>

### Soal #48: Algoritma "Cuci Mobil Otomatis"
1. Semprot air.
2. Sabun seluruh bodi.
3. Sikat bodi.
4. Bilas.
5. Keringkan.
Tahap mana yang menghilangkan kotoran secara fisik paling banyak?
A. 1
B. 3
C. 5
D. 4

<details>
<summary>💡 Hint</summary>
Sikat (3) adalah proses mekanik untuk melepaskan kotoran yang menempel kuat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 3 (Sikat bodi)**
Proses inti pembersihan dalam algoritma pencucian.
</details>

### Soal #49: Algoritma "Jalan Terpendek"
Tujuan di kota B. Jalur 1 (Macet, 10km, 30 menit). Jalur 2 (Lancer, 15km, 15 menit). Mana yang dipilih algoritma GPS tercepat?
A. Jalur 1 karena lebih pendek jaraknya.
B. Jalur 2 karena lebih sedikit waktunya.
C. Jalur 1 karena seru macetnya.
D. Jalur 2 karena jalannya lebih jauh.

<details>
<summary>💡 Hint</summary>
Optimasi algoritma bergantung pada kriteria: apakah mencari "Terpendek Jarak" atau "Tercepat Waktu"?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jalur 2 (Tercepat).**
Biasanya pengguna lebih memprioritaskan waktu tempuh dalam navigasi.
</details>

### Soal #50: Algoritma "Mode Hemat"
"Jika baterai < 20%, turunkan kecerahan layar ke 50%."
Baterai HP kamu 19%. Apa yang terjadi pada layar?
A. Layar mati.
B. Layar menjadi agak redup (50%).
C. Layar tetap terang.
D. HP langsung meledak.

<details>
<summary>💡 Hint</summary>
Kondisi "< 20%" sudah terpenuhi oleh angka 19%.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Layar menjadi agak redup.**
Implementasi manajemen energi otomatis.
</details>

### Soal #51: Algoritma "Kelipatan 5"
Tuliskan angka kelipatan 5 antara 1 sampai 21. Berapa angka terakhir yang ditulis?
A. 20
B. 21
C. 25
D. 15

<details>
<summary>💡 Hint</summary>
Bilangan kelipatan 5: 5, 10, 15, 20. Cek batas atasnya (21).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 20**
Angka 20 adalah kelipatan 5 terbesar yang masih di bawah 21.
</details>

### Soal #52: Algoritma "Parkir Mall"
1 jam pertama Rp 5.000. Setiap jam berikutnya Rp 2.000. Berapa biaya parkir 3 jam?
A. Rp 7.000
B. Rp 9.000
C. Rp 11.000
D. Rp 15.000

<details>
<summary>💡 Hint</summary>
Total = (Jam 1) + (Sisa Jam x Harga per jam).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 9.000**
$5.000 + (2 \times 2.000) = 5.000 + 4.000 = 9.000$.
</details>

### Soal #53: Algoritma "Trace Variabel"
1. $A = 5$
2. $B = A + 3$
3. $A = B - 2$
Berapa nilai $A$ dan $B$ sekarang?
A. $A=5, B=8$
B. $A=6, B=8$
C. $A=8, B=8$
D. $A=6, B=5$

<details>
<summary>💡 Hint</summary>
Ikuti baris demi baris. Nilai variabel bisa berubah (Update) seiring jalannya langkah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. A=6, B=8**
$B = 5+3=8$. Lalu $A = 8-2=6$.
</details>

### Soal #54: Algoritma "Cari Nama Terpanjang"
Daftar: "Ani", "Budi", "Candra". Manakah yang dipilih algoritma pencari kata terpanjang?
A. Ani
B. Budi
C. Candra
D. Semua sama

<details>
<summary>💡 Hint</summary>
Hitung jumlah karakter (huruf) pada masing-masing kata.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Candra**
Candra memiliki 6 huruf, lebih banyak dari Ani (3) dan Budi (4).
</details>

### Soal #55: Algoritma Penukaran (3 Variabel)
$X=1, Y=2, Z=3$.
1. Pindahkan isi $X$ ke $W$ (cadangan).
2. Pindahkan isi $Y$ ke $X$.
3. Pindahkan isi $Z$ ke $Y$.
4. Pindahkan isi $W$ ke $Z$.
Berapa urutan isi $X, Y, Z$ sekarang?
A. 2, 3, 1
B. 1, 2, 3
C. 3, 2, 1
D. 2, 1, 3

<details>
<summary>💡 Hint</summary>
Isi $X$ jadi 2, isi $Y$ jadi 3, isi $Z$ jadi nilai awal $X$ (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 2, 3, 1**
Ini adalah algoritma pergeseran nilai (*Shift*).
</details>

### Soal #56: Algoritma "Tiket Bioskop"
"Anak-anak (di bawah 12 thn) diskon 50%". Umur Dito 12 tahun tepat. Apakah diskon?
A. Ya, karena masih sekolah.
B. Tidak, karena syaratnya harus "di bawah" 12 (artinya 0-11 tahun).
C. Ya, karena 12 masih kecil.
D. Berkurang dikit.

<details>
<summary>💡 Hint</summary>
Perhatikan kata kunci "di bawah" (<) vs "di bawah atau sama dengan" ($\le$).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak diskon.**
Dalam logika kaku, 12 tidak lebih kecil dari 12.
</details>

### Soal #57: Algoritma Loop "Terhenti"
"Ulangi: Makan 1 suap nasi, sampai piring kosong". Jika piring sudah kosong dari awal, apa yang dilakukan?
A. Tetap makan sekali.
B. Tidak makan sama sekali (Langsung selesai).
C. Menangis.
D. Makan piringnya.

<details>
<summary>💡 Hint</summary>
Pengecekan kondisi dilakukan di awal sebelum aksi (While Loop).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak makan sama sekali.**
Jika kondisi berhenti sudah terpenuhi di awal, proses tidak dijalankan.
</details>

### Soal #58: Algoritma "Matikan Komputer"
Manakah langkah terakhir yang benar sesuai standar software?
A. Cabut kabel listrik.
B. Tunggu layar benar-benar gelap barulah cabut daya.
C. Klik tombol Start -> Shutdown.
D. Pencet tombol power di CPU berulang kali.

<details>
<summary>💡 Hint</summary>
Satu langkah krusial untuk memastikan semua data sudah tersimpan aman di disk sebelum daya hilang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tunggu layar gelap baru cabut daya.**
Shutdown software memicu proses penutupan file, langkah terakhir adalah memastikan hardware benar-benar mati.
</details>

### Soal #59: Algoritma "Cek Password"
"Input: Admin123". Password asli: "admin123". Apakah login berhasil?
A. Berhasil, karena hurufnya sama.
B. Gagal, karena 'A' besar berbeda with 'a' kecil.
C. Berhasil jika HP-nya ramah.
D. Berhasil jika usernamenya benar.

<details>
<summary>💡 Hint</summary>
Aplikasi keamanan hampir selalu membedakan casing (*Case Sensitive*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gagal.**
Ketelitian karakter sangat penting dalam algoritma otentikasi.
</details>

### Soal #60: Algoritma "Jalan di Labirin"
"Selalu pegang dinding sebelah kanan dan ikuti terus". Apakah algoritma ini menjamin kamu keluar?
A. Ya, untuk labirin tipe sederhana (tanpa pulau di tengah).
B. Tidak, hanya akan membuat pusing.
C. Ya, jika labirinnya terbuat dari kaca.
D. Tidak, kamu akan terjebak selamanya.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma klasik *Wall Follower*.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya (untuk mayoritas labirin standar).**
Teknik ini memastikan eksplorasi yang teratur di sepanjang sirkuit labirin.
</details>

### Soal #61: Algoritma Belanja di Kantin
Budi ingin membeli nasi (Rp 5.000) dan es teh (Rp 2.000). Dia punya uang Rp 10.000. Algoritma kembalian yang benar adalah...
A. $10.000 - 5.000 + 2.000$
B. $10.000 - (5.000 + 2.000)$
C. $(10.000 - 5.000) - 2.000$
D. Jawaban B dan C benar secara matematis.

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana uang total dikurangi oleh jumlah semua belanjaan sekaligus, atau dikurangi satu-persatu.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Jawaban B dan C benar.**
Dalam algoritma, kita bisa menjumlahkan pengeluaran dulu ($5.000+2.000=7.000$) baru dikurangi ($10.000-7.000=3.000$), atau mengurangi perlahan ($10.000-5.000=5.000$, lalu $5.000-2.000=3.000$).
</details>

### Soal #62: Algoritma "Download Game"
Kecepatan download 2 MB/detik. Ukuran game 120 MB. Berapa menit waktu yang dibutuhkan?
A. 60 menit
B. 1 menit
C. 10 menit
D. 2 menit

<details>
<summary>💡 Hint</summary>
Waktu (detik) = Total Ukuran / Kecepatan. Lalu ubah ke menit (1 menit = 60 detik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1 menit**
$120 / 2 = 60$ detik. 60 detik = 1 menit.
</details>

### Soal #63: Algoritma "Posting Foto IG"
Manakah langkah yang merupakan bagian dari "Proses" (bukan Input/Output)?
A. Memilih foto dari galeri.
B. Menulis caption.
C. Menerapkan filter efek pada foto.
D. Foto muncul di feed teman.

<details>
<summary>💡 Hint</summary>
Proses adalah tindakan mengubah atau memodifikasi data (foto) yang sudah ada.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Menerapkan filter.**
Input adalah foto/caption, output adalah tampilan di feed. Perubahan visual oleh filter adalah proses pengolahan citra.
</details>

### Soal #64: Algoritma "Antre Fotokopi"
Ada 3 siswa: A (10 lembar), B (50 lembar), C (5 lembar). Pemilik fotokopi ingin semua cepat selesai (tunggu paling singkat). Siapa yang harus difotokopi pertama?
A. Siswa B karena paling banyak untungnya.
B. Siswa A karena di tengah.
C. Siswa C karena paling sedikit jumlahnya (SJF - Shortest Job First).
D. Sesuai urutan kedatangan saja.

<details>
<summary>💡 Hint</summary>
Untuk meminimalkan waktu tunggu rata-rata, selesaikan tugas yang paling cepat (paling sedikit lembarannya) terlebih dahulu.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Siswa C.**
Ini adalah algoritma *Shortest Job First*. Jika C dikerjakan dulu (5 lembar), maka A dan B tidak perlu menunggu lama proses 50 lembar milik B.
</details>

### Soal #65: Algoritma "Pin HP (Brute Force)"
PIN HP terdiri dari 4 angka (0000-9999). Jika kamu mencoba dari 0000, 0001, 0002... sampai ketemu, apa nama algoritma ini?
A. Binary Search
B. Random Search
C. Brute Force (Linear Search)
D. Hacking Search

<details>
<summary>💡 Hint</summary>
Mencoba semua kemungkinan satu per satu tanpa strategi khusus.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Brute Force.**
Metode ini pasti berhasil tapi membutuhkan waktu paling lama jika kuncinya ada di angka besar (misal 9998).
</details>

### Soal #66: Algoritma "Mandi Pagi"
1. Gosok gigi.
2. Pakai baju.
3. Guyur badan dengan air.
4. Pakai sabun.
Manakah langkah yang melanggar logika jika diletakkan paling akhir?
A. 1
B. 2
C. 3
D. 4

<details>
<summary>💡 Hint</summary>
Kamu tidak bisa memakai baju (2) baru kemudian menyiram badan (3), baju akan basah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2 (Pakai baju).**
Memakai baju harus dilakukan setelah badan kering/selesai mandi.
</details>

### Soal #67: Algoritma "Belajar Ujian"
"Belajarlah 25 menit, istirahat 5 menit. Ulangi 4 kali."
Berapa total waktu yang dihabiskan untuk **belajar saja**?
A. 120 menit
B. 100 menit
C. 30 menit
D. 200 menit

<details>
<summary>💡 Hint</summary>
Hanya hitung durasi belajarnya: $25 \times 4$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 100 menit**
$25 \text{ menit} \times 4 \text{ siklus} = 100 \text{ menit}$.
</details>

### Soal #68: Algoritma "Urutan Rank Game"
Rank: Bronze, Silver, Gold, Platinum.
Bila sistem menggunakan algoritma $Rank\_Points > 1000$ untuk naik ke Silver. Budi punya 999 poin. Apa Rank Budi?
A. Silver
B. Bronze
C. Gold
D. Platinum

<details>
<summary>💡 Hint</summary>
999 belum lebih besar dari 1000.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bronze**
Kurang 1 poin saja tetap dianggap belum memenuhi syarat algoritma kenaikan tingkat.
</details>

### Soal #69: Algoritma "Cek Login Caps Lock"
Username: "SiswaSMA". Kamu mengetik "siswasma". Jika sistem bersifat *Case Sensitive*, apakah berhasil?
A. Berhasil, karena hurufnya sama.
B. Gagal, karena 'S' dan 's' berbeda.
C. Berhasil jika password benar.
D. Berhasil karena sistem memaafkan kesalahan kecil.

<details>
<summary>💡 Hint</summary>
Informatika sangat presisi. Perubahan besar-kecil dianggap data yang berbeda.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gagal.**
Case-sensitive berarti membedakan huruf besar dan kecil secara mutlak.
</details>

### Soal #70: Algoritma "E-Money"
1. Tempel kartu.
2. JIKA saldo cukup, MAKA pintu terbuka dan kurangi saldo.
3. JIKA TIDAK, MAKA bunyi "Tetot" dan pintu tetap tutup.
Apa yang disebut sebagai **Input** di sini?
A. Bunyi "Tetot".
B. Pintu terbuka.
C. Saldo berkurang.
D. Penempelan kartu dan data saldo kartu.

<details>
<summary>💡 Hint</summary>
Input adalah pemicu atau data awal yang diterima sensor.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Penempelan kartu dan saldo.**
Aktivitas fisik pengguna dan data di dalam kartu adalah sumber input bagi mesin.
</details>

### Soal #71: Algoritma "Cari Teman di Kerumunan"
Cara paling sistematis mencari teman yang memakai baju merah di lapangan upacara adalah...
A. Teriak sekencang mungkin.
B. Memindai barisan mulai dari pojok kiri depan satu-persatu ke kanan (Scanning).
C. Berlari acak ke tengah lapangan.
D. Menunggu di depan gerbang.

<details>
<summary>💡 Hint</summary>
Gunakan algoritma *Linear Search* visual yang teratur agar tidak ada area yang terlewat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memindai barisan secara teratur.**
Ini memastikan setiap objek (siswa) diperiksa setidaknya sekali.
</details>

### Soal #72: Algoritma "Menu GoFood"
Urutan: Masukkan alamat -> Pilih Restoran -> Pilih Makanan -> Bayar.
Kenapa alamat harus dimasukkan di awal?
A. Biar aplikasi tahu jarak dan ongkir sebelum kamu belanja.
B. Iseng saja.
C. Biar restorannya tahu kamu siapa.
D. Agar makanan tidak dingin.

<details>
<summary>💡 Hint</summary>
Alamat digunakan sebagai filter awal untuk menentukan restoran mana saja yang "Available" (tersedia) untuk menjangkaumu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menentukan jarak dan ongkir.**
Input lokasi adalah syarat efisiensi algoritma pengiriman.
</details>

### Soal #73: Algoritma "Sorting Tinggi" (Bubble Sort)
Ali (160), Budi (150). Instruksi: "Jika yang kiri lebih tinggi dari yang kanan, tukar posisi."
Apakah mereka bertukar posisi?
A. Tidak tetap di tempat.
B. Ya, Ali pindah ke kanan dan Budi ke kiri.
C. Bergantung perintah guru.
D. Keduanya jongkok.

<details>
<summary>💡 Hint</summary>
Bandingkan 160 (kiri) and 150 (kanan). 160 > 150 adalah Benar (Ya).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ya, mereka tukar posisi.**
Ini adalah satu langkah dasar dalam *Bubble Sort* untuk mengurutkan dari yang terkecil.
</details>

### Soal #74: Algoritma "Loop Matematika"
$N = 1$. Ulangi: $N = N \times 2$ sebanyak 4 kali. Apa hasil akhir $N$?
A. 8
B. 16
C. 4
D. 32

<details>
<summary>💡 Hint</summary>
$1 \times 2 = 2 \rightarrow 2 \times 2 = 4 \rightarrow 4 \times 2 = 8 \rightarrow 8 \times 2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 16**
Eksponensial 2 pangkat 4 ($2^4 = 16$).
</details>

### Soal #75: Algoritma "Kapasitas Lift"
Maksimum 5 orang. Jika ada 12 orang ingin naik, berapa kali lift harus bolak-balik?
A. 2 kali
B. 3 kali
C. 2,4 kali
D. 12 kali

<details>
<summary>💡 Hint</summary>
Gunakan pembulatan ke atas (*Ceiling*): $12 / 5 = 2.4$. Karena manusia tidak bisa dibagi, maka butuh satu trip lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 3 kali**
Trip 1 (5 orang), Trip 2 (5 orang), Trip 3 (2 orang). Total 12 orang.
</details>

### Soal #76: Algoritma "Isi Daya HP"
1. Colok charger ke listrik.
2. Hubungkan kabel ke HP.
3. JIKA daya naik, MAKA biarkan.
4. JIKA baterai 100%, MAKA cabut.
Apa "Exit Condition" (Kondisi Keluar) dari algoritma ini?
A. Daya naik.
B. Colok listrik.
C. Baterai mencapai 100%.
D. HP meledak.

<details>
<summary>💡 Hint</summary>
Condition yang membuat pengulangan/proses berhenti secara normal.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Baterai 100%.**
Inilah tujuan akhir dan titik henti algoritma pengisian daya.
</details>

### Soal #77: Algoritma "Cari Kunci Hilang"
Ibu bilang: "Cari di laci, kalau tidak ada cari di meja, kalau tidak ada cari di tas."
Kunci ternyata ada di meja. Laci sudah diperiksa. Apakah tas perlu diperiksa?
A. Perlu, buat jaga-jaga.
B. Tidak perlu, karena algoritma berhenti saat barang ditemukan.
C. Tergantung perintah ibu lagi.
D. Tasnya saja yang dibawa.

<details>
<summary>💡 Hint</summary>
Efisiensi berarti berhenti segera setelah solusi (Output) tercapai.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak perlu diperiksa.**
Dalam algoritma pencarian, kita berhenti memeriksa objek lain jika target sudah ditemukan.
</details>

### Soal #78: Algoritma "Sorting Nilai"
80, 95, 70. Urutkan dari yang **terbesar** (Descending).
A. 70, 80, 95
B. 95, 80, 70
C. 80, 70, 95
D. 95, 70, 80

<details>
<summary>💡 Hint</summary>
Urutan dari angka yang paling tinggi nilainya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 95, 80, 70**
Standard sorting descending untuk menentukan juara atau peringkat.
</details>

### Soal #79: Algoritma "Google Translate"
1. Terima input teks bahasa Inggris.
2. Cari padanan kata di database bahasa Indonesia.
3. Susun berdasarkan aturan tata bahasa (Grammar).
4. Tampilkan hasil.
Manakah yang merupakan tahapan **Abstraksi** di dalam algoritma ini?
A. Menampilkan hasil di layar.
B. Mengabaikan jenis font atau warna teks input dan hanya fokus pada makna katanya.
C. Mencari kata di database.
D. Mengetik teks di keyboard.

<details>
<summary>💡 Hint</summary>
Ingat, abstraksi adalah membuang detail yang tidak penting bagi proses inti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengabaikan font/warna.**
Bagi penerjemah, warna teks tidak penting, yang penting adalah makna katanya.
</details>

### Soal #80: Algoritma "Alarm Snooze"
"Bunyi alarm setiap 5 menit jika tombol snooze ditekan."
Alarm mulai jam 06:00. Kamu tekan snooze 3 kali. Jam berapa akhirnya kamu benar-benar bangun (asumsi setelah snooze ketiga langsung bangun)?
A. 06:05
B. 06:10
C. 06:15
D. 06:30

<details>
<summary>💡 Hint</summary>
Satu kali snooze = 5 menit. $3 \times 5 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 06:15**
$06:00 + (3 \times 5 \text{ menit}) = 06:15$.
</details>
### Soal #81: Algoritma "Pesan Driver"
Sistem mencari driver yang jaraknya kurang dari 2 km dari pemesan.
Driver A: 1.5 km. Driver B: 2.1 km. Driver C: 0.5 km.
Siapa yang masuk dalam radar sistem?
A. A saja
B. C saja
C. A dan C
D. Semuanya

<details>
<summary>💡 Hint</summary>
Filter kondisi: $Jarak < 2$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. A dan C.**
1.5 dan 0.5 lebih kecil dari 2, sedangkan 2.1 lebih besar.
</details>

### Soal #82: Algoritma "Password Wifi"
Password: 'internetgratis'. Temanmu mengetik 'internet gratis' (pake spasi). Kenapa gagal?
A. Karena spasi dianggap karakater kosong yang tetap dihitung oleh sistem.
B. Karena internet tidak pernah gratis.
C. Karena sinyal lemah.
D. Karena hurufnya kekecilan.

<details>
<summary>💡 Hint</summary>
Dalam string komputer, spasi memiliki kode biner sendiri (ASCII 32).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Spasi dihitung sebagai karakter.**
Kecuali algoritma diprogram untuk mengabaikan spasi (*trim*), maka input harus persis sama.
</details>

### Soal #83: Algoritma "Playlist Shuffle"
Bagaimana algoritma memutar lagu secara acak?
A. Selalu putar lagu favorit saja.
B. Memberikan angka acak (Random Number) pada setiap lagu dan memutarnya sesuai nomor tersebut.
C. Memutar lagu berdasarkan abjad tapi terbalik.
D. Menunggu perintah suara.

<details>
<summary>💡 Hint</summary>
Gunakan fungsi *Randomize* untuk menentukan urutan indek lagu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menggunakan angka acak.**
Ini menjamin variasi putar yang berbeda setiap kali mode Shuffle diaktifkan.
</details>

### Soal #84: Algoritma "Traffic Light" (Definiteness)
Lampu kuning berarti "Hati-hati". Kenapa instruksi ini dianggap kurang presisi bagi mobil otonom?
A. Karena warna kuning itu bagus.
B. Karena kata "Hati-hati" bermakna ganda (ambigu). Harusnya "Pelankan kecepatan hingga 20km/jam".
C. Karena mobil tidak bisa melihat warna.
D. Karena mobil otonom tidak punya hati.

<details>
<summary>💡 Hint</summary>
Algoritma butuh instruksi kuantitatif (angka/aksi pasti), bukan kualitatif (perasaan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bermakna ganda (Ambigu).**
Syarat *Definiteness* mengharuskan instruksi tidak menimbulkan banyak tafsir.
</details>

### Soal #85: Algoritma "Nabung Keinginan"
Beli sepatu Rp 300.000. Tabungan tiap hari Rp 10.000. Berapa hari sampai uang terkumpul?
A. 10 hari
B. 20 hari
C. 30 hari
D. 300 hari

<details>
<summary>💡 Hint</summary>
$Target / Harian = Jumlah Hari$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 30 hari.**
$300.000 / 10.000 = 30$.
</details>

### Soal #86: Algoritma "Mode Malam HP"
1. JIKA jam > 22:00, MAKA aktifkan filter cahaya kuning.
2. JIKA jam jam < 06:00, MAKA tetap aktifkan.
3. JIKA TIDAK, matikan.
Jam menunjukkan **23:30**. Apa warna layar?
A. Biru tajam
B. Putih terang
C. Kekuningan (Warm)
D. Hitam total

<details>
<summary>💡 Hint</summary>
Kondisi nomor 1 terpenuhi karena 23:30 lebih besar dari 22:00.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kekuningan (Warm).**
Logika "Night Shift" atau "Blue Light Filter" otomatis.
</details>

### Soal #87: Algoritma "Cari Teman Sebangku"
Kamu lupa teman sebangkumu siapa. Kamu mengecek daftar absen. Dimana biasanya teman sebangkumu berada di daftar?
A. Di urutan paling atas.
B. Di nomor yang berdekatan dengan nomor absenmu (misal tepat di atas atau di bawahmu).
C. Di paling bawah.
D. Tidak ada di absen.

<details>
<summary>💡 Hint</summary>
Sistem pembagian bangku sekolah seringkali menggunakan urutan absen (Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dekat dengan nomor absenmu.**
Pemanfaatan pola (Pattern Recognition) membantu mempercepat algoritma pencarian.
</details>

### Soal #88: Algoritma "Game RPG - Level Up"
"Setiap naik level, HP (Health Point) bertambah 10% dari HP sebelumnya."
HP Level 1: 100. Berapa HP Level 3?
A. 120
B. 110
C. 121
D. 130

<details>
<summary>💡 Hint</summary>
Lvl 2: $100 + (10\% \times 100) = 110$. Lvl 3: $110 + (10\% \times 110) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 121**
Penambahan bersifat bunga majemuk ($100 \rightarrow 110 \rightarrow 121$).
</details>

### Soal #89: Algoritma "Cek Keranjang Shopee"
Ada 5 barang di keranjang. Kamu ingin checkout semuanya. Langkah mana yang dilakukan berulang (Looping)?
A. Klik tombol "Checkout".
B. Memasukkan alamat pengiriman.
C. Menghitung (Harga barang x Jumlah) untuk setiap item satu-persatu.
D. Mengklik metode pembayaran.

<details>
<summary>💡 Hint</summary>
Looping terjadi pada proses yang harus dilakukan pada setiap individu di dalam kumpulan (Koleksi barang).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Menghitung harga per item.**
Sistem akan mengulang kalkulasi untuk item 1, lalu item 2, dan seterusnya.
</details>

### Soal #90: Algoritma "Lupa Password"
1. Masukkan email.
2. Klik "Kirim kode".
3. Cek kode di email.
4. Masukkan kode ke website.
5. Masukkan password baru 2 kali.
Kenapa disuruh masukkan password baru **2 kali**?
A. Biar website makin aman.
B. Sebagai mekanisme validasi (Input 1 harus sama dengan Input 2) untuk menghindari typo.
C. Iseng saja.
D. Biar kamu hafal.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma *Double Check* untuk meyakinkan data input sudah benar sebelum disimpan permanen.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mekanisme validasi typo.**
Kesalahan pengetikan satu huruf saja bisa membuat user tidak bisa login lagi nanti, maka dilakukan pengecekan kembar.
</details>

### Soal #91: Algoritma "Sortir Beras"
Kamu punya 1 kg beras campur krikil kecil. Algoritma paling pas adalah...
A. Mengambil satu per satu butir beras sampai krikil tersisa (Lambat).
B. Menggunakan ayakan/saringan yang lubangnya pas buat beras tapi menahan krikil (Abstraksi Fisik).
C. Mencuci beras sampai krikil hilang.
D. Memakan semuanya.

<details>
<summary>💡 Hint</summary>
Gunakan filter yang memanfaatkan perbedaan fisis (ukuran) antara beras dan krikil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menggunakan ayakan.**
Penggunaan alat (filter) jauh lebih efektif daripada pengecekan manual satu-persatu.
</details>

### Soal #92: Algoritma "Smart CCTV"
"JIKA wajah terdeteksi bukan anggota keluarga, MAKA kirim notifikasi bahaya."
Berapa output yang mungkin dari algoritma ini (binary)?
A. Banyak sekali.
B. Dua (Ya/Tidak atau Bahaya/Aman).
C. Tidak ada.
D. Wajah orang asing.

<details>
<summary>💡 Hint</summary>
Kondisi Boolean (If-Else) selalu menghasilkan salah satu dari dua pilihan aksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dua (Bahaya/Aman).**
Logika digital dasar berbasis pada dua kondisi nilai.
</details>

### Soal #93: Algoritma "Trace Jalur Tikus"
X=5, Y=10.
1. X = X + Y
2. Y = X - Y
3. X = X - Y
Apa nilai X dan Y sekarang?
A. X=5, Y=10
B. X=10, Y=5
C. X=15, Y=15
D. X=0, Y=0

<details>
<summary>💡 Hint</summary>
Langkah 1: $X=15$. Langkah 2: $Y=15-10=5$. Langkah 3: $X=15-5=10$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. X=10, Y=5**
Ini adalah algoritma klasik untuk **menukar isi dua variabel** tanpa variabel bantuan.
</details>

### Soal #94: Algoritma "Cuci Tangan Robot"
Sebuah instruksi: "Bilas tangan selama 20 detik."
Robot melakukan: Menaruh tangan di bawah kran tanpa membuka kran, diam 20 detik, selesai.
Salahnya di mana?
A. Waktunya kelamaan.
B. Instruksi kurang detail (Definiteness) - tidak ada perintah "Nyalakan kran".
C. Robotnya malas.
D. Kran airnya rusak.

<details>
<summary>💡 Hint</summary>
Komputer tidak punya akal sehat. Jika tidak diperintah "Buka air", ia tidak akan membukanya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kurang detail.**
Algoritma harus menyertakan semua langkah prasyarat sebelum aksi utama dilakukan.
</details>

### Soal #95: Algoritma "Password Wifi Kafe"
"Beli kopi, di struk ada kode, masukkan kode".
Kenapa kode di struk selalu berubah setiap hari?
A. Biar keren.
B. Agar orang di luar kafe tidak bisa pakai wifi selamanya (Keamanan & Finiteness Akses).
C. Tintanya masih banyak.
D. Kasirnya gabut.

<details>
<summary>💡 Hint</summary>
Pembatasan akses (Authorization) seringkali menggunakan algoritma waktu terbatas (*Time-based access*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Keamanan & Pembatasan Akses.**
Membatasi masa berlaku password adalah bagian dari desain keamanan algoritma jaringan.
</details>

### Soal #96: Algoritma "Sorting Pakaian"
Kamu ingin mengurutkan baju dari yang paling sering dipakai ke yang paling jarang. Ini disebut sorting berdasarkan...
A. Nama merk.
B. Warna.
C. Frekuensi (Popularity Sort).
D. Harga.

<details>
<summary>�� Hint</summary>
Pilih kriteria yang mencerminkan "jumlah penggunaan".
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Frekuensi.**
Algoritma ini sering dipakai YouTube untuk menampilkan "Most Viewed" videos.
</details>

### Soal #97: Algoritma "Naik Ojek Online"
1. Buka aplikasi.
2. Cari tujuan.
3. Pesan.
4. Tunggu driver.
5. Perjalanan.
6. Beri bintang.
Langkah 6 merupakan...
A. Input bagi driver.
B. Feedback bagi algoritma sistem untuk menilai performa driver.
C. Iseng saja.
D. Kewajiban moral.

<details>
<summary>💡 Hint</summary>
Data dari user di akhir proses digunakan sistem untuk meningkatkan kualitas layanan berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Feedback system.**
Data rating masuk ke algoritma reputasi driver dalam database pusat.
</details>

### Soal #98: Algoritma "Matematika Gampang"
"Tambahkan 1 ke angka X, ulangi sampai X mencapai 10". Jika mulai dari X = 11, apa yang terjadi?
A. Berhenti di 10.
B. Error, atau berputar selamanya (Infinite Loop) jika pengecekannya hanya "X == 10".
C. Kembali ke 0.
D. Angka 11 hilang.

<details>
<summary>💡 Hint</summary>
Jika kamu di angka 11 dan terus menambah, kamu tidak akan pernah bertemu angka 10.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Infinite Loop (atau berputar selamanya).**
Penting bagi algoritma memiliki syarat berhenti yang logis untuk setiap kemungkinan input.
</details>

### Soal #99: Algoritma "Cek Lulus Ujian"
Syarat: Nilai Matematika > 70 **DAN** Nilai Bahasa > 70.
Budi: Mat=90, Bahasa=65. Apakah Budi lulus?
A. Lulus, kan rata-ratanya tinggi.
B. Tidak Lulus, karena syarat DAN mewajibkan keduanya benar.
C. Lulus, bahasa bisa menyusul.
D. Tergantung kebijakan sekolah.

<details>
<summary>💡 Hint</summary>
Logika AND dalam algoritma: Benar + Salah = Salah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lulus.**
Karena salah satu syarat (Bahasa) tidak terpenuhi, maka hasil akhirnya False (Tidak).
</details>

### Soal #100: Algoritma "Kalkulator Sederhana"
Input: Angka1, Angka2, Operator (+).
Proses: Hasil = Angka1 + Angka2.
Apa yang terjadi jika Angka2 diisi huruf "A"?
A. Hasilnya jadi "Angka1A".
B. Terjadi error tipe data (Type Mismatch) karena huruf tidak bisa dijumlahkan secara matematis.
C. Kalkulator meledak.
D. Huruf A jadi angka 0.

<details>
<summary>💡 Hint</summary>
Algoritma butuh input dengan tipe data yang sesuai (*Integer/Float* vs *String*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Error tipe data.**
Sistem perlu memastikan input valid sebelum menjalankan proses aritmatika.
</details>
### Soal #101: Algoritma Membuka Pintu Digital
Instruksi: "Tempelkan kartu ID."
Budi menempelkan Kartu Pelajar miliknya. Pintu tidak terbuka. Kenapa?
A. Kartunya kotor.
B. Algoritma sistem hanya mengenali nomor seri kartu ID yang terdaftar di database.
C. Pintunya sedang tidur.
D. Kurang lama nempelnya.

<details>
<summary>💡 Hint</summary>
Algoritma memerlukan data yang terotentikasi (terdaftar) agar bisa memberikan akses (Output).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Belum terdaftar.**
Hanya input yang cocok dengan data referensi yang diizinkan oleh algoritma keamanan.
</details>

### Soal #102: Algoritma "Search" di Spotify
Kamu mengetik "Tulus". Spotify menampilkan penyanyi Tulus, lagu Tulus, dan playlist Tulus. Ini adalah contoh algoritma...
A. Sorting.
B. Searching & Categorizing.
C. Looping lagu.
D. Rekomendasi harian.

<details>
<summary>💡 Hint</summary>
Sistem mencari kata kunci di berbagai kategori data secara bersamaan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Searching & Categorizing.**
Mencari data dan mengelompokkannya agar user mudah memilih.
</details>

### Soal #103: Algoritma "E-Commerce - Wishlist"
Kenapa barang di wishlist tidak lantas mengurangi saldo kamu?
A. Karena website lupa.
B. Karena menaruh di wishlist adalah aksi penambahan data ke database "Keinginan", bukan eksekusi algoritma "Transaksi Pembayaran".
C. Saldo kamu sudah nol.
D. Barangnya gaib.

<details>
<summary>💡 Hint</summary>
Wishlist hanyalah penyimpanan data pasif (Input), bukan sebuah instruksi eksekusi pembelian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berbeda alur algoritma.**
Proses inventori dan pembayaran baru dimulai setelah user menekan tombol "Beli/Checkout".
</details>

### Soal #104: Algoritma "Robot Vakum"
Robot menabrak dinding, lalu putar balik. Langkah ini disebut...
A. Error sistem.
B. Penanganan kondisi (Condition Handling) berdasarkan input dari sensor jarak.
C. Robotnya pusing.
D. Menari-nari.

<details>
<summary>💡 Hint</summary>
Aksi dipicu oleh kondisi fisik yang dideteksi oleh sensor.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penanganan Kondisi.**
Jika (Jarak < 5cm) Maka (Putar Balik).
</details>

### Soal #105: Algoritma "Urutan Rank Kelas"
Ali (Juara 1) pindah sekolah. Apa yang dilakukan algoritma pengurutan juara?
A. Menghapus Ali dan memajukan Juara 2 menjadi Juara 1 (Update Data).
B. Juara 1 dibiarkan kosong.
C. Semua nilai diulang dari nol.
D. Mengajak Ali balik lagi.

<details>
<summary>💡 Hint</summary>
Sistem harus memperbarui data (*Refreshing*) agar informasi tetap relevan dengan kondisi terbaru.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Memajukan peringkat.**
Algoritma sorting perlu dijalankan ulang pada data yang tersisa.
</details>

### Soal #106: Algoritma "Otoritas Admin"
"Hanya admin yang bisa menghapus komentar". Budi (User Biasa) mencoba hapus komentar. Apa respon algoritma?
A. Menghapus komentarnya.
B. Tampilkan pesan: "Anda tidak memiliki akses".
C. Menghapus akun Budi.
D. Laptop mati.

<details>
<summary>💡 Hint</summary>
Algoritma pengecekan peran user (*Role-based access control*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tampilkan pesan penolakan.**
Sistem memblokir aksi karena peran user tidak sesuai dengan syarat algoritma.
</details>

### Soal #107: Algoritma "Koneksi Bluetooth"
Kenapa kamu harus memasukkan kode PIN saat pertama kali menyambungkan HP ke headphone?
A. Biar HP-nya tambah berat.
B. Algoritma *Handshake* (Perkenalan) untuk memastikan kedua perangkat boleh saling berkirim data secara aman.
C. Biar headphonenya cepat habis baterai.
D. Aturan pemerintah.

<details>
<summary>💡 Hint</summary>
Mencegah perangkat orang asing sembarangan menyambung ke perangkatmu tanpa izin.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algoritma Handshake.**
Proses sinkronisasi dan keamanan data awal.
</details>

### Soal #108: Algoritma "Loop Bintang"
Instruksi: "Tulis sebiji bintang (*), lalu spasi, ulangi 5 kali."
Hasil yang benar:
A. *****
B. * * * * *
C. **********
D. *
 *
 *

<details>
<summary>💡 Hint</summary>
Perhatikan ada instruksi "spasi" di dalam setiap kali pengulangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. * * * * * **
Penggabungan aksi penulisan karakter dan spasi di dalam sebuah loop.
</details>

### Soal #109: Algoritma "Cari Berkas di PC"
Kamu mencari file 'Tugas.docx' di folder yang berisi 1000 file. Algoritma paling cepat adalah...
A. Buka folder lalu liat satu-satu pake mata (Lambat).
B. Klik kanan lalu Refresh.
C. Ketik nama file di kolom Search di pojok kanan atas (Efisien).
D. Ganti nama foldernya.

<details>
<summary>💡 Hint</summary>
Fitur pencarian di OS menggunakan indeks data yang jauh lebih cepat daripada penglihatan manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Gunakan kolom Search.**
Memanfaatkan fungsi index searching bawaan OS.
</details>

### Soal #110: Algoritma "Antivirus - Scan"
Antivirus membandingkan potongan kode file dengan database virus yang ada. Jika cocok, file dikarantina. Ini adalah proses...
A. Abstraksi.
B. Pattern Matching (Pencocokan Pola).
C. Looping selamanya.
D. Hapus file acak.

<details>
<summary>💡 Hint</summary>
Mencari kemiripan antara dua benda (file vs database virus).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pattern Matching.**
Teknik dasar algoritma keamanan informatik.
</details>

### Soal #111: Algoritma "Update Game"
Update 1 GB. Kebutuhan storage kosong adalah 2 GB. Storage kamu tinggal 1.5 GB. Apa yang dilakukan algoritma installer?
A. Tetap update sampai HP macet.
B. Hapus file kamu diam-diam.
C. Tampilkan pesan "Ruang penyimpanan tidak cukup".
D. Download saja tapi tidak dipasang.

<details>
<summary>💡 Hint</summary>
Algoritma instalasi selalu mengecek prasyarat ruang (*Space requirement*) sebelum memulai proses.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Ruang tidak cukup.**
Pengecekan integritas dan ketersediaan sumber daya sebelum eksekusi.
</details>

### Soal #112: Algoritma "Tiket Kereta"
"Beli tiket untuk keberangkatan besok jam 08:00". Kenapa sistem menolak jika kamu membelinya besok jam 08:05?
A. Keretanya benci kamu.
B. Algoritma sistem melarang pembelian tiket jika $Waktu\_Sekarang > Waktu\_Berangkat$.
C. Kasirnya pulang.
D. Biar keretanya tidak keberatan.

<details>
<summary>💡 Hint</summary>
Logika waktu (*Time validation*): masa lalu tidak bisa dibeli.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Validasi waktu.**
Keakuratan data waktu sangat krusial dalam algoritma logistik.
</details>

### Soal #113: Algoritma "Filter Chat"
"Jika pesan mengandung kata kasar 'XXX', ganti jadi '***'".
Ini merupakan aplikasi algoritma...
A. Sorting abjad.
B. Find and Replace (Cari dan Ganti).
C. Penjumlahan angka.
D. Restart HP.

<details>
<summary>💡 Hint</summary>
Mencari teks spesifik dan menggantinya dengan teks lain.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Find and Replace.**
Algoritma pemrosesan kata dasar (String Manipulation).
</details>

### Soal #114: Algoritma "Lift Paling Dekat"
Ada 3 lift: L1 (Lantai 5), L2 (Lantai 8), L3 (Lantai 1). Kamu di Lantai 4 dan menekan tombol. Lift mana yang akan datang?
A. L1
B. L3
C. L2
D. Semuanya datang barengan.

<details>
<summary>💡 Hint</summary>
Hitung selisih lantai: |5-4|=1, |8-4|=4, |1-4|=3. Pilih selisih terkecil.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. L1.**
L1 adalah yang paling dekat (hanya beda 1 lantai) dengan lokasimu.
</details>

### Soal #115: Algoritma "Auto-Save"
"Simpan pekerjaan setiap 5 menit." Kenapa ini penting bagi user?
A. Biar laptop makin panas.
B. Agar jika terjadi mati lampu (Unexpected Termination), data yang hilang maksimal hanya 5 menit terakhir.
C. Biar baterai cepat habis.
D. Iseng saja.

<details>
<summary>💡 Hint</summary>
Mekanisme pencegahan kehilangan data (*Data recovery protection*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Meminimalkan kehilangan data.**
Algoritma rutin untuk menjaga keamanan hasil kerja pengguna.
</details>

### Soal #116: Algoritma "Saran Pertemanan FB"
Sistem menyarankan teman karena kamu punya 10 teman yang sama ("Mutual Friends"). Pola ini disebut...
A. Hacking.
B. Social Graph Analysis (Analisis Jaringan).
C. Mencuri data.
D. Memata-matai.

<details>
<summary>💡 Hint</summary>
Menganalisis hubungan antar titik (User) untuk menemukan kemiripan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Social Graph Analysis.**
Pemanfaatan relasi data dalam algoritma media sosial.
</details>

### Soal #117: Algoritma "Kalkulator Sederhana" (Division)
Apa "Exception" (Pengecualian) yang harus ditangani saat membuat algoritma pembagian?
A. Pembagian dengan angka 1.
B. Pembagian dengan angka 0 (karena hasilnya tak terdefinisi dan bikin sistem error).
C. Pembagian dengan angka genap.
D. Pembagian dengan nama kamu.

<details>
<summary>💡 Hint</summary>
Secara matematis, angka berapapun dibagi nol akan menghasilkan error fatal di komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pembagian dengan nol.**
Mencegah *Runtime Error* dengan memblokir input pembagi nol di awal algoritma.
</details>

### Soal #118: Algoritma "Mencari Jalur di Labirin" (Pegang Dinding Kiri)
Kebalikan dari soal sebelumnya (dinding kanan). Apakah hasilnya sama?
A. Tidak, akan tersesat.
B. Sama-sama menjamin jalan keluar asalkan dindingnya bersambung.
C. Tergantung sepatunya.
D. Lebih cepat yang kiri.

<details>
<summary>💡 Hint</summary>
Secara logis, konsep "Wall Following" berlaku universal baik kiri maupun kanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sama-sama menjamin keluar.**
Keduanya adalah variasi algoritma penelusuran jalur (*Pathfinding*).
</details>

### Soal #119: Algoritma "Cek Koneksi Internet"
1. Kirim sinyal kecil (Ping) ke server Google.
2. Tunggu balasan.
3. JIKA ada balasan, MAKA status "Terhubung".
4. JIKA TIDAK (Timeout), MAKA status "Tidak Terhubung".
Langkah 1 disebut...
A. Mengirim surat.
B. Request (Permintaan Data).
C. Hacking.
D. Output.

<details>
<summary>💡 Hint</summary>
Mengirim data awal untuk mengetes respon pihak lawan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Request.**
 Dasar algoritma komunikasi antar perangkat dalam jaringan internet.
</details>

### Soal #120: Algoritma "Seleksi Calon Ketua OSIS"
Kriteria: Kelas 11 **ATAU** Kelas 10 berprestasi.
Sandi: Kelas 11, tidak berprestasi. Apakah dia bisa jadi calon?
A. Bisa, karena syarat ATAU (OR) cukup salah satu yang benar.
B. Tidak, harus berprestasi.
C. Tunggu kelas 12.
D. Tanya guru.

<details>
<summary>💡 Hint</summary>
Logika OR: Benar + Salah = Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bisa.**
Sandi memenuhi syarat "Kelas 11", jadi kondisi prestasinya tidak wajib benar untuk lolos kriteria awal.

### Soal #121: Algoritma "Caesar Cipher" (Enkripsi Sederhana)
Aturan: Ganti setiap huruf dengan huruf ke-3 setelahnya (A jadi D, B jadi E, dst).
Apa hasil enkripsi dari kata "IBU"?
A. LDU
B. JCV
C. KDX
D. LEX

<details>
<summary>💡 Hint</summary>
I (+3) = L. B (+3) = E. U (+3) = X.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. LEX**
Ini adalah algoritma kriptografi klasik yang menggunakan pergeseran posisi alfabet.
</details>

### Soal #122: Algoritma "Data Compression" (RLE)
Data: "AAAAABBBCC". Versi ringkas: "5A3B2C".
Apa versi ringkas dari data "ZZZXXXXY"?
A. 3Z4X1Y
B. Z3X4Y1
C. 3Z4XY
D. ZZX Y

<details>
<summary>💡 Hint</summary>
Hitung jumlah setiap huruf berurutan, lalu tulis angka diikuti hurufnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 3Z4X1Y**
Ini disebut *Run-Length Encoding*, algoritma kompresi data tanpa kehilangan informasi (*lossless*).
</details>

### Soal #123: Algoritma "Penyeberangan Malam"
4 orang (A, B, C, D) harus menyeberang jembatan yang hanya kuat menahan 2 orang. Mereka punya 1 senter. Waktu: A(1m), B(2m), C(5m), D(10m). Jika dua orang jalan bareng, kecepatannya ikut yang paling lambat.
Berapa waktu minimal agar semua sampai di seberang?
A. 17 menit
B. 19 menit
C. 21 menit
D. 15 menit

<details>
<summary>💡 Hint</summary>
Strategi: Kirim yang tercepat (A & B) dulu, lalu A balik bawa senter, lalu kirim yang paling lambat (C & D), lalu B balik bawa senter, terakhir A & B menyeberang lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 17 menit**
(A B seberang = 2m) + (A balik = 1m) + (C D seberang = 10m) + (B balik = 2m) + (A B seberang = 2m) = 17 menit.
</details>

### Soal #124: Algoritma "Penjadwalan Tugas"
Pekerjaan: Cuci Piring (15m), Sapu (10m), Masak (30m). Kamu punya 2 orang pekerja. Berapa waktu tercepat semua tugas selesai?
A. 55 menit
B. 30 menit
C. 27.5 menit
D. 35 menit

<details>
<summary>💡 Hint</summary>
Orang 1 mengerjakan yang paling lama (Masak, 30m). Orang 2 mengerjakan sisanya (Cuci + Sapu, 25m). Total waktu ikut yang terlama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 30 menit**
Kedua orang bekerja secara paralel. Saat orang 1 selesai masak (30m), orang 2 sudah selesai menyapu dan mencuci piring (25m).
</details>

### Soal #125: Algoritma "Cari Angka Terbesar"
Daftar: [12, 45, 7, 23, 56, 10]. Apa langkah pertama algoritma pencari nilai maksimum?
A. Mengurutkan daftar.
B. Mengasumsikan angka pertama (12) sebagai "Paling Besar" sementara.
C. Menjumlahkan semua angka.
D. Menghapus angka terkecil.

<details>
<summary>💡 Hint</summary>
Algoritma butuh titik awal (pembanding) untuk memulai pencarian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengasumsikan angka pertama sebagai pembanding.**
Lalu bandingkan dengan angka berikutnya. Jika angka baru lebih besar, update nilai "Paling Besar" tersebut.
</details>

### Soal #126: Algoritma "Sorting Kartu"
Kamu punya kartu 7, 3, 9, 2. Kamu ingin mengurutkan dari kecil ke besar. Jika kamu menggunakan *Selection Sort*, apa langkah pertamanya?
A. Menukar 7 dan 2.
B. Mencari angka terkecil (2) di seluruh daftar, lalu menukarnya dengan posisi pertama (7).
C. Menukar 7 dan 3.
D. Mengocok kartu lagi.

<details>
<summary>💡 Hint</summary>
Selection Sort bekerja dengan "memilih" (select) target (terkecil/terbesar) dan menaruhnya di tempat yang benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Cari yang paling kecil lalu taruh di depan.**
Inilah inti dari algoritma *Selection Sort*.
</details>

### Soal #127: Algoritma "Kelipatan 3 dan 5" (FizzBuzz)
"Jika angka kelipatan 3 tulis 'Fizz', jika kelipatan 5 tulis 'Buzz', jika keduanya tulis 'FizzBuzz'".
Apa yang kamu tulis untuk angka **15**?
A. Fizz
B. Buzz
C. FizzBuzz
D. 15

<details>
<summary>💡 Hint</summary>
15 habis dibagi 3 (5/3=5$) DAN habis dibagi 5 (5/5=3$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. FizzBuzz.**
Logika pengkondisian bertingkat yang sering muncul dalam tes pemrograman dasar.
</details>

### Soal #128: Algoritma "Pencarian Biner" (Binary Search)
Cari angka 70 di daftar terurut: [10, 20, 30, 40, 50, 60, 70, 80, 90].
Dimana algoritma ini pertama kali mengecek?
A. Angka 10 (paling kiri).
B. Angka 90 (paling kanan).
C. Angka 50 (paling tengah).
D. Angka 70 langsung.

<details>
<summary>💡 Hint</summary>
Binary Search bekerja dengan membagi dua daftar dan mengecek nilai tengahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Angka 50 (Tengah).**
Jika 70 > 50, maka pencarian dilanjutkan hanya di sebelah kanan angka 50. Jauh lebih cepat dari cek satu-satu!
</details>

### Soal #129: Algoritma "Antrian Prioritas" (Priority Queue)
Di IGD Rumah Sakit, pasien A (Batuk), pasien B (Kecelakaan Parah), pasien C (Demam). Siapa yang dilayani dulu oleh algoritma medis?
A. Pasien A karena datang duluan.
B. Pasien B karena kondisinya paling kritis (Prioritas Tinggi).
C. Pasien C karena paling sopan.
D. Urut abjad nama pasien.

<details>
<summary>💡 Hint</summary>
Sistem ini mengabaikan urutan waktu jika ada data dengan atribut "Kepentingan" yang lebih tinggi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pasien B.**
Implementasi *Priority Queue* dimana urutan ditentukan oleh bobot nilai (urgensi medis).
</details>

### Soal #130: Algoritma "Penghitung Karakter"
Kalimat: "BELAJAR CT". Berapa jumlah karakter (termasuk spasi) sesuai hitungan algoritma komputer?
A. 9
B. 10
C. 11
D. 8

<details>
<summary>💡 Hint</summary>
B-E-L-A-J-A-R (7) + Spasi (1) + C-T (2).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10**
Spasi adalah karakter valid (ASCII 32) yang memiliki bobot memori yang sama dengan huruf.
</details>

### Soal #131: Algoritma "Rekursif" (Analogi Cermin)
Cermin di depan cermin akan menghasilkan pantulan di dalam pantulan yang terus memanjang. Dalam algoritma, fungsi yang memanggil dirinya sendiri disebut...
A. Looping
B. Rekursi (Recursion)
C. Mirroring
D. Infinity

<details>
<summary>💡 Hint</summary>
Sebuah proses yang definisinya mengandung proses itu sendiri.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rekursi.**
Contoh: Faktorial atau deret Fibonacci sering diselesaikan dengan algoritma rekursif.
</details>

### Soal #132: Algoritma "Pembersih Cache"
Aplikasi membersihkan file yang paling lama tidak dibuka (LRU - Least Recently Used).
File A (dibuka 1 jam lalu), File B (dibuka 1 menit lalu), File C (dibuka 1 hari lalu). Mana yang dihapus?
A. A
B. B
C. C
D. Semuanya

<details>
<summary>💡 Hint</summary>
LRU menghapus data "paling basi" atau paling lama diabaikan user.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. C.**
Karena sudah 1 hari tidak disentuh, dianggap paling tidak dibutuhkan saat memori penuh.
</details>

### Soal #133: Algoritma "Cari Kata di Kamus"
Kenapa mencari kata "Zebra" di kamus fisik sangat cepat?
A. Karena huruf Z sedikit.
B. Karena kamus adalah data yang sudah terurut (Ordered Data) sehingga kita bisa langsung ke bagian belakang.
C. Karena kita hafal letaknya.
D. Karena dibantu indeks warna.

<details>
<summary>💡 Hint</summary>
Data yang terurut memungkinkan penggunaan algoritma pencarian yang efisien (*Search optimization*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Data sudah terurut.**
Inilah alasan kenapa komputer selalu ingin mengurutkan data (Sorting) sebelum memproses pencarian.
</details>

### Soal #134: Algoritma "Eratosthenes" (Cari Bilangan Prima)
Langkah: Tulis angka 1-20. Coret semua kelipatan 2 (kecuali 2), coret semua kelipatan 3 (kecuali 3), dst. Angka yang tersisa adalah prima.
Manakah yang **TIDAK** tercoret?
A. 9
B. 15
C. 13
D. 1

<details>
<summary>💡 Hint</summary>
9 kelipatan 3. 15 kelipatan 5. 1 bukan prima.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 13**
13 hanya bisa dibagi 1 dan dirinya sendiri.
</details>

### Soal #135: Algoritma "Rasio Aspek Video"
Video 1920x1080 disederhanakan menjadi 16:9. Proses penyederhanaan ini menggunakan konsep matematik...
A. FPB (Faktor Persekutuan Terbesar) untuk membagi kedua angka.
B. KPK untuk mengali angka.
C. Pengurangan berulang.
D. Akar kuadrat.

<details>
<summary>💡 Hint</summary>
920 / 120 = 16$. 080 / 120 = 9$. 120 adalah pembagi terbesarnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. FPB.**
Algoritma penyederhanaan rasio gambar dalam multimedia.
</details>

### Soal #136: Algoritma "Stack" (Tumpukan Piring)
Prinsip LIFO (Last In First Out). Piring terakhir yang ditaruh adalah piring pertama yang diambil.
Jika kamu menaruh Piring Merah, lalu Biru, lalu Hijau. Piring mana yang kamu ambil pertama?
A. Merah
B. Biru
C. Hijau
D. Sembarang

<details>
<summary>💡 Hint</summary>
Pikirkan tumpukan fisik di dunia nyata.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Hijau.**
Piring paling atas (terakhir ditaruh) adalah yang paling mudah dijangkau pertama kali.
</details>

### Soal #137: Algoritma "Queue" (Antrian Tiket)
Prinsip FIFO (First In First Out). Orang pertama datang adalah yang pertama dilayani.
Orang A, B, C antre berurutan. Siapa yang keluar dari antrian paling akhir?
A. A
B. B
C. C
D. Semuanya bareng

<details>
<summary>💡 Hint</summary>
Yang pertama masuk, pertama keluar. Berarti yang terakhir masuk, terakhir keluar.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. C.**
Pasangan sejati dari Stack (LIFO) adalah Queue (FIFO).
</details>

### Soal #138: Algoritma "Checklist Keberangkatan"
1. Cek tiket.
2. Cek passport.
3. Cek bagasi.
Jika salah satu tidak ada, maka batal berangkat. Logika apa yang digunakan?
A. Logika OR (Salah satu ada sudah cukup).
B. Logika AND (Semua harus ada).
C. Logika NOT (Jangan ada semua).
D. Logika IF tunggal.

<details>
<summary>💡 Hint</summary>
Syarat mutlak yang tidak bisa ditawar mewajibkan semua kondisi bernilai Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Logika AND.**
Dalam algoritma sistem kritis, keamanan biasanya menggunakan gerbang logika AND.
</details>

### Soal #139: Algoritma "Nilai Rata-Rata"
Input: [70, 80, 90]. Algoritma: (Total Nilai) / (Jumlah Data).
Apa outputnya?
A. 240
B. 80
C. 75
D. 3

<details>
<summary>💡 Hint</summary>
 / 3 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 80**
Algoritma statistik dasar yang paling sering digunakan guru untuk nilai rapor.
</details>

### Soal #140: Algoritma "Auto-Correct"
Kamu mengetik "computir", sistem menyarankan "computer". Algoritma ini bekerja dengan menghitung...
A. Jumlah huruf yang sama.
B. Jarak Levenshtein (jumlah perubahan minimal yang diperlukan agar kata itu sama).
C. Panjang kata.
D. Warna font.

<details>
<summary>💡 Hint</summary>
Hanya butuh mengubah 'i' menjadi 'e' (1 langkah).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jarak Levenshtein (Edit Distance).**
Algoritma cerdas untuk mendeteksi kemiripan teks secara linguistik.
</details>
### Soal #141: Algoritma "Penghitung Mundur" (Looping)
Instruksi: "Tulis angka N, lalu kurangi N dengan 1. Ulangi sampai N = 0". Jika mulai dari N = 3, apa yang tertulis?
A. 3, 2, 1
B. 3, 2, 1, 0
C. 2, 1, 0
D. 3-2-1

<details>
<summary>💡 Hint</summary>
Perhatikan apakah angka 0 ikut ditulis sebelum kondisi berhenti dicek.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 3, 2, 1, 0**
Urutan standar algoritma hitung mundur (countdown).
</details>

### Soal #142: Algoritma "Pemilihan Jalur Bus"
Bus A (30 menit, Rp 5.000). Bus B (20 menit, Rp 10.000). Kamu punya uang Rp 7.000 dan buru-buru. Mana yang dipilih?
A. Bus B
B. Bus A
C. Tidak keduanya
D. Jalan kaki

<details>
<summary>💡 Hint</summary>
Syarat biaya (Cost) harus terpenuhi dulu ($\le 7.000$).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bus A.**
Meskipun Bus B lebih cepat, namun biayanya melebihi anggaranmu. Algoritma harus mematuhi batasan (*Constraint*) sebelum optimasi.
</details>

### Soal #143: Algoritma "Penerimaan Pesanan"
1. Terima pesanan.
2. JIKA stok > 0, MAKA kurangi stok dan kirim barang.
3. JIKA TIDAK, MAKA tampilkan "Habis".
Apa yang terjadi jika stok pas 0?
A. Kirim barang.
B. Tampilkan "Habis".
C. Stok jadi -1.
D. Sistem hang.

<details>
<summary>💡 Hint</summary>
Kondisi "stok > 0" tidak terpenuhi jika stok bernilai 0.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tampilkan "Habis".**
Logika pemrosesan inventori yang akurat.
</details>

### Soal #144: Algoritma "Router Internet"
Router menerima paketan data dan melihat alamat tujuannya. Proses ini mirip dengan...
A. Tukang pos menyortir surat berdasarkan kode pos.
B. Ibu memasak sayur.
C. Adik bermain bola.
D. Bapak membaca koran.

<details>
<summary>💡 Hint</summary>
Routing adalah proses pengiriman data ke alamat yang spesifik dan terdaftar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Tukang pos.**
Sistem pengalamatan (IP Address) bekerja seperti alamat rumah di dunia nyata.
</details>

### Soal #145: Algoritma "Keliling Segitiga"
Input: Sisi A, B, C. Rumus: A + B + C. Manakah input yang **Tidak Logis**?
A. 3, 4, 5
B. 10, 10, 10
C. 5, 0, 5
D. 7, 8, 9

<details>
<summary>💡 Hint</summary>
Sebuah segitiga tidak mungkin memiliki sisi bernilai 0 atau negatif.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 5, 0, 5**
Algoritma harus memiliki validasi input untuk mencegah hasil yang tidak masuk akal secara geometri.
</details>

### Soal #146: Algoritma "Password Strength" (Complexity)
Kriteria: Minimal 8 karakter, ada angka, ada huruf besar.
Manakah yang lolos seleksi?
A. siswasma123
B. SISWASMA
C. Siswa123
D. Siswasma123

<details>
<summary>�� Hint</summary>
Cek satu-persatu: Panjang $\ge 80 Ada angka? Ada Huruf Besar?
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Siswasma123**
Memenuhi ketiga kriteria keamanan algoritma password.
</details>

### Soal #147: Algoritma "Mencari Nama Terpendek"
Daftar: ["Budi", "Ali", "Candra"]. Manakah outputnya?
A. Budi
B. Ali
C. Candra
D. Semua sama

<details>
<summary>💡 Hint</summary>
Hitung jumlah huruf: Budi (4), Ali (3), Candra (6).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ali.**
Kebalikan dari pencarian nama terpanjang, algoritma ini mencari nilai minimum.
</details>

### Soal #148: Algoritma "Deteksi Genap/Ganjil"
Input: Angka X.
Langkah: JIKA X sisa bagi 2 == 0, MAKA "Genap", JIKA TIDAK "Ganjil".
Apa status angka **0**?
A. Genap
B. Ganjil
C. Netral
D. Error

<details>
<summary>💡 Hint</summary>
/usr/bin/bash / 2 = 0$ sisa 0.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Genap.**
Secara algoritma dan matematika, nol habis dibagi 2 dan termasuk bilangan genap.
</details>

### Soal #149: Algoritma "Sorting Nama" (Alphabetical)
Daftar: "Budi", "Ani", "Cici". Urutan A-Z yang benar:
A. Ani, Budi, Cici
B. Cici, Budi, Ani
C. Budi, Ani, Cici
D. Ani, Cici, Budi

<details>
<summary>💡 Hint</summary>
Urutkan berdasarkan huruf pertama setiap kata.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ani, Budi, Cici**
A -> B -> C.
</details>

### Soal #150: Algoritma "Trace Loop Bersarang"

Berapa banyak bintang yang tertulis?
A. 5
B. 6
C. 23
D. 2

<details>
<summary>💡 Hint</summary>
Total = (Jumlah Loop Luar) x (Jumlah Loop Dalam).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 6**
Setiap satu kali loop luar, bintang ditulis 3 kali. Karena ada 2 kali loop luar, maka  \times 3 = 6$.
</details>

### Soal #151: Algoritma "Login dengan Limit"
"Maksimal salah password 3 kali. Jika lebih, akun terkunci".
Budi salah 3 kali. Apakah terkunci?
A. Belum, baru akan terkunci di kesalahan ke-4.
B. Sudah terkunci.
C. Akun dihapus.
D. Tanya admin.

<details>
<summary>💡 Hint</summary>
Perhatikan kata "Jika lebih" (artinya > 3).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Belum terkunci.**
Dalam logika "Jika > 3", maka angka 3 masih diizinkan. Batas eksklusif vs inklusif sangat penting di OSN-K.
</details>

### Soal #152: Algoritma "Sensor Suhu Ruangan"
"Jika suhu > 30°C, nyalakan AC. Jika suhu < 20°C, nyalakan Pemanas."
Suhu saat ini **25°C**. Apa status AC dan Pemanas?
A. Keduanya nyala.
B. Keduanya mati.
C. AC nyala, Pemanas mati.
D. AC mati, Pemanas nyala.

<details>
<summary>💡 Hint</summary>
Cek kondisi satu-persatu. 25 tidak > 30, dan 25 tidak < 20.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Keduanya mati.**
Suhu 25 berada di rentang "Ideal" dimana tidak ada aksi yang perlu dijalankan.
</details>

### Soal #153: Algoritma "Urutan Rank Juara"
Ada 5 orang. Untuk menentukan peringkat 1 sampai 5, berapa kali minimal kamu harus membandingkan jika menggunakan urutan manual?
A. 1 kali
B. Banyak kali (tergantung algoritma)
C. 5 kali
D. 0 kali

<details>
<summary>💡 Hint</summary>
Sorting butuh perbandingan berulang antar elemen data.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Banyak kali.**
Untuk 5 data, bahkan algoritma tercepat pun butuh beberapa langkah perbandingan.
</details>

### Soal #154: Algoritma "Cari Jalan di Grid"
Kamu ingin pindah dari (0,0) ke (2,2). Hanya bisa gerak ke Kanan (K) atau Atas (A). Manakah jalur yang valid?
A. K-K-A-A
B. K-A-K-A
C. A-A-K-K
D. Semua benar

<details>
<summary>💡 Hint</summary>
Total langkah harus 2 kali ke Kanan dan 2 kali ke Atas.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Semua benar.**
Ada banyak algoritma (jalur) menuju tujuan yang sama dalam sebuah koordinat grid.
</details>

### Soal #155: Algoritma "Matematika Sisa" (Modulo)
7 \pmod 5 = ...$
A. 3
B. 2
C. 1
D. 0

<details>
<summary>💡 Hint</summary>
7 / 5 = 3$ sisa hmmm?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2**
 \times 3 = 15$. Sisa dari 17 adalah 2. Modulo adalah operasi kunci dalam algoritma kriptografi.
</details>

### Soal #156: Algoritma "Cek Koneksi" (Retry)
"Coba hubungkan wifi. Jika gagal, coba lagi sampai 5 kali."
Jika pada percobaan ke-2 berhasil, apakah percobaan ke-3 dilakukan?
A. Ya, sampai 5 kali genap.
B. Tidak, langsung lanjut ke proses internetan.
C. Tunggu instruksi user.
D. Restart HP.

<details>
<summary>💡 Hint</summary>
Kondisi loop adalah "Sampai berhasil" ATAU "Maksimal 5 kali".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak dilakukan.**
Algoritma yang efisien akan segera keluar dari loop (*Break*) jika tujuan sudah tercapai.
</details>

### Soal #157: Algoritma "Searching" (Linear)
Cari angka 9 di daftar [1, 3, 5, 7, 10]. Dimana posisi angka 9?
A. Terakhir
B. Di tengah
C. Tidak ada (Not Found)
D. Di antara 7 dan 10

<details>
<summary>💡 Hint</summary>
Lihat apakah angka 9 tertulis di dalam daftar tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Tidak ada.**
Penting bagi algoritma pencarian untuk memberikan status "Tidak Ditemukan" jika target tidak ada di database.
</details>

### Soal #158: Algoritma "Trace Logika"
1.  = 10$
2.  = 20$
3.  = Y$
4.  = X$
Berapa nilai $ dan 2
A. =20, Y=10$
B. =20, Y=20$
C. =10, Y=10$
D. =10, Y=20$

<details>
<summary>💡 Hint</summary>
Hati-hati! Di baris 3, $ berubah jadi 20. Di baris 4, $ mengambil nilai $ yang terbaru (yaitu 20).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. X=20, Y=20**
Tanpa variabel bantuan, nilai asli $ (10) telah terhapus di baris 3.
</details>

### Soal #159: Algoritma "Format Tanggal"
Input: 28 Maret 2026. Di komputer sering ditulis 2026-03-28. Alasannya?
A. Biar susah dibaca.
B. Agar mudah diurutkan (Sorting) secara otomatis dari tahun-bulan-hari.
C. Aturan dari Amerika.
D. Tidak ada alasan khusus.

<details>
<summary>💡 Hint</summary>
Jika diurutkan dari tahun, maka semua file di tahun yang sama akan mengelompok rapi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mudah diurutkan.**
Standard ISO 8601 didesain untuk efisiensi algoritma pengurutan data kronologis.
</details>

### Soal #160: Algoritma "Seleksi Beasiswa"
"Nilai > 80 **ATAU** dari keluarga kurang mampu".
Syifa: Nilai 75, dari keluarga mampu. Apakah lolos?
A. Lolos, nilainya lumayan.
B. Tidak Lolos, karena kedua syarat tidak terpenuhi.
C. Lolos salah satu.
D. Tanya rektor.

<details>
<summary>💡 Hint</summary>
Logika OR: Salah + Salah = Salah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lolos.**
Syifa tidak memenuhi kriteria prestasi maupun kriteria ekonomi.
</details>
### Soal #161: Algoritma "Merge Sort" (Pecah dan Gabung)
Langkah: Pecah daftar jadi dua, urutkan masing-masing, lalu gabungkan kembali.
Kenapa ini lebih cepat dari *Bubble Sort* untuk data yang sangat banyak?
A. Karena pengerjaannya "Divide and Conquer" (Pecah dan Taklukkan).
B. Karena warnanya lebih bagus.
C. Karena tidak butuh memori.
D. Karena dibantu AI.

<details>
<summary>💡 Hint</summary>
Mengurutkan dua kelompok kecil jauh lebih ringan beban prosesornya daripada mengurutkan satu kelompok raksasa sekaligus.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Divide and Conquer.**
Inilah strategi cerdas yang membuat algoritma bisa menangani jutaan data dalam sekejap.
</details>

### Soal #162: Algoritma "Graph" (Peta Teman)
Titik (Node) adalah teman, Garis (Edge) adalah hubungan pertemanan.
Ali kenal Budi. Budi kenal Cici. Ali tidak kenal Cici.
Berapa "Garis" yang harus ditarik?
A. 1
B. 2
C. 3
D. 0

<details>
<summary>💡 Hint</summary>
Garis hanya ditarik jika ada hubungan kenal secara langsung.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2**
Garis Ali-Budi (1) dan Garis Budi-Cici (2). Ini adalah dasar struktur data *Graph*.
</details>

### Soal #163: Algoritma "Binary Numbers" (Basis 2)
Dalam dunia komputer (biner), angka 1 berarti Nyala dan 0 berarti Mati.
Apa nilai biner dari angka **2** di dunia kita?
A. 11
B. 10
C. 01
D. 100

<details>
<summary>💡 Hint</summary>
Ingat urutan biner: 00 (0), 01 (1), 10 (2), 11 (3).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10**
Inilah dasar bagaimana algoritma bitwise mengolah data di level hardware.
</details>

### Soal #164: Algoritma "Shortest Path" (Dijkstra)
Kamu ingin pergi dari A ke C. Jalur 1 (A-B-C) jaraknya 5+5=10. Jalur 2 (A-C) jaraknya 12. Mana yang dipilih?
A. Jalur 2 karena langsung (tidak mampir-mampir).
B. Jalur 1 karena total jaraknya lebih pendek (5+5 < 12).
C. Jalur acak.
D. Sesuai arah angin.

<details>
<summary>💡 Hint</summary>
Algoritma selalu mengutamakan nilai total biaya (*Accumulated Cost*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jalur 1.**
Meski harus lewat B, namun total biayanya lebih efisien. Inilah inti dari algoritma navigasi.
</details>

### Soal #165: Algoritma "Input-Output" (GIGO)
GIGO adalah singkatan dari *Garbage In, Garbage Out*. Artinya...
A. Masukkan sampah ke komputer, nanti jadi emas.
B. Jika input datanya salah, maka outputnya pasti salah ("Sampah").
C. Komputer bisa membedakan sampah dan bukan.
D. Jangan buang sampah di depan laptop.

<details>
<summary>💡 Hint</summary>
Kevalidan hasil sangat bergantung pada kualitas data yang diberikan user.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Input salah = Output salah.**
Prinsip fundamental bagi perancang algoritma untuk memastikan validitas input.
</details>

### Soal #166: Algoritma "Palindrom"
Sebuah kata disebut palindrom jika dibaca depan-belakang sama. "RADAR" adalah palindrom.
Langkah algoritma: Balikkan kata, bandingkan dengan kata asli.
Mana yang merupakan palindrom?
A. KOMPUTER
B. CT
C. KATAK
D. ALGORITMA

<details>
<summary>💡 Hint</summary>
K-A-T-A-K dibalik tetap K-A-T-A-K.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. KATAK.**
Logika perbandingan string yang sering muncul dalam problem informatika.
</details>

### Soal #167: Algoritma "Sorting Tinggi" (Stable Sort)
Ali (160) dan Budi (160). Tinggi mereka sama.
Sebuah sorting disebut "Stabil" jika urutan mereka di daftar asli (Ali duluan) tidak berubah di daftar akhir.
Apa urutan yang stabil?
A. Ali, Budi
B. Budi, Ali
C. Budi, Budi
D. Sembarang

<details>
<summary>💡 Hint</summary>
Stabilitas menjaga integritas data yang memiliki nilai sama.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ali, Budi**
Urutan asli tetap terjaga meskipun nilai kriteria (tinggi) sama.
</details>

### Soal #168: Algoritma "Mode Tidur Laptop"
"Jika tidak ada aktivitas selama 10 menit, matikan layar."
Apa yang disebut sebagai **Aktivitas** oleh algoritma ini?
A. Kamu melihat layar dengan serius.
B. Pergerakan mouse atau penekanan tombol keyboard.
C. Kipas laptop berputar.
D. Layar sedang menyala.

<details>
<summary>💡 Hint</summary>
Komputer hanya bisa mendeteksi input fisik melalui periferal (mouse/keyboard/touch).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pergerakan mouse/keyboard.**
Sensor pasif ini menjadi input bagi timer mode tidur.
</details>

### Soal #169: Algoritma "Penghitung Ganjil"
Berapa jumlah bilangan ganjil antara 1 sampai 10?
A. 4
B. 5
C. 6
D. 10

<details>
<summary>💡 Hint</summary>
Bilangannya: 1, 3, 5, 7, 9.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 5**
Membangun logika pencacahan (*Counting*) dalam rentang data.
</details>

### Soal #170: Algoritma "Cari Teman Berdasarkan Hobi"
Ada 4 teman: A (Futsal), B (Musik), C (Futsal), D (Gambar).
Algoritma: "Pilih teman yang hobi Futsal **DAN** namanya mengandung huruf 'C'".
Siapa yang terpilih?
A. A
B. C
C. A dan C
D. Tidak ada

<details>
<summary>💡 Hint</summary>
Cek hobi: A dan C. Cek nama: 'A' tidak ada huruf C. 'C' ada huruf C.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. C.**
Aplikasi logika AND pada atribut data ganda.
</details>

### Soal #171: Algoritma "Bubble Sort" (Langkah Terakhir)
Daftar: [3, 2, 1]. Untuk mengurutkan jadi [1, 2, 3], berapa kali proses perbandingan & penukaran harus dilakukan?
A. 1 kali
B. Lebih dari satu kali.
C. 0 kali
D. 100 kali

<details>
<summary>💡 Hint</summary>
Bubble sort memindahkan angka pelan-pelan seperti gelembung udara.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lebih dari satu kali.**
Setiap angka harus dibandingkan dengan tetangganya berulang kali sampai posisi akhirnya benar.
</details>

### Soal #172: Algoritma "Routing Paket"
Kenapa jika satu kabel internet putus, internet di rumahmu tidak lantas mati total (jika kamu pakai jaringan besar)?
A. Karena internet gaib.
B. Karena algoritma perutean (Routing) mencari jalur alternatif secara otomatis (Redundancy).
C. Kabelnya nyambung sendiri.
D. Karena dibantu satelit.

<details>
<summary>💡 Hint</summary>
Jaringan internet dibangun seperti jaring laba-laba, bukan garis lurus.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jalur alternatif.**
Salah satu keunggulan desain algoritma distribusi data modern.
</details>

### Soal #173: Algoritma "Search" (Case Insensitive)
Cari kata "Informatika". Masukan user: "informatika".
Hasil: "Ditemukan".
Ini berarti algoritma pencarian bersifat...
A. Case Sensitive
B. Case Insensitive (Mengabaikan besar-kecil huruf).
C. Error
D. Beda bahasa

<details>
<summary>💡 Hint</summary>
Sistem sengaja menyamakan 'I' dan 'i' untuk mempermudah user.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Case Insensitive.**
Fitur kenyamanan dalam algoritma pencarian teks publik.
</details>

### Soal #174: Algoritma "Optimasi Makan Siang"
Antrean kantin panjang. Kamu ingin makan nasi uduk (5 menit saji) atau mie ayam (15 menit saji). Bel masuk 10 menit lagi. Mana yang kamu pesan secara logis?
A. Mie ayam karena enak.
B. Nasi uduk karena waktunya cukup.
C. Tidak jadi makan.
D. Bakso.

<details>
<summary>💡 Hint</summary>
$\text{Waktu Saji} \le \text{Sisa Waktu Istirahat}$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Nasi uduk.**
Pemilihan opsi berdasarkan batas waktu (*Deadline aware algorithm*).
</details>

### Soal #175: Algoritma "Hapus File Permanen"
"Apakah anda yakin ingin menghapus?" -> Klik Ya.
Kenapa sistem bertanya?
A. Biar user capek.
B. Sebagai mekanisme konfirmasi (Confirmation) untuk mencegah kesalahan fatal akibat ketidaksengajaan klik.
C. Iseng saja.
D. Biar sistem istirahat.

<details>
<summary>💡 Hint</summary>
Penghapusan data adalah proses yang tidak bisa dibatalkan (*Irreversible*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah kesalahan fatal.**
Langkah verifikasi tambahan dalam desain algoritma interaksi manusia-komputer (HCI).
</details>

### Soal #176: Algoritma "Cek Keranjang Belanja"
"Checkout" berhasil jika (Punya Alamat) **DAN** (Ada Stok) **DAN** (Metode Bayar Terpilih).
Jika Alamat Ada, Stok Ada, tapi belum pilih Bayar. Apa respon sistem?
A. Bayarin dulu.
B. Tombol checkout tetap mati/dinonaktifkan.
C. Langsung kirim barang.
D. Muncul diskon.

<details>
<summary>💡 Hint</summary>
Semua syarat AND harus bernilai Benar agar aksi dijalankan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tombol mati.**
Pencegahan eksekusi transaksi yang datanya belum lengkap.
</details>

### Soal #177: Algoritma "Password Expired"
"Ganti password setiap 3 bulan".
Jika Budi ganti password hari ini, kapan algoritma sistem akan memintanya ganti lagi?
A. Besok
B. 90 hari lagi
C. Tidak pernah
D. Satu tahun lagi

<details>
<summary>💡 Hint</summary>
 \text{ bulan} \approx 90 \text{ hari}$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 90 hari lagi.**
Penjadwalan keamanan berbasis durasi waktu (*Duration-based policy*).
</details>

### Soal #178: Algoritma "Sorting Alphabet" (Z to A)
Daftar: "Apel", "Ceri", "Belimbing". Urutkan Descending.
A. Apel, Belimbing, Ceri
B. Ceri, Belimbing, Apel
C. Belimbing, Apel, Ceri
D. Semua benar

<details>
<summary>💡 Hint</summary>
Urutkan dari abjad yang paling belakang (Z ke A).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ceri, Belimbing, Apel.**
C (3), B (2), A (1).
</details>

### Soal #179: Algoritma "Deteksi Virus Email"
"Jika lampiran berekstensi .exe, pindahkan ke Spam".
Sebuah file bernama 'FotoLiburan.exe' datang. Masuk mana?
A. Inbox
B. Spam
C. Trash
D. Draft

<details>
<summary>💡 Hint</summary>
Jangan tertipu oleh nama 'FotoLiburan', algoritma hanya melihat ekstensinya (.exe).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Spam.**
Abstraksi lampiran hanya berdasarkan jenis file demi keamanan.
</details>

### Soal #180: Algoritma "Keliling Lingkaran"
Input: jari-jari (r). Rumus:  \times \pi \times r$.
Bila  = 7$ dan $\pi = 22/7$. Berapa hasilnya?
A. 14
B. 22
C. 44
D. 154

<details>
<summary>💡 Hint</summary>
 \times (22/7) \times 7 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 44.**
Penghitungan presisi untuk output data geometri.
</details>
### Soal #181: Algoritma "Logika NOT" (Kebalikan)
Instruksi: "JIKA TIDAK Hujan, MAKA Pergi Main."
Kondisi saat ini: **Hujan**. Apakah kamu pergi main?
A. Ya
B. Tidak
C. Tunggu reda
D. Menangis

<details>
<summary>💡 Hint</summary>
Logika NOT membalikkan nilai: NOT True = False.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Karena syarat "Tidak Hujan" bernilai Salah (False), maka aksi "Pergi Main" tidak dijalankan.
</details>

### Soal #182: Algoritma "Cari Nilai Tengah" (Median)
Daftar nilai: [60, 70, 80, 90, 100]. Apa langkah pertama mencari Median?
A. Menjumlahkan semua nilai.
B. Memastikan daftar sudah terurut (Sorting).
C. Mencari nilai paling sering muncul.
D. Memilih nilai paling besar.

<details>
<summary>💡 Hint</summary>
Median adalah nilai tengah pada data yang **sudah terurut**.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pastikan data terurut.**
Tanpa sorting, angka di tengah fisik (posisi) belum tentu nilai tengah secara statistik.
</details>

### Soal #183: Algoritma "Pendaftaran Ekskul"
Syarat: (Siswa Kelas 10) **DAN** (Sehat Jasmani) **ATAU** (Hanya Rekomendasi Guru Khusus).
Andi: Kelas 11, Sehat, Punya Rekomendasi Guru. Apakah dia bisa daftar?
A. Bisa, karena punya Rekomendasi Guru (Syarat OR terpenuhi).
B. Tidak, karena dia Kelas 11.
C. Bisa, karena dia Sehat.
D. Tunggu tahun depan.

<details>
<summary>💡 Hint</summary>
$\text{Syarat} = (1 \text{ DAN } 2) \text{ OR } 3$. Jika 3 Benar, maka seluruhnya Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bisa.**
Logika OR memberikan jalur alternatif jika jalur utama (Kelas 10) tidak terpenuhi.
</details>

### Soal #184: Algoritma "Captcha" (Verification)
"Ketikkan teks bergelombang yang ada di gambar". Ini digunakan untuk membuktikan bahwa...
A. Layar HP-mu jernih.
B. Pengguna adalah manusia, bukan robot otomatis (Bot).
C. Kamu jago ngetik cepat.
D. Font-nya keren.

<details>
<summary>💡 Hint</summary>
Mengenali pola teks dalam gambar yang sudah didistorsi sangat sulit bagi algoritma bot sederhana.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuktikan pengguna adalah manusia.**
Alat pertahanan terhadap serangan algoritma otomatis.
</details>

### Soal #185: Algoritma "Kalkulator Sederhana" (Berapa Kali Klik?)
Kamu ingin menghitung  \times 3$ menggunakan **penambahan berulang**. Berapa kali kamu melakukan operasi tambah?
A. 2 kali (+5+5$)
B. 3 kali
C. 5 kali
D. 15 kali

<details>
<summary>�� Hint</summary>
 + 5 = \text{tambah 1x}$.  + 5 = \text{tambah 2x}$.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 2 kali.**
Operasi perkalian adalah bentuk abstraksi algoritma dari penjumlahan berulang.
</details>

### Soal #186: Algoritma "Antri Fotokopi" (Wait Time)
A (5m), B (10m). Jika B diproses dulu, berapa total waktu tunggu A?
A. 5 menit
B. 10 menit
C. 15 menit
D. 0 menit

<details>
<summary>💡 Hint</summary>
A harus menunggu sampai B selesai (10m).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10 menit.**
Waktu proses orang pertama adalah waktu tunggu bagi orang kedua di antrian.
</details>

### Soal #187: Algoritma "Pesan Makan" (Validation)
"Jika pesanan > Rp 50rb, berikan diskon 10%".
Harga makanan: Rp 49.999. Apakah dapet diskon?
A. Dapet, kan beda satu rupiah saja.
B. Tidak dapet, syaratnya harus lebih besar dari 50.000 (False).
C. Dapet jika kasirnya baik.
D. Dapet separo.

<details>
<summary>💡 Hint</summary>
Algoritma informatika tidak mengenal "toleransi kasihan", yang ada hanya nilai eksak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak dapet.**
Ketelitian perbandingan numerik adalah kunci dalam algoritma bisnis.
</details>

### Soal #188: Algoritma "Deteksi Phishing"
Kamu dapat email: "Akunmu diblokir, klik link ini: 'www.faceb00k-login.com'".
Kenapa sistem keamanan menandainya sebagai bahaya?
A. Karena link-nya panjang.
B. Karena menggunakan karakter angka '0' untuk menggantikan huruf 'o' (Misleading pattern).
C. Karena kamu tidak punya akun Facebook.
D. Karena internet lambat.

<details>
<summary>💡 Hint</summary>
Penipu sering menggunakan visual yang mirip tapi teks berbeda secara digital untuk menipu mata manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola teks yang mengecoh.**
Algoritma keamanan membandingkan domain asli vs domain input.
</details>

### Soal #189: Algoritma "Trace Variabel" (Swapping Bug)
1.  = 5$
2.  = 10$
3.  = Y$
4.  = X$
Apakah $ dan $ sudah tertukar nilainya (X=10, Y=5)?
A. Ya, sudah benar.
B. Tidak, nilainya sekarang =10$ dan =10$.
C. Tidak, nilainya =5$ and =5$.
D. Masih tetap.

<details>
<summary>💡 Hint</summary>
Perhatikan di langkah ke-4, $ sudah berubah menjadi 10.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak tertukar.**
Ini adalah kesalahan algoritma penukaran umum. Dibutuhkan variabel bantuan ( = X$) untuk menyimpan nilai asli.
</details>

### Soal #190: Algoritma "Rekomendasi Video YouTube"
YouTube memberikan video tentang 'Kucing' setelah kamu menonton 5 video tentang 'Kandang Kucing'. Pola pengulangan data ini disebut...
A. Memata-matai.
B. User Behavior Modeling (Pemodelan Perilaku Pengguna).
C. Iklan tersembunyi.
D. Error server.

<details>
<summary>💡 Hint</summary>
Sistem mempelajari kegemaranmu dari riwayat pencarian (Input history).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pemodelan Perilaku.**
Algoritma rekomendasi menggunakan pola minat user untuk memberikan output yang relevan.
</details>

### Soal #191: Algoritma "Cari Nama di Kertas Absen"
Ada 100 orang. Kamu cari namamu di daftar yang tidak urut (acak). Berapa kali paling sial (Max Steps) kamu harus mengecek?
A. 1 kali
B. 50 kali
C. 100 kali
D. Tidak terhitung

<details>
<summary>💡 Hint</summary>
Jika kamu yang paling sial, namamu ada di urutan paling bawah atau tidak ada di situ.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 100 kali.**
Pada algoritma *Linear Search*, kasus terburuk (*Worst Case*) adalah mengecek seluruh data satu-persatu.
</details>

### Soal #192: Algoritma "Binary Search" (Case: Tidak Ketemu)
Cari angka 25 di daftar: [10, 20, 30, 40, 50].
Langkah 1: Cek tengah (30). 25 < 30, maka cari di kiri ([10, 20]).
Langkah 2: Cek tengah antara 10-20.
Kapan proses ini berhenti?
A. Berputar selamanya.
B. Saat daftar pencarian sudah habis/kosong dan angka belum ditemukan.
C. Saat user menyerah.
D. Pas mencapai angka 50.

<details>
<summary>💡 Hint</summary>
Algoritma yang baik harus memiliki "Finiteness" (Titik berhenti).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Saat daftar habis.**
Pemberhentian yang logis sangat penting agar program tidak *hang*.
</details>

### Soal #193: Algoritma "Mode Hemat Energi"
"Matikan fitur lokasi JIKA baterai < 15%".
Baterai saat ini **15%**. Apakah lokasi dimatikan?
A. Ya, sudah kritis.
B. Belum, syaratnya harus "lebih kecil" dari 15.
C. Tergantung settingan.
D. Matikan total.

<details>
<summary>💡 Hint</summary>
Di informatika, '< 15' tidak sama dengan '$\le$ 15'.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Belum dimatikan.**
Logika batas angka sangat krusial dalam algoritma otomatis.
</details>

### Soal #194: Algoritma "Cleaning Service Robot"
1. Bergerak maju 1 meter.
2. Sedot debu.
3. Apakah ada tembok di depan?
4. JIKA ya, MAKA belok kanan.
5. Ulangi!
Langkah 3-4 adalah jenis instruksi...
A. Berurutan (Sequential).
B. Percabangan (Branching / Conditional).
C. Pengulangan (Looping).
D. Selesai.

<details>
<summary>💡 Hint</summary>
Instruksi yang memberikan pilihan arah berdasarkan kondisi tertentu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Percabangan.**
Inilah yang membuat robot nampak "pintar" karena bisa memilih respon yang berbeda-beda.
</details>

### Soal #195: Algoritma "Antrian Prioritas" (Lansia)
Di depan kasir ada antrian 5 orang anak muda. Datang satu Nenek berumur 80 tahun.
Sistem kasir: "Dahulukan Lansia di atas 70 tahun".
Apa posisi Nenek sekarang di antrian?
A. Tetap paling belakang.
B. Langsung jadi orang pertama dilayani (Front of queue).
C. Di tengah-tengah.
D. Ditemani cucu.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma *Preemptive Priority*.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Orang pertama.**
Data baru dengan prioritas tinggi memotong alur antrian normal.
</details>

### Soal #196: Algoritma "Cek Plagiarisme"
Guru membandingkan tugasmu dengan Google. Jika persentase kemiripan kata > 80%, dianggap nyontek.
Tugasmu: 79% mirip. Apa keputusan algoritma guru?
A. Nyontek.
B. Aman (Lolos), meski sangat mepet dengan batas.
C. Disuruh buat lagi.
D. Tugasnya dibakar.

<details>
<summary>💡 Hint</summary>
Algoritma patuh pada angka pembanding (*Threshold*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Aman.**
Batas kaku (Thresholding) adalah dasar dari setiap proses klasifikasi otomatis.
</details>

### Soal #197: Algoritma "Enkripsi Angka"
Angka Asli: 123. Rumus: (Angka + 10) x 2.
Apa angka yang terenkripsi?
A. 133
B. 266
C. 246
D. 256

<details>
<summary>💡 Hint</summary>
 = 133$. Lalu 33 \times 2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 266.**
Operasi aritmatika berantai untuk melindungi data dasar.
</details>

### Soal #198: Algoritma "Password Wifi" (Snooping)
Kamu mencuri dengar orang nyebut password wifi "123456". Ternyata passwordnya adalah "Ikan-Mas-Koki".
Kenapa kamu tidak bisa masuk meski password yang kamu dengar kelihatannya angka?
A. Jarak wifi kejauhan.
B. Karena password tersebut hanya jebakan/fake (Decoy algorithm).
C. Karena kamu salah dengar.
D. Wifi-nya dimatikan.

<details>
<summary>💡 Hint</summary>
Algoritma keamanan seringkali menggunakan *Honeypot* atau jebakan untuk mendeteksi penyusup.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algoritma Jebakan (Decoy).**
Sistem memberikan informasi palsu untuk melindungi yang asli.
</details>

### Soal #199: Algoritma "Kelipatan 10" (Count)
Ada angka 1 sampai 105. Berapa banyak angka kelipatan 10?
A. 10
B. 11
C. 100
D. 5

<details>
<summary>💡 Hint</summary>
10, 20, 30 ... sampai 100.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 10.**
Penghitungan iteratif sederhana dalam sebuah rentang data.
</details>

### Soal #200: Algoritma "Ujian Online" (Final Submit)
"Waktu ujian habis dalam 3 detik". Kamu klik tombol Submit pada detik ke-4. Apa yang dilakukan sistem?
A. Menolak jawabanmu karena batas waktu sudah terlampaui.
B. Menerima dengan alasan kasihan.
C. Komputer restart.
D. Memberikan soal baru.

<details>
<summary>💡 Hint</summary>
Algoritma harus konsisten dengan batasan waktu (*Time-out mechanism*).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menolak.**
Ketegasan batasan adalah inti dari algoritma keadilan dalam ujian kompetitif.
</details>

### Soal #201: Algoritma "Checklist Pagi"
1. Bangun tidur.
2. JIKA mandi >= 10 menit, MAKA sarapan di jalan.
3. JIKA mandi < 10 menit, MAKA sarapan di meja.
Andi mandi 10 menit tepat. Dimana dia sarapan?
A. Di meja.
B. Di jalan.
C. Tidak jadi sarapan.
D. Di kamar mandi.

<details>
<summary>💡 Hint</summary>
Syarat sarapan di jalan adalah mandi >= 10. Angka 10 termasuk ke dalam syarat tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di jalan.**
Logika inklusif (dengan tanda sama dengan) memasukkan nilai batas ke kategori atas.
</details>

### Soal #202: Algoritma "Sorting Nama" (Quick Sort Concept)
Kamu memilih satu nama (Pivot) "Budi". Lalu semua nama yang abjadnya sebelum 'B' dipindah ke kiri, dan setelah 'B' ke kanan.
Ini adalah langkah dasar dari algoritma...
A. Bubble Sort
B. Quick Sort
C. Selection Sort
D. Shuffle

<details>
<summary>💡 Hint</summary>
Membagi data berdasarkan satu titik acuan disebut pemisahan (*Partitioning*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Quick Sort.**
Salah satu algoritma pengurutan tercepat yang paling populer digunakan.
</details>

### Soal #203: Algoritma "Router - Hop Count"
Packet data menyeberang antar router. Setiap kali pindah router, status 'Hop' berkurang 1. Jika 'Hop' mencapai 0 tetapi belum sampai tujuan, paket tersebut akan dibuang. Tujuannya?
A. Biar paketnya istirahat.
B. Mencegah paket berputar selamanya di jaringan (Infinite Loop protection).
C. Biar internet makin lambat.
D. Biar router tidak kepanasan.

<details>
<summary>💡 Hint</summary>
Istilahnya adalah TTL (*Time to Live*). Gunanya untuk memberhentikan data yang tersesat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah infinite loop.**
Mekanisme penghentian paksa untuk menjaga kebersihan trafik jaringan.
</details>

### Soal #204: Algoritma "Cek Tahun Kabisat" (Urutan Benar)
1. JIKA habis dibagi 400, MAKA Kabisat.
2. JIKA TIDAK, namun habis dibagi 100, MAKA Bukan Kabisat.
3. JIKA TIDAK, namun habis dibagi 4, MAKA Kabisat.
Apa status tahun **1900**?
A. Kabisat.
B. Bukan Kabisat.
C. Tergantung bulan Februari.
D. Error algoritma.

<details>
<summary>💡 Hint</summary>
1900 tidak habis dibagi 400 (Lanjut ke langkah 2). 1900 habis dibagi 100 (Selesai).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bukan Kabisat.**
Aturan pengecualian tahun abad yang tidak habis dibagi 400.
</details>

### Soal #205: Algoritma "Kapasitas Server"
"Satu server kuat melayani 100 orang". Saat ini orang ke-101 masuk. Apa respon sistem cerdas?
A. Menendang orang pertama keluar.
B. Mengalihkan (Redirect) orang ke-101 ke server cadangan.
C. Server langsung terbakar.
D. Meminta semua orang pulang.

<details>
<summary>💡 Hint</summary>
Ini disebut strategi *Load Balancing* (Penyeimbang Beban).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengalihkan ke server lain.**
Algoritma pembagian beban kerja agar sistem tidak tumbang (*Crash*).
</details>

### Soal #206: Algoritma "Antivirus - Heuristic"
Antivirus tidak kenal virus baru ini, tapi virus ini melakukan tindakan "Hapus Semua File Sistem". Antivirus langsung memblokirnya.
Ini adalah algoritma pendeteksian berdasarkan...
A. Nama virus.
B. Perilaku (Behavior Algorithm).
C. Ukuran file.
D. Tanggal download.

<details>
<summary>💡 Hint</summary>
Mengenali bahaya dari ciri-ciri tindakan tak lazim, bukan dari identitas tertulis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perilaku.**
Algoritma cerdas yang bisa mendeteksi ancaman baru yang belum terdaftar di database.
</details>

### Soal #207: Algoritma "Ganti Rugi"
Pesan belanja: Rp 100rb. Barang rusak. Toko mengembalikan (Refund) 120% dari harga. Berapa uang yang diterima?
A. Rp 100.000
B. Rp 120.000
C. Rp 20.000
D. Rp 1.200.000

<details>
<summary>💡 Hint</summary>
00.000 \times 1.2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 120.000.**
Perhitungan sanksi atau insentif dalam algoritma kompensasi.
</details>

### Soal #208: Algoritma "Smart Home - Lampu"
1. JIKA hari sudah gelap (dari sensor cahaya).
2. DAN JIKA ada orang di ruangan (dari sensor infra merah).
3. MAKA nyalakan lampu.
Jika hari sudah gelap tapi ruangan kosong, apa yang terjadi?
A. Lampu menyala.
B. Lampu mati.
C. Sensor rusak.
D. Lampu kedap-kedip.

<details>
<summary>💡 Hint</summary>
Gerbang logika AND: Salah satu False membuat seluruh hasil False.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampu mati.**
Algoritma penghematan energi otomatis yang efektif.
</details>

### Soal #209: Algoritma "Pencarian Paling Cepat" (Google Index)
Kenapa Google bisa menampilkan 1 miliar hasil pencarian hanya dalam 0,5 detik?
A. Karena Google memakai komputer super.
B. Karena Google sudah memproses & mengurutkan (Index) seluruh web sebelum kamu bertanya.
C. Karena Google menebak-nebak saja.
D. Karena internet sangat cepat.

<details>
<summary>💡 Hint</summary>
Google tidak mencari satu-persatu di internet saat kamu ketik; mereka sudah punya "Daftar Isi" raksasa yang siap dibaca.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengindeksan (Indexing).**
Teknik optimasi pencarian tingkat tinggi untuk menangani data skala besar.
</details>

### Soal #210: Algoritma "Membuat Pola Barisan"
Ditetapkan barisan: 1, 3, 6, 10, ... Apa angka selanjutnya?
A. 13
B. 15
C. 14
D. 20

<details>
<summary>💡 Hint</summary>
+2=3$. +3=6$. +4=10$. Berarti 0+\dots? = \dots?$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 15**
Pola bilangan segitiga. Algoritma harus mampu mendeteksi kenaikan pola yang dinamis ($+2, +3, +4, +5$).
</details>
### Soal #211: Algoritma "Insertion Sort" (Analogi Main Kartu)
Kamu memegang kartu 5, 2, 8. Kamu ambil 2, sisipkan di sebelum 5. Lalu ambil 8, biarkan di tempat.
Proses menyisipkan data ke posisi yang benar satu-persatu ini disebut...
A. Insertion Sort.
B. Bubble Sort.
C. Selection Sort.
D. Quick Sort.

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana kamu merapikan kartu di tanganmu secara natural.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Insertion Sort.**
Algoritma ini sangat efisien untuk data yang jumlahnya sedikit atau sudah hampir terurut.
</details>

### Soal #212: Algoritma "Penghapusan Akun"
"Jika akun dihapus, MAKA hapus semua postingan akun tersebut dari database."
Apa yang terjadi jika algoritma ini lupa dijalankan (Bug)?
A. Akun tetap ada.
B. Postingan menjadi "Yatim Piatu" (Orphaned Data) yang tetap ada meski pemilik akun sudah tidak ada.
C. Database meledak.
D. User jadi senang.

<details>
<summary>💡 Hint</summary>
Data yang tidak memiliki referensi pemilik disebut data sampah yang membebani memori.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Postingan tetap ada.**
Inilah pentingnya algoritma penghapusan yang menyeluruh (*Cascading Delete*).
</details>

### Soal #213: Algoritma "Smart Chatbot"
User: "Halo". Bot: "Halo juga!".
User: "Jam berapa?". Bot: "Jam 12:00".
User: "xyz123". Bot: "Maaf, saya tidak mengerti".
Instruksi terakhir (xyz123) menunjukkan algoritma...
A. Error sistem.
B. Default Response (Respon Standar) untuk input yang tidak ada di database.
C. Bot sedang lelah.
D. Bot minta dipuji.

<details>
<summary>💡 Hint</summary>
Setiap algoritma harus memiliki penanganan untuk input yang tidak terduga (*Unrecognized input*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Default Response.**
Menjaga interaksi tetap elegan meskipun sistem tidak punya jawaban spesifik.
</details>

### Soal #214: Algoritma "Diskon Bertingkat"
"Diskon 10%, jika pakai kartu member diskon lagi 5% dari harga setelah diskon pertama."
Harga: Rp 100.000. Berapa harga akhirnya?
A. Rp 85.000
B. Rp 85.500
C. Rp 90.000
D. Rp 15.000

<details>
<summary>💡 Hint</summary>
Langkah 1: 00.000 - 10.000 = 90.000$. Langkah 2: 0.000 - (5\% \times 90.000) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 85.500.**
Perhitungan diskon majemuk yang sering digunakan dalam modul kasir.
</details>

### Soal #215: Algoritma "Cek Password" (Brute Force Protection)
"Setelah 3 kali salah, berikan jeda 1 menit sebelum bisa mencoba lagi."
Apa fungsi algoritma jeda ini?
A. Biar user istirahat.
B. Menghambat algoritma "Brute Force" (penebak otomatis) agar tidak bisa mencoba jutaan kali dalam sekejap.
C. Biar server dingin.
D. Biar user ingat passwordnya.

<details>
<summary>💡 Hint</summary>
Mempersulit peretas dengan membatasi kecepatan percobaan (*Rate Limiting*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghambat Brute Force.**
Keamanan algoritma login seringkali menggunakan faktor waktu sebagai pelindung tambahan.
</details>

### Soal #216: Algoritma "Shortest Task First" (Optimasi)
Tugas A (2 jam), Tugas B (1 jam), Tugas C (3 jam).
Agar total waktu antrean (tunggu) semua orang minimal, urutan mana yang benar?
A. C - A - B
B. B - A - C
C. A - B - C
D. Sembarang

<details>
<summary>💡 Hint</summary>
Selesaikan yang paling cepat dulu agar orang lain tidak menunggu lama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B - A - C.**
B (1 jam) + A (2 jam) + C (3 jam). Inilah algoritma penjadwalan CPU paling dasar.
</details>

### Soal #217: Algoritma "Search" (Wildcard)
Kamu mencari file dengan mengetik "Tugas*". Apa yang ditemukan sistem?
A. Hanya file bernama "Tugas".
B. Semua file yang diawali kata "Tugas" (misal: "TugasMTK", "TugasIPA").
C. File bergambar bintang.
D. Tidak ada hasil.

<details>
<summary>💡 Hint</summary>
Tanda bintang (*) berarti "Boleh apa saja setelah ini".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Diawali kata "Tugas".**
Pencarian fleksibel (*Wildcard Search*) menggunakan simbol untuk mewakili karakter acak.
</details>

### Soal #218: Algoritma "Kompresi Gambar" (Lossy)
Kenapa foto WhatsApp kualitasnya lebih rendah dari foto di Galeri?
A. WhatsApp sengaja merusak.
B. Algoritma kompresi WhatsApp membuang detail warna yang kurang terlihat mata manusia agar ukuran file kecil (Hemat Kuota).
C. HP kamu rusak.
D. Jaringan lemah.

<details>
<summary>💡 Hint</summary>
Abstraksi data gambar dengan membuang piksel yang dianggap tidak signifikan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kompresi data.**
Inilah *Lossy Compression*, algoritma yang menukar kualitas dengan efisiensi pengiriman.
</details>

### Soal #219: Algoritma "Urutan Rank Kelas" (Tie-Breaker)
Ali dan Budi punya nilai rata-rata sama (90). Ali absen 0 hari, Budi absen 2 hari.
Sistem: "Jika rata-rata sama, pilih yang absennya lebih sedikit".
Siapa juara 1?
A. Ali
B. Budi
C. Keduanya juara 1.
D. Tidak ada juara.

<details>
<summary>💡 Hint</summary>
Kriteria kedua (Absensi) digunakan sebagai pemutus seri (*Tie-Breaker*).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ali.**
Algoritma sorting tingkat lanjut seringkali memiliki beberapa kriteria berurutan.
</details>

### Soal #220: Algoritma "Loop Matematika" (Increment)
 = 0$. Ulangi:  = N + 2$. Ulangi sampai  > 10$.
Apa angka terakhir yang disimpan di 0
A. 10
B. 12
C. 11
D. 2

<details>
<summary>💡 Hint</summary>
0, 2, 4, 6, 8, 10 ... apakah 10 sudah > 10? Belum. Lanjut sekali lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 12.**
Loop berhenti segera setelah kondisi 2 > 10$ terpenuhi.
</details>

### Soal #221: Algoritma "Keliling Persegi" (Input Check)
Rumus:  \times 4$. Input: himBHs5$. Apa output yang benar bagi program yang aman?
A. -20
B. 20
C. Tampilkan pesan: "Input harus positif!".
D. 0

<details>
<summary>💡 Hint</summary>
Panjang benda tidak mungkin bernilai negatif.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Pesan Error.**
Pengecekan validitas input (*Sanitization*) mencegah algoritma menghasilkan data yang mustahil.
</details>

### Soal #222: Algoritma "Searching" (Index)
Daftar: [Apel, Jeruk, Mangga]. Di komputer, "Apel" berada di index nomor...
A. 1
B. 0
C. A
D. 3

<details>
<summary>💡 Hint</summary>
Mayoritas bahasa pemrograman modern memulai urutan (Array Index) dari angka 0.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0**
Urutan data komputer: 0, 1, 2, dst. Penting bagi pemahaman dasar CT.
</details>

### Soal #223: Algoritma "Block Teman"
"Jika Budi diblokir oleh Anda, maka Budi tidak bisa melihat postingan Anda."
Jika Budi membuat akun baru (palsu), apakah dia bisa melihat postingan Anda?
A. Tidak bisa, sistem pintar.
B. Bisa, karena identitas digitalnya (User ID) sudah berbeda di mata algoritma.
C. Tergantung settingan HP.
D. Postingan Anda hilang.

<details>
<summary>💡 Hint</summary>
Blokir biasanya berbasis pada Identitas Akun, bukan Identitas Fisik orangnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bisa.**
Kelemahan algoritma blokir sederhana yang tidak mengenali perangkat atau alamat IP.
</details>

### Soal #224: Algoritma "Pesan Makan" (Delivery Time)
Waktu kirim = (Jarak x 2 menit) + Waktu Masak (10 menit).
Jarak: 5 km. Berapa lama totalnya?
A. 10 menit
B. 20 menit
C. 25 menit
D. 30 menit

<details>
<summary>💡 Hint</summary>
 + 10 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 20 menit.**
Data input jarak diolah oleh rumus estimasi waktu (ETA algorithm).
</details>

### Soal #225: Algoritma "Sortir Berdasarkan Tanggal"
File A (1 Januari), File B (30 Desember tahun lalu), File C (1 Februari).
Urutan dari yang **Terbaru** (Newest to Oldest):
A. C - A - B
B. A - B - C
C. B - A - C
D. C - B - A

<details>
<summary>💡 Hint</summary>
Urutkan dari bulan yang paling jauh angkanya di kalender tahun ini.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. C (Februari) - A (Januari) - B (Desember lalu).**
Inilah logika pengurutan kronologis terbalik (Reverse Chronological).
</details>

### Soal #226: Algoritma "Kalkulator Pajak"
"Pajak 10% jika penghasilan > Rp 4jt. Jika tidak, pajak 0%."
Penghasilan Budi: Rp 4.000.000 tepat. Berapa pajaknya?
A. Rp 400.000
B. Rp 0
C. Rp 40.000
D. Serikhlasnya.

<details>
<summary>💡 Hint</summary>
Syaratnya adalah "lebih besar dari". Angka 4jt tidak lebih besar dari 4jt.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 0.**
Logika "Strictly Greater Than" (>) mengecualikan nilai batas itu sendiri.
</details>

### Soal #227: Algoritma "Game - Damage Calculation"
"Damage = Serangan - Pertahanan Musuh".
Serangan kamu: 50. Pertahanan Musuh: 70. Apa Damage-nya?
A. -20
B. 0 (Minimal damage biasanya tidak boleh negatif).
C. 50
D. Musuhnya kalah.

<details>
<summary>💡 Hint</summary>
Algoritma game biasanya menambahkan pengecekan: "Jika hasil < 0, maka set jadi 0".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0**
Logika pencegahan nilai negatif dalam simulasi sistem realitas fisik.
</details>

### Soal #228: Algoritma "Sorting Gelembung" (Bubble Sort Ascending)
Daftar: [5, 4, 3]. Setelah satu putaran (Round 1) penuh, angka mana yang pasti di posisi paling benar?
A. Angka 5 di paling belakang.
B. Angka 3 di paling depan.
C. Semua sudah rapi.
D. Angka 4 di tengah.

<details>
<summary>💡 Hint</summary>
Bubble sort mendorong angka terbesar ke ujung kanan "seperti gelembung".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Angka 5 di paling belakang.**
Setiap satu putaran, satu angka terbesar akan "mengapung" sampai ke posisi akhir yang seharusnya.
</details>

### Soal #229: Algoritma "Antivirus - Scan" (Partial Scan)
Kenapa scan folder tertentu lebih cepat daripada scan seluruh komputer?
A. Karena antivirus malas.
B. Karena jumlah data (Input Size) yang diproses lebih sedikit, sehingga langkah pengulangan pencarian lebih singkat.
C. Folder itu isinya virus semua.
D. Komputernya takut.

<details>
<summary>💡 Hint</summary>
Efisien waktu berbanding lurus dengan jumlah data yang harus diperiksa (*Linear Time Complexity*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Input Size lebih sedikit.**
Contoh nyata bagaimana abstraksi area pencarian menghemat waktu eksekusi.
</details>

### Soal #230: Algoritma "Mencari Nama" (Binary Search Trick)
Kamu mencari nama "Zulkifli" di buku telepon. Haruskah kamu mulai dari tengah?
A. Ya, selalu mulai dari tengah itu paling aman (Teori Binary Search).
B. Tidak, secara cerdas kita bisa langsung buka bagian belakang (Interpolation Search).
C. Mulai dari depan saja.
D. Tanya orang.

<details>
<summary>💡 Hint</summary>
Manusia sering menggunakan data "Kira-kira letaknya dimana" untuk memotong langkah lebih banyak lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Langsung ke belakang.**
Inilah optimasi algoritma pencarian jika kita tahu distribusi datanya (Z pasti di belakang).
</details>

### Soal #231: Algoritma "Cek Koneksi" (Ping)
Waktu ping: 500 ms. Artinya...
A. Internet super cepat.
B. Sinyal dikirim dan dibalas dalam waktu 0,5 detik (Cukup lambat untuk game online).
C. Provider kamu bangkrut.
D. Download film selesai dalam 0,5 detik.

<details>
<summary>💡 Hint</summary>
Ping mengukur waktu pulang-pergi paket data dalam milidetik (1000 ms = 1 detik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Waktu kirim-balas 0,5 detik.**
Parameter efisiensi latensi dalam algoritma jaringan.
</details>

### Soal #232: Algoritma "Matematika Bunga"
"Bunga 1% per bulan dari sisa uang". Uang: Rp 1.000.000. Setelah 1 bulan, berapa uangnya?
A. Rp 1.001.000
B. Rp 1.010.000
C. Rp 1.100.000
D. Rp 2.000.000

<details>
<summary>💡 Hint</summary>
\% \text{ dari } 1 \text{ juta} = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 1.010.000.**
\% \times 1.000.000 = 10.000$. Penambahan saldo otomatis oleh sistem perbankan.
</details>

### Soal #233: Algoritma "Lupa Password" (Security)
"Masukkan kode yang dikirim ke HP Anda". Ini merupakan pertahanan terhadap...
A. Orang yang tidak punya HP.
B. Orang yang tahu password Anda tapi tidak memegang HP Anda (Two-Factor Authentication).
C. Provider sinyal.
D. Iklan.

<details>
<summary>💡 Hint</summary>
Menambah lapisan keamanan di luar sekadar "apa yang dihafal" (Password).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Two-Factor Authentication (2FA).**
Algoritma keamanan yang menggabungkan dua kunci berbeda untuk akses akun.
</details>

### Soal #234: Algoritma "Sorting Warna"
Daftar: Merah, Putih, Biru. Urutkan berdasarkan "Urutan Warna Pelangi" (Me-Ji-Ku-Hi-Bi-Ni-U).
A. Merah - Biru - Putih
B. Merah - Putih - Biru
C. Putih - Merah - Biru
D. Biru - Merah - Putih

<details>
<summary>💡 Hint</summary>
Putih tidak ada di pelangi, biasanya ditaruh paling akhir (Default). Merah (Me) paling depan, Biru (Bi) setelahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Merah - Biru - Putih.**
Pengurutan data berdasarkan standar referensi tertentu (Custom Sort).
</details>

### Soal #235: Algoritma "Auto-Brightness"
"Jika cahaya lingkungan terang, naikkan kecerahan layar agar terbaca".
Siapa yang memberikan **Input** terang/gelap pada algoritma ini?
A. Mata user.
B. Sensor cahaya (Ambient Light Sensor) di dekat kamera depan.
C. Aplikasi penghemat baterai.
D. Google.

<details>
<summary>💡 Hint</summary>
Hardware pendeteksi rangsang cahaya di perangkat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor cahaya.**
Penerjemahan kondisi fisis menjadi data digital untuk diproses algoritma.
</details>

### Soal #236: Algoritma "Mode Gelap" (Dark Mode)
Kenapa sistem mengganti background putih jadi hitam?
A. Agar tulisan tidak terbaca.
B. Menghemat daya baterai (pada layar OLED) dan mengurangi kelelahan mata.
C. Biar HP-nya terlihat mahal.
D. Biar user cepat tidur.

<details>
<summary>💡 Hint</summary>
Pada layar tertentu, piksel warna hitam berarti lampu piksel tersebut mati (0 daya).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hemat daya & nyaman di mata.**
Optimasi antarmuka berdasarkan efisiensi energi hardware.
</details>

### Soal #237: Algoritma "Search" (Autocomplete)
Baru ketik "A-L-G-O", sistem sudah menyarankan "ALGORITMA". Ini bekerja dengan mencari...
A. Kata yang paling banyak dicari orang lain yang diawali huruf tersebut.
B. Kata yang paling kamu suka.
C. Nama temanmu.
D. Kata yang paling pendek.

<details>
<summary>💡 Hint</summary>
Memanfaatkan database frekuensi pencarian populer.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kata populer.**
Contoh nyata dari algoritma prediksi berbasis data besar (*Big Data*).
</details>

### Soal #238: Algoritma "Filter Chat" (Bukan Kata Kasar)
"Jika pesan mengandung 'MENANG', ganti jadi 'JUARA'".
Pesan: "SAYA MENANG LOMBA". Apa hasilnya?
A. SAYA JUARA LOMBA.
B. SAYA MENANG LOMBA.
C. SAYA *** LOMBA.
D. PESAN DIHAPUS.

<details>
<summary>💡 Hint</summary>
Algoritma cari dan ganti (*Replace*) mengganti per-kata secara spesifik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. SAYA JUARA LOMBA.**
Fungsi dasar manipulasi teks dalam sistem otomasi pesan.
</details>

### Soal #239: Algoritma "Matematika Jarak"
Kamu jalan 10 langkah ke Depan, lalu 4 langkah ke Belakang. Dimana posisi akhirmu dari titik awal?
A. 14 langkah di depan.
B. 6 langkah di depan.
C. 10 langkah di belakang.
D. 4 langkah di depan.

<details>
<summary>💡 Hint</summary>
0 - 4 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 6 langkah di depan.**
Logika posisi relatif dalam sistem koordinat sederhana.
</details>

### Soal #240: Algoritma "Antrean GoFood - Status"
1. Pesanan Diterima.
2. Driver Menuju Resto.
3. Driver Memesan.
4. Driver Mengantar.
5. Selesai.
Kenapa status ini penting?
A. Biar user tidak bosan.
B. Menunjukkan transparansi proses (Feedback) agar user tahu algoritma berjalan di tahap mana.
C. Biar drivernya bangga.
D. Biar makanannya makin enak.

<details>
<summary>💡 Hint</summary>
Setiap sistem harus memberikan informasi status saat menjalankan proses yang memakan waktu lama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Transparansi proses.**
Bagian dari "Sistem Informasi" untuk menjaga kepercayaan pengguna.
### Soal #241: Algoritma "Family Tree" (Tree Structure)
Dalam silsilah keluarga, Ayah berada di posisi atas, Anak di bawah. Struktur data ini disebut...
A. Linear List.
B. Tree (Pohon).
C. Grid.
D. Loop.

<details>
<summary>💡 Hint</summary>
Memiliki satu akar (Root) yang bercabang ke bawah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tree.**
Struktur hirarkis yang digunakan komputer untuk mengelola folder dan file.
</details>

### Soal #242: Algoritma "Sorting Usia"
Guru ingin membagi kelas jadi kelompok beranggotakan 2 orang dengan selisih usia paling sedikit. Algoritma apa yang harus guru lakukan pertama kali?
A. Memasangkan secara acak.
B. Mengurutkan (Sorting) seluruh siswa berdasarkan tanggal lahir.
C. Menghitung jumlah siswa.
D. Bertanya siapa yang mau berkelompok.

<details>
<summary>💡 Hint</summary>
Dengan data yang sudah terurut, dua orang yang paling mirip usianya pasti duduk berdekatan di daftar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sorting tanggal lahir.**
Penyelesaian masalah optimasi menggunakan data terurut.
</details>

### Soal #243: Algoritma "Chat - Read Receipt"
"Jika pesan sudah dibuka oleh penerima, ubah status 'Terkirim' menjadi 'Dibaca'".
Ini adalah contoh mekanisme...
A. Input user.
B. Event Trigger (Pemicu berdasarkan aksi tertentu).
C. Error aplikasi.
D. Penghapusan data.

<details>
<summary>💡 Hint</summary>
Perubahan status terjadi otomatis segera setelah "Event" (pesan dibuka) terdeteksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Event Trigger.**
Bagian dinamis dari desain algoritma aplikasi komunikasi.
</details>

### Soal #244: Algoritma "RAM vs Storage"
Data di RAM (Memori) akan hilang jika listrik mati, sedangkan di Storage (Harddisk) tidak.
Manakah algoritma yang **Paling Berisiko** jika tidak ada fitur Auto-save?
A. Algoritma pengetikan di layar (data disimpan di RAM).
B. Algoritma pemindahan file ke flashdisk.
C. Algoritma pencarian Google.
D. Algoritma ganti wallpaper.

<details>
<summary>💡 Hint</summary>
Data yang sedang diketik biasanya hanya mengambang di memori sementara.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hasil mengetik.**
Pentingnya memindahkan data dari yang mudah menguap (*Volatile*) ke yang permanen.
</details>

### Soal #245: Algoritma "Nilai KKM"
"Lulus jika (Nilai >= 75) **DAN** (Kehadiran >= 80%)".
Status: Nilai 100, Kehadiran 70%. Hasil?
A. Lulus
B. Tidak Lulus
C. Lulus Bersyarat
D. Tanya Wakasek

<details>
<summary>💡 Hint</summary>
Logika AND menuntut ketaatan pada **semua** aturan tanpa terkecuali.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lulus.**
Meskipun nilai sempurna, syarat kehadiran tidak terpenuhi (False).
</details>

### Soal #246: Algoritma "Kalkulator Sederhana" (Round)
Hasil asli: 7.9. Kamu ingin output dibulatkan ke bawah (*Floor*). Hasilnya?
A. 8
B. 7
C. 7.5
D. 0

<details>
<summary>💡 Hint</summary>
Pembulatan ke bawah mengabaikan desimal berapapun besarnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 7.**
Operasi pembulatan sering digunakan untuk indeks array atau pembagian jumlah barang.
</details>

### Soal #247: Algoritma "Cari Nama Unik"
Daftar: [Ani, Budi, Ani, Cici]. Algoritma penghapusan duplikat akan menghasilkan...
A. [Ani, Budi, Cici]
B. [Ani, Budi, Ani, Cici]
C. [Budi, Cici]
D. [Ani]

<details>
<summary>💡 Hint</summary>
Data yang sama hanya boleh muncul satu kali saja di hasil akhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Ani, Budi, Cici].**
Aplikasi pembersihan data (*De-duplication*) untuk efisiensi penyimpanan.
</details>

### Soal #248: Algoritma "Multi-Tasking" (OS)
Komputer seolah-olah menjalankan 10 aplikasi barengan. Rahasianya?
A. Prosesornya ada 1000.
B. Algoritma "Time Slicing" (Membagi waktu super cepat antar aplikasi sehingga mata manusia tidak menyadari gantiannya).
C. Aplikasinya saling bantu.
D. Ghaib.

<details>
<summary>💡 Hint</summary>
Prinsip penjadwalan CPU dalam Sistem Operasi modern.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pembagian waktu (Time Slicing).**
Kecepatan eksekusi ribuan kali per detik membuat ilusi keserentakan.
</details>

### Soal #249: Algoritma "Password Wifi" (Encryption Key)
Kenapa router minta password panjang?
A. Biar kabel tidak panas.
B. Semakin panjang password, semakin banyak kemungkinan kombinasi yang harus dicoba (Key Space Expansion).
C. Biar tidak ada yang pake.
D. Biar router tidak bosan.

<details>
<summary>💡 Hint</summary>
Algoritma Brute Force akan butuh waktu bertahun-tahun untuk menebak password yang sangat panjang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memperbanyak kombinasi.**
Prinsip dasar ketahanan kriptografi terhadap serangan tebakan.
</details>

### Soal #250: Algoritma "Sorting Ranking" (Informatika Konteks)
Kamu ingin mengurutkan 1000 pemenang lomba coding. Algoritma mana yang paling pas untuk menangani data besar tersebut secara cepat?
A. Bubble Sort.
B. Merge Sort atau Quick Sort.
C. Menunjuk manual satu per satu.
D. Tidak usah diurutkan.

<details>
<summary>💡 Hint</summary>
Gunakan konsep "Divide and Conquer" untuk kecepatan tinggi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Merge Sort / Quick Sort.**
Efisien secara algoritma (O(n log n)) jauh melampaui algoritma sederhana (O(n²)).
</details>

### Soal #251: Algoritma "Searching" (Linear vs Binary)
Dalam daftar 1.000.000 nama yang sudah terurut, pencarian biner butuh maksimal hanya 20 langkah. Pencarian satu-satu butuh maksimal...
A. 20 langkah juga.
B. 1.000.000 langkah.
C. 500.000 langkah.
D. 0 langkah.

<details>
<summary>💡 Hint</summary>
Linear search harus mengecek setiap elemen jika data ada di paling bawah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1.000.000 langkah.**
Inilah perbandingan efisiensi yang sangat jauh antara algoritma cerdas dan algoritma biasa.
</details>

### Soal #252: Algoritma "Smart Traffic Light"
"Jika panjang antrean mobil > 10, tambahkan durasi lampu hijau selama 5 detik."
Jika mobil ada 11, apa yang terjadi?
A. Lampu merah makin lama.
B. Lampu hijau jadi lebih lama dari biasanya.
C. Lampu mati.
D. Polisi datang.

<details>
<summary>💡 Hint</summary>
Pemanfaatan data *Real-time* untuk mengubah parameter proses secara dinamis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampu hijau lebih lama.**
Optimasi kemacetan berbasis algoritma adaptif.
</details>

### Soal #253: Algoritma "Lupa Password" (Identity Proof)
"Siapa nama guru favoritmu?". Ini adalah bagian dari algoritma...
A. Interogasi.
B. Pertanyaan Keamanan (Security Questions) untuk verifikasi identitas pemilik asli.
C. Ramalan masa depan.
D. Cerita sekolah.

<details>
<summary>💡 Hint</summary>
Metode otentikasi alternatif jika kunci utama (Password) hilang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pertanyaan Keamanan.**
Lapisan pertahanan terakhir dalam pemulihan akses akun.
</details>

### Soal #254: Algoritma "Sorting Nama" (Suffix Ignore)
Daftar: "Dr. Budi", "Prof. Ani", "Dr. Cici". Guru ingin urut berdasarkan nama asli (A-B-C).
Algoritma guru harus mengabaikan "Dr." dan "Prof.". Langkah ini disebut...
A. Data Cleaning (Pembersihan Data).
B. Data Deletion.
C. Data Masking.
D. Data Hiding.

<details>
<summary>💡 Hint</summary>
Menghapus gelar untuk mendapatkan data inti yang akan diolah (Abstraksi).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Data Cleaning.**
Persiapan data mentah menjadi data siap proses dalam algoritma sortir.
</details>

### Soal #255: Algoritma "Penghitung Tiket"
Terjual 100 tiket. Harga Rp 5.000. Tapi ada biaya admin Rp 1.000 per tiket. Berapa total uang bruto (kotor) yang terkumpul?
A. Rp 500.000
B. Rp 600.000
C. Rp 400.000
D. Rp 1.000

<details>
<summary>💡 Hint</summary>
 \times 100 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 600.000.**
Kalkulasi biaya total dalam algoritma sistem kasir online.
</details>

### Soal #256: Algoritma "Loop Ganjil"
Instruksi: "Tulis angka ganjil mulai dari 1. Berhenti jika jumlah angka yang ditulis sudah 3."
Apa hasilnya?
A. 1, 3, 5
B. 1, 3, 5, 7, 9
C. 1, 3
D. 3, 2, 1

<details>
<summary>💡 Hint</summary>
Cacah angka ganjil satu-persatu sampai tanganmu memegang 3 angka.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 1, 3, 5.**
Pengontrolan jumlah perulangan (*Count-controlled loop*) dalam algoritma.
</details>

### Soal #257: Algoritma "Koneksi Wifi" (Signal Strength)
"Sambungkan ke wifi yang sinyalnya paling kuat (Nilai dBm paling tinggi)".
Wifi A (-50), Wifi B (-80). Mana yang dipilih?
A. Wifi B (angkanya lebih besar 80).
B. Wifi A (secara fisik -50 lebih besar/mendekati nol daripada -80).
C. Sinyal yang namanya paling bagus.
D. Cari wifi lain.

<details>
<summary>💡 Hint</summary>
Dalam dBm, angka negatif yang lebih kecil menunjukkan sinyal yang lebih kuat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Wifi A.**
Logika perbandingan bilangan negatif dalam algoritma pemilihan jaringan.
</details>

### Soal #258: Algoritma "Auto-Save" (Condition)
Sistem menyimpan otomatis hanya jika ada perubahan teks (Dirty Flag). Jika kamu hanya membaca file selama 1 jam tanpa mengetik apapun, apakah sistem menyimpan?
A. Ya, kan sudah 1 jam.
B. Tidak, karena status 'Berubah' bernilai False.
C. Ya, secara random.
D. Simpan file baru.

<details>
<summary>💡 Hint</summary>
Efisien penyimpanan: Jangan menulis ke disk jika data tidak ada bedanya dengan yang lama (*Redundant write prevention*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Logika penghematan daya prosesor dan umur memori penyimpanan (*I/O optimization*).
</details>

### Soal #259: Algoritma "Searching" (Substring)
Cari file yang mengandung kata "Ujian".
File: "Persiapan_Ujian_MTK.pdf". Apakah ditemukan?
A. Tidak, namanya harus persis "Ujian".
B. Ya, ditemukan karena kata "Ujian" ada di dalam nama file tersebut.
C. Tergantung foldernya.
D. Masuk ke folder spam.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma pencarian teks sebagian (*Substring Search*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ya, ditemukan.**
Prinsip dasar pencarian file di Windows Explorer atau Finder.
</details>

### Soal #260: Algoritma "Sort Nama Keraton"
Pangeran A, Pangeran B, Raja C. Kamu ingin urutkan berdasarkan **Kekuasaan** (Paling tinggi di atas).
A. Pangeran A, Pangeran B, Raja C.
B. Raja C, Pangeran A, Pangeran B.
C. Pangeran B, Pangeran A, Raja C.
D. Urut abjad.

<details>
<summary>💡 Hint</summary>
Gunakan hirarki jabatan sebagai pembanding, bukan abjad.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Raja C (Atas).**
Struktur data hirarkis (Tree) diaplikasikan ke dalam urutan sorting.
</details>

### Soal #261: Algoritma "Trace Loop" (Sum)
 = 0$. Ulangi $ dari 1 sampai 3:  = Total + i$.
Berapa nilai 127
A. 3
B. 6
C. 1
D. 0

<details>
<summary>💡 Hint</summary>
 + 2 + 3 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 6.**
Algoritma akumulasi nilai (Summation) yang sangat sering digunakan dalam pemrograman.
</details>

### Soal #262: Algoritma "Block Ads"
"Jika alamat web mengandung kata 'iklan.com', jangan tampilkan konten dari sumber itu."
Sebuah website 'berita.com' memanggil file dari 'iklan.com/pop-up.jpg'. Apakah gambarnya muncul?
A. Muncul, kan di website berita.
B. Tidak muncul, karena sumber gambarnya diblokir oleh aturan algoritma.
C. Muncul separo.
D. Browser error.

<details>
<summary>💡 Hint</summary>
Sistem keamanan/filter melihat asal-usul setiap file yang dipanggil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak muncul.**
Cara kerja dasar ekstensi *Add-blocker* di browser internet.
</details>

### Soal #263: Algoritma "Ojek Online - Ongkir"
"Ongkir = Jarak x 2.000. Jika jarak > 10 km, tambah biaya tambahan 5.000."
Jarak rumahmu 11 km. Berapa ongkirnya?
A. Rp 22.000
B. Rp 27.000
C. Rp 20.000
D. Rp 11.000

<details>
<summary>💡 Hint</summary>
 + 5.000 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 27.000.**
Penambahan biaya bersyarat (*Surcharge algorithm*) dalam sistem transportasi.
</details>

### Soal #264: Algoritma "Memory - Copy Paste"
Saat kamu klik "Copy", data tersebut pergi kemana sementara?
A. Ke Harddisk (Penyimpanan lama).
B. Ke Clipboard (Bagian kecil di RAM).
C. Ke Google.
D. Hilang selamanya.

<details>
<summary>💡 Hint</summary>
Data harus disimpan di tempat yang aksesnya sangat cepat dan sementara.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Clipboard.**
Pemanfaatan alokasi memori sementara dalam algoritma manajemen sistem.
</details>

### Soal #265: Algoritma "Nilai Rata-rata" (Input Kosong)
Jika tidak ada nilai yang dimasukkan (0 data), apa hasil pembagian rata-rata secara algoritma?
A. 0.
B. Error "Division by Zero" (Pembagian dengan nol).
C. 100.
D. Menunggu selamanya.

<details>
<summary>💡 Hint</summary>
Pembilang 0, Penyebut 0. Matematika komputer tidak mengizinkan penyebut bernilai 0.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Error pembagian dengan nol.**
Pentingnya menangani kasus data kosong dalam perancangan aplikasi.
</details>

### Soal #266: Algoritma "Searching" (Find Friend)
Kamu mencari teman bernama "Andi". Ada 5 "Andi" di sekolah. Manakah yang dicari komputer jika kamu tidak memberikan detail lain?
A. Andi yang paling baik.
B. Semua orang bernama Andi ditampilkan (Multiple Results).
C. Andi yang paling ganteng/cantik.
D. Andi yang nomor absennya paling kecil saja.

<details>
<summary>💡 Hint</summary>
Searching tanpa filter unik (*Unique Key*) akan menghasilkan semua data yang cocok.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tampilkan semuanya.**
Tanpa parameter tambahan, hasil pencarian adalah himpunan semua data yang memenuhi syarat.
</details>

### Soal #267: Algoritma "Cek Password" (Hashing)
Sistem tidak menyimpan password aslimu ("123456"), tapi menyimpan kodenya ("#a%7x$"). Saat kamu login, sistem menyandikan inputmu dan membandingkan kodenya. Proses penyandian satu arah ini disebut...
A. Hashing.
B. Copying.
C. Printing.
D. Sorting.

<details>
<summary>💡 Hint</summary>
Mengubah data jadi kode unik yang tidak bisa dikembalikan ke asalnya demi keamanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hashing.**
Teknik keamanan algoritma standar industri untuk melindungi privasi user.
</details>

### Soal #268: Algoritma "Queue" (Print Task)
Dokumen A (Halaman 100), Dokumen B (Halaman 1). Dimasukkan berurutan ke printer. Dokumen mana yang tercetak selesai paling akhir?
A. Dokumen B.
B. Dokumen A.
C. Selesai bareng.
D. Tergantung tintanya.

<details>
<summary>💡 Hint</summary>
Printer memproses antrean berdasarkan urutan masuk (FIFO).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Dokumen B.**
Karena B harus menunggu printer menyelesaikan 100 halaman milik A dulu.
</details>

### Soal #269: Algoritma "Sorting" (Inverse)
Daftar: 1, 2, 3. Instruksi: "Tukar semua posisi depan ke belakang."
Hasil: 3, 2, 1. Operasi ini disebut...
A. Sorting.
B. Reverse (Pembalikkan).
C. Shuffling (Pengacakan).
D. Deleting.

<details>
<summary>💡 Hint</summary>
Membalikkan urutan urutan tanpa mengubah nilai datanya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Reverse.**
Aksi mendasar dalam memutar posisi data dalam struktur list/array.
</details>

### Soal #270: Algoritma "Matematika Binari" (8-bit)
Satu kotak biner hanya bisa menyimpan 0 atau 1. Berapa banyak kombinasi angka yang bisa dibuat dengan **3 kotak** biner (3-bit)?
A. 3 kombinasi.
B. 6 kombinasi.
C. 8 kombinasi (2 pangkat 3).
D. Tak terhingga.

<details>
<summary>💡 Hint</summary>
Hasilnya: 000, 001, 010, 011, 100, 101, 110, 111.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 8 kombinasi.**
Dasar kapasitas penyimpanan data digital dalam arsitektur komputer.
</details>

### Soal #271: Algoritma "Cari Buku" (Alphabetical)
Kamu mencari buku "Fisika". Rak diatur: [Biologi, Ekonomi, Kimia, Matematika]. Dimanakah letak buku Fisika jika disusun abjad?
A. Di antara Biologi dan Ekonomi.
B. Di antara Ekonomi dan Kimia.
C. Di ujung kanan rak.
D. Di rak lain.

<details>
<summary>💡 Hint</summary>
E (5), F (6), K (11). Fisika berawal dari F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Antara Ekonomi dan Kimia.**
Penerapan sorting abjad di dunia nyata untuk kemudahan pencarian.
</details>

### Soal #272: Algoritma "Checklist Kebersihan" (Loop)
"Sapu 10 ruangan. Jika sudah 5 ruangan, ambil air minum."
Kapan instruksi ambil air minum dilakukan?
A. Sebelum menyapu sama sekali.
B. Di tengah-tengah proses (Antara ruangan ke-5 dan ke-6).
C. Setelah semua 10 ruangan bersih.
D. Tidak perlu minum.

<details>
<summary>💡 Hint</summary>
Ini adalah instruksi bersyarat di dalam sebuah siklus (Loop with condition).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di tengah proses.**
Interupsi pengulangan berdasarkan jumlah (Iterasi) yang sudah terlaksana.
</details>

### Soal #273: Algoritma "Konversi Suhu"
Input: 100 Celsius. Algoritma:  + 32$. Berapa Fahrenheit?
A. 100 F
B. 212 F
C. 32 F
D. 180 F

<details>
<summary>�� Hint</summary>
 + 32 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 212 F.**
Penerjemahan formula matematik ke dalam algoritma konversi data.
</details>

### Soal #274: Algoritma "Urutan Rank Game" (XP)
XP kamu 1.500. Rank Silver (1.000 XP), Rank Gold (2.000 XP).
Apa status rank kamu?
A. Bronze.
B. Silver.
C. Gold.
D. Platinum.

<details>
<summary>💡 Hint</summary>
Kamu sudah melewati batas Silver, tapi belum mencapai batas Gold.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Silver.**
Prinsip "Level Thresholding" dalam desain aplikasi dan game.
</details>

### Soal #275: Algoritma "Backup Data" (Sync)
"Update file di HDD cadangan HANYA JIKA isi filenya berbeda dengan di HDD utama."
Strategi ini menghemat...
A. Listrik monitor.
B. Waktu dan keausan perangkat penyimpanan (Efisien).
C. Biaya parkir.
D. RAM.

<details>
<summary>💡 Hint</summary>
Jangan menulis ulang hal yang sama (Redundansi).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Waktu & Keausan.**
Prinsip efisiensi dalam algoritma sinkronisasi awan (*Cloud synchronization*).
</details>

### Soal #276: Algoritma "Deteksi Wajah"
Kenapa algoritma kamera bisa tahu mana "Mata" dan mana "Hidung"?
A. Kamera punya perasaan.
B. Algoritma mencari pola gelap-terang yang mirip dengan struktur wajah manusia (Pattern Recognition).
C. Ada orang kecil di dalam kamera.
D. Kamera menebak secara acak.

<details>
<summary>💡 Hint</summary>
Pemanfaatan data visual untuk mengenali objek secara matematis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pattern Recognition.**
Contoh tingkat lanjut dari pilar Computational Thinking dalam AI.
</details>

### Soal #277: Algoritma "Kelipatan 2" (Logaritma)
Angka 1 terus dikalikan 2. Berapa kali harus dikalikan agar angkanya $\ge 100127
A. 100 kali.
B. 7 kali (^7 = 128$).
C. 2 kali.
D. 50 kali.

<details>
<summary>💡 Hint</summary>
1, 2, 4, 8, 16, 32, 64, 128.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 7 kali.**
Pemahaman pertumbuhan eksponensial dalam algoritma efisiensi memori.
</details>

### Soal #278: Algoritma "Pilih Seragam"
"Jika Senin, Merah-Putih. Jika Jumat, Batik. Jika Lainnya, Abu-abu."
Hari ini adalah **Sabtu**. Apa seragamnya?
A. Merah-Putih.
B. Batik.
C. Abu-abu.
D. Baju bebas.

<details>
<summary>💡 Hint</summary>
Kategori "Lainnya" (Else/Default) akan mencakup semua hari selain Senin dan Jumat.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Abu-abu.**
Penanganan kondisi pengecualian (Else) dalam sebuah algoritma keputusan.
</details>

### Soal #279: Algoritma "Pencarian Paling Cepat" (Sorting First)
Kamu ingin mencari 10 barang di gudang. Lebih cepat mana secara algoritma?
A. Langsung cari satu-persatu di gudang yang berantakan.
B. Habiskan 5 menit untuk merapikan gudang (Sorting), lalu cari semuanya (Searching).
C. Minta teman carikan.
D. Biarkan barangnya hilang.

<details>
<summary>💡 Hint</summary>
Investasi waktu di awal (Sorting) akan memangkas waktu pencarian secara drastis untuk pencarian berulang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Merapikan dulu.**
Hubungan simbiosis antara algoritma Sorting dan Searching untuk efisiensi total.
</details>

### Soal #280: Algoritma "Trace Variabel" (Chain)
1.  = 10, B = 5$
2.  = A + B$
3.  = A - B$
4.  = A - B$
Apa nilai $ dan $ sekarang?
A. =5, B=10$
B. =10, B=5$
C. =15, B=15$
D. =0, B=0$

<details>
<summary>💡 Hint</summary>
Coba hitung lagi: L2 (=15$), L3 (=15-5=10$), L4 (=15-10=5$).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. A=5, B=10.**
Sudah diuji sebelumnya, ini adalah cara menukar nilai tanpa variabel ketiga.
</details>

### Soal #281: Algoritma "Penyortiran Surat"
Tukang pos menyisipkan surat ke alamat yang tepat sambil berjalan menyusuri jalan. Ini paling mirip dengan...
A. Insertion Sort.
B. Quick Sort.
C. Bubble Sort.
D. Random Shuffle.

<details>
<summary>💡 Hint</summary>
Menyisipkan data satu-persatu ke tumpukan yang sudah terurut.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Insertion Sort.**
Memahami kemiripan aktivitas manusia dengan pola algoritma komputer.
</details>

### Soal #282: Algoritma "Pesan Makan Online - Ongkir"
"Ongkir gratis jika total belanja > 100rb, atau ada Promo Kode."
Belanja 50rb, Pakai Promo Kode. Apakah gratis ongkir?
A. Tidak, belanjaannya kurang.
B. Ya, karena syarat ATAU (OR) cukup salah satu yang terpenuhi.
C. Bayar separo.
D. Tanya driver.

<details>
<summary>💡 Hint</summary>
Logika OR: Salah + Benar = Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ya, gratis ongkir.**
Aplikasi logika disjungsi dalam sistem pemasaran digital.
</details>

### Soal #283: Algoritma "Game - Respawn"
"Jika Darah == 0, pindahkan pemain ke Titik Awal (Start) dan isi Darah jadi 100."
Ini adalah jenis algoritma...
A. Reset Kondisi (State Reset).
B. Penghapusan Karakter.
C. Leveling Up.
D. Menang Game.

<details>
<summary>💡 Hint</summary>
Mengembalikan status game ke kondisi awal setelah sebuah "kekalahan" terdeteksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Reset Kondisi.**
Pengelolaan siklus hidup (Lifecycle) objek dalam sebuah algoritma interaktif.
</details>

### Soal #284: Algoritma "Searching" (Wildcard Advanced)
Kamu mencari file dengan "?.jpg". Tanda (?) mewakili 1 huruf bebas. Mana yang ketemu?
A. Foto123.jpg.
B. A.jpg.
C. Ujian.png.
D. Foto.exe.

<details>
<summary>💡 Hint</summary>
Cari yang nama file-nya hanya satu huruf saja.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. A.jpg.**
Aturan pencarian spesifik menggunakan simbol pengganti tunggal.
</details>

### Soal #285: Algoritma "Pembaruan Aplikasi"
"Download update HANYA di malam hari (00:00 - 05:00) saat internet murah."
Jika jam 14:00 kamu klik Update, apa yang dilakukan aplikasi cerdas?
A. Download langsung.
B. Menjadwalkan (Queue/Schedule) download untuk nanti malam.
C. Tidak melakukan apa-apa.
D. Restart HP.

<details>
<summary>💡 Hint</summary>
Sistem menunda eksekusi instruksi demi optimasi sumber daya (biaya).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menjadwalkan.**
Penggunaan antrian tertunda (*Deferred execution*) dalam algoritma sistem operasional.
</details>

### Soal #286: Algoritma "Cek Angka Sempurna"
"Sebuah angka sempurna jika jumlah pembaginya (selain angka itu sendiri) sama dengan angkanya."
Contoh 6. Pembaginya: 1, 2, 3. (+2+3 = 6$).
Apa status angka **28**? (Pembagi: 1, 2, 4, 7, 14)
A. Sempurna.
B. Tidak Sempurna.
C. Terlalu besar.
D. Angka ganjil.

<details>
<summary>💡 Hint</summary>
+2+4+7+14 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Sempurna.**
+2+4+7+14 = 28$. Algoritma pengecekan properti bilangan matematik.
</details>

### Soal #287: Algoritma "Antivirus" (Quarantine)
Kenapa file bervirus tidak langsung dihapus tapi dikarantina (pindah ke folder rahasia)?
A. Biar virusnya betah.
B. Mencegah file penting terhapus permanen jika ternyata antivirus "Salah Sangka" (False Positive).
C. Biar bisa dipelajari.
D. Biar hemat memori.

<details>
<summary>💡 Hint</summary>
Ini adalah langkah pencegahan terhadap *Irreversible Error* (kesalahan yang tidak bisa diperbaiki).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah False Positive.**
Langkah moderasi dalam algoritma keamanan sistem.
</details>

### Soal #288: Algoritma "Matematika Jarak"
Kamu mau ke lantai 10. Saat ini lift di lantai 12. Berapa jarak lantai yang harus ditempuh lift?
A. 22 lantai.
B. 2 lantai (Mutlak / Absolute Distance).
C. -2 lantai.
D. Lift tidak mau gerak.

<details>
<summary>💡 Hint</summary>
$|12 - 10| = ...$ Jarak selalu bernilai positif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2 lantai.**
Menggunakan fungsi nilai mutlak dalam algoritma pergerakan fisik.
</details>

### Soal #289: Algoritma "Password Strength"
Manakah yang paling sulit ditebak oleh algoritma peretas?
A. 12345678.
B. Pa55w0rd!.
C. r4k_buku_m3r4h (Kalimat unik dengan angka/simbol).
D. namaku_budi.

<details>
<summary>💡 Hint</summary>
Pilih yang memiliki entropi paling tinggi (gabungan kata acak, angka, dan panjang).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. r4k_buku_m3r4h.**
Panjang dan variasi karakter meningkatkan tingkat kesulitan algoritma tembus paksa.
</details>

### Soal #290: Algoritma "Sort Nama Buah" (Internal Logic)
Daftar: "Apel", "Ceri", "Pisang".
Langkah 1: Jika "Apel" < "Ceri", Biarkan.
Langkah 2: Jika "Ceri" < "Pisang", Biarkan.
Langkah 3: Urutan selesai.
Metode pengecekan tetangga ini paling mirip...
A. Bubble Sort.
B. Selection Sort.
C. Insertion Sort.
D. Quick Sort.

<details>
<summary>💡 Hint</summary>
Pengecekan dan penukaran posisi bersebelahan adalah ciri khas Bubble.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bubble Sort.**
Algoritma pengurutan paling intuitif untuk dipelajari pertama kali.
</details>

### Soal #291: Algoritma "Cari Nama Jalan"
Kamu sedang di GPS. Kamu melihat garis biru yang menunjukkan jalur.
Dibalik layar, GPS menghitung ribuan kombinasi titik. Struktur pangkalan data ini disebut...
A. Graph (Kumpulan titik yang saling terhubung).
B. List (Daftar belanja).
C. Stack (Tumpukan).
D. Table (Tabel).

<details>
<summary>💡 Hint</summary>
Representasi peta digital dalam komputer menggunakan titik (Node) dan ruas jalan (Edge).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Graph.**
Struktur data paling krusial untuk algoritma navigasi dan media sosial.
</details>

### Soal #292: Algoritma "Mode Terang/Gelap" (Sensor)
Jika jam > 18:00, ganti jadi Dark Mode.
Jika cahaya ruangan < 10 lux, ganti jadi Dark Mode.
Kamu sedang di dalam kamar gelap total pada jam 12:00 Siang. Apa mode layarnya?
A. Terang (kan masih siang).
B. Gelap (karena syarat cahaya terpenuhi).
C. Kedap-kedip.
D. Mati.

<details>
<summary>💡 Hint</summary>
Logika OR: Syarat cahaya bernilai Benar, maka layar jadi Gelap.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gelap.**
Sistem merespon kondisi lingkungan demi kenyamanan pengguna secara otomatis.
</details>

### Soal #293: Algoritma "Hapus File"
"Hapus file Task1.zip". Kenapa sistem bilang "File sedang digunakan"?
A. File-nya takut dibuang.
B. Algoritma sistem mengunci (Lock) file yang sedang dibuka aplikasi lain untuk mencegah kerusakan data.
C. Kamu salah ketik nama.
D. Harddisk penuh.

<details>
<summary>💡 Hint</summary>
Adanya mekanisme penguncian memori (*Memory Locking*) untuk keamanan *file system*.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mekanisme Kunci (Lock).**
Aturan penting dalam algoritma manajemen file di sistem operasi.
</details>

### Soal #294: Algoritma "Isi Bensin Otomatis"
Sistem Pom Bensin: "Isi sampai Rp 50.000 atau Tangki Penuh".
Jika tangki penuh di harga Rp 40.000, apakah pengisian berlanjut sampai Rp 50.000?
A. Ya, kan perintahnya 50rb.
B. Tidak, sistem berhenti karena tangki penuh sudah tercapai (Condition stop).
C. Bensin tumpah ke jalan.
D. Mesin meledak.

<details>
<summary>💡 Hint</summary>
Gunakan logika OR untuk titik henti (*Exit Condition*). Mana yang tercapai duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak/Berhenti.**
Keamanan fisik lebih diutamakan daripada target angka dalam algoritma industri.
</details>

### Soal #295: Algoritma "Username Unik"
Kamu ingin nama 'Budi'. Sistem bilang: 'Username sudah digunakan'.
Algoritma pendaftaran melakukan aksi...
A. Bertanya ke temanmu.
B. Mengecek seluruh kolom 'Username' di database apakah ada yang isinya "Budi".
C. Menebak-nebak saja.
D. Menghapus akun Budi lama.

<details>
<summary>💡 Hint</summary>
Searching validasi keunikan data sebelum merekam data baru.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Cek duplikasi di database.**
Prinsip integritas data (*Uniqueness constraint*) dalam algoritma sistem informasi.
</details>

### Soal #296: Algoritma "Nilai Rata-rata Pelajaran"
Ada 2 nilai: Mat (80), Fisika (90). Kenapa rata-ratanya bisa jadi 85?
A. Hasil tebakan.
B. Karena  / 2 = 85$.
C. Karena 80 dan 90 berdekatan.
D. Kebetulan saja.

<details>
<summary>💡 Hint</summary>
Rumus matematika baku yang diterapkan dalam urutan langkah algoritma.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perhitungan matematis.**
Meskipun simpel, ini adalah desain algoritma pengolah nilai paling dasar.
</details>

### Soal #297: Algoritma "Sorting Z-A" (Reverse Alphabetical)
Daftar: Jeruk, Apel, Mangga. Urutan Z ke A:
A. Apel, Jeruk, Mangga.
B. Mangga, Jeruk, Apel.
C. Jeruk, Mangga, Apel.
D. Apel, Mangga, Jeruk.

<details>
<summary>💡 Hint</summary>
M (13) > J (10) > A (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mangga - Jeruk - Apel.**
Algoritma sortir terbalik untuk daftar tertentu (misal: "Terakhir diubah").
</details>

### Soal #298: Algoritma "Matematika Binari 2-bit"
Ada 2 lampu (Saklar). Berapa banyak kemungkinan nyala-mati yang ada?
A. 2 (Mati-mati, Nyala-nyala).
B. 4 (MM, MN, NM, NN).
C. 8.
D. 1.

<details>
<summary>💡 Hint</summary>
 \text{ pangkat } 2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 4 kombinasi.**
Struktur logika biner dasar yang menjadi fondasi seluruh algoritma komputer.
</details>

### Soal #299: Algoritma "Otoritas OSN-K"
Siapa yang berhak mengubah nilai jawabanmu di database pusat setelah ujian selesai?
A. Kamu sendiri (User).
B. Hanya Panitia Pusat dengan akses kunci Admin (Administrator Privilege).
C. Siapa saja yang bisa internetan.
D. Tidak ada.

<details>
<summary>💡 Hint</summary>
Membatasi akses penulisan data (*Write access*) hanya kepada pihak yang berhak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hanya Admin.**
Keamanan algoritma akses data yang mencegah kecurangan dalam sistem.
</details>

### Soal #300: Algoritma "Selesai Materi"
Instruksi: "Jika pertanyaan ke-300 selesai, tampilkan ucapan selamat dan lanjut ke bab evaluasi."
Apa status kamu sekarang?
A. Belum selesai.
B. Selamat! Kamu sudah menyelesaikan bank soal CP Algoritma. Siap lanjut ke tantangan berikutnya?
C. Error materi.
D. Mengulang dari soal nomor 1.

<details>
<summary>💡 Hint</summary>
Kondisi "Pertanyaan 300 selesai" sudah tercapai.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Selamat!**
Inilah akhir dari disain algoritma materi "Algorithm Design" kita. Kamu hebat!
</details>

---
[< Materi Sebelumnya: Abstraction](./04-abstraction.md) | [Materi Selanjutnya: Latihan Soal Campuran](../README.md)
[< Kembali ke Beranda Materi](../README.md)
