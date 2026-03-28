# 04. Abstraksi - Bagian 3 (Soal 101-150)

[< Bagian 2 (51-100)](04-abstraction-part-2.md) | [🏠 Indeks](../04-abstraction.md) | [Bagian 4 (151-200) >](04-abstraction-part-4.md)

---
### Soal #101: Abstraksi pada "Menu Pilihan Karakter" di Game RPG
Di layar pilih karakter, hanya ada statistik: `Strength, Agility, Intelligence`. Mengapa?
A. Karena game-nya kekurangan memori untuk mencatat detail lain.
B. Agar pemain bisa fokus membandingkan peran karakter berdasarkan pola kemampuannya (Abstraksi Atribut).
C. Karena nama-nama itu terdengar keren.
D. Karena pembuat game tidak tahu hobi karakternya.

<details>
<summary>💡 Hint</summary>
Atribut kunci digunakan untuk membedakan satu entitas dari entitas lain dalam sebuah sistem.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fokus membandingkan peran berdasarkan atribut.**
Game desain menggunakan abstraksi atribut untuk menciptakan keseimbangan (Balance) dalam permainan.
</details>

### Soal #102: Abstraksi pada "Ikon Baterai Lemah" (Warna Merah)
Saat baterai 10% warnanya jadi merah. Apa yang diabstraksi?
A. Harga baterai baru.
B. Ambang batas (Threshold) keamanan tegangan listrik yang menandakan perangkat harus segera dicas.
C. Bahwa HP-mu sedang marah.
D. Alur listrik yang keluar dari HP.

<details>
<summary>💡 Hint</summary>
Urutan status (Hijau -> Kuning -> Merah) mengabstraksi data numerik menjadi peringatan psikologis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ambang batas keamanan tegangan.**
Visualisasi status darurat mempermudah interaksi manusia dengan mesin.
</details>

### Soal #103: Abstraksi pada "Diagram Garis" (Line Chart)
Grafik harga emas menunjukkan naik turun setiap hari. Apa yang **DIABSTRAKSI**?
A. Nama toko emas yang menjualnya.
B. Fluktuasi ribuan transaksi jual-beli di pasar global menjadi satu garis tren harga rata-rata.
C. Berat emas dalam batang.
D. Kebahagiaan orang yang punya emas.

<details>
<summary>💡 Hint</summary>
Trend visual menyederhanakan data angka yang sangat banyak dari berbagai sumber.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fluktuasi ribuan transaksi menjadi garis tren.**
Visualisasi data adalah bentuk abstraksi statistik untuk memudahkan analisis pola.
</details>

### Soal #104: Deskripsi "Sekolah" bagi Dinas Kota
Bagi Pemerintah Kota, sebuah sekolah diabstraksi sebagai: `Nama_Sekolah, Alamat, Jumlah_Murid, Akreditasi`. Manakah detail yang **DIABSTRAKSI** (tidak dicatat)?
A. Nama sekolahnya.
B. Warna cat tiap ruang kelas dan merk sapu di sekolah itu.
C. Nilai akreditasi sekolah.
D. Alamat sekolah.

<details>
<summary>💡 Hint</summary>
Detail operasional mikro tidak relevan untuk pemetaan fasilitas pendidikan secara makro.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Warna cat ruang kelas dan merk sapu.**
Pemodelan data administratif selalu mengabaikan detail fisik yang tidak berpengaruh pada kebijakan.
</details>

### Soal #105: Abstraksi pada "Ikon Speaker" (Mute)
Ikon speaker dengan tanda silang ($\times$) berarti suara mati. Apa yang **DIABSTRAKSI**?
A. Jenis musik yang sedang diputar.
B. Penghentian aliran sinyal listrik ke speaker transduser oleh sistem audio komputer.
C. Harga speaker tersebut.
D. Nama merk software music-nya.

<details>
<summary>💡 Hint</summary>
Simbol visual mengabstraksi status sirkuit elektronik audio.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penghentian aliran sinyal listrik.**
Control interface mengabstraksi fungsi hardware yang kompleks menjadi status biner (On/Off).
</details>

### Soal #106: Abstraksi pada "Resep Kue" (Teknik Campur)
Resep menulis: "Kocok telur sampai mengembang". Apa yang diabstraksi?
A. Berapa jumlah butir telurnya.
B. Kecepatan rotasi mixer dalam unit RPM dan ikatan kimia protein telur yang berubah menjadi busa gas.
C. Nama merk telurnya.
D. Warna mangkuk pengocoknya.

<details>
<summary>💡 Hint</summary>
Instruksi memasak menyederhanakan fenomena kimia-fisika menjadi hasil visual/tekstur yang bisa dikenali manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kecepatan rotasi mixer dan ikatan kimia protein.**
Instruksi praktis adalah abstraksi dari proses sains yang mendasarinya.
</details>

