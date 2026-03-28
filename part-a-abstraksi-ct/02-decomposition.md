# 02. Decomposition (Dekomposisi)

> *"Gajah hanya bisa dimakan satu gigitan demi satu gigitan."* — Pepatah populer tentang menyelesaikan masalah besar.

## Apa itu Dekomposisi?

**Dekomposisi** adalah proses memecah masalah yang kompleks atau besar menjadi bagian-bagian yang lebih kecil, lebih sederhana, dan lebih mudah dikelola. 

Bayangkan jika Anda diminta untuk "Membangun sebuah Pesawat Terbang". Anda pasti akan bingung mulai dari mana. Namun, jika masalah itu dipecah menjadi:
1. Merancang sayap.
2. Membuat mesin.
3. Menyusun sistem navigasi.
4. Membangun kursi penumpang.
...maka setiap bagian tersebut menjadi jauh lebih mudah dikerjakan.

---

## Mengapa Kita Butuh Dekomposisi?

1. **Mengurangi Kewalahan**: Masalah besar seringkali menakutkan. Dengan memecahnya, beban mental kita berkurang.
2. **Spesialisasi**: Kita bisa fokus pada satu detail tanpa terganggu detail lainnya.
3. **Kemudahan Debugging**: Jika ada bagian yang rusak (misal: mesin pesawat), kita tahu persis di mana harus mencari kesalahannya tanpa harus membongkar seluruh pesawat.
4. **Paralelisasi**: Dalam tim, tugas yang sudah dipecah bisa dikerjakan oleh orang yang berbeda secara bersamaan.

---

## Contoh Penerapan Dekomposisi

### 🏠 Contoh 1: Kehidupan Nyata (Membersihkan Kamar)
Jika kamarmu sangat berantakan, jangan berpikir "Saya harus membersihkan kamar". Cobalah pecah menjadi:
- **Tugas A**: Membereskan buku di atas meja.
- **Tugas B**: Memasukkan baju kotor ke keranjang.
- **Tugas C**: Menyapu lantai.
- **Tugas D**: Merapikan tempat tidur.

### 💻 Contoh 2: Informatika (Membuat Website)
Seorang programmer memecah pembuatan website menjadi:
- **Frontend**: Apa yang dilihat pengguna (tombol, warna).
- **Backend**: Logika di balik layar (cara simpan data).
- **Database**: Tempat menyimpan data permanen.

### 🏆 Contoh 3: Strategi OSN-K
Saat menghadapi **Soal Part B (Studi Kasus)** yang sangat panjang, dekomposisilah menjadi:
- Apa inputnya?
- Apa aturannya?
- Apa output yang diminta?
- Simulasikan untuk data yang kecil dulu.

---

## Cara Melakukan Dekomposisi (Step-by-Step)

1. **Amati Masalah**: Lihat secara keseluruhan.
2. **Identifikasi Komponen**: Cari bagian-bagian yang bisa berdiri sendiri.
3. **Pecah Lagi (Nested)**: Jika bagian tersebut masih terlihat besar, pecah lagi hingga mencapai ukuran yang "bisa diselesaikan dalam sekali duduk".
4. **Hubungkan Kembali**: Pastikan setelah semua bagian kecil selesai, mereka bisa digabungkan kembali menjadi solusi yang utuh.

---

## ❓ Latihan Soal

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

### Soal #51: Rantai Pasok Produk (Supply Chain)
Dekomposisi manakah yang paling tepat untuk sub-masalah **"Distribusi Barang"** dalam skala nasional?
A. Memulai produksi di pabrik besar.
B. Menentukan rute truk pengangkut, pemilihan gudang transit, dan jadwal pengiriman.
C. Menciptakan iklan produk di televisi.
D. Mengatur desain kemasan produk agar lebih ringan.

<details>
<summary>💡 Hint</summary>
Distribusi berfokus pada perpindahan barang dari produsen ke konsumen.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rute truk, gudang transit, dan jadwal.**
Ketiga hal tersebut adalah komponen operasional dalam mendistribusikan barang secara luas.
</details>

### Soal #52: Sistem Tiket Layanan Pelanggan
Saat pelanggan mengeluh, sistem memecah tiket tersebut. Manakah yang termasuk sub-masalah **"Prioritas Tiket"**?
A. Menentukan tingkat urgensi masalah (Low, Medium, High).
B. Mengirimkan email balasan otomatis "Terima Kasih".
C. Menyimpan nama lengkap pelanggan dalam database.
D. Menampilkan foto profil admin yang melayani.

<details>
<summary>💡 Hint</summary>
Prioritas berarti menentukan mana yang harus dilayani lebih dahulu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menentukan tingkat urgensi (Low, Medium, High).**
Klasifikasi urgensi adalah cara sistem melakukan dekomposisi terhadap antrean bantuan.
</details>

### Soal #53: Sponsor Acara (Sponsorship)
Tim pencari dana membagi tugas pencarian sponsor. Manakah dekomposisi tugas untuk **"Follow-up Sponsor"**?
A. Membuat daftar 100 perusahaan target.
B. Menghubungi kembali narahubung perusahaan setelah proposal dikirim.
C. Mendesain poster acara yang memuat logo perusahaan.
D. Menghitung total dana yang sudah terkumpul.

