# 06. Logika & Antrian - Latihan Soal Bagian 2 (51-100)

### Soal #64: Logika Gerbang Logika Bertingkat
Hasil dari (A AND B) OR (NOT (A OR B)) jika A=T, B=F adalah...
A. Benar
B. Salah
C. Mungkin
D. Error

<details>
<summary>💡 Hint</summary>
Kerjakan (A AND B) = F. Kerjakan (A OR B) = T, lalu NOT-kan jadi F. F OR F = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
F OR F = Salah.
</details>

### Soal #65: Antrian "Buffer" Video
Video dibagi menjadi potongan: [Part1, Part2, Part3, Part4].
Player memutar Part1, lalu Part2. Tiba-tiba internet putus saat sedang memuat Part3.
Potongan mana yang sudah SIAP diputar (buffered) tapi belum ditonton?
A. Part1
B. Part2
C. Part3
D. Part4

<details>
<summary>💡 Hint</summary>
Buffer adalah antrian data yang sudah sampai tapi belum diproses.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Part3.**
Part 1 dan 2 sudah ditonton (Keluar antrian). Part 3 sedang dimuat/siap di antrian.
</details>

### Soal #66: Logika "Akses VIP"
Akses diberikan JIKA (Punya Tiket=T) **AND** (NOT Masuk Daftar Hitam=T).
Budi punya tiket, tapi namanya ada di Daftar Hitam. Apakah ia bisa akses?
A. Bisa
B. Tidak Bisa
C. Bisa tapi bayar
D. Tanya Manager

<details>
<summary>💡 Hint</summary>
Daftar Hitam = T, maka NOT Daftar Hitam = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Bisa.**
T AND F = Salah.
</details>

### Soal #67: Stack "Kamera Belakang"
Kamu memotret: [Foto1, Foto2, Foto3]. Kamera menyimpannya ke galeri.
Ponsel menampilkan foto TERBARU di posisi paling atas halaman galeri. Ini mirip prinsip...
A. Queue
B. Stack
C. Table
D. List

<details>
<summary>💡 Hint</summary>
Aksi terakhir (Foto 3) muncul pertama kali di hadapanmu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Stack (LIFO).**
Meskipun galeri adalah daftar, tapi tampilan "Terbaru di Atas" mengikuti pola tumpukan.
</details>

### Soal #68: Antrian Tol (Banyak Gerbang)
Mobil: [M1, M2, M3, M4]. Ada 2 gerbang tol (G1, G2).
M1 ke G1, M2 ke G2. Jika pelayanan G1 lebih lambat 2x lipat dari G2, siapa yang mungkin keluar tol lebih dulu?
A. M1
B. M2
C. M3
D. M4

<details>
<summary>💡 Hint</summary>
Antrian paralel dipengaruhi oleh kecepatan pelayanannya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. M2.**
Karena G2 lebih cepat, M2 akan selesai lebih dulu meskipun mereka sampai hampir bersamaan.
</details>

### Soal #69: Logika XOR "Gunting Batu Kertas"
Jika Gunting(1), Batu(2), Kertas(3). 
Aturan: Pemain menang JIKA (Pilihan1 XOR Pilihan2) bernilai GANJIL.
P1 pilih Gunting(1), P2 pilih Batu(2). Siapa yang menang? (1 XOR 2 = 3).
A. Pemain Menang
B. Pemain Kalah
C. Seri
D. Error

<details>
<summary>💡 Hint</summary>
3 adalah bilangan Ganjil.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pemain Menang.**
Sesuai aturan buatan soal (XOR ganjil = menang), maka hasilnya menang.
</details>

### Soal #70: Stack "Buku yang dipinjam"
Budi meminjam: [A, B, C]. Sampai rumah ia meletakkannya bertumpuk (A di bawah, C di atas).
Budi membaca buku yang paling atas tiap malam. Buku ke-2 yang ia selesaikan adalah...
A. A
B. B
C. C
D. Semuanya

