# 01. Pengenalan Computational Thinking

**Computational Thinking (CT)** bukan hanya tentang cara memprogram komputer, melainkan cara manusia berpikir untuk menyelesaikan masalah secara sistematis dan efisien.

## 4 Pilar Utama CT

### 1. Decomposition (Dekomposisi)
**Membagi masalah besar menjadi bagian-bagian kecil** yang lebih mudah dipahami dan dikelola.
- **Analogi LEGO**: Saat merakit set LEGO besar, Anda merakit bagian per bagian (seperti roda dulu, lalu badan mobil).
- **Contoh Kehidupan Nyata**: Memasak makan malam besar untuk keluarga. Anda membaginya menjadi: belanja bahan, memotong sayur, memasak nasi, dan menggoreng lauk.
- **Contoh di Informatika**: Sebelum membuat aplikasi "Chatting", kita membaginya menjadi: sistem registrasi, fitur pengiriman pesan, dan penyimpanan data.

### 2. Pattern Recognition (Pengenalan Pola)
**Mencari kesamaan atau keteraturan** di dalam masalah yang pernah kita temui.
- **Analogi Cuaca**: Anda membawa payung karena mengenali pola awan mendung dan kelembapan udara yang biasanya berujung pada hujan.
- **Contoh Kehidupan Nyata**: Menyadari bahwa setiap hari Jumat sore jalanan di depan rumah selalu macet parah karena orang pulang kantor lebih awal.
- **Contoh di Informatika**: Programmer menggunakan "loop" (perulangan) karena menyadari ada instruksi yang dilakukan secara berulang dengan pola yang sama.

### 3. Abstraction (Abstraksi)
**Fokus hanya pada informasi penting** dan mengabaikan detail yang tidak relevan.
- **Analogi Remote TV**: Anda cukup tahu tombol "Volume Up" menambah suara. Anda tidak perlu tahu bagaimana sinyal inframerah bekerja di dalamnya.
- **Contoh Kehidupan Nyata**: Menggunakan Smartphone. Anda bisa menelepon tanpa harus tahu bagaimana prosesor mengolah sinyal radio atau bagaimana layar sentuh bekerja secara mendalam.
- **Contoh di Informatika**: Menggunakan fungsi `print()` untuk menampilkan teks di layar tanpa tahu bagaimana perintah tersebut mengontrol ribuan piksel secara elektrik.

### 4. Algorithm Design (Perancangan Algoritma)
**Menyusun langkah-langkah logis** (set instruksi) untuk menyelesaikan masalah secara berurutan.
- **Analogi Resep**: Sebuah resep masakan yang menjelaskan urutan memotong bahan, memasak, hingga menghidangkan.
- **Contoh Kehidupan Nyata**: Langkah-langkah mengikat tali sepatu atau urutan memakai seragam sekolah dari awal sampai rapi.
- **Contoh di Informatika**: Menentukan urutan pengecekan login: 1) Cek username, 2) Cek password, 3) Jika benar, arahkan ke dashboard.

---

## 🏆 Mengapa CT Penting untuk OSN-K?

Di OSN-K Informatika, banyak soal yang seolah-olah "tidak ada hubungannya dengan coding". Namun, di situlah letak ujian sesungguhnya.

| Pilar CT | Penerapan di Soal OSN-K |
| :--- | :--- |
| **Decomposition** | Memecah soal cerita yang panjang menjadi poin-poin data yang diketahui. |
| **Pattern Recognition** | Mengenali bahwa sebuah soal sebenarnya adalah variasi dari soal "Knapsack" atau "Shortest Path". |
| **Abstraction** | Mengabaikan narasi cerita (misal: "Budi pergi ke pasar...") dan fokus pada graf/angka di baliknya. |
| **Algorithm Design** | Melakukan *dry run* pada algoritma manual yang diberikan di soal Part B. |

### Tips OSN-K:
Gunakan **Abstraksi** untuk membuang distraktor dan **Pengenalan Pola** untuk menemukan shortcut tanpa harus menghitung manual satu per satu.

---

## ❓ Latihan Soal

### Soal #01: Konsep Abstraksi
Manakah dari berikut ini yang merupakan contoh **Abstraksi** dalam kehidupan sehari-hari?
A. Memasak nasi dengan mengikuti langkah-langkah di bungkus beras.
B. Melihat peta kereta api yang hanya menampilkan jalur dan stasiun, tanpa detail jalan raya atau gedung di atasnya.
C. Membagi tugas membersihkan rumah menjadi: menyapu, mengepel, dan cuci piring.
D. Menyadari bahwa setiap hari Senin jam 7 pagi jalanan selalu macet.

<details>
<summary>💡 Hint</summary>
Pikirkan tentang "penyederhanaan" dan "pengabaian detail".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Melihat peta kereta api.**
Peta tersebut mengabaikan detail yang tidak relevan (gedung, pohon, gang kecil) agar pengguna fokus pada informasi yang dibutuhkan (rute kereta).
</details>