<details>
<summary>💡 Hint</summary>
Follow-up adalah tindakan "menindaklanjuti" setelah komunikasi awal.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghubungi kembali narahubung.**
Tindakan proaktif menanyakan kelanjutan proposal adalah inti dari follow-up.
</details>

### Soal #54: Manajemen Inventaris Gudang
Dekomposisi yang tepat untuk fitur **"Stok Opname"** (Pengecekan stok fisik) adalah...
A. Melakukan penjualan besar-besaran (cuci gudang).
B. Menghitung jumlah barang di rak dan mencocokkannya dengan data di sistem.
C. Memberikan label harga baru pada setiap barang.
D. Mengunci gudang agar tidak ada pencuri masuk.

<details>
<summary>💡 Hint</summary>
Stok opname adalah proses "audit" jumlah barang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghitung barang rak vs data sistem.**
Perbandingan data fisik dan digital adalah komponen utama dari stok opname.
</details>

### Soal #55: Sistem Gaji Karyawan (Payroll)
Manakah dekomposisi yang tepat untuk perhitungan **"Gaji Bersih"** (Take Home Pay)?
A. Gaji Pokok + Tunjangan - Potongan (Pajak/BPJS).
B. Hanya menghitung jumlah hari lembur saja.
C. Memberikan bonus kepada semua karyawan tanpa kecuali.
D. Menghitung biaya operasional kantor secara keseluruhan.

<details>
<summary>💡 Hint</summary>
Gaji bersih adalah apa yang diterima setelah penambahan dan pengurangan wajib.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Gaji Pokok + Tunjangan - Potongan.**
Rumus ini adalah dekomposisi matematis dari komponen penyusun gaji karyawan.
</details>

### Soal #56: Survei Riset Pasar
Manakah sub-masalah dari dekomposisi **"Penyusunan Kuesioner"**?
A. Membagikan link survei di grup WhatsApp.
B. Memilih jenis pertanyaan (pilihan ganda, skala likert, atau esai).
C. Menghitung rata-rata jawaban responden.
D. Memberikan hadiah pulsa kepada yang mengisi survei.

<details>
<summary>💡 Hint</summary>
Penyusunan berarti proses "merancang" instrumen survei.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memilih jenis pertanyaan.**
Menentukan format pertanyaan adalah komponen teknis dalam menyusun kuesioner.
</details>

### Soal #57: Audit Finansial
Seorang auditor membedah laporan keuangan sebuah organisasi. Manakah yang masuk sub-masalah **"Verifikasi Transaksi"**?
A. Mengecek kecocokan antara nota fisik dengan entri di buku besar.
B. Menjelaskan visi misi organisasi kepada publik.
C. Menentukan tanggal libur massal karyawan.
D. Menggambar grafik pertumbuhan keuntungan yang terlihat bagus.

<details>
<summary>💡 Hint</summary>
Verifikasi transaksi berarti membuktikan "kebenaran" catatan uang.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mengecek nota fisik vs buku besar.**
Pembuktian data melalui dokumen fisik adalah langkah inti dari verifikasi audit.
</details>

### Soal #58: Pengelolaan Sampah Plastik
Dalam program pengurangan limbah plastik, dekomposisi manakah yang merupakan bagian dari **"Upcycling"**?
A. Membakar sampah plastik di halaman rumah.
B. Mengubah botol plastik bekas menjadi pot tanaman atau tas belanja.
C. Membuang plastik ke tempat pembuangan akhir (TPA).
D. Menggunakan kantong plastik baru setiap kali berbelanja.

<details>
<summary>💡 Hint</summary>
Upcycling berarti memberikan "nilai tambah" pada barang bekas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengubah botol plastik menjadi pot/tas.**
Memberikan fungsi baru pada limbah adalah dekomposisi kreatif dari konsep upcycling.
</details>

### Soal #59: Proyek Reboisasi
Dekomposisi tugas untuk proyek penanaman kembali hutan yang gundul adalah...
A. Menggambar peta hutan di atas kertas.
B. Pembibitan pohon, persiapan lahan, penanaman, dan pemeliharaan rutin.
C. Mencari tahu nama-nama penebang hutan liar.
D. Menunggu hujan turun sepanjang tahun.

<details>
<summary>💡 Hint</summary>
Pikirkan siklus hidup penanaman dari awal hingga tumbuh besar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pembibitan, lahan, penanaman, dan pemeliharaan.**
Langkah-langkah tersebut adalah sub-proses penyusun keberhasilan reboisasi.
</details>

### Soal #60: Alur IGD Rumah Sakit
Saat pasien masuk IGD (Instalasi Gawat Darurat), perawat melakukan dekomposisi penanganan. Manakah tahap **"Triage"**?
A. Mengoperasi pasien dengan segera.
B. Menilai tingkat keparahan kondisi pasien untuk menentukan urutan penanganan.
C. Menanyakan metode pembayaran (asuransi atau mandiri).
D. Menghibur keluarga pasien agar tidak menangis.

<details>
<summary>💡 Hint</summary>
Triage adalah sistem seleksi pasien berdasarkan kegawatdaruratan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menilai tingkat keparahan kondisi.**
Memisahkan mana yang kritis dan mana yang stabil adalah dekomposisi medis di IGD.
</details>

