🔙 **Kembali ke Materi:** [Materi 04 Abstraction](../04-abstraction.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 04. Abstraksi - Bagian 1 (Soal 1-50)

[🏠 Indeks](../04-abstraction.md) | [Bagian 2 (51-100) >](04-abstraction-part-2.md)

---
## Latihan Soal: Abstraksi (Set #1)

Mari uji kemampuanmu dalam membedakan mana detail yang penting dan mana yang bisa diabstraksi.

### Soal #1: Navigasi Bus
Seorang sopir bus perlu tahu rute perjalanan dari kota A ke kota B. Manakah detail yang **HARUS** ada (tidak boleh diabstraksi) untuk tujuan navigasi?
A. Jenis musik yang didengarkan penumpang.
B. Nama-nama persimpangan jalan dan arah belokan.
C. Warna baju yang dipakai sopir bus lain.
D. Jumlah total baut di roda bus.

<details>
<summary>💡 Hint</summary>
Pikirkan: jika detail ini hilang, apakah bus bisa sampai ke tujuan?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Nama persimpangan dan arah belokan.**
Ini adalah elemen inti navigasi. Detail lainnya tidak relevan untuk menentukan arah bus.
</details>

### Soal #2: Resep Masakan
Ibu ingin membuat nasi goreng mengikuti resep di buku. Manakah detail dalam resep yang merupakan hasil abstraksi?
A. "Gunakan 2 siung bawang putih"
B. "Masak sampai harum"
C. Ikon gambar nasi goreng di pojok halaman.
D. Suhu api kompor dalam derajat Kelvin secara presisi.

<details>
<summary>💡 Hint</summary>
Abstraksi menyederhanakan detail teknis yang terlalu rumit menjadi instruksi yang mudah dipahami.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. "Masak sampai harum".**
Ini adalah instruksi abstrak. Ia mengabstraksi detail teknis seperti suhu api tepatnya berapa atau berapa menit detiknya, cukup gunakan indikasi "harum".
</details>

### Soal #3: Pemodelan Siswa
Sebuah aplikasi "Perpustakaan Digital" ingin mencatat data peminjam buku (siswa). Detail mana yang **PALING TIDAK PENTING** (harus diabstraksi)?
A. Nama Lengkap
B. Nomor Induk Siswa (NIS)
C. Makanan favorit siswa
D. Judul buku yang dipinjam

<details>
<summary>💡 Hint</summary>
Tujuannya adalah administrasi perpustakaan. Apakah tahu siswa suka bakso membantu proses pinjam buku?
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Makanan favorit siswa.**
Detail ini tidak relevan dengan sistem perpustakaan dan hanya menambah beban data yang tidak perlu.
</details>

### Soal #4: Ikon Tombol "Save"
Di banyak aplikasi, tombol "Simpan" masih menggunakan ikon Disket (Floppy Disk), padahal zaman sekarang kita sudah tidak pakai disket lagi. Ini adalah contoh abstraksi yang bertujuan untuk...
A. Mengingatkan sejarah komputer.
B. Menjadi simbol universal (metafora) tindakan menyimpan data bagi pengguna.
C. Menjual disket yang sudah tidak laku.
D. Membingungkan anak muda.

<details>
<summary>💡 Hint</summary>
Ikon mengabstraksi proses penulisan data ke dalam storage menjadi satu gambar yang mudah dikenali maksudnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menjadi simbol universal.**
Abstraksi visual mempermudah pengguna memahami fungsi tanpa harus tahu cara kerja penyimpanan data di sistem.
</details>

### Soal #5: Black Box Televisi
Kamu menekan tombol "Volume Up" di remot TV, dan suara TV membesar. Kamu tidak tahu bagaimana sinyal inframerah diubah menjadi aliran listrik di speaker. Ini membuktikan bahwa...
A. TV itu ajaib.
B. Detail teknis internal TV telah diabstraksi bagi pengguna melalui antarmuka remot.
C. Remot TV lebih pintar daripada manusia.
D. Kamu tidak perlu belajar fisika.

<details>
<summary>💡 Hint</summary>
"Black Box" adalah konsep di mana kita tahu Input dan Output-nya, tapi tidak perlu tahu proses rumit di dalamnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Detail teknis internal TV telah diabstraksi.**
Abstraksi memungkinkan kita menggunakan teknologi canggih tanpa harus menjadi ahli di bidang tersebut.
</details>

### Soal #6: Abstrak Soal OSN-K
"Budi memiliki 5 apel. Ia memberikan 2 apel ke Siti. Siti sangat senang karena sore itu cuacanya cerah dan ia sedang haus."
Model matematika paling sederhana untuk cerita di atas (sebagai hasil abstraksi) adalah...
A. $5 - 2 +$ Cuaca Cerah
B. $5 - 2 = 3$
C. Budi + Siti = Apel
D. Siti haus saat cuaca cerah.

<details>
<summary>💡 Hint</summary>
Abaikan detail emosi dan cuaca yang tidak mempengaruhi jumlah apel.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 5 - 2 = 3.**
Abstraksi membuang narasi non-logis untuk mendapatkan inti perhitungan matematikanya.
</details>

### Soal #7: Alamat Pengiriman
Saat mengirim paket lewat kurir kargo, detail mana yang **KRUSIAL** (tidak boleh diabstraksi)?
A. Nama orang tua pengirim.
B. Kodepos dan Nomor Telepon penerima.
C. Alasan pengirim mengirim paket tersebut.
D. Warna baju kurir saat menjemput paket.

<details>
<summary>💡 Hint</summary>
Tanpa detail ini, paket berisiko tidak sampai atau tidak bisa dikonfirmasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kodepos dan Nomor Telepon penerima.**
Kodepos membantu sortir lokasi secara efisien (abstraksi wilayah), dan nomor telepon penting untuk koordinasi pengantaran.
</details>

### Soal #8: Kartu Identitas (KTP)
Di kartu KTP, terdapat foto wajah. Foto wajah ini merupakan abstraksi dari...
A. Kepribadian orang tersebut.
B. Penampilan fisik seseorang untuk tujuan identifikasi visual.
C. Seluruh sejarah hidup orang tersebut.
D. Keinginan orang tersebut untuk menjadi artis.

<details>
<summary>💡 Hint</summary>
Foto hanya mengambil satu aspek (visual) dan mengabaikan jutaan aspek lain dari seorang manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Penampilan fisik untuk identifikasi.**
Foto adalah "snapshot" atau abstraksi visual dari identitas seseorang.
</details>

### Soal #9: Deskripsi Lowongan Kerja
Sebuah iklan lowongan kerja menulis: "Dibutuhkan Admin, minim. SMA, mahir Excel."
Detail mana yang **DIABSTRAKSI** (dibuang) dari iklan tersebut?
A. Syarat pendidikan.
B. Kemampuan teknis yang dicari.
C. Jadwal makan siang harian karyawan secara mendetail.
D. Nama posisi pekerjaan.

<details>
<summary>💡 Hint</summary>
Iklan hanya menampilkan "inti" agar pencari kerja bisa langsung memutuskan.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Jadwal makan siang harian.**
Detail operasional harian seperti itu tidak relevan untuk diumumkan di tahap awal iklan lowongan.
</details>

### Soal #10: Diagram Alir (Flowchart)
Dalam Flowchart, kita menggunakan simbol **Ketupat** untuk "Keputusan (Ya/Tidak)". Simbol ini mengabstraksi apa?
A. Gambar orang yang sedang berpikir.
B. Ribuan baris kode logika `IF-ELSE` di komputer menjadi satu simbol visual sederhana.
C. Bahwa programmer suka makan ketupat.
D. Bahwa hidup itu penuh pilihan sulit.

<details>
<summary>💡 Hint</summary>
Diagram menyederhanakan struktur kode yang kompleks menjadi alur logika yang universal.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyederhanakan kode IF-ELSE jadi simbol.**
Flowchart adalah abstraksi visual dari logika pemrograman.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyederhanakan kode IF-ELSE jadi simbol.**
Flowchart adalah abstraksi visual dari logika pemrograman.
</details>

### Soal #11: Ikon "Home" di Browser
Ikon berbentuk rumah digunakan untuk kembali ke halaman utama. Ini membuktikan pola abstraksi...
A. Browser ingin kamu tinggal di rumah saja.
B. Gambar rumah digunakan sebagai metafora bagi tujuan awal/pusat navigasi.
C. Pembuat browser adalah arsitek bangunan.
D. Ikon itu sebenarnya adalah data koordinat GPS rumahmu.

<details>
<summary>💡 Hint</summary>
Ikon mengabstraksi konsep "Halaman Utama" menjadi simbol yang mudah dimengerti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Metafora tujuan awal.**
Abstraksi visual mempermudah navigasi bagi pengguna awam.
</details>

### Soal #12: Mesin Kopi Otomatis
Kamu hanya menekan tombol "Cappuccino" dan mesin bekerja sendiri. Manakah detail yang **DIABSTRAKSI** dari pengguna?
A. Harga kopinya.
B. Tekanan air dan durasi penggilingan biji kopi di dalam mesin.
C. Nama menu yang dipilih.
D. Keberadaan cangkir di bawah corot mesin.

<details>
<summary>💡 Hint</summary>
Pikirkan apa yang terjadi di dalam bodi mesin yang tidak kamu lihat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tekanan air dan durasi penggilingan.**
Pengguna hanya perlu tahu interface tombol, bukan mekanisme internalnya.
</details>

### Soal #13: Model Grafik Batang
Data jumlah penduduk: Desa A(500), Desa B(200). Di grafik batang, Desa A digambar lebih tinggi. Apa yang diabstraksi di sini?
A. Nama jalan di Desa A.
B. Perbedaan jumlah penduduk yang nyata menjadi perbandingan tinggi batang secara visual.
C. Jenis kelamin penduduk.
D. Pekerjaan penduduk.

<details>
<summary>💡 Hint</summary>
Grafik hanya mengambil aspek "Jumlah" (Kuantitas) dan membuang detail identitas perorangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perbandingan jumlah penduduk menjadi tinggi batang.**
Grafik adalah abstraksi data angka menjadi representasi visual.
</details>

### Soal #14: Pengaturan AC (Remot)
Kamu menyetel suhu $24^\circ C$. Kamu tidak perlu mengatur berapa putaran kipas di luar ruangan atau berapa banyak gas freon yang mengalir. Ini adalah contoh...
A. Penghematan daya.
B. Abstraksi kontrol sistem yang kompleks melalui parameter suhu sederhana.
C. Kerusakan sensor AC.
D. Keajaiban alat elektronik.

<details>
<summary>💡 Hint</summary>
Input sederhana menghasilkan output kompleks tanpa intervensi detail dari pengguna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi kontrol sistem.**
User Interface (Remot) mengabstraksi mekanisme termodinamika AC.
</details>

### Soal #15: Avatar di Game Online
Karaktermu berbentuk ksatria gagah, tapi di database game, kamu hanyalah barisan angka ID: `109283`. Mengapa ada Avatar?
A. Agar server tidak berat.
B. Sebagai abstraksi visual dari data statistik pemain agar permainan terasa menyenangkan.
C. Karena angka itu membosankan.
D. Biar pemain bisa pamer baju.

<details>
<summary>💡 Hint</summary>
Avatar menyederhanakan representasi data pemain menjadi objek yang bisa dikenali secara visual.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi visual dari data statistik.**
Pemain berinteraksi dengan visual, namun mesin berinteraksi dengan data abstraknya.
</details>

### Soal #16: Login Password
Saat mengetik sandi, yang muncul di layar adalah tanda bintang atau titik (`****`). Apa yang diabstraksi?
A. Kecepatan jari tanganmu.
B. Karakter asli yang kamu ketik, demi tujuan keamanan visual.
C. Bahwa HP-mu tidak bisa membaca huruf.
D. Alur listrik dari keyboard ke layar.

<details>
<summary>💡 Hint</summary>
Abstraksi digunakan untuk menyembunyikan informasi sensitif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Karakter asli demi keamanan.**
Sistem mengabstraksi input rahasia menjadi simbol generik agar tidak terlihat orang lain.
</details>

### Soal #17: Pemodelan Cuaca di Berita
Penyiar berkata: "Hari ini cerah berawan". Di layar ada ikon matahari tertutup awan kecil. Apa yang **DIABSTRAKSI**?
A. Kelembapan udara, kecepatan angin tepatnya, dan tekanan barometrik.
B. Nama presenter cuacanya.
C. Hari dan jam siaran.
D. Biaya produksi acaranya.

<details>
<summary>💡 Hint</summary>
Laporan cuaca meringkas data fisik atmosfer menjadi status yang mudah dipahami warga.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kelembapan, kecepatan angin, dan tekanan.**
Detail teknis meteorologi diabstraksi menjadi status "Cerah Berawan".
</details>

### Soal #18: Deskripsi Barang di Toko Online
Iklan HP menulis: "Kamera 108MP, Baterai 5000mAh". Mengapa tidak disebutkan jenis baut yang dipakai atau bahan kimia di dalam baterainya?
A. Karena penjualnya tidak tahu.
B. Karena informasi tersebut tidak relevan bagi mayoritas pembeli untuk mengambil keputusan.
C. Agar iklannya pendek.
D. Karena itu rahasia perusahaan.

<details>
<summary>💡 Hint</summary>
Abstraksi informasi membantu konsumen fokus pada fitur utama (selling point).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Informasi tidak relevan bagi pembeli.**
Pemasaran selalu melakukan abstraksi produk menjadi fitur-fitur kunci.
</details>

### Soal #19: Lampu Lalu Lintas
Sopir hanya perlu tahu "Merah = Berhenti". Sopir tidak perlu tahu berapa tegangan voltase lampu tersebut. Apa kegunaan abstraksi di sini?
A. Biar lampu nggak cepat putus.
B. Menjamin keamanan dan kecepatan pengambilan keputusan di jalan raya.
C. Biar polisi tidak perlu kerja.
D. Agar jalanan terlihat warna-warni.

<details>
<summary>💡 Hint</summary>
Hanya satu sinyal (warna) yang dibutuhkan untuk mengontrol arus kendaraan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Keamanan dan kecepatan keputusan.**
Abstraksi warna lampu adalah standar komunikasi universal di jalan.
</details>

### Soal #20: Penggunaan Fungsi `print("Hello")`
Dalam coding, kamu hanya menulis `print`. Kamu tidak perlu tahu bagaimana CPU memerintahkan setiap pixel di layar menyala untuk membentuk huruf. Ini adalah contoh...
A. Kemalasan programmer.
B. Abstraksi tingkat tinggi (High-level abstraction) dalam bahasa pemrograman.
C. Kerusakan layar komputer.
D. Bahwa komputer bisa membaca pikiranmu.

<details>
<summary>💡 Hint</summary>
Bahasa pemrograman modern menyembunyikan detail hardware yang sangat rumit.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi tingkat tinggi.**
Satu perintah sederhana mengaktifkan ribuan instruksi mesin di bawahnya.
</details>

### Soal #21: Model Rangka Tubuh (Biologi)
Di laboratorium biologi ada patung rangka manusia. Patung itu tidak memiliki kulit, otot, atau organ dalam. Mengapa?
A. Karena patungnya belum selesai dibuat.
B. Agar siswa bisa fokus mempelajari pola susunan tulang (abstraksi anatomis).
C. Biar tidak menakutkan.
D. Karena tulang adalah bagian tubuh yang paling awet.

<details>
<summary>💡 Hint</summary>
Hanya satu sistem (tulang) yang ditonjolkan, detail sistem lain dibuang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fokus mempelajari susunan tulang.**
Model edukasi menggunakan abstraksi untuk mengisolasi objek yang sedang dipelajari.
</details>

### Soal #22: Alamat IP vs Domain Name
Kamu mengetik `google.com`, bukan angka rumit seperti `172.217.13.110`. Web browser melakukan abstraksi berupa...
A. Mengubah angka menjadi kata agar mudah diingat manusia.
B. Menghapus situs web yang tidak aman.
C. Mempercepat koneksi internet.
D. Biar pemilik web bisa pamer nama.

<details>
<summary>💡 Hint</summary>
Manusia lebih mudah mengingat kata daripada urutan angka yang panjang.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mengubah angka menjadi kata.**
Nama domain adalah abstraksi dari alamat numerik server internet.
</details>

### Soal #23: Petunjuk Arah "Belok Kanan"
Temanmu memberi petunjuk: "Nanti di depan ada minimarket, kamu belok kanan". Apa detail yang **DIABSTRAKSI** oleh temanmu?
A. Nama jalan setelah belokan.
B. Derajat kemiringan belokan (misal $92.4^\circ$).
C. Warna cat gedung minimarketnya.
D. Bahwa kamu harus belok.

<details>
<summary>💡 Hint</summary>
Mana yang terlalu teknis/presisi sehingga biasanya tidak digunakan dalam percakapan sehari-hari?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Derajat kemiringan belokan.**
Instruksi "Belok Kanan" sudah cukup mewakili aksi tanpa perlu data geometri yang berlebihan.
</details>

### Soal #24: Mode "Hemat Baterai" di HP
Saat mode ini aktif, HP menurunkan kecerahan dan mematikan aplikasi latar belakang. Kamu tidak perlu memilih satu per satu mana yang mati. Ini adalah contoh...
A. Kerusakan layar.
B. Abstraksi sekumpulan instruksi optimasi menjadi satu tombol pengaturan.
C. HP sedang lelah.
D. Efek samping penggunaan internet yang terlalu lama.

<details>
<summary>💡 Hint</summary>
Satu aksi (Klik Mode Hemat) memicu banyak sub-aksi di sistem.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi sekumpulan instruksi.**
Software menyembunyikan detail teknis penghematan daya dari pengguna.
</details>

### Soal #25: Struktur Organisasi Kelas
Nama "Ketua Kelas" mengabstraksi...
A. Hobi dan nilai ulangannya.
B. Peran dan tanggung jawab seseorang dalam memimpin kelas, siapapun orangnya.
C. Bahwa dia paling pintar di kelas.
D. Bahwa dia tidak perlu belajar.

<details>
<summary>💡 Hint</summary>
"Ketua Kelas" adalah jabatan (posisi), detail pribadi orangnya tidak mengubah peran tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Peran dan tanggung jawab.**
Jabatan adalah bentuk abstraksi dari fungsi sosial seseorang dalam kelompok.
</details>

### Soal #26: Abstraksi dalam Game Catur
Di komputer, bidak "Kuda" digambarkan seperti kepala kuda. Padahal aslinya itu hanyalah variabel data yang memiliki aturan gerak pola L. Visual kepala kuda itu bertujuan untuk...
A. Membuat game terlihat lebih mahal.
B. Mempermudah pemain mengenali peran dan aturan gerak bidak tersebut secara cepat (abstraksi konseptual).
C. Biar mirip dengan catur kayu asli.
D. Menghibur anak-anak.

<details>
<summary>💡 Hint</summary>
Gambar membantu otak menghubungkan objek dengan fungsinya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mempermudah mengenali peran.**
Desain grafis dalam game seringkali merupakan abstraksi dari logika matematika di belakangnya.
</details>

### Soal #27: Pemodelan Rute Kereta Api
Diagram rute KRL/MRT menunjukkan stasiun sebagai titik dan jalur sebagai garis lurus, bukan belokan asli relnya. Mengapa ini cara yang benar?
A. Biar murah biaya cetaknya.
B. Karena bagi penumpang, urutan stasiun lebih penting daripada kelokan geografis yang akurat.
C. Karena rel kereta memang lurus semua.
D. Supaya penumpang tidak pusing melihat peta.

<details>
<summary>💡 Hint</summary>
Detail geografis dibuang agar pola konektivitas terlihat jelas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Urutan stasiun lebih penting.**
Ini adalah "Peta Topologis", sebuah abstraksi geografi yang legendaris kemudahannya.
</details>

### Soal #28: Instruksi "Klik Kanan"
Saat kamu diperintah "Klik Kanan pada file itu", apa yang diabstraksi?
A. Koordinat presisi kursor ($x,y$) di layar saat kamu menekan tombol mouse.
B. Arah kamu memegang mouse.
C. Kecepatan jarimu saat menekan.
D. Warna casing mousenya.

<details>
<summary>💡 Hint</summary>
Komputer butuh data $X,Y$ untuk tahu mana yang diklik, tapi manusia cukup tahu "Di atas file".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Koordinat presisi kursor.**
Antarmuka visual mengabstraksi data spasial menjadi interaksi objek.
</details>

### Soal #29: Daftar Menu di Restoran
Menu menampilkan gambar makanan dan harga. Detail apa yang **DIABSTRAKSI**?
A. Harga per porsi.
B. Nama masakannya.
C. Stok bahan mentah di gudang dan gaji koki yang memasaknya.
D. Foto makanannya.

<details>
<summary>💡 Hint</summary>
Konsumen hanya butuh informasi untuk memilih, bukan laporan keuangan restoran.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Stok bahan dan gaji koki.**
Informasi operasional dapur diabstraksi melalui lembar menu.
</details>

### Soal #30: Abstraksi pada Remot TV
Hampir semua remot TV punya tombol angka 0-9. Apa kegunaannya secara abstrak?
A. Biar kita bisa belajar matematika sambil nonton.
B. Mengabstraksi pemilihan frekuensi siaran yang rumit menjadi nomor saluran yang sederhana.
C. Biar remotnya terlihat penuh tombol.
D. Karena jumlah jari manusia ada sepuluh.

<details>
<summary>💡 Hint</summary>
Frekuensi gelombang elektromagnetik sangat sulit dihafal, angka 1, 2, 3... sangat mudah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengabstraksi pemilihan frekuensi.**
Nomor saluran adalah label abstrak untuk rentang frekuensi frekuensi TV.
</details>

### Soal #31: Deskripsi Warna "#FF0000"
Dalam desain web, warna MERAH direpresentasikan dengan kode `#FF0000`. Bagi manusia, kita cukup bilang "Merah". Manakah pernyataan yang benar?
A. "Merah" adalah abstraksi bahasa untuk kode teknis warna tersebut.
B. Kode `#FF0000` lebih mudah diucapkan daripada kata "Merah".
C. Desainer tidak boleh memakai kata "Merah".
D. Komputer sebenarnya suka warna biru.

<details>
<summary>💡 Hint</summary>
Bahasa manusia menyederhanakan spektrum warna yang kompleks.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. "Merah" adalah abstraksi bahasa.**
Kata-kata adalah label abstrak untuk konsep yang lebih teknis atau fisik.
</details>

### Soal #32: Simulasi Penerbangan (Flight Sim)
Pilot belajar menggunakan simulasi. Di simulasi, tekanan udara dan getaran dibuat semirip mungkin lewat software. Simulasi itu sendiri adalah...
A. Game biasa.
B. Abstraksi dari pengalaman terbang asli yang dirancang untuk fokus pada pelatihan kendali.
C. Hal yang membuang waktu.
D. Cara agar maskapai tidak perlu beli bensin.

<details>
<summary>💡 Hint</summary>
Abstraksi digunakan untuk menciptakan lingkungan tiruan yang aman tapi representatif.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi dari pengalaman asli.**
Simulasi menyaring risiko bahaya tapi mempertahankan pola kontrol pesawat yang inti.
</details>

### Soal #33: Abstraksi pada Uang Kertas
Uang kertas Rp100.000 hanyalah selembar kertas, tapi kita bisa menukarnya dengan banyak barang. Kertas ini mengabstraksi...
A. Pohon yang ditebang untuk buat kertasnya.
B. Nilai ekonomi dan daya beli yang dijamin oleh negara.
C. Gambar pahlawan yang ada di situ.
D. Dompet tempat penyimpanannya.

<details>
<summary>💡 Hint</summary>
Benda fisik (kertas) mewakili konsep abstrak (kekayaan/nilai).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Nilai ekonomi dan daya beli.**
Uang adalah salah satu bentuk abstraksi paling kuat dalam peradaban manusia.
</details>

### Soal #34: Pengisian Formulir Biodata
Nama, Alamat, tgl lahir. Di bagian "Alamat", kamu tidak perlu menulis titik koordinat lintang dan bujur rumahmu. Mengapa?
A. Karena alamat kata-kata lebih mudah diverifikasi oleh manusia.
B. Karena GPS itu rahasia.
C. Karena formulirnya kekecilan.
D. Karena robot tidak bisa membaca alamat.

<details>
<summary>💡 Hint</summary>
Alamat (Jalan - Nomor - Kota) adalah sistem abstraksi lokasi yang intuitif bagi manusia.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Alamat kata-kata lebih mudah.**
Sistem penamaan alamat adalah cara kita mengabstraksi lokasi di permukaan bumi.
</details>

### Soal #35: Ikon Baterai di HP
Ikon baterai menunjukkan warna hijau penuh. Apa yang **DIABSTRAKSI** di sini?
A. Bahan kimia Lithium di dalam baterai.
B. Tegangan voltase listrik yang tersisa secara akurat (misal 3.82V).
C. Merk pabrik baterainya.
D. Berat HP-mu saat baterai penuh.

<details>
<summary>💡 Hint</summary>
Indikator visual menyederhanakan data sensor menjadi status yang mudah dipahami.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tegangan voltase listrik.**
Angka voltase yang naik turun diabstraksi menjadi persentase 0-100% atau bar warna.
</details>

### Soal #36: Model Atom (Kimia)
Gambar atom dengan bola kecil di tengah dan garis melingkar elektron. Model ini mengabstraksi...
A. Kenyataannya bahwa posisi elektron sebenarnya berupa "awan probabilitas" yang sangat rumit.
B. Nama ilmuwan yang menemukannya.
C. Berapa harga emas di pasar.
D. Aroma dari atom tersebut.

<details>
<summary>💡 Hint</summary>
Model atom sekolah dibuat sederhana agar mudah dibayangkan pola reaksinya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menyederhanakan pola awan probabilitas.**
Model Bohr adalah bentuk abstraksi ilmiah untuk tujuan pembelajaran dasar.
</details>

### Soal #37: Penggunaan Alat Musik "Keyboard" (Organ)
Kamu menekan tuts "C", suara piano keluar. Padahal itu adalah file suara digital yang diputar. Apa yang diabstraksi dari pemain?
A. Nama lagu yang dimainkan.
B. Proses pemrosesan data digital (Sampling) di dalam chip sirkuit keyboard.
C. Berapa jumlah tombol hitamnya.
D. Bagaimana cara memainkannya.

<details>
<summary>💡 Hint</summary>
Interface tuts piano mengabstraksi teknologi synthesizer di dalamnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pemrosesan data digital.**
Pemain musik hanya fokus pada pola nada, bukan pola aliran data di prosesor.
</details>

### Soal #38: Abstraksi pada Jam Dinding
Jam analog yang berdetak menunjukkan waktu. Apa yang **DIABSTRAKSI**?
A. Rotasi bumi terhadap matahari di luar angkasa.
B. Warna jarum jamnya.
C. Berapa harga baterai jam itu.
D. Siapa yang menggantung jam itu.

<details>
<summary>💡 Hint</summary>
Jam adalah alat yang mengabstraksi fenomena astronomi menjadi durasi 12 atau 24 jam.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Rotasi bumi terhadap matahari.**
Satuan detik, menit, dan jam adalah abstraksi manusia untuk mengukur waktu.
</details>

### Soal #39: Deskripsi "Bebek" untuk AI
Jika kamu diminta menjelaskan "Bebek" ke komputer agar ia bisa mengenalinya, manakah detail yang merupakan **Abstraksi Kunci**?
A. "Punya sayap, paruh datar, suka berenang, bunyi kwek-kwek."
B. "Suka makan nasi sisa di warung pojok hari Selasa."
C. "Bisa lari kalau dikejar anak kecil berbaju merah."
D. "Matanya berwarna hitam mengkilap di bawah sinar lampu."

<details>
<summary>💡 Hint</summary>
Pilih karakteristik umum yang selalu ada pada semua bebek (Generalisasi).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Sayap, paruh, berenang, kwek-kwek.**
Ciri-ciri ini adalah pola esensial untuk memodelkan objek bebek secara abstrak.
</details>

### Soal #40: Abstraksi di Video Call
Kamu melihat wajah temanmu di layar. Apa yang **DIABSTRAKSI** oleh aplikasi (seperti WhatsApp/Zoom) dari pandanganmu?
A. Kecepatan internet yang naik turun.
B. Proses kompresi video, pengubahan cahaya jadi sinyal digital, dan transmisi lewat kabel bawah laut.
C. Nama teman yang diajak bicara.
D. Topik percakapan kalian.

<details>
<summary>💡 Hint</summary>
Teknologi bekerja keras di latar belakang agar kamu bisa merasakan pengalaman yang mulus.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Proses kompresi dan transmisi.**
Aplikasi menyembunyikan kerumitan jaringan global agar kamu fokus pada komunikasi.
</details>

### Soal #41: Struktur File Folder
Kamu memasukkan file foto ke folder "Liburan". Secara fisik di harddisk, data itu tersebar di berbagai piringan magnetik. Folder tersebut adalah...
A. Tempat sampah rahasia.
B. Abstraksi logika untuk memudahkan manusia mengorganisir data secara tematis.
C. Hal yang memperlambat komputer.
D. Gambar yang tidak berguna.

<details>
<summary>💡 Hint</summary>
Sistem file mengabstraksi lokasi penyimpanan fisik menjadi struktur pohon yang rapi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Abstraksi logika organisasi data.**
Manusia lebih mudah mengelola "Folder" daripada "Sektor Harddisk Nomor 902".
</details>

### Soal #42: Tombol "Like" di Media Sosial
Kamu mengklik gambar hati, dan angka jumlah like bertambah 1. Apa yang diabstraksi?
A. Perasaan senang orang yang mengirim like.
B. Proses pengiriman request ke database server, pembaruan angka, dan notifikasi ke HP pemilik postingan.
C. Bahwa kamu menyukai fotonya.
D. Biar internet makin ramai.

<details>
<summary>💡 Hint</summary>
Satu klik sederhana memicu sinkronisasi data global di server perusahaan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Proses request server dan pembaruan data.**
Interaksi sederhana (klik) menyembunyikan alur kerja backend yang sibuk.
</details>

### Soal #43: Ikon Gembok di Alamat Web (HTTPS)
Saat melihat gembok hijau di pojok browser, kamu merasa aman. Apa yang diabstraksi?
A. Kunci fisik gembok itu disimpan di kantor Google.
B. Protokol enkripsi SSL/TLS, pertukaran kunci rahasia, dan verifikasi sertifikat digital yang sangat rumit.
C. Bahwa website itu tidak akan pernah tutup.
D. Bahwa webnya bagus desainnya.

<details>
<summary>💡 Hint</summary>
Keamanan digital adalah matematika yang sangat rumit, ikon gembok adalah hasil abstraksinya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Protokol enkripsi SSL/TLS.**
Visual sederhana (Gembok) mengomunikasikan status keamanan yang kompleks kepada pengguna.
</details>

### Soal #44: Penggunaan Google Search
Kamu mengetik "Cara buat nasi goreng". Hasilnya keluar dalam 0.5 detik. Apa yang **DIABSTRAKSI**?
A. Bahwa Google punya banyak komputer.
B. Proses *crawling* jutaan web, pengindeksan data, dan algoritma *ranking* untuk mencari hasil paling relevan.
C. Tulisan yang kamu ketik di kotak pencarian.
D. Jumlah total orang yang mencari hal yang sama.

<details>
<summary>💡 Hint</summary>
Kamu hanya melihat "Kotak Input" dan "Halaman Hasil", bukan mesin pencarinya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Proses crawling, indexing, dan ranking.**
Layanan web mengabstraksi mesin raksasa di belakangnya menjadi satu halaman sederhana.
</details>

### Soal #45: Deskripsi "Sahabat"
Budi berkata: "Andi adalah sahabatku". Kata "Sahabat" mengabstraksi...
A. Nama asli Andi.
B. Jutaan kenangan, kesetiaan, dan interaksi emosional dalam satu label hubungan.
C. Bahwa Andi punya uang banyak.
D. Tanggal lahir Andi.

<details>
<summary>💡 Hint</summary>
Satu kata bisa mewakili konsep hubungan yang sangat dalam dan luas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jutaan kenangan dan interaksi emosional.**
Bahasa sosial adalah bentuk abstraksi perilaku manusia.
</details>

### Soal #46: Penggunaan Mikroskop
Kamu melihat bakteri lewat mikroskop. Mikroskop membantu kamu melakukan...
A. Abstraksi detail: mengabaikan lingkungan sekitar yang lebar dan fokus pada benda yang sangat kecil.
B. Melakukan perbaikan pada mata yang rusak.
C. Membuat bakteri jadi lebih besar ukurannya secara fisik.
D. Mengambil foto bakteri untuk Instagram.

<details>
<summary>💡 Hint</summary>
Alat bantu visual membantu kita melakukan "Penyaringan" (Zoom In) pada detail tertentu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Fokus pada detail kecil.**
Penyempitan fokus (Zooming) adalah teknik abstraksi spasial.
</details>

### Soal #47: Abstraksi pada Robot Vacuum (Penyedot Debu Otomatis)
Kamu hanya menekan "Start". Robot jalan sendiri, menghindari kaki meja, dan kembali ke tempat cas. Apa yang diabstraksi dari kamu?
A. Suara bising mesin penyedotnya.
B. Algoritma pemetaan ruangan, deteksi sensor tabrakan, dan manajemen daya baterai.
C. Bahwa rumahmu kotor.
D. Jalur yang dilalui robot di lantai.

<details>
<summary>💡 Hint</summary>
Otomasi adalah puncak dari abstraksi tugas manusia (menyapu) menjadi tugas mesin.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Algoritma pemetaan dan sensor.**
Robotika menggunakan abstraksi tingkat tinggi agar mesin bisa mandiri.
</details>

### Soal #48: Peringatan "Sisa Kuota Internet 1GB"
Provider mengirim SMS: "Sisa kuota anda 1GB". Apa yang diabstraksi?
A. Kecepatan download saat ini.
B. Perhitungan jutaan byte data yang telah kamu gunakan untuk buka video, chat, dan game.
C. Nama aplikasi yang paling sering dibuka.
D. Berapa lama lagi 1GB itu akan habis.

<details>
<summary>💡 Hint</summary>
Total penggunaan data diabstraksi menjadi angka bulat (1GB).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perhitungan jutaan byte data.**
Penyajian informasi ringkas memudahkan pengguna mengontrol konsumsi datanya.
</details>

### Soal #49: Abstraksi pada Kode Warna Rambut
Di salon ada pilihan: "Hitam Alami, Coklat Kopi, Merah Berani". Nama-nama ini mengabstraksi...
A. Perasaan orang yang mengecat rambut.
B. Campuran senyawa kimia peroksida dan pigmen dengan dosis tertentu di dalam cat rambut tersebut.
C. Nama salonnya.
D. Harga satu kotak cat rambut.

<details>
<summary>💡 Hint</summary>
Label kreatif (Coklat Kopi) lebih mudah dipilih pelanggan daripada formula kimia.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Campuran senyawa kimia.**
Penamaan produk menggunakan abstraksi untuk meningkatkan daya tarik dan kemudahan pilihan.
</details>

### Soal #50: Abstraksi Soal Matematika (Geometri)
"Ada sebuah kolam berbentuk lingkaran dengan jari-jari 7 meter. Di pinggirnya dipasangi pagar."
Inti masalah (model abstrak) untuk menghitung panjang pagar adalah...
A. Mencari Keliling Lingkaran ($2 \times \pi \times r$).
B. Mencari Luas Lingkaran ($\pi \times r^2$).
C. Mencari volume air di kolam.
D. Mencari harga pagar per meter.

<details>
<summary>💡 Hint</summary>
Pagar berada di sekeliling pinggir kolam.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mencari Keliling Lingkaran.**
Dekomposisi deskripsi benda (kolam/pagar) menjadi rumus geometri adalah langkah abstraksi matematis.
</details>