### Soal #107: Ikon "Pen" (Edit)
Ikon pulpen digunakan untuk mengedit teks. Apa yang **DIABSTRAKSI**?
A. Bahwa kamu harus menulis di layar pakai tinta.
B. Perintah ke database untuk mengubah isi (Update) pada baris data tabel yang bersangkutan.
C. Warna pulpen yang kamu punya di tas.
D. Harga pulpen asli di toko buku.

<details>
<summary>💡 Hint</summary>
Metafora alat tulis menyederhanakan fungsi manipulasi data digital (CRUD).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perintah Update data di database.**
Simbol visual mengabstraksi operasi logika basis data yang sangat teknis.
</details>

### Soal #108: Abstraksi pada "Ikon Lokasi" (Pin Map)
Tanda "Pin" di peta menunjukkan posisi tokomu. Apa yang diabstraksi?
A. Bahwa tokomu berbentuk pin besi raksasa.
B. Koordinat numerik Lintang dan Bujur di database Google Maps.
C. Nama pemilik toko.
D. Daftar harga barang di toko tersebut.

<details>
<summary>💡 Hint</summary>
Titik visual (Pin) adalah wakil dari data spasial numerik di sistem informasi geografis (GIS).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Koordinat numerik Lintang dan Bujur.**
Abstraksi visual mempermudah navigasi manusia di atas data geospasial yang rumit.
</details>

### Soal #109: Abstraksi pada "Search Result" (Cuplikan Teks)
Saat cari di Google, muncul judul dan cuplikan 2 baris teks. Apa yang diabstraksi?
A. Seluruh isi artikel asli yang mungkin sangat panjang (misal 2000 kata).
B. Bahwa artikel itu tidak penting.
C. Nama orang yang mengetik artikel itu.
D. Warna background website aslinya.

<details>
<summary>💡 Hint</summary>
Cuplikan (Snippet) meringkas informasi agar pembaca bisa cepat menyaring relevansi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Seluruh isi artikel asli yang panjang.**
Meringkas (Summarization) adalah bentuk abstraksi konten untuk efisiensi waktu baca.
</details>

### Soal #110: Abstraksi pada "Diagram Silsilah Keluarga"
Garis penghubung antar kotak nama menunjukkan hubungan orang tua dan anak. Apa yang **DIABSTRAKSI**?
A. Nama-nama anggota keluarga.
B. Hubungan emosional, percakapan harian, dan sejarah hidup setiap orang dalam garis tersebut.
C. Tanggal lahir anggota keluarga.
D. Di mana mereka tinggal.

<details>
<summary>💡 Hint</summary>
Diagram silsilah hanya mengambil pola keterhubungan genetik/hukum dan membuang detail kehidupan pribadi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hubungan emosional dan sejarah hidup.**
Abstraksi silsilah fokus pada struktur keturunan tanpa beban narasi biografi setiap orang.
</details>

### Soal #111: Abstraksi pada "Ikon Speaker Bluetooth"
Ikon berbentuk huruf "B" bergaya runcing menandakan koneksi Bluetooth. Apa yang **DIABSTRAKSI**?
A. Nama perangkat yang terhubung.
B. Protokol komunikasi nirkabel jarak pendek menggunakan gelombang radio 2.4 GHz.
C. Volume musik yang keluar.
D. Sisa baterai speaker tersebut.

<details>
<summary>💡 Hint</summary>
Interface visual menyederhanakan standar teknologi komunikasi nirkabel yang rumit.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Protokol komunikasi nirkabel 2.4 GHz.**
Ikon adalah simbol abstrak untuk teknologi komunikasi data antar perangkat.
</details>

### Soal #112: Abstraksi pada "Indikator Bensin Mobil"
Jarum menunjukkan huruf "F" (Full) atau "E" (Empty). Apa yang **DIABSTRAKSI**?
A. Jenis bensin (Pertalite/Pertamax).
B. Jumlah liter bensin secara presisi dalam tangki dan tekanan fluida di dalamnya.
C. Nama SPBU tempat mengisi bensin.
D. Harga bensin per liter.

<details>
<summary>💡 Hint</summary>
Pengemudi hanya butuh estimasi kapasitas (0-100%) daripada angka liter yang terus berubah saat mobil berguncang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jumlah liter bensin secara presisi.**
Abstraksi indikator menyederhanakan data sensor menjadi informasi status yang fungsional.
</details>

### Soal #113: Model "Gerhana Matahari" (Edukasi)
Guru menggunakan bola tenis sebagai Bulan dan bola basket sebagai Bumi. Model ini mengabstraksi...
A. Jarak sebenarnya antar planet yang sangat jauh dan ukuran aslinya yang raksasa.
B. Bahwa Bulan itu sebenarnya adalah bola tenis.
C. Bahwa Matahari itu tidak panas.
D. Nama astronom yang menemukan gerhana.