### Soal #61: Distribusi Vaksin
Logistik vaksin COVID-19 sangat rumit. Manakah dekomposisi tugas untuk **"Cold Chain Management"**?
A. Memberikan suntikan kepada masyarakat luas.
B. Memastikan suhu penyimpanan tetap stabil di -70 hingga 2 derajat Celcius selama perjalanan.
C. Mencatat nama-nama penerima vaksin di database nasional.
D. Membuat poster kampanye "Ayo Vaksin".

<details>
<summary>💡 Hint</summary>
Cold Chain (Rantai Dingin) berfokus pada suhu penyimpanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memastikan suhu penyimpanan stabil.**
Pengaturan suhu konstan adalah sub-masalah teknis paling kritis dalam distribusi vaksin sensitif.
</details>

### Soal #62: Sistem Pemurnian Air
Dalam alat filtrasi air sederhana, dekomposisi lapisan penyaringnya biasanya terdiri dari...
A. Pasir, kerikil, ijuk, dan arang.
B. Besi, tembaga, dan emas.
C. Plastik, kertas, dan kain lap.
D. Gula, kopi, dan krim nabati.

<details>
<summary>💡 Hint</summary>
Gunakan material alami yang bisa menyaring kotoran fisik dan kimia.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pasir, kerikil, ijuk, dan arang.**
Setiap lapisan memiliki tugas dekomposisi penyaringan yang berbeda (kotoran besar vs partikel kecil).
</details>

### Soal #63: Konservasi Satwa Langka
Manakah sub-masalah dari dekomposisi **"Monitoring Habitat"** Orang Utan?
A. Memindahkan semua orang utan ke kebun binatang di luar negeri.
B. Memasang kamera jebak (camera trap) dan menggunakan citra satelit untuk cek luas hutan.
C. Menamai setiap bayi orang utan yang lahir dengan nama unik.
D. Menghitung jumlah wisatawan yang datang melihat orang utan.

<details>
<summary>💡 Hint</summary>
Monitoring berarti "memantau" kondisi lingkungan secara berkala.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memasang kamera jebak dan citra satelit.**
Teknologi ini membantu pengawas memantau kondisi habitat tanpa mengganggu satwa.
</details>

### Soal #64: Kampanye Kesehatan Masyarakat
Dekomposisi tugas untuk kampanye "Berhenti Merokok" yang efektif adalah...
A. Menyuruh orang berhenti merokok sekarang juga dengan berteriak.
B. Edukasi bahaya medis, pemberian konseling, dan bantuan terapi pengganti nikotin.
C. Menaikkan harga rokok setinggi mungkin tanpa sosialisasi.
D. Memarahi penjual rokok di pinggir jalan.

<details>
<summary>💡 Hint</summary>
Solusi kompleks membutuhkan pendekatan edukasi dan bantuan medis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Edukasi, Konseling, dan Terapi.**
Memecah kampanye menjadi langkah-langkah persuasif dan medis memberikan hasil yang lebih permanen.
</details>

### Soal #65: Desain Program Fitnes
Seorang pelatih (personal trainer) memecah program latihan seorang pemula. Manakah yang masuk sub-masalah **"Nutritional Planning"**?
A. Menghitung asupan kalori harian dan keseimbangan protein, lemak, serta karbohidrat.
B. Mengangkat beban maksimal di hari pertama latihan.
C. Membeli baju olahraga terbaru.
D. Berlari maraton selama 5 jam tanpa istirahat.

<details>
<summary>💡 Hint</summary>
Nutrisi berhubungan dengan asupan makanan ke dalam tubuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kalori harian dan keseimbangan makronutrisi.**
Dekomposisi diet adalah bagian krusial selain latihan fisik di gym.
</details>

### Soal #66: Pertanian Organik
Dekomposisi sistem pertanian organik yang membedakannya dengan pertanian konvensional adalah...
A. Menggunakan pestisida kimia sebanyak mungkin.
B. Penggunaan pupuk kompos alami dan sistem rotasi tanaman tanpa bahan sintetis.
C. Membajak sawah menggunakan traktor paling canggih.
D. Menanam hanya satu jenis tanaman saja di seluruh lahan (monokultur).

<details>
<summary>💡 Hint</summary>
Organik berarti kembali ke cara alami dan menjaga keberlanjutan tanah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pupuk kompos dan rotasi tanaman.**
Dekomposisi nutrisi tanah organik bergantung pada keseimbangan ekosistem alami.
</details>

### Soal #67: Pemilahan Sampah di Sumber (Rumah Tangga)
Dekomposisi sampah rumah tangga menjadi 3 kategori utama yang disarankan adalah...
A. Sampah dari Ayah, Ibu, dan Anak.
B. Sampah Pagi, Siang, dan Malam.
C. Sampah Organik (sisa makanan), Anorganik (plastik/kertas), dan B3 (baterai/listrik).
D. Sampah Wangi, Sampah Bau, dan Sampah Sangat Bau.

<details>
<summary>💡 Hint</summary>
Pecah berdasarkan karakteristik material agar mudah diolah kembali.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Organik, Anorganik, dan B3.**
Pengumpulan sampah berdasarkan kategori material mempermudah proses daur ulang.
</details>

