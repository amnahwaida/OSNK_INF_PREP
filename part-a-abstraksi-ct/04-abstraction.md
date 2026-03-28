# Abstraksi (Abstraction): Fokus pada Hal yang Penting

> **"Abstraksi adalah seni melupakan hal-hal yang tidak penting agar kita bisa fokus pada apa yang benar-benar penting."**

Selamat datang di modul **Abstraksi**! Jika **Dekomposisi** adalah memecah masalah, dan **Pattern Recognition** adalah mencari kemiripan, maka **Abstraksi** adalah proses penyederhanaan.

Dalam dunia informatika dan kehidupan sehari-hari, kita seringkali "tenggelam" dalam detail yang terlalu rumit. Abstraksi membantu kita menarik diri ke atas, melihat gambaran besar, dan mengabaikan detail teknis yang tidak relevan untuk tujuan kita saat ini.

---

## 1. Apa itu Abstraksi?

Secara sederhana, **Abstraksi** adalah proses menyaring (filtering) informasi. Kita mengambil inti sari dari sebuah objek atau masalah dan membuang detail-detail yang hanya akan membingungkan kita.

### Mengapa Abstraksi Penting?
1.  **Mengurangi Kompleksitas**: Membuat masalah yang rumit jadi lebih mudah dikelola.
2.  **Efisiensi**: Kita tidak perlu belajar ulang segalanya dari nol.
3.  **Generalisasi**: Memungkinkan kita membuat satu solusi yang bisa dipakai untuk banyak hal (karena kita fokus pada pola intinya).

---

## 2. Analogi di Kehidupan Nyata

Mari kita lihat bagaimana otak kita melakukan abstraksi setiap hari tanpa kita sadari:

### A. Analogi Peta (Maps)
Bayangkan jika Google Maps menunjukkan setiap helai rumput, setiap kerikil di jalan, dan setiap daun di pohon. 
*   **Apakah berguna?** Tidak, itu justru membuat peta sangat lambat dibuka dan susah dibaca.
*   **Abstraknya**: Peta hanya menampilkan garis jalan, nama tempat, dan ikon bangunan penting. Detail seperti "warna cat pagar rumah Pak RT" dibuang karena tidak penting untuk navigasi.

### B. Analogi Menyetir Mobil
Untuk bisa menyetir mobil dari rumah ke sekolah, apakah kamu harus tahu bagaimana piston bergerak di dalam mesin atau bagaimana sistem pembakaran bensin bekerja?
*   **Jawabannya**: Tidak.
*   **Abstraknya**: Pengemudi hanya perlu memahami interface (antarmuka) sederhana: **Setir, Gas, Rem, dan Gigi**. Mesin di dalam kap mobil adalah "Black Box" (kotak hitam) yang detailnya diabstraksi bagi si pengemudi.

### C. Analogi Pemesanan Pizza
Saat memesan Pizza lewat telepon, kamu hanya peduli pada: **Jenis Pizza, Ukuran, dan Alamat Pengiriman**.
*   Kamu tidak perlu tahu siapa koki yang memasak, suhu ovennya berapa derajat, atau lewat jalur mana kurirnya berangkat.
*   Detail internal dapur itu **diabstraksi** dari pelanggan.

---

## 3. Abstraksi dalam Dunia Informatika

Dalam pemrograman dan sistem komputer, abstraksi adalah jantung dari segalanya:

### A. Ikon Interface (GUI)
Di layar HP-mu, ada ikon **Tempat Sampah (Trash)**. 
*   Secara fisik, tidak ada tempat sampah beneran di dalam HP. 
*   Ikon itu adalah **abstraksi** dari ribuan baris kode yang berfungsi menghapus lokasi memori di *storage*. Kita lebih mudah mengklik gambar tong sampah daripada menulis kode perintah hapus secara manual.

### B. Fungsi (Functions)
Pernahkah kamu menggunakan kalkulator untuk menghitung Akar Kuadrat ($\sqrt{x}$)?
*   Kamu tinggal menekan tombolnya, dan hasilnya keluar. 
*   Detail matematika rumit di balik perhitungan akar itu diabstraksi menjadi satu tombol sederhana. Dalam *coding*, ini disebut **Fungsi**.

### C. Pemodelan Data
Jika seorang programmer ingin membuat sistem "Absensi Sekolah", ia akan melakukan abstraksi pada objek **Siswa**.
*   **Data yang Penting**: Nama, NIS, Kelas, Status Kehadiran.
*   **Data yang Tidak Penting**: Hobi, makanan favorit, ukuran sepatu, warna rambut.
*   Programmer hanya mengambil data yang relevan dengan tujuan sistem.

---

## 4. Relevansi dengan OSN-K Informatika

Dalam kompetisi OSN-K, soal seringkali disajikan dalam bentuk cerita yang panjang dan bertele-tele. Kemampuan Abstraksi diuji saat kamu:
1.  **Membuang "Bumbu" Cerita**: Mengabaikan nama tokoh atau latar belakang cerita yang tidak berpengaruh pada logika matematika soal.
2.  **Membuat Model Matematika**: Mengubah cerita tentang "bebek yang berbaris" menjadi deret angka atau graf (diagram titik dan garis).
3.  **Menemukan Inti Masalah**: Langsung tahu bahwa soal tersebut sebenarnya hanyalah soal "mencari nilai terkecil" atau "mencari rute terpendek".

---


## 📚 Daftar Isi Soal

Untuk memudahkan pembacaan dan menghindari kendala rendering pada GitHub, bank soal ini dibagi menjadi beberapa bagian:

1. [Bagian 1: Soal 1 - 50](04-abstraction/04-abstraction-part-1.md)
2. [Bagian 2: Soal 51 - 100](04-abstraction/04-abstraction-part-2.md)
3. [Bagian 3: Soal 101 - 150](04-abstraction/04-abstraction-part-3.md)
4. [Bagian 4: Soal 151 - 200](04-abstraction/04-abstraction-part-4.md)
5. [Bagian 5: Soal 201 - 250](04-abstraction/04-abstraction-part-5.md)

---

[< Materi Sebelumnya: Pattern Recognition](./03-pattern-recognition/03-pattern-recognition-part-5.md) | [Materi Selanjutnya: Algorithm Design](./05-algorithm-design.md)
[< Kembali ke Beranda Materi](../README.md)