<details>
<summary>💡 Hint</summary>
Model fisik menyederhanakan skala astronomis agar muat di dalam ruang kelas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Jarak dan ukuran sebenarnya.**
Abstraksi skala membantu siswa memahami hubungan posisi benda langit tanpa harus melihat objek aslinya.
</details>

### Soal #114: Abstraksi pada "Fitur Autocorrect"
Saat salah ketik "Hlo", HP langsung mengubah jadi "Halo". Apa yang diabstraksi?
A. Bahwa kamu jari-jarinya besar.
B. Algoritma pencocokan pola kata (Levensthein Distance) dan probabilitas bahasa di latar belakang.
C. Warna keyboard digital kamu.
D. Siapa yang kamu kirimi pesan.

<details>
<summary>💡 Hint</summary>
Otomasi perbaikan teks menyembunyikan perhitungan linguistik komputer dari pengguna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algoritma pencocokan pola kata.**
Software mengabstraksi kecerdasan bahasa menjadi fitur kenyamanan mengetik.
</details>

### Soal #115: Ikon "Airplane Mode"
Ikon pesawat digunakan untuk mematikan semua sinyal radio. Apa yang **DIABSTRAKSI**?
A. Bahwa kamu akan segera naik pesawat.
B. Prosedur pemutusan aliran daya ke modul WiFi, Bluetooth, dan Seluler secara bersamaan.
C. Nama maskapai penerbangan.
D. Kecepatan pesawat saat terbang.

<details>
<summary>💡 Hint</summary>
Satu perintah (Satu Klik) mengontrol banyak komponen hardware radio di dalam HP.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Prosedur pemutusan daya ke berbagai modul radio.**
Abstraksi sistem pengamanan penerbangan memudahkan pengguna patuh pada aturan keamanan.
</details>

### Soal #116: Abstraksi pada "Remote AC" (Mode Dry)
Mode "Dry" (Tetes Air) mengurangi kelembapan udara. Apa yang diabstraksi dari pengguna?
A. Suara kompresor AC.
B. Penyesuaian suhu koil pendingin agar air di udara mengembun, tanpa mendinginkan ruangan secara drastis.
C. Harga tagihan listrik.
D. Kecepatan angin di luar rumah.

<details>
<summary>💡 Hint</summary>
Mekanisme siklus refrigerasi yang rumit diabstraksi menjadi satu ikon status kelembapan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penyesuaian suhu koil pendingin untuk kondensasi.**
Interface menyembunyikan logika operasional mesin di bawah mode penggunaan sederhana.
</details>

### Soal #117: Abstraksi pada "Username"
Nama pengguna `@budi_keren` di media sosial adalah abstraksi dari...
A. Alamat rumah asli Budi.
B. Baris data identitas unik (ID) di database server yang mungkin berupa angka panjang.
C. Bahwa Budi memang orang yang keren.
D. Hobi Budi saat waktu luang.

<details>
<summary>💡 Hint</summary>
Nama yang mudah dibaca manusia mewakili data identitas yang kaku bagi mesin.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Baris data identitas unik di database.**
Abstraksi identitas digital mempermudah interaksi sosial antar pengguna komputer.
</details>

### Soal #118: Model "Peta Kontur" (Geografi)
Garis-garis melingkar di peta menunjukkan ketinggian gunung. Apa yang **DIABSTRAKSI**?
A. Jenis batuan dan pepohonan di gunung tersebut.
B. Bentuk permukaan tanah 3 dimensi yang rumit menjadi representasi garis 2 dimensi yang informatif.
C. Nama pendaki yang pernah ke sana.
D. Suhu udara di puncak gunung.

<details>
<summary>💡 Hint</summary>
Abstraksi geometris mengubah koordinat $Z$ (tinggi) menjadi pola garis datar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bentuk 3D rumit menjadi garis 2D.**
Visualisasi data geografis menggunakan abstraksi untuk memudahkan analisis topografi.
</details>

### Soal #119: Abstraksi pada "Lampu Indikator CAPS LOCK"
Lampu di keyboard menyala saat CAPS LOCK aktif. Apa yang diabstraksi?
A. Bahwa kamu sedang marah (mengetik huruf besar).
B. Sinyal input dari kontroler keyboard yang mengubah pemetaan karakter (Mapping) di software sistem operasi.
C. Berapa jumlah tombol di keyboard.
D. Merk switch keyboardnya.

<details>
<summary>💡 Hint</summary>
Satu lampu kecil mewakili perubahan logika sistem dalam memproses setiap tombol yang kamu tekan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perubahan pemetaan karakter di software.**
Status logika sistem diabstraksi menjadi indikator hardware yang sederhana.
</details>