### Soal #68: Proses Kompilasi Program (Compilation)
Seorang compiler memecah kode programmu sebelum jadi file .exe. Manakah tahap **"Lexical Analysis"**?
A. Menjalankan program di Windows.
B. Memecah baris teks program menjadi potongan kecil (tokens) seperti kata kunci, angka, dan simbol.
C. Mengecek apakah logika program sudah benar.
D. Mengubah warna teks di code editor.

<details>
<summary>💡 Hint</summary>
Lexical berhubungan dengan "analisis kata" atau simbol.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memecah teks menjadi potongan kecil (tokens).**
Lexer adalah bagian pertama yang melakukan dekomposisi teks mentah menjadi entitas yang dimengerti compiler.
</details>

### Soal #69: Proses Booting Komputer
Saat kamu menekan tombol power, komputer melakukan dekomposisi langkah booting. Manakah tahap **"POST"** (Power-On Self-Test)?
A. Menampilkan pilihan wallpaper desktop.
B. Melakukan pengecekan kesehatan hardware (RAM, CPU, Keyboard) secara otomatis di awal.
C. Masuk ke halaman login Windows.
D. Memutar lagu pengiring saat masuk ke sistem.

<details>
<summary>💡 Hint</summary>
Self-Test berarti komputer "memeriksa dirinya sendiri" apakah siap dijalankan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengecekan hardware awal.**
Sistem memecah pengecekan per komponen hardware sebelum mengizinkan sistem operasi berjalan.
</details>

### Soal #70: Sharding Database
Dalam database raksasa (seperti YouTube), data dipecah agar tidak terlalu berat. Proses ini disebut Sharding. Contoh dekomposisi sharding adalah...
A. Menghapus semua postingan lama.
B. Membagi data pengguna berdasarkan wilayah (Misal: Server Asia, Server Eropa, Server Amerika).
C. Mengganti nama database menjadi lebih pendek.
D. Menggunakan font yang berbeda untuk setiap tabel.

<details>
<summary>💡 Hint</summary>
Sharding berarti memecah satu tabel database raksasa menjadi beberapa tabel kecil di server berbeda.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membagi data berdasarkan wilayah.**
Memecah beban database per lokasi geografis adalah teknik dekomposisi data tingkat lanjut.
</details>

### Soal #71: Feature Engineering (Machine Learning)
Sebelum melatih AI, data harus didekomposisi. Manakah kegiatan **"Feature Extraction"**?
A. Membiarkan AI belajar sendiri tanpa data apapun.
B. Mengambil informasi penting (seperti pixel tepi gambar) untuk membantu AI mengenali wajah.
C. Meningkatkan harga jual model AI di pasaran.
D. Menghapus semua label pada data latihan.

<details>
<summary>💡 Hint</summary>
Feature berarti "ciri khas" atau "informasi penting" dari data mentah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengambil informasi penting (tepi gambar).**
Dekomposisi data mentah menjadi ciri-ciri khusus mempermudah AI untuk belajar.
</details>

### Soal #72: Cybersecurity Pen-Testing
Seorang "White Hat Hacker" melakukan simulasi serangan (Pen-test). Manakah tahap **"Reconnaissance"**?
A. Langsung merusak server perusahaan.
B. Mengumpulkan informasi publik tentang target (IP Address, email karyawan, dll) sebelum menyerang.
C. Menulis laporan hasil peretasan.
D. Meminta uang kepada pemilik perusahaan.

<details>
<summary>💡 Hint</summary>
Reconnaissance berarti fase "pengintaian" atau pengumpulan data awal.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengumpulkan informasi publik.**
Fase ini adalah dekomposisi langkah awal dalam memahami pertahanan sistem target.
</details>

### Soal #73: Routing Paket Data
Saat kamu kirim chat WA, pesanmu dipecah menjadi paket-paket kecil. Tugas **Router** dalam dekomposisi pengiriman ini adalah...
A. Menghapus paket yang terlihat mencurigakan.
B. Menentukan jalur tercepat ke alamat tujuan untuk setiap paket data.
C. Mengubah warna teks chat menjadi biru.
D. Menyimpan paket data tersebut selamanya di dalam memori router.

<details>
<summary>💡 Hint</summary>
Router bertindak sebagai "polisi lalu lintas" paket data.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menentukan jalur tercepat ke tujuan.**
Dekomposisi rute per paket memastikan pesan sampai dengan efisien meskipun lewat jalur yang berbeda-beda.
</details>

### Soal #74: Kompresi Data Run-Length Encoding (RLE)
Jika kita punya data warna: `AAAAABBBCCCC`, RLE mengompresnya menjadi `5A3B4C`. Apa langkah dekomposisi utamanya?
A. Menghapus semua huruf yang ada.
B. Menghitung jumlah perulangan karakter yang sama secara berurutan.
C. Mengganti huruf dengan angka secara acak.
D. Membalikkan urutan huruf dari belakang ke depan.

<details>
<summary>💡 Hint</summary>
Fokus pada "pola perulangan" (Pattern Recognition) yang didekomposisi menjadi angka jumlah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghitung jumlah perulangan karakter.**
Dekomposisi urutan panjang menjadi "Jumlah + Karakter" adalah dasar kompresi RLE.
</details>

