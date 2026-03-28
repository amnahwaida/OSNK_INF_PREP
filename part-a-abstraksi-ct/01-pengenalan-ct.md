# 01. Pengenalan Computational Thinking

**Computational Thinking (CT)** bukan hanya tentang cara memprogram komputer, melainkan cara manusia berpikir untuk menyelesaikan masalah secara sistematis dan efisien.

## 4 Pilar Utama CT

### 1. Decomposition (Dekomposisi)
**Membagi masalah besar menjadi bagian-bagian kecil** yang lebih mudah dipahami dan dikelola.
- **Analogi**: Saat Anda ingin merakit set LEGO yang besar, Anda tidak membukanya semua sekaligus. Anda mulai dengan merakit bagian dasar, lalu dinding, lalu atap.
- **Contoh di Informatika**: Sebelum membuat aplikasi "Chatting", kita membaginya menjadi: sistem registrasi, sistem pengiriman pesan, dan sistem database.

### 2. Pattern Recognition (Pengenalan Pola)
**Mencari kesamaan atau keteraturan** di dalam masalah yang pernah kita temui.
- **Analogi**: Anda tahu kapan harus membawa payung karena Anda mengenali pola awan mendung dan kelembapan udara yang biasanya berujung pada hujan.
- **Contoh di Informatika**: Programmer menggunakan "loop" (perulangan) karena mereka menyadari ada instruksi yang dilakukan secara berulang-ulang dengan pola yang sama.

### 3. Abstraction (Abstraksi)
**Fokus hanya pada informasi penting** dan mengabaikan detail-detail yang tidak relevan dengan solusi.
- **Analogi**: Saat Anda menggunakan remote TV, Anda cukup tahu tombol mana untuk "Volume Up". Anda tidak perlu tahu bagaimana sinyal inframerah tersebut dikirim atau bagaimana sirkuit listrik di dalamnya bekerja.
- **Contoh di Informatika**: Menggunakan fungsi `print()` tanpa harus tahu bagaimana komputer memerintahkan piksel pada layar untuk menyala satu per satu.

### 4. Algorithm Design (Perancangan Algoritma)
**Menyusun langkah-langkah logis** (set instruksi) untuk menyelesaikan masalah secara berurutan.
- **Analogi**: Sebuah resep masakan yang menjelaskan urutan memotong bahan, memasak, hingga menghidangkan.
- **Contoh di Informatika**: Menentukan urutan pengecekan login: 1) Cek username ada di database, 2) Cek password cocok, 3) Jika ya, arahkan ke dashboard.

---

## 🏆 Mengapa CT Penting untuk OSN-K?

Di OSN-K Informatika, Anda akan menemui banyak soal yang seolah-olah "tidak ada hubungannya dengan coding". Namun, di situlah letak ujian sesungguhnya.

| Pilar CT | Penerapan di Soal OSN-K |
| :--- | :--- |
| **Decomposition** | Memecah soal cerita yang panjang menjadi poin-poin data yang diketahui. |
| **Pattern Recognition** | Mengenali bahwa sebuah soal sebenarnya adalah variasi dari soal "Knapsack" atau "Shortest Path". |
| **Abstraction** | Mengabaikan narasi cerita (misal: "Budi pergi ke pasar...") dan fokus pada graf/angka di baliknya. |
| **Algorithm Design** | Melakukan *dry run* pada algoritma manual yang diberikan di soal Part B. |

### Tips OSN-K:
Seringkali, soal OSN-K memberikan batasan waktu yang sangat ketat. Gunakan **Abstraksi** untuk membuang distraktor dan **Pengenalan Pola** untuk menemukan cara cepat (shortcut) tanpa harus menghitung manual satu per satu.

---

## ❓ Latihan Soal Lanjut

### Soal #01: Konsep Abstraksi
*(Lihat di atas)*

### Soal #02: Konsep Dekomposisi
*(Lihat di atas)*

### Soal #03: Konsep Pengenalan Pola
*(Lihat di atas)*

### Soal #04: Konsep Algoritma
*(Lihat di atas)*

### Soal #05: Abstraksi dalam Graf
Diberikan sebuah peta kota dengan 10 persimpangan dan 15 jalan. Setiap jalan memiliki batasan beban kendaraan. Anda diminta mencari rute tercepat dari titik A ke B. Dalam proses ini, Anda memutuskan untuk mengabaikan jenis aspal jalan dan warna lampu merah di setiap persimpangan.
Pilar CT apa yang Anda gunakan?
A. Decomposition  
B. Pattern Recognition  
C. Abstraction  
D. Algorithm Design  

<details>
<summary>💡 Hint</summary>
Anda membuang informasi "aspal" dan "warna lampu" karena tidak berpengaruh pada "rute tercepat".
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