### Soal #120: Abstraksi pada "Barcode Harga"
Kasir men-scan barcode, dan nama barang muncul di layar. Apa yang **DIABSTRAKSI** bagi kasir?
A. Warna kemasan barangnya.
B. Pencarian data di tabel inventory gudang berdasarkan kode numerik yang diwakili oleh garis-garis barcode.
C. Berapa sisa stok barang tersebut.
D. Nama pabrik pembuat barangnya.

<details>
<summary>💡 Hint</summary>
Teknologi scanning mengotomasi pencarian data manual yang lambat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pencarian data di tabel inventory.**
Abstraksi identifikasi produk mempercepat proses transaksi di toko modern.
</details>

### Soal #121: Model "Sistem Tata Surya" (Animasi)
Dalam animasi belajar, planet-planet berputar mengelilingi matahari. Apa yang **DIABSTRAKSI**?
A. Bahwa bumi itu bulat.
B. Kecepatan rotasi asli, skala jarak yang sangat jauh, dan pengaruh gravitasi benda langit lain yang tidak ditampilkan.
C. Nama setiap planet.
D. Warna matahari.

<details>
<summary>💡 Hint</summary>
Animasi menyederhanakan mekanika langit agar mudah diamati gerakannya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kecepatan asli, skala jarak, dan gravitasi kompleks.**
Abstraksi visual membantu pemahaman konsep dasar astronomi tanpa detail yang mengganggu.
</details>

### Soal #122: Abstraksi pada "Tombol Power" ($\circlearrowright$)
Kamu menekan tombol power, dan komputer menyala. Apa yang **DIABSTRAKSI**?
A. Aliran listrik dari PLN ke stopkontak.
B. Proses pengiriman sinyal ke motherboard, inisialisasi BIOS/UEFI, pencarian file sistem operasi di storage, dan loading memori.
C. Berapa lama kamu sudah mematikan komputer.
D. Merk kabel power yang dipakai.

<details>
<summary>💡 Hint</summary>
Proses "Booting" yang sangat teknis dimulai dari satu interaksi fisik sederhana.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Proses inisialisasi hardware dan booting OS.**
Tombol power adalah interface abstraksi untuk memulai operasional mesin digital.
</details>

### Soal #123: Abstraksi pada "Alamat Pengiriman" (Drop Point)
Kurir mengantar paket ke "Drop Point" terdekat, bukan langsung ke rumahmu. Drop Point sendiri adalah sebuah...
A. Tempat pembuangan paket.
B. Abstraksi lokasi penerimaan kolektif untuk meningkatkan efisiensi rute kurir utama.
C. Kantor polisi.
D. Tempat istirahat kurir.

<details>
<summary>💡 Hint</summary>
Logistik menggunakan titik transit sebagai cara mengelola ribuan alamat yang tersebar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi lokasi penerimaan kolektif.**
Pemanfaatan titik transit (Hub) adalah bentuk abstraksi jaringan distribusi barang.
</details>

### Soal #124: Ikon "Refresh" (Panah Melengkung)
Kamu klik refresh, halaman web dimuat ulang. Apa yang **DIABSTRAKSI**?
A. Bahwa internet kamu lambat.
B. Pengiriman request HTTP GET ke server, pengambilan data terbaru, pembersihan memori cache browser, dan rendering ulang elemen web.
C. Nama pemilik website tersebut.
D. Jumlah total pengunjung web itu.

<details>
<summary>💡 Hint</summary>
Satu perintah koordinasi menyegarkan seluruh tampilan data dari sumber aslinya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Request HTTP GET, update cache, dan re-rendering.**
User interface mengabstraksi siklus komunikasi client-server menjadi satu tombol aksi.
</details>

### Soal #125: Abstraksi pada "Smart Lock" (Akses Fingerprint)
Pintu terbuka saat jarimu ditempelkan. Apa yang diabstraksi?
A. Garis-garis unik di kulit jarimu.
B. Pemrosesan citra (image processing) sidik jari, perbandingan dengan data terenkripsi di memori, dan kontrol motor mekanik pengunci pintu.
C. Harga gagang pintunya.
D. Nama orang yang punya jari tersebut.

<details>
<summary>💡 Hint</summary>
Sistem keamanan otomatis mengabstraksi proses identitas diri menjadi kunci digital unik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pemrosesan citra, enkripsi, dan kontrol motor.**
Teknologi biometrik mengabstraksi keamanan fisik menjadi manajemen data identitas digital.
</details>

### Soal #126: Abstraksi pada "Laporan Nilai" (Rapor)
Nilai Matematika Budi adalah "A". Apa yang **DIABSTRAKSI**?
A. Nama guru matematika Budi.
B. Ratusan jam belajar, puluhan tugas, dan hasil ujian yang diringkas menjadi satu kategori kualitas (Huruf).
C. Berapa harga buku tulis Budi.
D. Warna baju Budi saat ujian.