### Soal #75: Enkripsi dan Dekripsi
Dalam sistem pesan rahasia, manakah sub-masalah dari fase **"Key Exchange"**?
A. Menulis pesan panjang di atas kertas.
B. Menyepakati "kunci rahasia" antara pengirim dan penerima agar bisa membuka pesan.
C. Membuang pesan yang tidak sengaja dibaca orang lain.
D. Menggunakan bahasa daerah agar tidak dimengerti orang luar.

<details>
<summary>💡 Hint</summary>
Tanpa kunci, pesan yang terenkripsi (acak) tidak bisa didekripsi (dibaca).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyepakati "kunci rahasia".**
Pertukaran kunci adalah komponen fondasi dari keamanan data modern.
</details>

### Soal #76: Manajemen Memori (Garbage Collection)
Sistem operasi melakukan dekomposisi memori untuk menjaga performa. Apa tugas dari **"Garbage Collector"**?
A. Menghapus file sampah di Recycle Bin secara manual.
B. Mengidentifikasi dan membebaskan memori yang sudah tidak digunakan oleh program lagi.
C. Menambah kapasitas RAM secara fisik tanpa membuka casing komputer.
D. Mengatur urutan ikon di Desktop.

<details>
<summary>💡 Hint</summary>
Fokus pada efisiensi penggunaan memori RAM selama program berjalan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membebaskan memori yang tidak digunakan.**
Dekomposisi siklus hidup data di memori membantu sistem mengelola sumber daya dengan efisien.
</details>

### Soal #77: Desain API Endpoint
Dalam merancang API untuk aplikasi cuaca, manakah dekomposisi endpoint yang paling logis?
A. `/getWeatherToday`, `/getWeatherWeekly`, dan `/getCityCoordinates`.
B. `/downloadNewMovies` dan `/uploadProfilePicture`.
C. `/playMusic` dan `/stopMusic`.
D. `/openBrowser` dan `/closeBrowser`.

<details>
<summary>💡 Hint</summary>
API endpoint harus mencerminkan fungsi spesifik yang disediakan oleh layanan (service).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. WeatherToday, WeatherWeekly, dan CityCoordinates.**
Endpoint tersebut memecah fungsionalitas aplikasi cuaca menjadi akses data yang spesifik.
</details>

### Soal #78: Pelestarian Monumen Sejarah
Dekomposisi tugas untuk merestorasi candi yang runtuh adalah...
A. Mengganti semua batu lama dengan batu semen baru agar cepat selesai.
B. Pendataan setiap fragmen batu, pembersihan manual, penyusunan kembali (anastilosis), dan penguatan struktur.
C. Menjadikan candi tersebut sebagai lahan parkir kendaraan.
D. Mengecat candi dengan warna-warni agar terlihat modern.

<details>
<summary>💡 Hint</summary>
Proses restorasi arkeologi sangat teliti dan menjaga keaslian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pendataan, pembersihan, penyusunan, dan penguatan.**
Langkah-langkah sistematis ini adalah dekomposisi standar dalam pelestarian benda cagar budaya.
</details>

### Soal #79: Festival Budaya Tradisional
Panitia festival membagi tugas besar. Manakah yang masuk dalam dekomposisi **"Seksi Acara"**?
A. Menghubungi penyedia jasa tenda dan panggung.
B. Menyusun rundown (jadwal) penampilan tari, musik, dan upacara adat.
C. Membeli bahan makanan untuk dapur umum.
D. Mencari investor untuk mendanai festival tahun depan.

<details>
<summary>💡 Hint</summary>
Seksi acara fokus pada konten dan durasi pertunjukan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyusun rundown penampilan.**
Jadwal dan konten panggung adalah komponen inti dari manajemen acara.
</details>

### Soal #80: Penerjemahan Sastra Klasik
Seorang penerjemah memecah masalah saat menerjemahkan buku setebal 500 halaman. Manakah yang termasuk sub-masalah **"Localization"**?
A. Menghitung jumlah kata dalam satu bab.
B. Menyesuaikan peribahasa asing agar maknanya tetap dimengerti oleh budaya lokal pembaca.
C. Mengganti jenis huruf (font) buku menjadi lebih besar.
D. Mencetak buku di percetakan terdekat.

<details>
<summary>💡 Hint</summary>
Lokalisasi berarti menyesuaikan konteks agar relevan dengan budaya target.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan peribahasa asing.**
Memecah bahasa tidak hanya soal kata, tapi soal rasa dan konteks budaya (lokalisasi).
</details>

### Soal #81: Ekskavasi Arkeologi
Dekomposisi area penggalian situs purbakala biasanya menggunakan sistem...
A. Menggali secara acak di mana saja sesuka hati.
B. Membuat sistem grid (kotak-kotak) untuk memetakan lokasi penemuan setiap artefak secara presisi.
C. Menggunakan alat berat agar semua tanah terangkat dalam sekejap.
D. Menunggu artefak muncul sendiri ke permukaan saat hujan.