<details>
<summary>💡 Hint</summary>
Selesaikan C dulu (malam 1), lalu selesaikan B (malam 2).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
Urutan baca: C -> B -> A. Maka buku ke-2 adalah B.
</details>

### Soal #71: Logika "Sensor Suhu"
Kipas menyala JIKA (Suhu > 30) **OR** (Asap Terdeteksi=T).
Suhu saat ini 25 derajat, dan ada orang merokok (Asap=T). Status kipas?
A. Mati
B. Menyala
C. Berputar pelan
D. Rusak

<details>
<summary>💡 Hint</summary>
OR hanya butuh satu syarat untuk menyala.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyala.**
Kondisi "Asap Terdeteksi" sudah cukup untuk menyalakan kipas.
</details>

### Soal #72: Antrian "Playlist" Lagu
Playlist: [Lagu1, Lagu2, Lagu3]. 
Kamu klik "Shuffle" (Acak). Apakah sistem ini masih menggunakan prinsip Queue murni?
A. Ya
B. Tidak
C. Tergantung lagu
D. Hanya jika volumenya besar

<details>
<summary>💡 Hint</summary>
Queue murni harus urut sesuai kedatangan/urutan daftar (FIFO).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Shuffle mengacak urutan, sehingga merusak prinsip FIFO.
</details>

### Soal #73: Stack "Piring Makan" (Pop 2x)
Tumpukan: [P1, P2, P3, P4, P5].
Ibu mengambil 2 piring paling atas untuk makan malam. Sisa piring di tumpukan adalah?
A. P4, P5
B. P1, P2, P3
C. P1, P2
D. P3, P4, P5

<details>
<summary>💡 Hint</summary>
Yang diambil adalah yang paling atas (P5 dan P4).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. P1, P2, P3.**
LIFO: P5 keluar, lalu P4 keluar. Tersisa yang di bawah.
</details>

### Soal #74: Logika "Password & OTP"
Akses Bank diberikan JIKA (Password Benar) **AND** (OTP Benar).
Kamu tahu NOT (OTP Benar) adalah SALAH. Berarti status OTP-mu?
A. Benar
B. Salah
C. Kadaluarsa
D. Tidak terkirim

<details>
<summary>💡 Hint</summary>
NOT (X) = Salah, maka X = ...
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
Jika "Tidak Benar" adalah salah, maka itu berarti "Benar".
</details>

### Soal #75: Antrian "Restoran Cepat Saji"
Antrian: [Andi, Budi].
Pelayan memanggil "Budi" lebih dulu karena pesanannya cuma minum, sedangkan Andi pesan banyak.
Prinsip apa yang digunakan restoran ini?
A. FIFO (Queue)
B. SJF (Shortest Job First / Tugas Terpendek Duluan)
C. LIFO (Stack)
D. Random

<details>
<summary>💡 Hint</summary>
Meskipun Andi datang duluan, Budi dilayani karena lebih cepat selesai.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. SJF (Shortest Job First).**
Ini adalah variasi antrian yang memprioritaskan tugas yang paling cepat beres.
</details>

### Soal #76: Logika NAND Universal
Jika kamu hanya punya gerbang NAND, kamu bisa membuat gerbang NOT dengan cara...
A. Menghubungkan satu input ke dua kaki NAND.
B. Menghubungkan output NAND ke inputnya sendiri.
C. Menambah baterai.
D. Tidak bisa dilakukan.

<details>
<summary>💡 Hint</summary>
Ingat Soal #56: A NAND A = NOT A.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menghubungkan satu input ke dua kaki NAND.**
Dengan memasukkan nilai yang sama ke kedua input NAND, hasilnya adalah negasi (NOT).
</details>

### Soal #77: Stack "Simpan Game" (Save Slot)
Slot Save: [Slot1, Slot2, Slot3].
Kamu selalu menimpa (overwrite) slot yang terakhir kali kamu gunakan. Jika terakhir kamu pakai Slot 3, lalu kamu save lagi, slot mana yang berubah?
A. Slot 1
B. Slot 3
C. Slot 2
D. Semua slot