<details>
<summary>💡 Hint</summary>
Huruf nilai mewakili evaluasi menyeluruh (abstraksi kualitatif) dari proses belajar yang panjang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Evaluasi proses belajar dan hasil ujian yang diringkas.**
Sistem penilaian menggunakan abstraksi untuk memudahkan pelaporan perkembangan pendidikan.
</details>

### Soal #127: Ikon "Bell" (Notifikasi)
Ikon lonceng digunakan untuk melihat pesan masuk terbaru. Apa yang **DIABSTRAKSI**?
A. Suara lonceng yang asli.
B. Antrian pesan di server aplikasi yang terus diperbarui secara real-time melalui teknologi Push Notification.
C. Nama orang yang mengirim notifikasi.
D. Berapa banyak orang yang suka dengan postinganmu.

<details>
<summary>💡 Hint</summary>
Simbol visual menyederhanakan akses ke daftar aktivitas terbaru di aplikasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Antrian pesan real-time dan Push Notification.**
Interface notifikasi mengabstraksi aliran data aktivitas menjadi daftar yang mudah dibaca pengguna.
</details>

### Soal #128: Abstraksi pada "Lampu Sinyal Kereta Api"
Lampu Hijau berarti jalan aman. Apa yang **DIABSTRAKSI** bagi masinis?
A. Berapa jumlah gerbong kereta.
B. Kondisi sensor di lintasan rel berkilo-kilometer di depan, posisi kereta lain, dan status jembatan/terowongan.
C. Nama stasiun tujuan berikutnya.
D. Berapa harga tiket penumpangnya.

<details>
<summary>💡 Hint</summary>
Satu warna lampu mewakili kesimpulan atas ribuan pemeriksaan sistem keamanan jalur kereta.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kondisi sensor dan posisi seluruh kereta di lintasan.**
Abstraksi kontrol jalur menjamin keselamatan perjalanan tanpa harus memeriksa rel secara manual.
</details>

### Soal #129: Abstraksi pada "Ikon Baterai Kritis" (Tanda Seru)
Ikon baterai muncul tanda seru merah. Apa yang **DIABSTRAKSI**?
A. Kerusakan fisik baterai.
B. Tegangan listrik yang sudah di bawah batas minimum sistem operasi sebelum melakukan shutdown paksa.
C. Bahwa HP-mu sedang panik.
D. Berapa sisa menit pastinya HP akan mati.

<details>
<summary>💡 Hint</summary>
Peringatan visual menyederhanakan manajemen daya darurat bagi pengguna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tegangan di bawah batas minimum sistem.**
Status darurat hardware diabstraksi menjadi sinyal peringatan visual yang mendesak.
</details>

### Soal #130: Abstraksi pada "Game Sepakbola" (Digital)
Saat tekan tombol "Tembak", karakter game menendang bola. Apa yang **DIABSTRAKSI**?
A. Kelelahan fisik atlet aslinya.
B. Perhitungan fisika trayektori bola, animasi karakter 3D, dan logika deteksi gol di software game.
C. Nama stadion tempat bermain.
D. Berapa harga sepatu bola yang dipakai karakter.

<details>
<summary>💡 Hint</summary>
Input tombol mengaktifkan simulasi olahraga yang kompleks di dalam game engine.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Trayektori fisika, animasi, dan logika game.**
Game menggunakan abstraksi interaksi agar pemain bisa merasakan sensasi olahraga lewat kendali sederhana.
</details>

### Soal #131: Abstraksi pada "Ikon Speaker" (Gelombang Suara)
Ikon speaker dengan satu, dua, atau tiga baris gelombang menunjukkan tingkat volume. Apa yang **DIABSTRAKSI**?
A. Jenis instrumen musik yang dimainkan.
B. Amplitudo gelombang audio dan daya listrik yang disuplai ke speaker.
C. Nama penyanyi yang sedang didengarkan.
D. Lirik lagu yang sedang diputar.

<details>
<summary>💡 Hint</summary>
Visual menyederhanakan parameter intensitas energi suara menjadi indikator level yang intuitif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Amplitudo audio dan daya listrik.**
Control interface mengabstraksi variabel fisika suara menjadi pilihan pengaturan bagi pengguna.
</details>

### Soal #132: Abstraksi pada "Smart TV" (Daftar Film)
Halaman depan Netflix menunjukkan gambar poster film. Apa yang **DIABSTRAKSI**?
A. Nama sutradara filmnya.
B. Ribuan file fragmen video (Chunks) yang tersimpan di server CDN global yang siap di-stream saat diklik.
C. Berapa harga kuota internet untuk nonton film itu.
D. Berapa lama durasi filmnya.

