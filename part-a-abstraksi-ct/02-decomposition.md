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

---
[< Kembali ke Beranda Materi](../README.md) | [Materi Selanjutnya: Pattern Recognition](./03-pattern-recognition.md)