### Soal #02: Konsep Dekomposisi
Andi ingin memperbaiki sepeda yang rantainya sering lepas. Langkah pertama yang dilakukan Andi adalah memeriksa kondisi gigi sepeda, lalu kondisi rantai, lalu posisi gir belakang. 
Teknik CT apa yang sedang diterapkan Andi?
A. Decomposition  
B. Pattern Recognition  
C. Abstraction  
D. Algorithm Design  

<details>
<summary>💡 Hint</summary>
Andi memecah masalah besar "Sepeda Rusak" menjadi pemeriksaan pada "Gigi", "Rantai", dan "Gir".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Decomposition.**
Andi membagi masalah sistem sepeda yang kompleks menjadi komponen-komponen yang lebih kecil untuk diperiksa satu per satu.
</details>

### Soal #03: Konsep Pengenalan Pola
Seorang dokter melihat riwayat pasien yang sering batuk setiap kali musim bunga tiba (bulan Oktober-November). Dokter tersebut menyimpulkan bahwa pasien memiliki alergi musiman.
Pilar CT manakah yang paling menonjol digunakan dokter tersebut?
A. Abstraction  
B. Pattern Recognition  
C. Algorithm Design  
D. Decomposition  

<details>
<summary>💡 Hint</summary>
Dokter melihat "kejadian yang berulang" di waktu yang sama setiap tahun.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pattern Recognition.**
Dokter mengenali keteraturan waktu (Oktober-November) dan gejala yang sama (batuk) untuk membuat kesimpulan.
</details>

### Soal #04: Konsep Algoritma
Urutkan instruksi berikut agar menjadi algoritma membuat teh manis yang benar:
1. Tuangkan air panas ke dalam gelas.
2. Masukkan kantong teh dan celupkan hingga air berubah warna.
3. Tambahkan gula secukupnya.
4. Siapkan gelas dan sendok.
5. Aduk hingga gula larut.

A. 4-1-2-3-5  
B. 1-2-3-4-5  
C. 4-2-1-3-5  
D. 4-1-3-2-5  

<details>
<summary>💡 Hint</summary>
Perhatikan prasyarat (pre-condition) sebelum melakukan langkah berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4-1-2-3-5** (Mempersiapkan alat -> Tuang air -> Teh -> Gula -> Aduk).
</details>

### Soal #05: Abstraksi dalam Graf
Diberikan sebuah peta kota dengan 10 persimpangan dan 15 jalan. Setiap jalan memiliki batasan beban kendaraan. Anda diminta mencari rute tercepat dari titik A ke B. Dalam proses ini, Anda memutuskan untuk mengabaikan jenis aspal jalan dan warna lampu merah di setiap persimpangan.
Pilar CT apa yang Anda gunakan?
A. Decomposition  
B. Pattern Recognition  
C. Abstraction  
D. Algorithm Design  

<details>
<summary>💡 Hint</summary>
Anda membuang informasi "aspal" dan "warna lampu" karena tidak berpengaruh pada rute tercepat.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Abstraction.**
Menyaring informasi yang tidak relevan dengan tujuan akhir adalah inti dari Abstraksi.
</details>

### Soal #06: Pola dalam Barisan Bilangan
Seorang kontestan OSN melihat sebuah barisan: 2, 6, 12, 20, 30, ...
Ia menyadari bahwa angka ke-n dapat dirumuskan sebagai $n \times (n+1)$. 
Apa pilar CT yang digunakan untuk menemukan rumus tersebut?
A. Decomposition  
B. Pattern Recognition  
C. Abstraction  
D. Algorithm Design  

<details>
<summary>💡 Hint</summary>
Kontestan tersebut mencari "aturan umum" dari sekumpulan data yang ada.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pattern Recognition.**
Menemukan keteraturan atau formula umum dari data numerik adalah contoh pengenalan pola.
</details>

### Soal #07: Algoritma Pencarian Efektif
Jika Anda diminta mencari satu kata di dalam kamus setebal 1000 halaman, dan Anda memilih untuk membuka halaman tengah, lalu membuang setengah bagian yang tidak mungkin berisi kata tersebut, dan mengulangi langkah tersebut hingga ketemu. 
Strategi ini merupakan perancangan...
A. Decomposition  
B. Pattern Recognition  
C. Abstraction  
D. Algorithm Design  

<details>
<summary>💡 Hint</summary>
Ini adalah langkah-langkah sistematis (Binary Search) untuk mencapai solusi.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Algorithm Design.**
Meskipun menggunakan pemecahan masalah (binary search), fokus pada "langkah-langkah prosedur" menjadikannya perancangan algoritma.
</details>

---
[< Kembali ke Materi Part A](./README.md)