<details>
<summary>💡 Hint</summary>
Grid membantu arkeolog memecah area luas menjadi sel-sel kecil yang terkendali.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuat sistem grid (kotak-kotak).**
Sistem grid adalah penerapan dekomposisi spasial untuk mempermudah pendataan temuan.
</details>

### Soal #82: Kurasi Museum
Seorang kurator memecah pameran museum bertema "Era Kerajaan Nusantara". Manakah dekomposisi sub-tema yang paling masuk akal?
A. Berdasarkan urutan kronologi waktu (Abad 4, Abad 7, Abad 13, dst).
B. Berdasarkan harga tiket masuk pengunjung.
C. Berdasarkan jenis makanan yang dijual di kantin museum.
D. Berdasarkan merk sepatu kurator yang digunakan saat bekerja.

<details>
<summary>💡 Hint</summary>
Pameran sejarah paling umum dipecah berdasarkan urutan waktu kejadian.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Berdasarkan urutan kronologi waktu.**
Dekomposisi waktu mempermudah pengunjung memahami alur sejarah secara logis.
</details>

### Soal #83: Riset Silsilah Keluarga (Genealogy)
Dalam menelusuri garis keturunan keluarga besar, langkah dekomposisi pertamamu adalah...
A. Mewawancarai anggota keluarga yang paling tua (Kakek/Nenek) untuk mencatat nama-nama leluhur.
B. Mencari nama orang asing di internet yang memiliki marga yang sama.
C. Mengganti namamu sendiri agar terlihat lebih bangsawan.
D. Mengabaikan semua kerabat yang lokasinya jauh.

<details>
<summary>💡 Hint</summary>
Mulailah dari sumber data primer terdekat dan paling akurat.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mewawancarai anggota keluarga tertua.**
Informasi dari saksi sejarah adalah komponen fondasi dalam membangun pohon keluarga.
</details>

### Soal #84: Program Pertukaran Pelajar
Dekomposisi tugas untuk keberangkatan pertukaran pelajar internasional adalah...
A. Menangis karena harus meninggalkan teman di rumah.
B. Pengurusan visa, latihan bahasa, orientasi budaya, dan persiapan perlengkapan musim dingin.
C. Membeli oleh-oleh sebelum sampai di negara tujuan.
D. Berhenti belajar karena sudah merasa pintar.

<details>
<summary>💡 Hint</summary>
Pikirkan segala kebutuhan administratif dan adaptasi sebelum berangkat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Visa, bahasa, budaya, dan perlengkapan.**
Ketiganya adalah sub-masalah krusial yang harus diselesaikan satu per satu.
</details>

### Soal #85: Dokumenter Sejarah Lokal
Dekomposisi proses pembuatan film dokumenter tentang legenda desa setempat meliputi...
A. Membuat cerita fiksi yang penuh dengan naga dan sihir.
B. Pengumpulan arsip foto, wawancara tokoh masyarakat, dan pengambilan gambar saksi sejarah.
C. Meniru gaya pembuatan film Hollywood yang sangat mahal.
D. Menyebarkan rumor yang belum tentu benar agar filmnya viral.

<details>
<summary>💡 Hint</summary>
Dokumenter sejarah bergantung pada fakta dan bukti yang dipecah dari berbagai sumber.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Arsip foto, wawancara, dan saksi sejarah.**
Ketiganya adalah komponen data penyusun keaslian cerita dokumenter.
</details>

### Soal #86: Restorasi Foto Tua
Saat memperbaiki foto digital yang sobek dan pudar, dekomposisi langkah editingnya adalah...
A. Menghapus foto tersebut karena sudah rusak.
B. Penyesuaian kontras, perbaikan bagian sobek menggunakan tool "healing", dan pewarnaan ulang (re-coloring).
C. Mencetak foto yang rusak berkali-kali.
D. Meletakkan foto di bawah sinar matahari langsung agar warnanya kembali.

<details>
<summary>💡 Hint</summary>
Pecah perbaikan menjadi aspek cahaya, fisik, dan warna.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kontras, Healing sobekan, dan Re-coloring.**
Teknik dekomposisi masalah visual ini sering digunakan oleh editor foto profesional.
</details>

### Soal #87: Dokumentasi Warisan Kuliner
Untuk mendaftarkan sebuah makanan tradisional ke UNESCO sebagai warisan budaya, manakah dekomposisi data yang diperlukan?
A. Sejarah asal-usul, daftar bahan asli, cara pembuatan tradisional, dan filosofi makanan.
B. Daftar nama orang yang suka memakan makanan tersebut.
C. Jumlah kalori dan lemak jenuh dalam seporsi makanan.
D. Nama perusahaan besar yang memproduksi makanan serupa secara instan.

<details>
<summary>💡 Hint</summary>
Fokus pada nilai sejarah dan budaya yang melekat pada makanan tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Sejarah, bahan, cara buat, dan filosofi.**
Empat komponen ini menjelaskan identitas utuh dari sebuah warisan kuliner.
</details>

### Soal #88: Membangun Jembatan
Insinyur memecah pembangunan jembatan besar menjadi beberapa fase. Manakah yang masuk dalam **"Geotechnical Analysis"**?
A. Memilih warna cat pipa jembatan.
B. Mengetes kekuatan tanah di dasar sungai untuk menentukan kedalaman pondasi.
C. Meresmikan jembatan dengan mengundang pejabat.
D. Menghitung jumlah kendaraan yang lewat setiap menit.