<details>
<summary>💡 Hint</summary>
Last used = Top of focus.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Slot 3.**
Fokus aplikasi biasanya tertuju pada aksi terakhir yang dilakukan.
</details>

### Soal #78: Antrian "Print" (Urutan Balik)
Tugas masuk: T1, T2, T3. 
Ternyata Printer dipasang terbalik, sehingga yang diproses adalah yang paling baru datang.
Sistem ini berubah dari Queue menjadi...
A. Circular Queue
B. Stack
C. Priority Queue
D. Matrix

<details>
<summary>💡 Hint</summary>
Baru datang = Terakhir masuk. Diproses = Keluar duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Stack.**
Karena yang terakhir masuk menjadi yang pertama keluar (LIFO).
</details>

### Soal #79: Logika "Iklan YouTube"
Iklan muncul JIKA (NOT Berlangganan Premium) **AND** (Video Bukan Milik Pemerintah).
Ahmad berlangganan Premium. Apakah Ahmad melihat iklan?
A. Ya
B. Tidak
C. Hanya di awal
D. Di tengah-tengah

<details>
<summary>💡 Hint</summary>
Premium=T, maka NOT Premium=F. F AND apapun = ...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Logika AND akan langsung bernilai SALAH jika salah satu syaratnya (NOT Premium) adalah salah.
</details>

### Soal #80: Stack "Cuci Piring"
Kamu mencuci piring kotor: [P1, P2, P3]. Kamu menumpuknya yang bersih.
Tiba-tiba piring P2 retak saat hendak ditaruh. Kamu membuangnya.
Urutan piring di tumpukan bersih (dari bawah) adalah...
A. [P1, P2, P3]
B. [P1, P3]
C. [P3, P1]
D. [P2, P3]

<details>
<summary>💡 Hint</summary>
P1 ditaruh pertama (di bawah). P2 gagal ditaruh. P3 ditaruh di atas P1.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. [P1, P3].**
Urutan tumpukan: P1 (paling bawah), lalu P3 di atasnya.
</details>

### Soal #81: Logika "Rem Otomatis Mobil"
Rem bekerja JIKA (Ada Halangan Dalam 2 Meter) **AND** (Kecepatan > 10 km/jam).
Mobil berjalan 5 km/jam dan ada kucing lewat di depan (jarak 1 meter). Apakah mobil mengerem otomatis?
A. Ya
B. Tidak
C. Kucing tertabrak
D. Ban pecah

<details>
<summary>💡 Hint</summary>
Syarat kecepatan (5 > 10) bernilai SALAH.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Sistem tidak aktif karena kecepatan mobil terlalu rendah (berdasarkan aturan logika di soal).
</details>

### Soal #82: Antrian Kereta Malam
Gerbong: [G1, G2, G3, G4].
Gerbong G4 dilepas di tengah jalan karena rusak. Urutan gerbong sisa adalah...
A. [G1, G2, G3]
B. [G4, G3, G2, G1]
C. [G1, G2, G4]
D. Kosong

<details>
<summary>💡 Hint</summary>
Gerbong di belakang G3 hilang, sisanya tetap.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [G1, G2, G3].**
Urutan dari depan (G1) tetap terjaga.
</details>

### Soal #83: Stack "Topi Pesulap"
Pesulap memasukkan: Syal, Kelinci, Bunga.
Ia mengambil 2 benda. Jika benda pertama adalah Bunga, benda kedua yang keluar adalah?
A. Syal
B. Kelinci
C. Burung
D. Bunga lagi

<details>
<summary>💡 Hint</summary>
LIFO: Bunga adalah yang terakhir masuk. Sebelum bunga adalah Kelinci.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kelinci.**
Urutan keluar: Bunga -> Kelinci -> Syal.
</details>

### Soal #84: Logika NAND dan NOR (Gabungan)
(T NAND T) **OR** (F NOR F) = ...
A. Benar
B. Salah
C. Mungkin
D. Error

<details>
<summary>💡 Hint</summary>
T NAND T = F. F NOR F = T. F OR T = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
Salah OR Benar = Benar.
</details>

