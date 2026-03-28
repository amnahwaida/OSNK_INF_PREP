🔙 **Kembali ke Materi:** [Materi 05 Algorithm Design](../05-algorithm-design.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 05. Algorithm Design - Bagian 3 (Soal 101-150)

[< Bagian 2 (51-100)](05-algorithm-design-part-2.md) | [🏠 Indeks](../05-algorithm-design.md) | [Bagian 4 (151-200) >](05-algorithm-design-part-4.md)

---
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


---
[< Bagian 2 (51-100)](05-algorithm-design-part-2.md) | [🏠 Indeks](../05-algorithm-design.md) | [Bagian 4 (151-200) >](05-algorithm-design-part-4.md)