<details>
<summary>💡 Hint</summary>
Geo-technical berhubungan dengan karakteristik bumi/tanah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengetes kekuatan tanah dasar sungai.**
Analisis tanah adalah sub-masalah teknik sipil yang menentukan keamanan struktur di atasnya.
</details>

### Soal #89: Instalasi Panel Surya
Dekomposisi sistem pembangkit listrik tenaga surya (PLTS) rumah tangga terdiri dari...
A. Kaca jendela, kabel listrik, dan saklar lampu.
B. Panel surya, Inverter (pengubah arus), Baterai penyimpanan, dan Charge Controller.
C. Kincir angin, dinamo, dan generator.
D. Arang, kayu bakar, dan korek api.

<details>
<summary>💡 Hint</summary>
Sistem ini membutuhkan komponen penangkap, pengubah, dan penyimpan energi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Panel, Inverter, Baterai, dan Controller.**
Setiap komponen memiliki perannya masing-masing dalam mengubah sinar matahari menjadi listrik siap pakai.
</details>

### Soal #90: Desain Pencakar Langit
Manakah dekomposisi sistem keamanan yang paling kritis pada gedung tinggi?
A. Pemasangan lift yang sangat cepat (super-speed elevator).
B. Sistem deteksi asap, sprinkler otomatis, tangga darurat, dan struktur tahan gempa.
C. Membuat taman di lantai paling atas (roof-garden).
D. Mewarnai kaca gedung dengan warna biru agar terlihat menyatu dengan langit.

<details>
<summary>💡 Hint</summary>
Keamanan berarti melindungi penghuni dari bahaya kebakaran dan bencana alam.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Deteksi asap, sprinkler, tangga darurat, tahan gempa.**
Ini adalah dekomposisi dari protokol keamanan gedung modern yang komprehensif.
</details>

### Soal #91: Perencanaan Jaringan Kereta Api
Manakah tugas yang masuk dalam dekomposisi **"Signaling System"**?
A. Menjual tiket di stasiun pusat.
B. Mengatur lampu lalu lintas kereta dan sensor posisi kereta agar tidak terjadi tabrakan.
C. Membersihkan gerbong kereta setiap malam.
D. Menentukan jenis kursi untuk kelas eksekutif.

<details>
<summary>💡 Hint</summary>
Signaling berhubungan dengan komunikasi dan kontrol pergerakan kereta.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampu lalu lintas dan sensor posisi kereta.**
Signaling adalah sub-masalah infrastruktur yang paling vital bagi keselamatan perjalanan kereta api.
</details>

### Soal #92: Manajemen Jaringan Listrik (Power Grid)
Saat terjadi mati lampu massal (blackout), PLN melakukan dekomposisi pelacakan gangguan. Langkah pertamanya adalah...
A. Mengganti semua tiang listrik di seluruh kota.
B. Melakukan pengecekan tegangan pada gardu induk, lalu sub-gardu, kemudian trafo lingkungan.
C. Menunggu pelanggan menelepon baru kemudian bertindak.
D. Menulis permohonan maaf di media sosial tanpa melakukan perbaikan.

<details>
<summary>💡 Hint</summary>
Lakukan pengecekan dari sumber utama ke hilir secara berjenjang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gardu induk -> Sub-gardu -> Trafo.**
Isolasi masalah berjenjang membantu menemukan titik kerusakan kabel atau trafo dengan efektif.
</details>

### Soal #93: Peluncuran Satelit
Dekomposisi misi luar angkasa biasanya dibagi menjadi fase-fase berikut. Manakah tahap **"Orbital Insertion"**?
A. Persiapan roket di landasan pacu.
B. Menempatkan satelit pada ketinggian dan kemiringan yang tepat agar tetap mengorbit bumi.
C. Mengambil foto permukaan bumi dan mengirimnya ke pusat kontrol.
D. Menjatuhkan sisa roket ke tengah samudra.

<details>
<summary>💡 Hint</summary>
Orbital Insertion berarti "memasukkan" benda ke orbit yang diinginkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menempatkan satelit pada orbitnya.**
Ini adalah langkah kritikal dalam dekomposisi misi antariksa setelah peluncuran.
</details>

### Soal #94: Kabel Bawah Laut
Dekomposisi sistem internet antar benua adalah...
A. Mengirim sinyal melalui balon udara yang terbang sangat tinggi.
B. Pemasangan kabel fiber optik di dasar samudra, repeater (penguat sinyal), dan stasiun pendaratan kabel.
C. Menggunakan merpati pos untuk membawa harddisk berisi data.
D. Mengandalkan sinyal radio dari menara yang ada di gunung.

<details>
<summary>💡 Hint</summary>
Internet dunia saat ini 99% bergantung pada infrastruktur fisik di bawah laut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Fiber optik samudra, Repeater, dan Stasiun pendaratan.**
Inilah komponen utama penyusun jaringan internet global yang kita gunakan.
</details>