### Soal #85: Antrian "Call Center"
Penelepon: [P1, P2]. 
Operator 1 sibuk bicara dengan P1. Jika P1 mematikan telepon tepat saat P3 menelepon, siapakah yang akan dilayani selanjutnya?
A. P2
B. P3
C. Keduanya
D. Tidak ada

<details>
<summary>💡 Hint</summary>
P2 sudah mengantri lebih lama daripada P3.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. P2.**
Prinsip FIFO: orang yang datang lebih dulu (P2) harus dilayani lebih dulu.
</details>

### Soal #86: Logika "Status Pesanan"
Pesanan SELESAI jika (Barang Sampai=T) **AND** (Pembeli Klik Terima=T).
Pembeli belum klik terima, tapi barang sudah sampai di teras. Status pesanan?
A. Selesai
B. Belum Selesai (Pending)
C. Hilang
D. Dibayar

<details>
<summary>💡 Hint</summary>
Satu syarat (Terima) bernilai SALAH.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Belum Selesai (Pending).**
Syarat AND membutuhkan kedua konfirmasi untuk menjadi SELESAI.
</details>

### Soal #87: Stack "Batu bata"
Tukang menyusun bata ke atas: [B1, B2, B3, B4].
Istri tukang butuh 1 bata untuk mengganjal pintu, ia mengambil yang paling atas. Lalu tukang sdar dan menaruh B5.
Urutan bata dari bawah sekarang adalah...
A. [B1, B2, B3, B5]
B. [B1, B2, B3, B4, B5]
C. [B1, B2, B3]
D. [B5, B3, B2, B1]

<details>
<summary>💡 Hint</summary>
B4 diambil, lalu B5 menempati posisi yang ditinggalkan (di atas B3).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [B1, B2, B3, B5].**
Tumpukan akhir memiliki B5 di puncak.
</details>

### Soal #88: Antrian "Ganti Shift"
Karyawan Antre Makan: [K1, K2]. 
Tiba-tiba jam istirahat habis. K1 sudah ambil nasi, tapi K2 belum. Mereka harus kembali bekerja.
Jika nanti mereka kembali antre, dan urutannya harus adil, siapa yang di depan?
A. K1
B. K2
C. Karyawan baru
D. Bebas

<details>
<summary>💡 Hint</summary>
K2 belum makan sama sekali, sedangkan K1 sudah proses ambil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. K2.**
Logika keadilan (FIFO) mengharuskan yang belum dilayani (K2) mendapat giliran lebih dulu.
</details>

### Soal #89: Logika "Auto-Save"
Game Save Otomatis JIKA (Menang Boss) **OR** (Setiap 10 Menit).
Baru main 5 menit, tapi sudah menang lawan Boss. Apakah game tersimpan?
A. Ya
B. Tidak
C. Tunggu 5 menit lagi
D. Hanya jika ada memori

<details>
<summary>💡 Hint</summary>
Logika OR: Syarat "Menang Boss" sudah terpenuhi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
Salah satu pemicu sudah aktif.
</details>

### Soal #90: Stack "Container Bak Truk"
Truk diisi: [Pojok depan: Beras, Terigu, Gula :Belakang].
Saat dibongkar di gudang, barang mana yang keluar pertama kali?
A. Beras
B. Terigu
C. Gula
D. Truknya

<details>
<summary>💡 Hint</summary>
Pintu truk ada di belakang. Yang terakhir masuk (Gula) adalah yang paling dekat pintu.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Gula.**
Prinsip LIFO berlaku karena akses hanya dari satu arah (belakang).
</details>

### Soal #91: Logika XOR pada Pin Pintu
Kombinasi benar jika (Digit1 XOR Digit2) = 1.
Jika digit pertama adalah 1, digit kedua harus...
A. 1
B. 0
C. 2
D. Sembarang

<details>
<summary>💡 Hint</summary>
1 XOR X = 1. Maka X harus berbeda dari 1.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0.**
Agar XOR menghasilkan 1, kedua input harus berbeda.
</details>

