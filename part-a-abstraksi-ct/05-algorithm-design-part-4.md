# 05. Algorithm Design - Bagian 4 (Soal 151-200)

[< Bagian 3 (101-150)](05-algorithm-design-part-3.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 5 (201-250) >](05-algorithm-design-part-5.md)

---
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


---
[< Bagian 3 (101-150)](05-algorithm-design-part-3.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 5 (201-250) >](05-algorithm-design-part-5.md)
