# Part C: Pemahaman Kode C++ (Compiler Manusia)

Selamat datang di Tahap Akhir Simulasi OSN-K Informatika! 🏆

Jika Part A melatih **Logika Abstraksimu** dan Part B melatih **Naluri Jejak Algoritmamu**, maka Part C ini adalah **Batalyon Pengeksekusi**.
Di sinilah kamu akan diuji kemampuannya untuk membaca, membedah, dan meniru cara kerja komputer saat mengeksekusi kumpulan teks bahasa alien bernama: `C++`.

Jangan panik! Di OSN-K, kamu **TIDAK DIMINTA MENGODING DARI NOL DI DEPAN KOMPUTER**. 
Tugasmu hanyalah menjadi *"Compiler Manusia"*: Duduk tenang memegang pensil, membaca kodingan C++ yang sudah disediakan juri di kertas soal, dan menebak: *"Nih kodingan bakal ngeluarin angka berapa ya di layar?"*

Untuk bisa meramal *output* tersebut dengan presisi $100\%$, kita akan membedah 6 pilar anatomi C++ menggunakan bahasa kehidupan nyata anak SMA sehari-hari:

---

## 📚 Indeks Materi Part C

### 1. [Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)](./01-tipe-data-dan-operator-dasar.md)
Bagaimana komputer menyimpan identitas barang? Mengapa membagi angka `5 / 2` di C++ hasilnya malah `2` (bukan $2.5$)? Kita bahas sifat kejam kotak *Integer* dan seni memanipulasi sisa bagi (*Modulo* `%`) layaknya bagi-bagi kelereng mutlak tanpa pecahan.

### 2. [Percabangan & Logika Boolean (Razia Guru BP)](./02-percabangan-dan-boolean-logika.md)
Kapan blok kode dieksekusi dan kapan diabaikan? Memahami gerbang logika `If-Else` dan sifat egois evaluasi sirkuit pendek (`Short-Circuit && dan ||`). Kalau rambutmu sudah panjang (Salah di syarat pertama), Guru BP tidak sudi lagi mengecek warna sepatumu di syarat kedua!

### 3. [Perulangan & Array (Trek Lari & Playlist Spotify)](./03-perulangan-dan-manipulasi-array.md)
Membedah putaran `For`, `While`, dan `Do-While`. Memahami batas akhir iterasi sebuah Array (`Index Out of Bounds`). Termasuk membedah kekuatan gaib tombol `Break` (Hancurkan mesin lagunya, berhenti lari!) vs tombol `Continue` (Lagu ini jelek, letih, tolong di-Skip ke lagu sebelahnya!).

### 4. [Fungsi & Parameter (Nyontek PR Tip-Ex)](./04-fungsi-dan-parameter-referensi.md)
OSN-K sangat memuja trik jebakan lempar-lemparan fungsi. Bedakan antara *Pass-by-Value* (Minta tolong dikirim Fotokopian PR-nya, jadi kalau dirobek gak ngaruh ke aslinya) versus *Pass-by-Reference* simbol `&` (Meminjamkan BUKU ASLI PR-mu kepada teman, jika dia coret-coret Tip-Ex maka tugasmu ikut bocor dan berubah!).

### 5. [Rekursi & Call Stack (Tugas Rantai Minta Uang Jajan)](./05-rekursi-dan-call-stack.md)
Bos terakhir kodingan OSN-K! "Fungsi yang memanggil dirinya sendiri". Jangan dihafal lurus, tapi proyeksikan layaknya *Tumpukan Piring (LIFO)* yang mundur berantai. Adik minta Ibu, Ibu minta Ayah, Ayah ke Mesin ATM. Rekursi takkan tercetak ke layar sebelum "Uang Ayah cair dari ATM" (Base Case tercapai).

### 6. [Operasi Bitwise Tingkat Lanjut (Cheat Code Tombol Rahasia)](./06-operasi-bitwise-dasar.md)
Array dimanipulasi dengan operator planet luar `&, |, ^, <<, >>`. Kita singkirkan desimal matematika dan pakai analogi *Saklar Lampu LED*. Membongkar trik sakti `XOR (^)` si pembalik keadaan yang setia (tombol ditekan ganjil menyala, ditekan genap kembali mati alias lenyap!).

---

Sudah memanaskan ujung pensil burammu? 
Ayo kita mulai menerjemahkan bahasa alien pertama: **[01 - Tipe Data & Operator Dasar](./01-tipe-data-dan-operator-dasar.md)**!
