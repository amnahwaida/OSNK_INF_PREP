# 03. Pengenalan Pola - Bagian 5 (Soal 201-250)

[< Bagian 4 (151-200)](03-pattern-recognition-part-4.md) | [🏠 Indeks](../03-pattern-recognition.md)

---
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