<details>
<summary>💡 Hint</summary>
Satu gambar (Poster) mewakili akses ke konten digital raksasa yang tersebar di internet.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fragmen video yang tersimpan di server CDN.**
Layanan streaming mengabstraksi infrastruktur distribusi konten di balik interface pemilihan film.
</details>

### Soal #133: Abstraksi pada "Suhu Udara di HP"
HP menulis: "Jakarta $32^\circ C$". Apa yang **DIABSTRAKSI**?
A. Di mana posisi matahari sekarang.
B. Ribuan data sensor cuaca di berbagai titik kota yang dirata-rata untuk mewakili kondisi umum wilayah tersebut.
C. Berapa harga es teh di Jakarta.
D. Nama aplikasi prakiraan cuacanya.

<details>
<summary>💡 Hint</summary>
Angka tunggal adalah hasil pengolahan data spasial (Spatial Aggregation) yang luas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rata-rata ribuan data sensor cuaca.**
Aplikasi cuaca menggunakan abstraksi meteorologi untuk memberikan ringkasan status atmosfer kota.
</details>

### Soal #134: Ikon "Gembok Terbuka" (Unlock)
Simbol gembok terbuka digunakan untuk melepaskan proteksi data atau akses. Apa yang **DIABSTRAKSI**?
A. Kunci besi yang berkarat.
B. Penghapusan restriksi izin (Permission) pada file atau direktori di dalam sistem keamanan software.
C. Nama orang yang membuka gembok.
D. Berapa banyak orang yang boleh masuk.

<details>
<summary>💡 Hint</summary>
Simbol visual menyederhanakan perubahan status akses (Authorization) di sistem komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penghapusan restriksi izin pada sistem software.**
Abstraksi kontrol akses mempermudah manajemen privasi dan keamanan data pengguna.
</details>

### Soal #135: Abstraksi pada "Alat Musik Drum Digital"
Kamu memukul pad karet, dan suara drum asli terdengar. Apa yang diabstraksi?
A. Tekanan udara saat memukul drum asli.
B. Deteksi tekanan (Velocity) pada sensor piezoelektrik yang memicu pemutaran sampel audio berkualitas tinggi.
C. Nama merk pad karetnya.
D. Berapa banyak stik drum yang kamu punya.

<details>
<summary>💡 Hint</summary>
Teknologi digital menyalin karakteristik akustik instrumen asli ke dalam sistem elektronik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor piezoelektrik dan pemicu sampel audio.**
Drum digital mengabstraksi kerumitan instrumen perkusi menjadi pengalaman bermain yang ringkas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor piezoelektrik dan pemicu sampel audio.**
Drum digital mengabstraksi kerumitan instrumen perkusi menjadi pengalaman bermain yang ringkas.
</details>

### Soal #136: Abstraksi pada "Ikon Baterai Berwarna Hijau"
Warna hijau berarti baterai sehat/penuh. Apa yang **DIABSTRAKSI** di sini?
A. Bahan kimia Lithium-ion di dalam baterai.
B. Status kapasitas yang berada di atas rentang aman sistem (misal > 80%).
C. Harga cas HP kamu.
D. Berapa jam lagi kamu akan main HP.

<details>
<summary>💡 Hint</summary>
Kategori warna menyederhanakan interpretasi data persentase yang spesifik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Status kapasitas di atas rentang aman.**
Indikator status mengabstraksi data kesehatan hardware menjadi sinyal visual yang menenangkan pengguna.
</details>

### Soal #137: Abstraksi pada "Rating Bintang Hotel"
Hotel "Bintang 5" memiliki standar fasilitas tertentu. Apa yang **DIABSTRAKSI**?
A. Nama setiap staf yang bekerja di hotel itu.
B. Ratusan kriteria fasilitas (Kolam renang, WiFi, Menu, Luas Kamar) yang diringkas dalam satu klasifikasi prestise.
C. Berapa tahun hotel itu sudah berdiri.
D. Warna cat luar gedung hotel tersebut.

<details>
<summary>💡 Hint</summary>
Klasifikasi standar Industri menyederhanakan perbandingan kualitas layanan bagi konsumen.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ratusan kriteria fasilitas yang diringkas.**
Sistem rating menggunakan abstraksi kualitas untuk memandu keputusan pasar secara cepat.
</details>

### Soal #138: Ikon "Penghapus" (Eraser) di Paint
Ikon penghapus digunakan untuk membersihkan gambar. Apa yang **DIABSTRAKSI**?
A. Gesekan karet penghapus asli di kertas.
B. Pengubahan nilai warna setiap pixel yang dilalui kursor kembali menjadi nilai warna latar belakang (misal Putih).
C. Berapa lama kamu sudah menggambar.
D. Nama merk software gambarnya.

