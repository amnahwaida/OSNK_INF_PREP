🔙 **Kembali ke Materi:** [Materi 05 Algorithm Design](../05-algorithm-design.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 05. Algorithm Design - Bagian 6 (Soal 251-300)

[< Bagian 5 (201-250)](05-algorithm-design-part-5.md) | [🏠 Indeks](../05-algorithm-design.md)

---
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
[< Bagian 5 (201-250)](05-algorithm-design-part-5.md) | [🏠 Indeks](../05-algorithm-design.md)