### Soal #95: Konstruksi Terowongan
Seorang insinyur menggunakan dekomposisi saat menggunakan mesin bor raksasa (TBM) untuk membuat terowongan MRT. Manakah yang masuk sub-masalah **"Structural Lining"**?
A. Menggali tanah menggunakan gigi bor yang sangat tajam.
B. Memasang segmen-segmen beton melingkar untuk memperkuat dinding terowongan agar tidak runtuh.
C. Mengangkut sisa tanah galian ke luar terowongan.
D. Menentukan nama stasiun MRT yang akan dibangun.

<details>
<summary>💡 Hint</summary>
Lining berhubungan dengan "pelapisan" atau penguatan dinding terowongan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memasang segmen beton penguat.**
Dinding beton tersebut adalah komponen penyusun stabilitas terowongan bawah tanah.
</details>

### Soal #96: Sinkronisasi Lampu Lalu Lintas
Dekomposisi algoritma "Green Wave" (gelombang hijau) di jalan raya adalah...
A. Memberikan lampu merah sepanjang waktu agar tidak ada kecelakaan.
B. Menyesuaikan waktu nyala lampu hijau antar persimpangan berdasarkan kecepatan rata-rata kendaraan.
C. Mematikan semua lampu lalu lintas saat malam hari.
D. Menyuruh polisi berdiri di setiap persimpangan secara manual.

<details>
<summary>💡 Hint</summary>
Green Wave bertujuan agar kendaraan tidak perlu berhenti berkali-kali di setiap persimpangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan waktu nyala lampu antar persimpangan.**
Sinkronisasi waktu adalah dekomposisi dari sistem manajemen lalu lintas yang efisien.
</details>

### Soal #97: Pengolahan Limbah Cair (Wastewater Treatment)
Manakah dekomposisi tahap **"Secondary Treatment"** dalam pabrik pengolahan limbah?
A. Menyaring sampah plastik dan kayu besar menggunakan screen besar.
B. Menggunakan bakteri untuk menguraikan sisa-sisa bahan organik secara biologis.
C. Menambahkan zat pewarna agar air terlihat lebih jernih.
D. Membuang air limbah langsung ke sungai tanpa proses apapun.

<details>
<summary>💡 Hint</summary>
Tahap sekunder biasanya menggunakan proses biologi untuk memecah zat pencemar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menggunakan bakteri pengurai.**
Dekomposisi biologis adalah sub-masalah kimiawi yang sangat penting dalam menjaga kelestarian air.
</details>

### Soal #98: Pembersihan Sampah Luar Angkasa
Dekomposisi misi "Space Debris Cleanup" yang paling masuk akal adalah...
A. Mengirim magnet raksasa untuk menarik semua sampah besi.
B. Identifikasi objek berbahaya, penangkapan menggunakan harpun/jaring, dan pendorongan ke atmosfer bumi untuk dibakar.
C. Meledakkan sampah menggunakan nuklir di orbit bumi.
D. Menunggu sampah tersebut jatuh sendiri ke bumi dalam 1000 tahun.

<details>
<summary>💡 Hint</summary>
Masalah sampah antariksa membutuhkan tahapan identifikasi, penangkapan, dan eliminasi yang aman.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Identifikasi, Penangkapan, dan Pendorongan ke atmosfer.**
Langkah-langkah tersebut adalah dekomposisi dari solusi teknis futuristik untuk membersihkan orbit bumi.
</details>

### Soal #99: Desain Kota Berkelanjutan (Sustainable City)
Dalam merancang kota masa depan, dekomposisi pilar **"Urban Mobility"** harus mencakup...
A. Pembangunan jalan tol yang seluas mungkin di tengah kota.
B. Integrasi transportasi umum massal, jalur sepeda, dan area pejalan kaki (pedestrian) yang nyaman.
C. Larangan bagi orang miskin untuk masuk ke area pusat kota.
D. Mengimpor semua bahan pangan dari luar negeri tanpa pertanian lokal.

<details>
<summary>💡 Hint</summary>
Mobilitas perkotaan modern berfokus pada pengurangan ketergantungan pada kendaraan pribadi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Transportasi umum, jalur sepeda, dan pedestrian.**
Sub-komponen ini membentuk sistem mobilitas kota yang sehat dan rendah polusi.
</details>

### Soal #100: Persiapan OSN-K Informatika 2026
Selamat! Kamu sudah sampai di soal terakhir. Apa langkah dekomposisi persiapanmu mulai hari ini?
A. Belajar 24 jam sehari tanpa tidur sampai hari H.
B. Memahami pilar CT, berlatih Dry Run, belajar bahasa C++, dan simulasi soal tahun-tahun sebelumnya secara rutin.
C. Bermain game sepanjang waktu dan berharap ada keajaiban.
D. Mengumpulkan semua buku olimpiade tapi tidak pernah membacanya.

<details>
<summary>💡 Hint</summary>
Kunci sukses olimpiade adalah persiapan yang terstruktur dan konsisten.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. CT, Dry Run, C++, dan Simulasi Soal.**
Dekomposisi rencana belajar yang merangkum semua aspek kompetensi akan membawamu meraih medali emas! 🏅
</details>

---
[< Kembali ke Beranda Materi](../README.md) | [Materi Selanjutnya: Pattern Recognition](./03-pattern-recognition.md)