### Soal #92: Antrian "Bus Sekolah"
Bus berhenti di 3 halte. Halte 1 naik: A, B. Halte 2 naik: C.
Saat di Halte 3, ada 2 orang turun. Siapakah mereka (asumsi bus sangat penuh dan orang turun lewat pintu depan)?
A. A dan B
B. C dan B
C. A dan C
D. B dan C

<details>
<summary>💡 Hint</summary>
Turun lewat pintu yang sama dengan pintu naik = Stack (LIFO).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. C dan B.**
C naik terakhir, maka saat turun ia yang paling dekat pintu. Setelah C, baru B.
</details>

### Soal #93: Stack "Kerupuk dalam Kaleng"
Masukkan kerupuk: Putih, Kuning, Cokelat.
Kamu ingin makan kerupuk Putih. Berapa kerupuk yang harus kamu keluarkan minimal?
A. 1
B. 2
C. 3
D. 0

<details>
<summary>💡 Hint</summary>
Putih ada di dasar kaleng. Cokelat dan Kuning ada di atasnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 3.**
Kamu harus mengeluarkan Cokelat, lalu Kuning, baru bisa ambil Putih.
</details>

### Soal #94: Logika "Sensor Hujan & Wiper"
Wiper bergerak JIKA (Hujan Terdeteksi) **AND** (NOT Mobil Berhenti).
Hujan deras, tapi mobil sedang parkir (berhenti). Apakah wiper bergerak?
A. Ya
B. Tidak
C. Patah
D. Bergerak pelan

<details>
<summary>💡 Hint</summary>
Mobil berhenti = T, maka NOT mobil berhenti = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Sistem menghemat energi saat mobil tidak berjalan (berdasarkan logika soal).
</details>

### Soal #95: Antrian "Tiket Online"
Server down selama 10 menit. Ribuan orang klik "Beli" bersamaan.
Saat server pulih, pesanan mana yang datanya masuk duluan ke memori server?
A. Yang koneksi internetnya paling cepat (Low Latency).
B. Yang paling tua umurnya.
C. Yang paling mahal harganya.
D. Random.

<details>
<summary>💡 Hint</summary>
Dalam kompetisi waktu nyata, kecepatan "sampai" ke gerbang server adalah kunci.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Yang koneksi internetnya paling cepat.**
Ia yang "Enqueue" pertama kali di memori server.
</details>

### Soal #96: Logika "Lampu Tidur"
Lampu OFF JIKA (Hari Siang) **OR** (Lampu Utama Nyala).
Kamar gelap (Hari Malam), tapi kamu menyalakan Lampu Utama yang terang. Apakah Lampu Tidur OFF?
A. Ya (OFF)
B. Tidak (ON)
C. Berkedip
D. Rusak

<details>
<summary>💡 Hint</summary>
Salah satu syarat (Lampu Utama Nyala) bernilai BENAR.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya (OFF).**
Logika OR sudah terpenuhi oleh kondisi kedua.
</details>

### Soal #97: Stack "Kartu Solitaire"
Tumpukan: [7 Merah, 6 Hitam, 5 Merah].
Kamu harus menaruh kartu 4 Hitam di atasnya. Jika kamu ingin mengambil kartu 6 Hitam, apa yang harus dilakukan?
A. Ambil 5 Merah saja.
B. Ambil 4 Hitam dan 5 Merah.
C. Ambil langsung dari tengah.
D. Tidak bisa diambil.

<details>
<summary>💡 Hint</summary>
Aturan Stack: Tidak boleh ambil dari tengah tanpa memindahkan yang di atasnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ambil 4 Hitam dan 5 Merah.**
Keduanya menutup akses ke kartu 6 Hitam.
</details>

### Soal #98: Antrian "Toko Kelontong"
Antre: [Nenek, Anak Muda]. 
Nenek lupa dompet di mobil, ia pergi ambil (keluar antre). Anak Muda maju. 
Tiba-tiba Nenek datang lagi. Di mana posisi Nenek sekarang menurut aturan Queue adil?
A. Paling depan lagi.
B. Di belakang Anak Muda.
C. Di rumah saja.
D. Memotong antrean.

