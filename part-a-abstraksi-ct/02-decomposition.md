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

---
[< Kembali ke Beranda Materi](../README.md) | [Materi Selanjutnya: Pattern Recognition](./03-pattern-recognition.md)
