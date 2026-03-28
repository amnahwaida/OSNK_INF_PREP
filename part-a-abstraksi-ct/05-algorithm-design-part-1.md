# 05. Algorithm Design - Bagian 1 (Soal 1-50)

[🏠 Indeks](05-algorithm-design.md) | [Bagian 2 (51-100) >](05-algorithm-design-part-2.md)

---
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


---
[🏠 Indeks](05-algorithm-design.md) | [Bagian 2 (51-100) >](05-algorithm-design-part-2.md)
