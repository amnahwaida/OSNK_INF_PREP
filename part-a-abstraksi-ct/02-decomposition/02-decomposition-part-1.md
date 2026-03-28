🔙 **Kembali ke Materi:** [Materi 02 Decomposition](../02-decomposition.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 02. Decomposition - Bagian 1 (Soal 1-50)

[🏠 Indeks](../02-decomposition.md) | [Bagian 2 (51-100) >](02-decomposition-part-2.md)

---
### Soal #01: Analisis Tugas
Sekolahmu akan mengadakan acara pentas seni (Pensi). Kamu ditunjuk sebagai ketua panitia. 
Manakah di bawah ini yang merupakan contoh dekomposisi tugas yang paling efektif?
A. Memerintahkan semua orang untuk bekerja di hari H.
B. Membagi panitia menjadi divisi: Konsumsi, Dokumentasi, Acara, dan Perlengkapan.
C. Mengerjakan semua tugas sendirian agar hasilnya sempurna.
D. Berdoa agar acara berjalan lancar tanpa rencana.

<details>
<summary>💡 Hint</summary>
Pikirkan tentang pembagian peran dan tanggung jawab yang spesifik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membagi panitia menjadi divisi.**
Dengan membagi menjadi divisi-divisi kecil (Konsumsi, Dokumentasi, dll), masalah besar "Mengadakan Pensi" menjadi lebih terorganisir dan mudah dikelola.
</details>

### Soal #02: Dekomposisi pada Robot
Sebuah robot diminta untuk: "Pergi ke toko, beli roti, dan kembali ke rumah."
Jika kita melakukan dekomposisi pada perintah tersebut, langkah manakah yang **TIDAK** termasuk dalam sub-masalah "Beli Roti"?
A. Mencari rak roti di dalam toko.
B. Memilih jenis roti yang diinginkan.
C. Menghitung uang kembalian di kasir.
D. Memastikan pintu rumah sudah terkunci sebelum berangkat.

<details>
<summary>💡 Hint</summary>
Fokus hanya pada proses transaksi/kegiatan di dalam toko roti.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Memastikan pintu rumah terkunci.**
Langkah ini adalah bagian dari persiapan "Berangkat", bukan bagian dari sub-masalah "Beli Roti".
</details>

### Soal #03: Manfaat Tersembunyi
Kenapa dekomposisi sangat membantu saat kita sedang menulis kode program (coding)?
A. Agar kode program menjadi lebih panjang dan terlihat keren.
B. Agar kita bisa menemukan letak kesalahan (bug) dengan lebih cepat pada bagian tertentu.
C. Agar komputer bekerja lebih cepat saat menjalankan program.
D. Agar kita tidak perlu belajar pilar CT yang lainnya.

<details>
<summary>💡 Hint</summary>
Ingat poin tentang "Ease of Debugging".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Agar kita bisa menemukan letak kesalahan (bug) dengan lebih cepat.**
Jika program error di bagian "Simpan Data", kita cukup mengecek modul database saja tanpa perlu mengecek modul lainnya.
</details>

### Soal #04: Kasus OSN-K
Diberikan soal: "Berapa banyak angka antara 1-100 yang habis dibagi 3 tetapi tidak habis dibagi 5?"
Langkah dekomposisi pertama yang paling tepat adalah...
1. Mencari angka yang habis dibagi 3 dari 1-100.
2. Mencari angka yang habis dibagi 5 dari hasil langkah 1.
3. Mencari angka yang habis dibagi 15.

Strategi yang benar dalam memecah masalah ini adalah...
A. Hanya langkah 1.
B. Langkah 1 dikurangi hasil langkah 3.
C. Menjumlahkan langkah 1 and langkah 2.
D. Mencari rata-rata antara langkah 1 dan 2.

<details>
<summary>💡 Hint</summary>
Gunakan konsep Diagram Venn: (Habis dibagi 3) - (Habis dibagi 3 DAN 5).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Langkah 1 dikurangi hasil langkah 3.**
Langkah 1 (Habis dibagi 3) adalah masalah utama, lalu kita "membuang" bagian yang tidak diinginkan (habis dibagi 5, yang berarti kelipatan 15).
</details>

### Soal #05: Perencanaan Studi Wisata
Dalam merencanakan studi wisata sekolah ke Museum Nasional, panitia membagi tugas besar menjadi beberapa sub-tugas. Manakah di bawah ini yang merupakan dekomposisi yang tepat untuk sub-tugas **"Transportasi"**?
A. Memesan bus, menentukan rute perjalanan, dan mengumpulkan biaya bensin.
B. Membeli tiket masuk museum dan memesan pemandu wisata.
C. Menyiapkan kotak P3K dan daftar nama peserta.
D. Mendata menu makan siang untuk siswa dan guru.

<details>
<summary>💡 Hint</summary>
Fokus pada segala hal yang berkaitan dengan "perjalanan/kendaraan".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Memesan bus, menentukan rute, dan biaya bensin.**
Ketiga hal tersebut adalah komponen penyusun dari masalah besar "Transportasi".
</details>

### Soal #06: Teka-Teki Koin Berat
Anda memiliki 9 koin yang terlihat identik, namun salah satunya sedikit lebih berat. Anda memiliki timbangan neraca (dua lengan). Strategi pertama dalam CT (Dekomposisi) untuk mencari koin berat tersebut dengan langkah minimal adalah...
A. Menimbang koin satu per satu (koin 1 vs koin 2, koin 2 vs koin 3, dst).
B. Membagi 9 koin menjadi 3 grup yang masing-masing berisi 3 koin.
C. Membagi 9 koin menjadi 2 grup (4 koin dan 5 koin).
D. Langsung menebak koin mana yang paling berat.

<details>
<summary>💡 Hint</summary>
Dekomposisi yang efisien seringkali membagi masalah menjadi bagian-bagian yang seimbang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membagi menjadi 3 grup berisi 3 koin.**
Ini adalah langkah awal algoritma *Divide and Conquer*. Dengan menimbang dua grup berisi 3 koin, kita bisa tahu di grup mana koin berat berada (hanya dalam 1 kali timbang).
</details>

### Soal #07: Pembuatan Aplikasi Kalkulator
Jika Anda diminta membuat program kalkulator scientific, proses dekomposisi mana yang paling masuk akal untuk fungsi **"Operasi Matematika Dasar"**?
A. Membuat fungsi terpisah untuk Penjumlahan, Pengurangan, Perkalian, dan Pembagian.
B. Membuat satu fungsi raksasa yang berisi ribuan baris kode untuk semua hitungan.
C. Fokus pada desain warna tombol kalkulator terlebih dahulu.
D. Menunggu instruksi lebih lanjut dari guru tanpa menulis kode.

<details>
<summary>💡 Hint</summary>
Ingat: "Setiap bagian kecil harus bisa berdiri sendiri dan mudah diuji."
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Membuat fungsi terpisah (Tambah, Kurang, Kali, Bagi).**
Memecah operasi besar menjadi fungsi-fungsi kecil membuat kode lebih rapi, mudah diperbaiki, dan bisa digunakan kembali.
</details>

### Soal #08: Membuat Sandwich
Kamu ingin membuat sandwich lapis tiga yang sempurna. Langkah dekomposisi mana yang paling tepat untuk sub-masalah **"Persiapan Bahan"**?
A. Menyiapkan roti, mentega, keju, dan selada di atas meja.
B. Memakan sandwich setelah selesai dibuat.
C. Membersihkan piring setelah makan.
D. Membeli sandwich di toko terdekat.

<details>
<summary>💡 Hint</summary>
Pikirkan tahap sebelum perakitan dilakukan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menyiapkan roti, mentega, keju, dan selada.**
Menyiapkan bahan adalah komponen awal sebelum proses pembuatan sandwich dimulai.
</details>

### Soal #09: Menulis Makalah Penelitian
Seorang siswa SMA diminta menulis makalah tentang pemanasan global. Dekomposisi tugas yang benar adalah...
A. Menulis langsung dari bab 1 sampai selesai dalam satu jam.
B. Membagi tugas menjadi: Riset data, Membuat Outline, Menulis Draft, dan Revisi.
C. Membaca makalah orang lain dan menyalinnya.
D. Menunggu ide muncul sendiri tanpa melakukan riset.

<details>
<summary>💡 Hint</summary>
Proses menulis ilmiah membutuhkan tahapan yang sistematis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Riset, Outline, Menulis Draft, dan Revisi.**
Membagi penulisan menjadi fase-fase tersebut membuat prosesnya lebih teratur dan berkualitas.
</details>

### Soal #10: Pengembangan Aplikasi Sekolah
Tim IT sekolah ingin membuat aplikasi "E-Kantin". Manakah sub-masalah yang merupakan bagian dari **"Sistem Pembayaran"**?
A. Menampilkan menu makanan hari ini.
B. Mengintegrasikan saldo kartu siswa dengan transaksi kantin.
C. Desain logo aplikasi yang menarik.
D. Menghitung jumlah kalori dalam setiap makanan.

<details>
<summary>💡 Hint</summary>
Fokus pada aspek pertukaran nilai/uang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Integrasi saldo dengan transaksi.**
Saldo dan transaksi adalah bagian inti dari sub-masalah pembayaran.
</details>

### Soal #11: Panitia Upacara 17 Agustus
Sebagai panitia upacara, kamu membagi tugas menjadi Seksi Upacara, Seksi Perlengkapan, dan Seksi Konsumsi. Manakah tugas yang masuk dalam **Seksi Perlengkapan**?
A. Menentukan petugas pengibar bendera.
B. Menyiapkan sound system, tiang bendera, dan podium.
C. Membeli nasi kotak untuk peserta upacara.
D. Mengatur barisan siswa di lapangan.

<details>
<summary>💡 Hint</summary>
Fokus pada alat dan benda fisik yang dibutuhkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sound system, tiang bendera, dan podium.**
Benda-benda fisik pendukung upacara adalah tanggung jawab seksi perlengkapan.
</details>

### Soal #12: Melacak Bug (Debugging)
Program kalkulatormu error saat melakukan pembagian dengan angka nol. Dekomposisi pengecekan yang harus kamu lakukan adalah...
A. Mengecek seluruh ribuan baris kode dari awal.
B. Fokus mengecek fungsi `pembagian()` dan menambahkan validasi input.
C. Menghapus seluruh program dan membuat baru.
D. Mengganti warna latar belakang aplikasi agar terlihat lebih bagus.

<details>
<summary>💡 Hint</summary>
Gunakan dekomposisi untuk mengisolasi lokasi kesalahan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fokus mengecek fungsi pembagian().**
Isolasi masalah pada bagian yang relevan adalah manfaat utama dekomposisi dalam coding.
</details>

### Soal #13: Desain Sistem Perpustakaan
Dalam merancang sistem manajemen perpustakaan digital, manakah dekomposisi yang tepat untuk fitur **"Manajemen Anggota"**?
A. Pendaftaran anggota baru, pembaruan data, dan penghapusan akun.
B. Pencarian judul buku berdasarkan kategori.
C. Menghitung denda keterlambatan buku.
D. Menampilkan riwayat peminjaman buku.

<details>
<summary>💡 Hint</summary>
Pikirkan segala hal yang berkaitan dengan identitas pengguna.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pendaftaran, pembaruan data, dan penghapusan akun.**
Ketiga hal tersebut mengelola siklus hidup data anggota.
</details>

### Soal #14: Menghitung Luas Bangun Kompleks
Kamu diminta menghitung luas sebuah bangun datar berbentuk "L". Dekomposisi matematika yang paling mudah adalah...
A. Mengukur keliling bangun tersebut.
B. Membagi bangun "L" menjadi dua buah persegi panjang yang lebih kecil.
C. Menebak luasnya berdasarkan perasaan.
D. Mencari rumus luas bangun "L" di buku yang mungkin tidak ada.

<details>
<summary>💡 Hint</summary>
Pecah bangun asing menjadi bangun yang kamu sudah tahu rumusnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membagi menjadi dua persegi panjang.**
Ini adalah penerapan dekomposisi dalam geometri untuk memudahkan perhitungan.
</details>

### Soal #15: Manajemen Restoran
Manajer restoran membagi tim menjadi "Front of House" (Pelayanan) dan "Back of House" (Dapur). Manakah tugas **Back of House**?
A. Menyambut tamu di pintu depan.
B. Mencuci piring dan memasak pesanan makanan.
C. Menyajikan minuman ke meja pelanggan.
D. Mengantarkan tagihan pembayaran.

<details>
<summary>💡 Hint</summary>
Fokus pada kegiatan di area produksi makanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencuci piring dan memasak.**
Aktivitas produksi dan kebersihan area belakang adalah tugas tim dapur.
</details>

### Soal #16: Robot Penyilah Sampah
Sebuah robot diprogram untuk memilah sampah menjadi: Organik, Plastik, dan Kertas. Manakah sub-masalah dari fase **"Identifikasi Sampah"**?
A. Menggerakkan lengan robot ke tempat sampah plastik.
B. Mendeteksi tekstur dan material benda menggunakan sensor.
C. Membuang sampah ke laut.
D. Menghitung total berat sampah yang sudah dipilah.

<details>
<summary>💡 Hint</summary>
Identifikasi berarti "mengenali" sebelum melakukan aksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mendeteksi tekstur dan material menggunakan sensor.**
Sensor membantu robot mengidentifikasi jenis sampah sebelum dipindahkan.
</details>

### Soal #17: Membangun Rumah Pohon
Dekomposisi langkah pembangunan rumah pohon yang paling logis adalah...
A. Mengecat dinding dulu, lalu mencari pohon yang kuat.
B. Mencari pohon kuat, membuat lantai dasar, membangun dinding, lalu atap.
C. Membeli sofa empuk untuk di dalam rumah pohon.
D. Mengajak teman untuk bermain di pohon yang belum ada rumahnya.

<details>
<summary>💡 Hint</summary>
Urutan logis (Algorithm Design) seringkali dimulai dari dekomposisi struktur yang benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pohon kuat -> Lantai -> Dinding -> Atap.**
Ini adalah dekomposisi struktur fisik bangunan dari bawah ke atas.
</details>

### Soal #18: Puzzle 1000 Keping
Strategi dekomposisi yang biasa digunakan untuk menyelesaikan puzzle raksasa adalah...
A. Mencoba memasangkan dua keping secara acak sampai ketemu.
B. Memilah kepingan berdasarkan warna atau mencari kepingan bagian pinggir (frame).
C. Melihat gambar di kotak puzzle saja tanpa menyusunnya.
D. Langsung menempelkan semua kepingan dengan lem.

<details>
<summary>💡 Hint</summary>
Cari bagian yang paling mudah diidentifikasi atau kelompokkan berdasarkan ciri tertentu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memilah berdasarkan warna atau Frame.**
Mengelompokkan kepingan adalah dekomposisi masalah besar menjadi grup-grup kecil yang lebih mudah dicari pasangannya.
</details>

### Soal #19: Turnamen Olahraga Sekolah
Panitia OSIS membagi turnamen futsal menjadi: Registrasi, Jadwal Pertandingan, dan Logistik Pertandingan. Manakah tugas **Logistik Pertandingan**?
A. Menyiapkan bola, gawang, peluit wasit, dan rompi pemain.
B. Mencatat skor akhir pertandingan di papan skor.
C. Menerima uang pendaftaran dari tiap kelas.
D. Menentukan siapa yang melawan siapa di babak final.

<details>
<summary>💡 Hint</summary>
Logistik berhubungan dengan kebutuhan barang dan peralatan operasional.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bola, gawang, peluit, dan rompi.**
Peralatan fisik untuk kelancaran pertandingan adalah bagian dari logistik.
</details>

### Soal #20: Membuat Video YouTube
Seorang YouTuber melakukan dekomposisi proses pembuatan konten. Manakah yang termasuk dalam sub-masalah **"Post-Production"**?
A. Menulis skrip dan ide konten.
B. Merekam video menggunakan kamera dan mikrofon.
C. Melakukan editing, menambahkan musik, dan color grading.
D. Membagikan link video ke media sosial.

<details>
<summary>💡 Hint</summary>
Post-production berarti proses "setelah" rekaman selesai.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Editing, musik, dan color grading.**
Semua kegiatan pengolahan hasil rekaman masuk kedaam post-production.
</details>

### Soal #21: Analisis Kalimat Kompleks
Dalam pelajaran Bahasa Indonesia, kamu diminta menganalisis kalimat: "Budi memakan roti yang dibelikan ibunya saat mereka pergi ke pasar kemarin." 
Dekomposisi kalimat ini untuk memahami strukturnya adalah...
A. Mencari antonim dari kata "makan".
B. Memecah kalimat menjadi: Induk kalimat (Budi makan roti) dan anak kalimat (yang dibelikan ibunya...).
C. Membaca kalimat tersebut berulang-ulang dengan suara keras.
D. Menghitung jumlah huruf vokal dalam kalimat tersebut.

<details>
<summary>💡 Hint</summary>
Memecah kalimat menjadi struktur subjek, predikat, objek, dan keterangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memecah menjadi Induk dan Anak kalimat.**
Dekomposisi linguistik membantu memahami hubungan antar bagian dalam kalimat kompleks.
</details>

### Soal #22: Masalah Koneksi Internet
Internet di rumahmu tiba-tiba mati. Dekomposisi pengecekan yang sistematis adalah...
A. Langsung menelepon penyedia layanan internet (ISP) untuk marah-marah.
B. Cek lampu indikator modem, cek kabel LAN/Wi-Fi, lalu cek perangkat lain (HP/Laptop).
C. Membeli router baru yang lebih mahal.
D. Mematikan listrik seluruh rumah agar modem ikut mati.

<details>
<summary>💡 Hint</summary>
Cek dari bagian yang paling dekat/mudah dijangkau sebelum ke yang lebih luas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampu modem -> Kabel -> Perangkat lain.**
Isolasi masalah per komponen membantu menemukan penyebab internet mati dengan cepat.
</details>

### Soal #23: Desain Profil Media Sosial
Jika kamu diminta mendesain halaman profil pengguna, dekomposisi elemen visualnya adalah...
A. Mengatur server agar aplikasi tidak lag.
B. Membagi menjadi: Foto profil, Header/Banner, Bio, dan Daftar Postingan.
C. Mencari teman sebanyak-banyaknya di aplikasi tersebut.
D. Menentukan harga langganan premium.

<details>
<summary>💡 Hint</summary>
Fokus pada komponen yang muncul di layar (UI components).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Foto profil, Header, Bio, dan Postingan.**
Ini adalah dekomposisi elemen antarmuka pengguna (UI) pada halaman profil.
</details>

### Soal #24: Perhitungan Anggaran Bulanan
Andi ingin menabung 500rb per bulan. Ia melakukan dekomposisi pengeluaran menjadi: Makan, Transportasi, Hiburan, dan Tabungan. 
Manakah yang merupakan sub-masalah dari **"Evaluasi Pengeluaran"**?
A. Menghitung total biaya makan dalam sebulan.
B. Meminta uang tambahan ke orang tua.
C. Membeli barang bermerek yang sedang diskon.
D. Menuliskan cita-cita masa depan di buku harian.

<details>
<summary>💡 Hint</summary>
Evaluasi berarti meninjau kembali apa yang sudah dikeluarkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menghitung total biaya makan.**
Menghitung pengeluaran per kategori adalah langkah awal dalam mengevaluasi apakah anggaran sudah sesuai target.
</details>

### Soal #25: Acara Donor Darah
Panitia donor darah membagi tugas menjadi: Registrasi, Pemeriksaan Kesehatan, dan Area Donor. Tugas **Pemeriksaan Kesehatan** adalah...
A. Mencatat nama dan alamat pendonor.
B. Mengecek tekanan darah dan kadar hemoglobin.
C. Memberikan susu dan telur setelah donor.
D. Membuang jarum suntik bekas ke tempat sampah medis.

<details>
<summary>💡 Hint</summary>
Fokus pada tahap pengecekan kelayakan pendonor secara medis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengecek tekanan darah dan hemoglobin.**
Ini adalah langkah krusial untuk menentukan apakah seseorang boleh mendonorkan darahnya.
</details>

### Soal #26: Mengurutkan Kartu (Sorting)
Kamu memiliki setumpuk kartu acak dan ingin mengurutkannya dari A sampai K. Langkah dekomposisi pertamamu adalah...
A. Membuang kartu yang gambarnya tidak bagus.
B. Membagi kartu menjadi 4 tumpukan berdasarkan lambangnya (Hati, Sekop, Wajik, Keriting).
C. Mengocok kembali kartu tersebut secara terus-menerus.
D. Memberikan kartu tersebut kepada orang lain untuk diurutkan.

<details>
<summary>💡 Hint</summary>
Membagi masalah besar (52 kartu) menjadi kelompok kecil (13 kartu per lambang).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membagi berdasarkan lambang.**
Mengelompokkan berdasarkan ciri tertentu adalah langkah awal dekomposisi dalam algoritma pengurutan.
</details>

### Soal #27: Analisis Eksperimen Sains
Dalam praktikum biologi tentang pertumbuhan tanaman, dekomposisi pengamatanmu meliputi...
A. Hanya melihat hasil akhirnya setelah satu bulan.
B. Mencatat tinggi batang, jumlah daun, dan warna daun setiap 3 hari sekali.
C. Membeli tanaman plastik agar tidak perlu disiram.
D. Menggambar sketsa tanaman saat kamu merasa bosan.

<details>
<summary>💡 Hint</summary>
Pecah pengamatan menjadi parameter-parameter yang bisa diukur secara rutin.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencatat tinggi batang, jumlah daun, dan warna daun.**
Parameter-parameter tersebut adalah sub-bagian dari data pertumbuhan tanaman yang sedang diteliti.
</details>

### Soal #28: Pesan Antar Makanan (Food Delivery)
Dalam sistem aplikasi pesan antar makanan, dekomposisi manakah yang paling tepat untuk sub-masalah **"Tracking Driver"**?
A. Memilih menu restoran favorit.
B. Mengupdate koordinat GPS driver ke peta di layar pengguna.
C. Menghitung total biaya ongkir.
D. Memberikan rating bintang 5 setelah makanan sampai.

<details>
<summary>💡 Hint</summary>
Fokus pada pemantauan posisi real-time.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengupdate koordinat GPS driver.**
Tracking sangat bergantung pada pertukaran data lokasi antara driver dan aplikasi.
</details>

### Soal #29: Aplikasi Ride-Hailing
Aplikasi ojek online memecah sistemnya menjadi berbagai bagian. Manakah tugas sub-masalah **"Manajemen Tarif"**?
A. Mencari driver terdekat dengan lokasi penjemputan.
B. Menghitung biaya berdasarkan jarak dan lonjakan permintaan (surge price).
C. Mengirim notifikasi "Driver Berangkat" ke HP pengguna.
D. Menyimpan riwayat perjalanan selama satu bulan.

<details>
<summary>💡 Hint</summary>
Pikirkan segala hal yang menentukan berapa rupiah yang harus bayar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghitung biaya berdasarkan jarak dan lonjakan.**
Penentuan tarif adalah inti dari manajemen harga dalam ride-hailing.
</details>

### Soal #30: Proses Checkout E-Commerce
Saat kamu berbelanja online, tahap checkout dibagi menjadi beberapa langkah. Manakah bagian dari dekomposisi **"Verifikasi Pembayaran"**?
A. Memilih jasa pengiriman (JNE, SiCepat, dll).
B. Mengecek apakah dana sudah masuk ke rekening penampung (Escrow).
C. Memasukkan alamat lengkap rumah.
D. Menuliskan catatan untuk penjual.

<details>
<summary>💡 Hint</summary>
Verifikasi berarti "memastikan" transaksi uang telah berhasil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengecek saldo masuk di rekening penampung.**
Verifikasi pembayaran dilakukan sistem untuk memastikan penjual aman untuk mengirim barang.
</details>

### Soal #31: Algoritma Media Sosial
Algoritma "For You Page" memecah penilaian postingan menjadi beberapa metrik. Manakah yang termasuk sub-masalah **"Engagement Rate"**?
A. Jumlah Like, Share, dan rata-rata waktu tonton (watch time).
B. Jam berapa postingan tersebut diunggah.
C. Jenis filter yang digunakan pada video.
D. Berapa banyak sisa baterai di HP penonton.

<details>
<summary>💡 Hint</summary>
Engagement berarti "interaksi" penonton dengan konten.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Like, Share, dan Watch Time.**
Interaksi aktif dan pasif pengguna menentukan seberapa menarik konten tersebut bagi algoritma.
</details>

### Soal #32: Navigasi GPS
Google Maps memecah masalah pencarian rute menjadi beberapa komponen. Manakah dekomposisi tugas untuk **"Deteksi Kemacetan"**?
A. Menampilkan nama-nama gedung di sepanjang jalan.
B. Menganalisis kecepatan rata-rata pengguna lain di jalur yang sama.
C. Menghitung jarak tempuh dalam kilometer.
D. Mengatur suara instruksi belok kiri/kanan.

<details>
<summary>💡 Hint</summary>
Macat dideteksi dari perlambatan pergerakan masif di satu titik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menganalisis kecepatan rata-rata pengguna lain.**
Data anonim dari ribuan pengguna membantu sistem menyimpulkan adanya kemacetan.
</details>

### Soal #33: Smart Home Automation
Dalam sistem lampu pintar (smart lights), manakah sub-masalah dari fase **"Trigger Sensor"**?
A. Menghidupkan saklar secara manual.
B. Mendeteksi gerakan manusia di dalam ruangan untuk menyalakan lampu otomatis.
C. Membayar tagihan listrik di akhir bulan.
D. Mengganti bohlam yang sudah putus.

<details>
<summary>💡 Hint</summary>
Trigger berarti "pemicu" otomatisasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mendeteksi gerakan manusia.**
Sensor gerak bertindak sebagai pemicu (trigger) agar sistem menjalankan instruksi nyala lampu.
</details>

### Soal #34: Sinkronisasi Cloud Storage
Komponen utama dari dekomposisi sistem **"Syncing File"** (seperti Google Drive) adalah...
A. Mengubah nama file menjadi lebih pendek.
B. Mengecek perbedaan versi file antara yang ada di HP dan yang ada di Server.
C. Menghapus semua file lama agar storage tidak penuh.
D. Memilih warna ikon folder yang cantik.

<details>
<summary>💡 Hint</summary>
Sinkronisasi berarti "menyamakan" data di dua tempat berbeda.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengecek perbedaan versi (versioning).**
Hanya file yang berubah yang akan diunggah/diunduh untuk menghemat bandwidth.
</details>

### Soal #35: Platform Video Call
Saat melakukan Zoom, sistem memecah beban kerjanya. Manakah tugas sub-masalah **"Audio Processing"**?
A. Menampilkan wajah peserta di layar utama.
B. Melakukan peredaman bising (noise cancellation) agar suara jernih.
C. Mengelola daftar chat yang masuk.
D. Menghitung durasi rapat yang sudah berjalan.

<details>
<summary>💡 Hint</summary>
Fokus pada pengolahan gelombang suara.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Peredaman bising (Noise Cancellation).**
Fokus pada kejernihan suara adalah bagian krusial dari pemrosesan audio.
</details>

### Soal #36: Dompet Digital (E-Wallet)
Manakah dekomposisi yang tepat untuk fitur **"Riwayat Transaksi"**?
A. Mentransfer uang ke sesama pengguna.
B. Menampilkan daftar pengeluaran dan pemasukan berdasarkan tanggal.
C. Meminta kode OTP saat hendak login.
D. Menemukan merchant terdekat yang mendukung QRIS.

<details>
<summary>💡 Hint</summary>
Riwayat berarti "catatan masa lalu".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Daftar pengeluaran dan pemasukan per tanggal.**
Menampilkan data historis adalah fungsi utama dari riwayat transaksi.
</details>

### Soal #37: Tingkat Kesulitan Game
Seorang pembuat game memecah masalah "Game Difficulty". Manakah yang masuk sub-masalah **"AI Behavior Expansion"**?
A. Meningkatkan jumlah HP (nyawa) musuh.
B. Membuat musuh bisa melakukan taktik mengepung pemain di level sulit.
C. Memperindah grafis pemandangan pohon.
D. Memberikan diskon pembelian item di toko game.

<details>
<summary>💡 Hint</summary>
Behavior berarti "perilaku" atau kecerdasan buatan musuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Taktik mengepung pemain.**
Meningkatkan kecerdasan strategi musuh adalah dekomposisi dari tingkat kesulitan yang lebih kompleks.
</details>

### Soal #38: Melukis Mural
Langkah dekomposisi pertama dalam melukis mural di dinding sekolah yang besar adalah...
A. Langsung mewarnai semua bidang dengan cat minyak.
B. Membuat sketsa garis besar (outline) di dinding menggunakan pensil/kapur.
C. Memberikan tanda tangan seniman di pojok bawah.
D. Merobohkan dinding jika gambarnya salah.

<details>
<summary>💡 Hint</summary>
Mulailah dari kerangka dasar sebelum masuk ke detail warna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuat sketsa garis besar (outline).**
Outline adalah dekomposisi visual yang menjadi panduan untuk langkah berikutnya.
</details>

### Soal #39: Mengarang Lagu
Seorang musisi membagi pembuatan lagu menjadi beberapa bagian. Manakah tugas sub-masalah **"Arrangement"**?
A. Menentukan urutan Intro, Verse, Chorus, dan Outro.
B. Menulis lirik bertema patah hati.
C. Menemukan nada dasar yang pas untuk penyanyi.
D. Menjual kaset lagu di pasar.

<details>
<summary>💡 Hint</summary>
Arrangement berarti "penyusunan" struktur lagu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menentukan urutan Intro, Verse, Chorus, Outro.**
Penyusunan struktur adalah inti dari aransemen sebuah karya musik.
</details>

### Soal #40: Koreografi Tari
Dekomposisi dalam melatih tarian grup yang rumit adalah...
A. Meminta semua penari menari sesuka hati.
B. Memecah gerakan menjadi hitungan 1-8 dan melatihnya per bagian.
C. Hanya fokus pada kostum tanpa latihan gerak.
D. Menutup mata saat musik dimulai.

<details>
<summary>💡 Hint</summary>
Pecah durasi waktu yang panjang menjadi potongan kecil (hitungan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memecah menjadi hitungan 1-8.**
Melatih per fraksi waktu mempermudah penari menghafal gerakan yang kompleks.
</details>

### Soal #41: Produksi Teater
Sutradara membagi produksi teater menjadi: Casting, Latihan, Artistik, dan Pemasaran. Tugas **Tim Artistik** meliputi...
A. Memilih aktor yang cocok untuk peran utama.
B. Merancang dekorasi panggung, pencahayaan, dan properti.
C. Menjual tiket di pintu masuk gedung.
D. Memastikan semua pemain hafal naskah.

<details>
<summary>💡 Hint</summary>
Artistik berhubungan dengan keindahan visual panggung.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dekorasi panggung dan pencahayaan.**
Komponen visual pendukung pertunjukan adalah tanggung jawab tim artistik.
</details>

### Soal #42: Desain Logo
Dekomposisi tugas saat mendesain logo sebuah brand adalah...
A. Menggunakan semua warna pelangi agar terlihat ceria.
B. Menentukan filosofi warna, pemilihan tipografi (font), dan bentuk simbol.
C. Menunggu komputer menggambar sendiri secara otomatis.
D. Menggambar logo yang persis dengan brand terkenal lainnya.

<details>
<summary>💡 Hint</summary>
Logo terdiri dari konsep warna, teks, dan lambang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Filosofi warna, tipografi, dan simbol.**
Memecah elemen visual logo membantu menciptakan identitas brand yang kuat.
</details>

### Soal #43: Menulis Komik
Manakah dekomposisi tugas yang benar untuk fase **"Pencritaan (Storytelling)"** dalam komik?
A. Membeli kertas komik yang paling mahal.
B. Membuat naskah dialog dan pembagian panel (storyboard).
C. Mewarnai semua halaman dengan spidol.
D. Mempromosikan komik di media sosial.

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana alur cerita dituangkan ke dalam kotak-kotak gambar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Naskah dialog dan pembagian panel.**
Storyboard adalah dekomposisi dari alur cerita menjadi urutan gambar.
</details>

### Soal #44: Membangun Set Film
Tim properti film harus membangun set "Kantor Tahun 1980-an". Manakah dekomposisi barang yang **TIDAK** relevan?
A. Komputer tabung kuno.
B. Mesin ketik manual.
C. Smartphone lipat terbaru.
D. Telepon kabel putar.

<details>
<summary>💡 Hint</summary>
Dekomposisi harus relevan dengan "Konteks Sesuai Zaman".
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Smartphone lipat terbaru.**
Barang ini merusak dekomposisi tema sejarah yang ingin dibangun.
</details>

### Soal #45: Fashion Show
Manajer acara fashion show memecah tugasnya. Manakah yang termasuk sub-masalah **"Backstage Coordination"**?
A. Memastikan urutan model keluar ke panggung tepat waktu.
B. Menghitung total keuntungan dari penjualan baju.
C. Memberikan sambutan di atas panggung.
D. Memesan karpet merah untuk pintu masuk.

<details>
<summary>💡 Hint</summary>
Backstage berarti "di belakang panggung" selama acara berlangsung.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Memastikan urutan model.**
Manajemen alur keluar-masuk model adalah kunci kelancaran sebuah fashion show.
</details>

### Soal #46: Animasi Frame-by-Frame
Seorang animator memecah gerakan "Orang Berjalan". Langkah dekomposisinya adalah...
A. Menggambar orang diam saja.
B. Membuat gambar kunci (Keyframes) posisi kaki saat melangkah, lalu mengisi gambar di antaranya (in-between).
C. Menggunakan AI untuk generate video tanpa menggambar sama sekali.
D. Menggambar 1000 gambar yang persis sama.

<details>
<summary>💡 Hint</summary>
Gerakan kompleks dipecah menjadi titik-titik perubahan posisi utama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuat Keyframes.**
Keyframes adalah dekomposisi gerakan menjadi pose-pose utama yang menentukan alur animasi.
</details>

### Soal #47: Produksi Podcast
Manakah tugas yang merupakan bagian dari dekomposisi **"Pra-Produksi"** Podcast?
A. Mengedit rekaman suara yang terlalu bising.
B. Menentukan topik bahasan dan menyusun daftar pertanyaan untuk narasumber.
C. Mengunggah file audio ke Spotify.
D. Membeli mikrofon baru saat rekaman sedang berjalan.

<details>
<summary>💡 Hint</summary>
Pra-produksi berarti "sebelum" tombol record ditekan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menentukan topik dan daftar pertanyaan.**
Persiapan materi adalah langkah dekomposisi terpenting sebelum memulai percakapan.
</details>

### Soal #48: Membuka Kedai Kopi
Dekomposisi rencana bisnis kedai kopi yang paling krusial di awal adalah...
A. Mencari lokasi, menentukan supplier biji kopi, dan menghitung modal peralatan.
B. Memikirkan gaya baju yang akan dipakai barista.
C. Menghitung jumlah followes akun kedai di Instagram.
D. Menunggu pelanggan datang dengan sendirinya tanpa promosi.

<details>
<summary>💡 Hint</summary>
Fokus pada pondasi operasional dan bahan baku.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Lokasi, Supplier, dan Modal.**
Ketiga hal tersebut adalah komponen dasar yang menentukan keberlangsungan bisnis.
</details>

### Soal #49: Kampanye Pemasaran Digital
Manakah tugas yang masuk dalam dekomposisi **"Analisis Target Pasar"**?
A. Menentukan usia, minat, dan lokasi geografis calon pembeli.
B. Memberikan diskon 50% untuk semua produk.
C. Membuat video iklan yang sangat mahal.
D. Membayar influencer untuk mempromosikan barang.

<details>
<summary>💡 Hint</summary>
Analisis target pasar berarti "mengenal siapa yang akan membeli".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menentukan usia, minat, dan lokasi.**
Mengenali profil pelanggan adalah dekomposisi dari strategi pemasaran yang efektif.
</details>

### Soal #50: Investasi Saham
Seorang investor melakukan dekomposisi analisis terhadap suatu perusahaan. Manakah yang masuk sub-masalah **"Analisis Fundamental"**?
A. Melihat grafik naik-turun harga dalam 5 menit terakhir.
B. Mengecek laporan keuangan tahunan dan keuntungan bersih perusahaan.
C. Mendengar saran dari orang asing di internet yang tidak dikenal.
D. Menebak-nebak masa depan tanpa data.

<details>
<summary>💡 Hint</summary>
Analisis fundamental berfokus pada "kesehatan" bisnis perusahaan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Laporan keuangan dan keuntungan.**
Memecah kinerja perusahaan melalui angka finansial adalah inti dari analisis fundamental.
</details>