<details>
<summary>💡 Hint</summary>
Metafora alat fisik menyederhanakan manipulasi matriks pixel di memori komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengubahan nilai warna pixel menjadi warna latar.**
Toolbox grafis mengabstraksi algoritma manipulasi gambar menjadi interaksi kanvas yang intuitif.
</details>

### Soal #139: Abstraksi pada "Data Transaksi M-Banking"
Hanya tertulis: `Nama_Penerima, Nominal, Tanggal`. Apa yang **DIABSTRAKSI**?
A. Alamat rumah penerima uang.
B. Aliran data saldo antar database bank yang berbeda melalui jaringan *clearing* antar bank.
C. Warna kartu ATM penerima.
D. Berapa banyak orang yang ikut antre di bank saat itu.

<details>
<summary>💡 Hint</summary>
Laporan mutasi rekening menyederhanakan pergerakan aset finansial digital di sistem perbankan global.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Aliran data saldo antar database bank melalui jaringan clearing.**
Layanan finansial mengabstraksi kerumitan akuntansi perbankan menjadi daftar riwayat transaksi bagi nasabah.
</details>

### Soal #140: Ikon "MicroSD Card" (Storage)
Ikon kartu kecil digunakan untuk melihat isi memori tambahan. Apa yang **DIABSTRAKSI**?
A. Struktur fisik chip semikonduktor di dalam kartu tersebut.
B. Sistem file (FAT32/exFAT) yang mengelola pengalamatan data pada sel-sel memori flash.
C. Nama merk kartu memorinya.
D. Berapa harga kartu memori itu di toko.

<details>
<summary>💡 Hint</summary>
Simbol visual menyederhanakan akses ke media penyimpanan data elektronik yang kompleks.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sistem file yang mengelola pengalamatan data.**
Interface storage mengabstraksi mekanisme penyimpanan fisik menjadi hirarki file yang mudah dikelola.
</details>

### Soal #141: Abstraksi pada "Ikon Baterai Pengisian" (Petir)
Simbol petir ($\lightning$) berarti HP sedang dicas. Apa yang **DIABSTRAKSI**?
A. Suara aliran listrik dari stopkontak.
B. Proses masuknya arus searah (DC) ke dalam sel baterai dan reaksi kimia perpindahan ion lithium di dalamnya.
C. Merk kepala charger yang digunakan.
D. Berapa watt sisa daya di rumahmu.

<details>
<summary>💡 Hint</summary>
Status visual menyederhanakan fenomena elektrokimia pengisian daya menjadi status "Charging".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Arus DC dan reaksi kimia perpindahan ion lithium.**
Indikator charging mengabstraksi manajemen daya hardware bagi kenyamanan pengguna.
</details>

### Soal #142: Abstraksi pada "Navigasi Menu di Website"
Menu: "Home, Produk, Tentang Kami, Kontak". Nama-nama ini mengabstraksi...
A. Nama orang yang membuat website tersebut.
B. Kumpulan halaman web (HTML files) dan database terkait yang dikelompokkan berdasarkan tema konten.
C. Warna latar belakang website tersebut.
D. Lokasi server fisik tempat file web disimpan.

<details>
<summary>💡 Hint</summary>
Struktur menu menyederhanakan arsitektur informasi (Web Architecture) menjadi poin navigasi yang logis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kumpulan file HTML dan database bertema sama.**
Abstraksi menu mempermudah pengunjung menemukan informasi tanpa harus tahu struktur file server.
</details>

### Soal #143: Ikon "Gembok Terkunci" (Proteksi Data)
Ikon gembok pada sebuah file menandakan file tersebut tidak bisa diedit (Read-Only). Apa yang **DIABSTRAKSI**?
A. Logam fisik gembok yang kuat.
B. Pengaturan atribut izin penulisan (Write Permission) di dalam tabel metadata sistem operasi.
C. Nama pemilik file asli tersebut.
D. Berapa KB ukuran file tersebut.

<details>
<summary>💡 Hint</summary>
Visual menyederhanakan status proteksi integritas data di sistem komputer.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengaturan atribut izin penulisan di metadata.**
Keamanan file mengabstraksi algoritma kontrol akses menjadi simbol status visual.
</details>

### Soal #144: Abstraksi pada "Search Suggestion" (Prediksi Kata)
Baru ketik "Cara ...", muncul "Cara menggambar". Apa yang **DIABSTRAKSI**?
A. Pikiran pengguna yang sedang bingung.
B. Analisis statistik miliaran query pencarian populer yang diolah oleh mesin pencari secara instan.
C. Kecepatan tangan pengguna saat mengetik.
D. Nama aplikasi yang digunakan untuk mencari.

<details>
<summary>💡 Hint</summary>
Fungsi saran menyederhanakan pencarian data masal menjadi pilihan cepat bagi pengguna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Analisis statistik miliaran query pencarian populer.**
Fitur autocomplete mengabstraksi kecanggihan pemrosesan Big Data di balik interface kolom input.
</details>

