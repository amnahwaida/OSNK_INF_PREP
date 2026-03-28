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

---
[< Materi Sebelumnya: Abstraction](./04-abstraction.md) | [Materi Selanjutnya: Latihan Soal Campuran](../README.md)
[< Kembali ke Beranda Materi](../README.md)