<details>
<summary>💡 Hint</summary>
Sekali keluar dari antrean, saat masuk kembali dianggap sebagai Enqueue baru (paling belakang).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di belakang Anak Muda.**
Urutan didasarkan pada kehadiran saat ini di barisan.
</details>

### Soal #99: Logika NAND dan NOT (Ganda)
NOT (A NAND B) sama dengan...
A. A OR B
B. A AND B
C. A XOR B
D. NOT A

<details>
<summary>💡 Hint</summary>
NAND adalah NOT-AND. Maka NOT (NOT-AND) = ...
</details>

<details>
<summary>✅ Jawaban</summary>
**B. A AND B.**
Dua negasi yang bertemu akan saling membatalkan.
</details>

### Soal #100: Refleksi 100 Soal
Setelah mengerjakan 100 soal, kamu tahu bahwa Logika dan Antrian adalah tentang...
A. Menghafal tabel kebenaran saja.
B. Memahami aliran data dan syarat keputusan (Input -> Syarat -> Output).
C. Belajar coding bahasa C++.
D. Menebak jawaban yang paling panjang.

<details>
<summary>💡 Hint</summary>
Pilihlah jawaban yang paling mencerminkan Computational Thinking.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memahami aliran data dan syarat keputusan.**
Inti dari pilar CT adalah proses berpikirnya, bukan sekadar hasil akhirnya.
</details>

### Soal #101: Variabel Logika (P, Q, R)
Tentukan nilai dari $(P \text{ AND } Q) \text{ OR } (\text{NOT } R)$ jika $P = \text{Benar}, Q = \text{Salah}, R = \text{Salah}$.
A. Benar
B. Salah
C. Kosong
D. Error

<details>
<summary>💡 Hint</summary>
(B AND S) = S. NOT S = B. S OR B = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
</details>

### Soal #102: Logika "Pendaftaran Lomba"
Syarat: (Kelas 10 **OR** Kelas 11) **AND** (Nilai Informatika > 80).
Budi Kelas 12, Nilai Informatika 95. Apakah boleh mendaftar?
A. Boleh
B. Tidak Boleh
C. Boleh jika ada izin
D. Otomatis Lulus

<details>
<summary>💡 Hint</summary>
Syarat kelas tidak terpenuhi (F OR F = F).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Boleh.**
</details>

### Soal #103: Antrian "Drive-Thru" (Sequence)
Antrian: [M1, M2, M3]. 
1. M1 selesai. 
2. M4 datang. 
3. M2 selesai. 
4. M5 datang.
Berapa mobil yang ada di antrian sekarang?
A. 2
B. 3
C. 4
D. 5

<details>
<summary>💡 Hint</summary>
Awal 3, keluar 2, masuk 2.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 3.**
Mobil yang tersisa: [M3, M4, M5].
</details>

### Soal #104: Stack "Penyimpanan Senjata Game"
Dalam game, kamu hanya bisa membawa 1 senjata aktif. Senjata baru akan menggantikan yang lama, dan yang lama disimpan di tas (Stack).
Urutan ambil: [Pedang, Panah, Kapak]. 
Jika kamu membuang Kapak, senjata apa yang otomatis kamu pegang?
A. Pedang
B. Panah
C. Tangan Kosong
D. Perisai

<details>
<summary>💡 Hint</summary>
LIFO: Senjata sebelum Kapak adalah Panah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Panah.**
</details>

### Soal #105: Logika NAND Kompleks
Hasil dari $(T \text{ NAND } F) \text{ AND } (T \text{ NAND } T)$ adalah...
A. Benar
B. Salah
C. T
D. F

<details>
<summary>💡 Hint</summary>
(T NAND F) = T. (T NAND T) = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
T AND F = Salah.
</details>