### Soal #145: Abstraksi pada "Ikon Baterai Habis" (X atau Kosong)
Ikon baterai kosong dengan garis merah tipis. Apa yang **DIABSTRAKSI**?
A. Bahwa baterainya hilang.
B. Kapasitas tegangan yang sudah di ambang kritis untuk menjaga kestabilan sirkuit utama.
C. Bahwa HP-mu ingin istirahat.
D. Berapa harga baterai pengganti.

<details>
<summary>💡 Hint</summary>
Peringatan status energi menyederhanakan parameter fisik kelistrikan bagi keselamatan perangkat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kapasitas tegangan di ambang kritis sirkuit.**
Abstraksi status energi darurat memastikan pengguna mematikan perangkat dengan benar sebelum mati total.
</details>

### Soal #146: Abstraksi pada "Ikon Folder" (Katalog Gambar)
Isi folder "Foto Kucing" hanyalah bintik pixel di harddisk. Folder adalah...
A. Tempat menyimpan kucing asli.
B. Penamaan abstrak untuk mengelompokkan set data yang memiliki keterkaitan tema visual.
C. Gambar yang tidak memiliki arti logika.
D. Bahwa komputer itu pintar organisasi.

<details>
<summary>💡 Hint</summary>
Pengorganisasian data menggunakan label tematik (Abstraksi Klasifikasi) untuk mempermudah pencarian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penamaan abstrak untuk kelompok data bertema sama.**
Sistem file mengabstraksi lokasi penyimpanan fisik menjadi struktur logika yang manusiawi.
</details>

### Soal #147: Abstraksi pada "Fitur Filter Foto"
Kamu memilih filter "Vintage", dan foto jadi coklat tua. Apa yang **DIABSTRAKSI**?
A. Umur foto tersebut secara asli.
B. Operasi matematika koordinat warna (Lookup Table/LUT) pada setiap pixel di gambar tersebut secara massal.
C. Keindahan wajah orang di dalam foto.
D. Merk HP yang digunakan untuk memotret.

<details>
<summary>💡 Hint</summary>
Software mengabstraksi pengolahan citra digital (Image Processing) menjadi pilihan gaya visual sederhana.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Operasi matematika koordinat warna (LUT) massal.**
Editor foto menyembunyikan rumus kalkulasi warna di bawah antarmuka pemilihan filter.
</details>

### Soal #148: Ikon "Magnifying Glass" (Cari)
Kaca pembesar digunakan untuk fungsi pencarian. Apa yang **DIABSTRAKSI**?
A. Bahwa tulisannya terlalu kecil untuk dibaca.
B. Algoritma pencocokan string (Pattern Matching) dalam database untuk menemukan data yang diinginkan.
C. Nama orang yang mencari data.
D. Harga kaca pembesar asli di toko optik.

<details>
<summary>💡 Hint</summary>
Simbol visual menyederhanakan aksi penemuan informasi di dalam tumpukan data digital.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algoritma pencocokan string (Pattern Matching).**
Interface pencarian mengabstraksi mekanisme *retrieval* data di latar belakang sistem.
</details>

### Soal #149: Abstraksi pada "Indikator Suhu Air" (Dispenser)
Lampu merah menyala saat air mendidih. Apa yang **DIABSTRAKSI**?
A. Bahwa airnya marah (panas).
B. Pembacaan sensor suhu (NTC/Thermistor) yang menutup jalur listrik ke elemen pemanas setelah mencapai $95^\circ C$.
C. Berapa liter air yang tersisa di dalam galon.
D. Nama merk dispenser tersebut.

<details>
<summary>💡 Hint</summary>
Status visual menyederhanakan kontrol suhu otomatis di dalam alat elektronik rumah tangga.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pembacaan sensor suhu dan kontrol elemen pemanas.**
Abstraksi kontrol sistem menyembunyikan mekanisme proteksi panas di balik lampu indikator sederhana.
</details>

### Soal #150: Abstraksi pada "Tombol Volume" (Fisik)
Kamu menekan tombol samping HP, dan suara membesar. Apa yang **DIABSTRAKSI**?
A. Tekanan jarimu pada plastik tombol.
B. Pengiriman sinyal interupsi ke CPU, penyesuaian gain audio di chip soundcard, dan pembaruan visual bar volume di layar.
C. Judul lagu yang sedang diputar.
D. Nama merk casing HP kamu.

<details>
<summary>💡 Hint</summary>
Interaksi fisik sederhana memicu rangkaian instruksi software and hardware untuk mengubah intensitas suara.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sinyal interupsi CPU, gain soundcard, dan update bar visual.**
Interface kontrol volume mengabstraksi manajemen audio sistem demi kenyamanan pengguna.
</details>

