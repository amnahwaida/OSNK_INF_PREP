🔙 **Kembali ke Materi:** [Materi 06 Logika Dan Antrian](../06-logika-dan-antrian.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 06. Logika & Antrian - Latihan Soal Bagian 3 (101-150)

### Soal #114: Logika "Lampu Kamar Mandi"
Lampu menyala JIKA (Ada Orang) **AND** (NOT Hari Siang). 
Di luar sedang mendung gelap (Hari dianggap Malam), dan Budi masuk kamar mandi. 
Apakah lampu menyala?
A. Ya
B. Tidak
C. Kadang-kadang
D. Tergantung saklar

<details>
<summary>💡 Hint</summary>
(Ada orang = T) AND (NOT Siang = T).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
</details>

### Soal #115: Antrian "Masuk Tol"
Mobil A, B, C antre di gardu tol. Mobil B tiba-tiba mogok dan didorong keluar jalur. 
Urutan keluar gardu tol adalah...
A. A lalu C
B. A lalu B
C. C lalu A
D. B lalu C

<details>
<summary>💡 Hint</summary>
B hilang dari antrian.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. A lalu C.**
</details>

### Soal #116: Logika "Diskon Belanja"
Diskon 20% diberikan JIKA (Total > 100rb) **AND** (Punya Kode Promo **OR** Hari Minggu). 
Total belanja 150rb, Hari Selasa, Tidak punya kode promo. Dapat diskon?
A. Dapat
B. Tidak Dapat
C. Dapat 10%
D. Dapat jika minta kasir

<details>
<summary>💡 Hint</summary>
(T) AND (F OR F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Dapat.**
</details>

### Soal #117: Stack "Koin di Celengan"
Koin masuk: [100, 200, 500]. 
Celengan dibongkar dari lubang yang sama (satu lubang). 
Koin pertama yang keluar adalah...
A. 100
B. 200
C. 500
D. Semuanya

<details>
<summary>💡 Hint</summary>
Lubang yang sama = LIFO.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 500.**
</details>

### Soal #118: Logika NOR (P OR Q OR R)
Pernyataan $(P \text{ OR } Q \text{ OR } R)$ bernilai SALAH jika...
A. Semuanya Salah
B. Salah satu Salah
C. Semuanya Benar
D. Salah satu Benar

<details>
<summary>💡 Hint</summary>
Logika OR menghasilkan BENAR jika ada minimal SATU yang Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Semuanya Salah.**
</details>

### Soal #119: Antrian "Update Game"
Update 1 (1GB), Update 2 (2GB), Update 3 (500MB). 
Sistem mengunduh secara berurutan. Jika internet putus setelah 2.5GB terunduh, update mana yang sudah SELESAI?
A. Update 1 dan 2
B. Update 1 saja
C. Update 3 saja
D. Semuanya

<details>
<summary>💡 Hint</summary>
U1(1) + U2(2) = 3GB. Baru terunduh 2.5GB.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Update 1 saja.**
Update 2 baru selesai 1.5GB (belum utuh).
</details>

### Soal #120: Stack "Buku yang Dikembalikan"
Tumpukan: [Fisika, Kimia]. 
Budi mengembalikan Biologi, lalu mengambil 1 buku. 
Lalu Andi mengembalikan Matematika, lalu mengambil 1 buku. 
Buku apa yang ada di paling atas sekarang?
A. Matematika
B. Biologi
C. Kimia
D. Fisika

<details>
<summary>💡 Hint</summary>
1. [F, K, Bio] -> Ambil 1: [F, K]. 2. [F, K, Mat] -> Ambil 1: [F, K].
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kimia.**
</details>

### Soal #121: Logika "Sensor Pintu Otomatis"
Pintu terbuka JIKA (Sensor Dalam Terdeteksi) **OR** (Sensor Luar Terdeteksi) **AND** (NOT Listrik Mati). 
Listrik mati, tapi Budi berdiri di depan sensor. Apakah pintu terbuka?
A. Terbuka
B. Tertutup
C. Terjepit
D. Rusak

<details>
<summary>💡 Hint</summary>
AND (NOT Listrik Mati) = AND (Salah). Apapun hasilnya di depan, jika di-AND-kan dengan Salah maka...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tertutup.**
</details>

### Soal #122: Antrian "Panggilan Masuk"
Telepon: [P1, P2, P3]. 
Operator hanya bisa bicara dengan 1 orang. P1 menutup telepon sebelum diangkat. 
Siapa yang bicara dengan operator sekarang?
A. P1
B. P2
C. P3
D. Tidak ada

<details>
<summary>💡 Hint</summary>
Antrian bergeser.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. P2.**
</details>

### Soal #123: Stack "Wadah Peluru"
Peluru masuk: [Merah, Kuning, Hijau]. 
Jika ditembakkan 1 kali (keluar peluru), peluru warna apa yang keluar?
A. Merah
B. Kuning
C. Hijau
D. Biru

<details>
<summary>💡 Hint</summary>
LIFO: Terakhir masuk adalah yang pertama keluar moncong.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Hijau.**
</details>

### Soal #124: Logika "Keamanan Password"
Password kuat JIKA (Panjang > 8) **AND** (Ada Angka **OR** Ada Simbol). 
Password: "Admin123" (Panjang 8). Apakah ini password kuat?
A. Ya
B. Tidak
C. Hampir
D. Sangat Kuat

<details>
<summary>💡 Hint</summary>
Syarat panjang harus LEBIH DARI 8 (8 > 8 adalah SALAH).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #125: De Morgan pada 3 Variabel
NOT (A AND B AND C) sama dengan...
A. NOT A OR NOT B OR NOT C
B. NOT A AND NOT B AND NOT C
C. A OR B OR C
D. NOT A OR B AND C

<details>
<summary>💡 Hint</summary>
Semua AND berubah jadi OR, dan semua variabel diberi NOT.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. NOT A OR NOT B OR NOT C.**
</details>

### Soal #126: Kombinasi Queue-Stack (Reverse)
Data: [1, 2, 3] masuk ke Queue. 
Satu per satu dikeluarkan dari Queue dan dimasukkan ke Stack. 
Isi Stack sekarang (dari bawah ke atas) adalah?
A. [1, 2, 3]
B. [3, 2, 1]
C. [1, 3, 2]
D. [2, 1, 3]

<details>
<summary>💡 Hint</summary>
1 keluar duluan dari Queue, masuk ke dasar Stack.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [1, 2, 3].**
</details>

### Soal #127: Antrian "Pasien Dokter"
Dokter memanggil pasien: [A, B, C, D]. 
Baru saja A masuk, datang Pasien Darurat (E). Dokter harus mendahulukan E. 
Setelah E selesai, siapa yang dipanggil selanjutnya?
A. A (lanjutan)
B. B
C. C
D. D

<details>
<summary>💡 Hint</summary>
A sudah di dalam. Urutan antrian di luar tetap [B, C, D].
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
</details>

### Soal #128: Stack "Warna Cat"
Tumpukan kaleng: [Merah, Biru, Kuning]. 
Kamu mengambil 1 kaleng (Kuning), mengecat, lalu mengembalikannya ke tumpukan. 
Lalu kamu mengambil 2 kaleng sekaligus dari atas. Warna apa yang kamu ambil?
A. Kuning dan Biru
B. Merah dan Biru
C. Kuning dan Merah
D. Biru saja

<details>
<summary>💡 Hint</summary>
[M, B, K] -> -K: [M, B] -> +K: [M, B, K]. Ambil 2 teratas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kuning dan Biru.**
</details>

### Soal #129: Logika "Robot Penyedot Debu"
Robot jalan JIKA (Baterai > 10%) **AND** (NOT Tangki Penuh). 
Baterai 50%, Tangki Penuh. Apakah robot jalan?
A. Jalan
B. Berhenti/Kembali ke dock
C. Meledak
D. Terus menyedot

<details>
<summary>💡 Hint</summary>
NOT (T) = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berhenti/Kembali ke dock.**
</details>

### Soal #130: Antrian "Download Manager"
Antrian: [File1, File2, File3]. 
File 1 gagal download (error), sistem otomatis lanjut ke berikutnya. 
Urutan download yang berhasil (asumsi sisanya lancar) adalah...
A. [File2, File3]
B. [File1, File2, File3]
C. [File3, File2]
D. [File2]

<details>
<summary>💡 Hint</summary>
Error = Dequeue tanpa hasil.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [File2, File3].**
</details>

### Soal #131: Stack "History Chat"
Chat terakhir: "Apa kabar?". Chat sebelumnya: "Halo". Chat paling lama: "Tes". 
Jika kamu menghapus (delete) chat paling baru, chat mana yang sekarang muncul paling atas?
A. "Halo"
B. "Tes"
C. "Apa kabar?"
D. Kosong

<details>
<summary>💡 Hint</summary>
LIFO: Hapus yang teratas, yang di bawahnya naik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. "Halo".**
</details>

### Soal #132: Logika "Lampu Emergency"
Lampu Nyala JIKA (NOT Listrik PLN Nyala) **AND** (Saklar Lampu ON). 
Listrik PLN mati, Saklar Lampu OFF. Apakah lampu nyala?
A. Nyala
B. Mati
C. Berkedip
D. Rusak

<details>
<summary>💡 Hint</summary>
(T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mati.**
</details>

### Soal #133: Antrian "Stadion"
Ribuan orang antre di Pintu A dan Pintu B. 
Jika Pintu A punya 1 petugas dan Pintu B punya 3 petugas, pintu mana yang antreannya lebih cepat habis?
A. Pintu A
B. Pintu B
C. Sama saja
D. Tergantung cuaca

<details>
<summary>💡 Hint</summary>
Banyak petugas = Kecepatan Dequeue lebih tinggi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pintu B.**
</details>

### Soal #134: Stack "Penyimpanan Kayu"
Kayu ditumpuk: [K1, K2, K3, K4]. 
Rayap memakan K1 (paling bawah). Apa yang terjadi pada tumpukan?
A. Seluruh tumpukan turun ke bawah.
B. Tumpukan tetap melayang.
C. Tumpukan hancur.
D. K4 hilang.

<details>
<summary>💡 Hint</summary>
Dalam dunia nyata, penyangga bawah hilang mengakibatkan atasnya turun. Dalam Stack komputer, ini disebut penghapusan elemen dasar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Seluruh tumpukan turun/runtuh.**
</details>

### Soal #135: Logika "Absensi Digital"
Absen dihitung JIKA (Jam Datang <= 07:00) **OR** (Ada Izin Sakit). 
Budi datang jam 07:15 dan tidak ada izin. Apakah Budi dianggap absen (hadir)?
A. Ya (Hadir)
B. Tidak (Alpa)
C. Setengah Hari
D. Terlambat

<details>
<summary>💡 Hint</summary>
(F OR F) = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak (Alpa).**
</details>

### Soal #136: Antrian "Pengiriman Paket"
Gudang mengirim: [Batam, Medan, Jakarta]. 
Truck hanya muat 2 paket. Paket mana yang masih menunggu di gudang?
A. Batam
B. Medan
C. Jakarta
D. Tidak ada

<details>
<summary>💡 Hint</summary>
FIFO: Paket ke-3 harus menunggu truck berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Jakarta.**
</details>

### Soal #137: Stack "Buku yang Ditandai" (Bookmark)
Kamu membaca buku Halaman 1-100. Kamu menaruh pembatas (Bookmark) di halaman 50. 
Lalu kamu menaruh lagi di halaman 80. Jika kamu ingin kembali ke tanda terakhir, di halaman berapa kamu berhenti?
A. 50
B. 80
C. 100
D. 1

<details>
<summary>💡 Hint</summary>
Terakhir ditaruh = Teratas di Stack memori.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 80.**
</details>

### Soal #138: Logika XOR "Pencahayaan"
Dua lampu (L1 dan L2). Ruangan cukup terang JIKA (L1 XOR L2). 
Jika kedua lampu dinyalakan bersamaan, apakah ruangan "Cukup Terang"?
A. Ya (Cukup Terang)
B. Tidak (Terlalu Terang/Salah)
C. Gelap
D. Tergantung jendela

<details>
<summary>💡 Hint</summary>
T XOR T = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Berdasarkan aturan XOR, jika keduanya sama (Sama-sama nyala), hasilnya justru SALAH.
</details>

### Soal #139: Antrian "Update Status"
Pesan Status: [S1, S2, S3]. 
Karena jaringan lemot, S2 terkirim setelah S3. 
Apakah sistem ini masih mengikuti Queue murni?
A. Masih
B. Tidak murni (OutOfOrder)
C. Hanya di pagi hari
D. Ya, jika S1 sampai

<details>
<summary>💡 Hint</summary>
Queue murni mengharuskan urutan kirim = urutan sampai.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak murni (OutOfOrder).**
</details>

### Soal #140: Stack "Setumpuk Kartu Remi"
Kartu: [Waru, Keriting, Tempe, Wajik]. (Tempe adalah kartu bonus). 
Kamu membuang Wajik, lalu mengambil 2 kartu. Kartu apa yang terakhir kamu pegang?
A. Keriting
B. Waru
C. Tempe
D. Wajik

<details>
<summary>💡 Hint</summary>
1. [W, K, T] -> Ambil 1 (T) -> Sisa [W, K] -> Ambil 1 lagi (K).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Keriting.**
</details>

### Soal #141: Logika "Kelayakan Terbang"
Pesawat boleh terbang JIKA (Cuaca Cerah) **AND** (Bahan Bakar > 50%) **AND** (NOT Ada Kerusakan Mekanis). 
Data: Mendung (Cerah=F), BBM 80%, Mesin Bagus. Apakah pesawat terbang?
A. Terbang
B. Delay/Batal
C. Terbang rendah
D. Tergantung Pilot

<details>
<summary>💡 Hint</summary>
(F) AND (T) AND (T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Delay/Batal.**
</details>

### Soal #142: Antrian "Mesin ATM"
Antrian: [A, B, C]. 
A sedang di dalam mesin. Tiba-tiba mesin rusak. 
Apa yang harus dilakukan agar antrian tetap adil saat mesin diperbaiki?
A. Menghapus antrian dan mulai dari awal.
B. B dan C tetap menunggu di posisi mereka.
C. C maju ke depan B.
D. A masuk lagi ke belakang C.

<details>
<summary>💡 Hint</summary>
Menjaga urutan = Menjaga keadilan (FIFO).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B dan C tetap menunggu.**
</details>

### Soal #143: Stack "Penyimpanan Peluru Nerf"
Isi: [Biru, Biru, Orange]. 
Kamu menembakkan peluru Orange ke sasaran, lalu memasukkan peluru Hijau. 
Warna peluru di moncong sekarang adalah?
A. Biru
B. Hijau
C. Orange
D. Kosong

<details>
<summary>💡 Hint</summary>
[B, B] -> +H: [B, B, H].
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hijau.**
</details>

### Soal #144: Logika "Lampu Tidur" (Negasi Ganda)
Lampu Mati JIKA NOT (Hari Gelap). 
Hari Gelap = Benar. Jadi Lampu Mati?
A. Ya
B. Tidak
C. Sedang-sedang saja
D. Rusak

<details>
<summary>💡 Hint</summary>
NOT (T) = F. Jadi "Lampu Mati" adalah Salah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak (Artinya Menyala).**
</details>

### Soal #145: Antrian "Flash Sale"
Stok: 1 HP. 
P1 klik beli jam 10:00:01. P2 klik beli jam 10:00:00. P3 klik beli jam 10:00:02. 
Siapa yang dapat HP?
A. P1
B. P2
C. P3
D. Admin

<details>
<summary>💡 Hint</summary>
FIFO: Jam paling awal (10:00:00) yang masuk antrian memori server duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. P2.**
</details>

### Soal #146: Logika "Akses Internet"
Bisa internetan JIKA (Ada Kuota) **OR** (Ada WiFi). 
Punya kuota tapi di daerah tersebut tidak ada sinyal (Kuota dianggap F). Ada WiFi tapi lemot (WiFi dianggap T). Bisa internetan?
A. Bisa
B. Tidak Bisa
C. Sangat Lambat
D. Harus beli kuota lagi

<details>
<summary>💡 Hint</summary>
(F OR T) = T.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bisa.**
</details>

### Soal #147: Stack "Tumpukan Kado"
Kado: [Bawah: Sepatu, Tas, Jam :Atas]. 
Ahmad mengambil kado paling atas (Jam). Lalu ia menaruh kado cokelat di atas Tas. 
Jika adiknya mengambil satu kado dari tumpukan itu, kado apa yang ia ambil?
A. Sepatu
B. Tas
C. Jam
D. Cokelat

<details>
<summary>💡 Hint</summary>
[Sepatu, Tas] -> +Cokelat: [Sepatu, Tas, Cokelat].
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Cokelat.**
</details>

### Soal #148: Logika NAND Identitas
Hasil dari x NAND x selalu sama dengan...
A. x
B. NOT x
C. 1
D. 0

<details>
<summary>💡 Hint</summary>
Jika x=1: 1 NAND 1 = 0. Jika x=0: 0 NAND 0 = 1.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. NOT x.**
</details>

### Soal #149: Antrian "Antar Makanan"
Antrian: [M1, M2, M3]. 
Driver M1 motornya bocor, ia memberikan pesanannya ke driver M4. 
M4 harus mengantar pesanan M1 SEKARANG. 
Bagaimana posisi M2 dan M3?
A. Tetap harus menunggu M4 selesai.
B. Maju ke depan M4.
C. Menjadi admin.
D. Berhenti mengantar.

<details>
<summary>💡 Hint</summary>
Urutan antrian fisik boleh berubah orangnya, tapi gilirannya tetap di depan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Tetap menunggu.**
</details>

### Soal #150: Refleksi Pertengahan
Dari soal 1-150, manakah yang paling sering menyebabkan Error pada sistem Antrian/Tumpukan?
A. Menambah data terlalu banyak (Overflow).
B. Mengambil dari yang kosong (Underflow).
C. Listrik mati.
D. Lupa password.

<details>
<summary>💡 Hint</summary>
Keduanya (A dan B) adalah kesalahan logika dasar pemrograman.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengambil dari yang kosong (Underflow).**
(Meskipun A juga benar, Underflow sering terjadi pada logika loop yang salah).
</details>

### Soal #151: Logika "Sistem Alarm"
Alarm Berbunyi JIKA (Asap Terdeteksi) **AND** (NOT Jendela Terbuka). 
Data: Asap Terdeteksi = Benar, Jendela Terbuka = Benar. Apakah alarm berbunyi?
A. Ya
B. Tidak
C. Berkedip
D. Error

<details>
<summary>💡 Hint</summary>
(T) AND (NOT T) = T AND F = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #152: Antrian "Kasir Self-Service"
Antrian: [A, B, C]. 
A sedang scan barang. Tiba-tiba mesin A error. Petugas memindahkan A ke mesin cadangan. 
Siapa yang sekarang dilayani di mesin A (setelah diperbaiki)?
A. A
B. B
C. C
D. Petugas

<details>
<summary>💡 Hint</summary>
B adalah orang kedua yang sedang menunggu giliran.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
</details>

### Soal #153: Stack "Penyimpanan Balok"
Balok: [Bawah: Merah, Hijau, Biru :Atas]. 
Ambil 1 (Biru), taruh Kuning, ambil 1 (Kuning). 
Balok apa yang paling atas sekarang?
A. Biru
B. Hijau
C. Merah
D. Kuning

<details>
<summary>💡 Hint</summary>
[M, H] -> Biru diambil. [M, H] -> Kuning ditaruh. [M, H, K] -> Kuning diambil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hijau.**
</details>

### Soal #154: Logika XOR "Pintu Ganda"
Pintu terbuka JIKA (Kunci A **XOR** Kunci B). 
Jika kedua kunci diputar bersamaan ke posisi ON, apakah pintu terbuka?
A. Ya
B. Tidak
C. Tergantung pintu
D. Kunci Patah

<details>
<summary>💡 Hint</summary>
T XOR T = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #155: Antrian "Pesan GoFood"
Pesanan: [P1, P2]. 
Baru saja P1 diambil driver, masuk P3. 
Urutan pesanan di restoran yang belum diambil driver adalah...
A. [P2, P3]
B. [P1, P2, P3]
C. [P3, P2]
D. [P1]

<details>
<summary>💡 Hint</summary>
P1 sudah keluar dari antre restoran.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [P2, P3].**
</details>

### Soal #156: Logika "Beasiswa Luar Negeri"
Lolos jika: (IPK > 3.5) **AND** (IELTS > 6.5) **AND** (NOT Ada Catatan Kriminal). 
IPK 3.8, IELTS 7.0, Ada Catatan Kriminal. Lolos?
A. Lolos
B. Tidak Lolos
C. Lolos Bersyarat
D. Tunggu 1 tahun

<details>
<summary>💡 Hint</summary>
(T) AND (T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lolos.**
</details>

### Soal #157: Stack "Undo" (Tumpukan 5)
Aksi: [1, 2, 3, 4, 5]. 
Undo 3 kali. Apa aksi terakhir yang masih berlaku?
A. 1
B. 2
C. 3
D. 5

<details>
<summary>💡 Hint</summary>
Undo 1(5), Undo 2(4), Undo 3(3). Sisa [1, 2].
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2.**
</details>

### Soal #158: Logika "Lampu Otomatis"
Lampu Nyala jika: (Malam **AND** Ada Orang) **OR** (Darurat). 
Data: Siang, Ada Orang, Darurat=Benar. Lampu nyala?
A. Ya
B. Tidak
C. Berkedip
D. Rusak

<details>
<summary>💡 Hint</summary>
(F AND T) OR (T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
</details>

### Soal #159: Antrian "Bus" (First In Last Out?)
Sebuah bus satu pintu (naik dan turun lewat pintu yang sama). 
Penumpang: [A, B, C]. A naik duluan, C naik terakhir. 
Siapa yang turun duluan?
A. A
B. B
C. C
D. Supir

<details>
<summary>💡 Hint</summary>
Satu pintu = Stack (LIFO).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. C.**
</details>

### Soal #160: Stack "Buku yang Ditumpuk"
Tumpukan: [Sains, Agama, Seni]. 
Kamu mengambil Seni, taruh Olahraga, taruh Musik. 
Buku apa yang ada di urutan ke-2 dari bawah?
A. Sains
B. Agama
C. Seni
D. Olahraga

<details>
<summary>💡 Hint</summary>
[Sains, Agama] -> +Olahraga -> +Musik. [Sains, Agama, Olahraga, Musik].
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Agama.**
</details>

### Soal #161: Logika "Kupon Makan"
Dapat makan gratis JIKA (Punya Kupon) **OR** (Ulang Tahun Hari Ini). 
Budi punya kupon tapi bukan ulang tahunnya. Dapat makan gratis?
A. Dapat
B. Tidak Dapat
C. Bayar Setengah
D. Tanya Pelayan

<details>
<summary>💡 Hint</summary>
Logika OR: Salah satu Benar = Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Dapat.**
</details>

### Soal #162: Antrian "Bank" (2 Loket)
Antrian: [A, B, C, D]. Loket 1 kosong, Loket 2 kosong. 
A ke Loket 1, B ke Loket 2. Siapa yang maju saat salah satu loket selesai?
A. C
B. D
C. A
D. B

<details>
<summary>💡 Hint</summary>
FIFO: C adalah urutan berikutnya di baris tunggu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. C.**
</details>

### Soal #163: Stack "Satu Lubang"
Wadah kelereng satu lubang: [Merah, Kuning, Hijau]. 
Kelereng Merah dimasukkan pertama. 
Kelereng apa yang keluar ke-2 jika dikosongkan?
A. Merah
B. Kuning
C. Hijau
D. Biru

<details>
<summary>💡 Hint</summary>
Keluar 1: Hijau. Keluar 2: Kuning.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kuning.**
</details>
---
[< Kembali ke Indeks Materi](../06-logika-dan-antrian.md) | [< Bagian Sebelumnya](./06-logika-dan-antrian-part-2.md) | [Bagian Selanjutnya >](./06-logika-dan-antrian-part-4.md)