### Soal #106: Antrian "Chat Group"
Pesan masuk: [A, B, C, D]. 
Server down, lalu pesan B dan C terhapus karena error. 
Urutan pesan yang muncul saat server nyala kembali adalah...
A. [A, D]
B. [D, A]
C. [A, B, C, D]
D. [D, C, B, A]

<details>
<summary>💡 Hint</summary>
FIFO: Urutan waktu kirim tetap terjaga untuk pesan yang tersisa.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [A, D].**
</details>

### Soal #107: Stack "Undo" 3 Tingkat
Aksi: [Ketik "Halo", Cetak Tebal, Ubah Warna Merah]. 
Kamu menekan Ctrl+Z sebanyak 2 kali. Apa kondisi teks sekarang?
A. "Halo" (biasa)
B. "Halo" (cetak tebal)
C. Kosong
D. Teks Merah

<details>
<summary>💡 Hint</summary>
Undo 1: Warna hilang. Undo 2: Cetak tebal hilang.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. "Halo" (biasa).**
</details>

### Soal #108: Logika XOR "Deteksi Beda"
XOR sering digunakan untuk mengecek apakah dua data berbeda. 
Data1 = 1010, Data2 = 1011. 
Digit ke-4 (paling kanan) jika di-XOR menghasilkan?
A. 0
B. 1
C. 2
D. Sama

<details>
<summary>💡 Hint</summary>
0 XOR 1 = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1.**
</details>

### Soal #109: Antrian "Lift" (Kapasitas 3)
Orang: [A, B, C, D, E, F]. 
Lift mengangkut 3 orang sekali jalan. Pada tarikan kedua, siapa saja yang naik?
A. A, B, C
B. D, E, F
C. C, D, E
D. A, C, E

<details>
<summary>💡 Hint</summary>
Tarikan 1: A, B, C.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. D, E, F.**
</details>

### Soal #110: Stack "Buku di Perpustakaan"
Petugas mengembalikan buku ke rak: [Sejarah, Komik, Novel].
Buku Sejarah diletakkan paling bawah. Jika ada siswa ingin meminjam novel, berapa buku yang harus diangkat?
A. 0 (Langsung ambil)
B. 1
C. 2
D. 3

<details>
<summary>💡 Hint</summary>
Novel ada di paling atas tumpukan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 0 (Langsung ambil).**
</details>

### Soal #111: Logika "Kelulusan Jalur Prestasi"
Lulus jika: (Juara 1 Lomba Nasional) **OR** (Ranking 1 Kelas **AND** Nilai Rata-rata > 90).
Ani Ranking 2, tapi Juara 1 Lomba Nasional. Apakah Ani Lulus?
A. Lulus
B. Tidak Lulus
C. Tunggu perbaikan
D. Harus tes ulang

<details>
<summary>💡 Hint</summary>
Logika OR: Juara Nasional sudah BENAR.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Lulus.**
</details>

### Soal #112: Antrian "Loading Data" (Queue vs Priority)
Data: [Kecil, Besar, Menengah]. 
Sistem memproses data yang paling kecil ukurannya lebih dulu untuk menghemat memori. 
Urutan prosesnya adalah...
A. Kecil -> Menengah -> Besar
B. Kecil -> Besar -> Menengah
C. Besar -> Menengah -> Kecil
D. Menengah -> Kecil -> Besar

<details>
<summary>💡 Hint</summary>
Ini adalah Priority Queue berdasarkan ukuran.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kecil -> Menengah -> Besar.**
</details>

### Soal #113: Stack "Piring Prasmanan"
Tumpukan piring ada 10. Jika tamu mengambil piring ke-11 sementara tumpukan kosong, sistem akan mengalami...
A. Overflow
B. Underflow
C. Success
D. Restart

<details>
<summary>💡 Hint</summary>
Mengambil data dari tempat kosong = Underflow.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Underflow.**
</details>
---
[< Kembali ke Indeks Materi](../06-logika-dan-antrian.md) | [< Bagian Sebelumnya](./06-logika-dan-antrian-part-1.md) | [Bagian Selanjutnya >](./06-logika-dan-antrian-part-3.md)
