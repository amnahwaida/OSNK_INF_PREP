# 2. Percabangan & Logika Boolean (Seni Razia Komputer)
 
 Sekarang saatnya kamu menjadi Pak Dengklek sebagai Polisi Gerbang Tol (atau Guru BP).
 Kode di OSN-K penuh dengan blok pengawal keamanan yang disebut **Percabangan (`if`, `else if`, `else`)** yang dirakit menggunakan gembok kode **Logika Boolean (`&&` AND, `||` OR)**.
 
 Mesin C++ itu **Super Kaku** dan **Super Egois Pemalas**. Mari kita bongkar anatomi kedua sikap buruk mesin ini supaya kamu tidak terjebak men-Trace cabang yang salah.
 
 ---
 
 ## 📋 A. Pemanasan: Hukum Kurung Kurawal `{ }`
 
 Sebelum masuk ke gerbang, ada satu aturan main yang paling sering menjebak murid di soal kertas: **Batas Wilayah Kekuasaan**.
 
 1. **Pakai `{ }` (Blok)**: Semua perintah di dalam kurung kurawal adalah milik si `if`.
 2. **Tanpa `{ }` (Satu Baris)**: Jika tidak ada kurung kurawal, si `if` **HANYA BERKUASA ATAS SATU BARIS** tepat di bawahnya.
 
 **Jebakan Penglihatan:**
 ```cpp
 if (x > 10)
     y = 5;
     z = 10; // Baris ini BUKAN bagian dari if! Ia akan dijalankan APAPUN yang terjadi.
 ```
 *Hati-hati:* Juri sering menaruh baris `z = 10` menjorok ke dalam (*indentasi*) padahal aslinya ia merdeka. Jangan tertipu mata!
 
 ---
 
 ## 🚦 B. Gembok Persyaratan (`if`, `else if`, `else`)
 
 Percabangan `if` menuntut pelacakan variabel di lembar buram-mu harus **100% presisi**.
 
 ```cpp
 int nyawa = 5;
 
 if (nyawa > 5) {
     printf("Bos Nyala");
 } else if (nyawa == 5) {
     printf("Siaga Satu");
 } else {
     printf("Game Over");
 }
 ```
 
 **Analisis Compiler Manusia-mu:**
 - Baris `if (nyawa > 5)`: Apakah $5$ lebih besar dari $5$? **SALAH (FALSE)**!
 - Baris `else if (nyawa == 5)`: Apakah $5$ sama presisi eksak dengan $5$?  **BENAR (TRUE)**. Cetak `Siaga Satu`.
 - **PENTING:** Begitu satu pintu terbuka (Kondisi BENAR), seluruh pintu `else` di bawahnya langsung **GHAIB / HILANG**. Mesin tidak akan mengecek pintu lainnya lagi.
 
 ---
 
 ## ⚠️ C. Jebakan Batman: `==` vs `=`
 
 OSN Informatika hobinya memakan *kewarasan* matamu:
 - `x == 5`: Ini TANDA TANYA *"Apakah X itu 5?"*
 - `x = 5`: Ini TANDA PERINTAH MUTLAK *"Ganti isi kotak X sekarang jadi bernilai 5, lalu hasilnya dianggap BENAR!"*
 
 ```cpp
 int x = 10;
 if (x = 5) { // <--- X DIPAKSA JADI 5, DAN IF-NYA TEMBUS (TRUE)!
    // Hati-hati, nilai x sekarang sudah berubah selamanya jadi 5.
 }
 ```
 
 ---
 
 ## 🧨 D. Jebakan Double-Action: Penugasan + Perbandingan
 
 Juri terkadang menggabungkan dua perintah dalam satu kurung `if`. Ini adalah gabungan dari materi Tipe Data dan Percabangan.
 ```cpp
 int a = 20;
 if ((a = 1) > 0) {
     printf("a sekarang = %d", a);
 }
 ```
 **Hukum Robot C++:**
 1. Kerjakan di dalam kurung dulu: `(a = 1)`. Artinya: "Laci `a` dibongkar isinya, diganti jadi angka **1**."
 2. Gunakan angka baru tersebut (`1`) untuk dibandingkan: `1 > 0`.
 3. Apakah `1 > 0`? **BENAR (TRUE)**!
 4. Hasil cetaknya: **`a sekarang = 1`**. 
 *(Jangan terjebak mengira `a` masih 20! Juri baru saja "mencuci otak" variabelmu).*
 
 ---
 
 ## ⛓️ E. Jebakan Rantai Palsu (`10 < 5 < 20`)
 
 Hati-hati, kodingan di kertas seringkali mencoba membodohi insting matematika-mu! Bisakah kamu menebak hasil `if (10 < 5 < 20)`?
 - **Robot C++:** "Oit, gue kerjain dari kiri!"
   1. `10 < 5` dihitung duluan, hasilnya **0** (False).
   2. Sekarang rumusnya jadi `0 < 20`.
   3. Apakah 0 lebih kecil dari 20? **BETUL BANGET (TRUE)**!
 
 **Pelajaran:** Jangan pernah menggabung perbandingan seperti gerbong kereta api. Gunakan `&&` jika ingin mengecek rentang angka. (Contoh: `if (10 < 5 && 5 < 20)`).
 
 ---
 
 ## ⚡ F. Operator Logika (`&&`, `||`, `!`)
 
 - `&&` (DAN / AND): DUA-DUANYA WAJIB BENAR!
 - `||` (ATAU / OR): CUKUP SALAH SATU AJA BENAR, BERES!
 - `!` (TIDAK / NOT): Kacamata kebalikan (Benar jadi Salah).
 
 ---
 
 ## ⚖️ G. Hukum Kasta Logika (Siapa Lebih Kuat?)
 
 Jika ada banyak operator logika berjejer tanpa kurung, ikuti urutan kasta ini:
 1. `!` (Kasta Tertinggi / Penguasa)
 2. `&&` (Kasta Menengah / Lengket)
 3. `||` (Kasta Rakyat / Longgar)
 
 *Contoh:* `A || B && C` dikerjakan sebagai `A || (B && C)`. **AND lebih lengket daripada OR!**
 
 ---
 
 ## 💤 H. Evaluasi Sirkuit-Pendek (Sirkuit Pemalas)
 
 Mesin C++ sifatnya egois memikirkan jalan pintas (**Short-Circuit Evaluation**).
 
 **1. Kemalasan AND (`&&`)**
 Dalam `A && B`, **JIKA KONDISI `A` SUDAH FALSE**, C++ **MENOLAK MEMBACA KONDISI `B`!**
 - *Analogi:* Jika syarat masuk klub adalah (Bawa KTP && Bawa Tiket). Begitu kamu bilang "Saya gak bawa KTP", penjaga pintu langsung mengusirmu tanpa peduli kamu bawa tiket atau tidak.
 
 **2. Kemalasan OR (`||`)**
 Dalam `A || B`, **JIKA KONDISI `A` SUDAH TRUE**, C++ **MENOLAK MEMBACA KONDISI `B`!**
 - *Analogi:* Jika syarat dapet permen adalah (Punya Kupon Biru || Punya Kupon Merah). Begitu kamu sodorkan Kupon Biru, kamu langsung dapet permen. Penjaga gak akan tanya lagi kamu punya kupon merah atau nggak. Hadiah sudah di tangan!
 
 ---
 
 ## 🧬 I. Misteri "Angka adalah Kebenaran"
 
 Di kodingan OSN-K, kamu akan sering melihat `if` yang isinya angka mentah, bukan perbandingan.
 ```cpp
 int x = 5;
 if (x) { ... }
 ```
 **Aturan Robot C++:**
 - **Angka `0`** = **FALSE** (Salah).
 - **Angka APAPUN SELAIN `0`** (1, 5, -100, 999) = **TRUE** (Benar).
 
 ---
 
 ## 🎰 J. Vending Machine (`switch - case`)
 
 Kadang kita punya banyak pilihan angka yang saklek. Daripada pakai `else if` kepanjangan, C++ pakai `switch`.
 ```cpp
 switch (pilih) {
     case 1: printf("Kopi"); break;
     case 2: printf("Teh"); break;
     default: printf("Air Putih");
 }
 ```
 **Jebakan `break`:** Jika ada `case` yang lupa dikasih `break`, mesin akan "Bablas" menjalankan perintah di bawahnya secara berurutan sampai ketemu `break` berikutnya!
 
 ---
 
 ## ✂️ K. Cabang Kilat (Ternary Operator `? :`)
 
 Inilah cara orang sibuk menulis `if-else` dalam satu baris.
 ```cpp
 int hasil = (uang > 10) ? 100 : 0;
 ```
 **Cara Baca:** `"Apakah uang > 10? Jika IYA ambil 100, Jika TIDAK ambil 0"`.
 Struktur: `(Kondisi) ? [Jika Benar] : [Jika Salah];`
 
 ---
 
 ## 🕵️ L. Misteri "Dangling Else" (Siapa Pemilik Gembok?)
 
 Jika kamu melihat kode bertingkat tanpa tanda kurung `{ }`, siapakah pemilik `else` yang sebenarnya?
 ```cpp
 if (a > 5)
     if (b > 10)
         printf("Jackpot!");
 else
     printf("Zonk!");
 ```
 - **Insting Murid:** "Kalau `a > 5` salah, pasti lari ke `else Zonk!`."
 - **Hukum C++ (Dangling Else):** "`else` akan selalu menempel pada `if` paling dekat di atasnya yang belum punya pasangan."
 - Jadi, `else Zonk!` di atas adalah milik `if (b > 10)`. Kalau `a > 5` saja sudah salah, program **TIDAK AKAN MENCETAK APAPUN** (Karena `else` ikut hilang bersama `if` induknya yang dia tempel).
 
 ---
 
 ## 🌀 M. Analogi Labirin Keputusan
 
 ### 🚪 1. Nested If: Pintu Keamanan Berlapis
 Syarat di dalam hanya diperiksa jika syarat luar sudah lolos. (Sidik jari hanya diminta jika PIN kartu sudah benar).
 
 ### 🍜 2. Else-If Chain: Menu Kantin
 Begitu satu pilihan (Soto) tersedia, kamu kenyang dan tidak mencolek pilihan lain (Bakso/Mie Ayam).
 
 ---
 
 ## 📜 N. Rangkuman: Cara Berpikir Cabang
 
 1. **Pintu Tunggal**: Dalam satu blok `if-else if-else`, **Cuma ada SATU** blok yang bisa tembus.
 2. **Sirkuit Pendek**: Selalu cek sisi kiri `&&` atau `||` dulu. Kalau sudah cukup menentukan hasil, abaikan sisi kanan (jangan di-trace!).
 3. **Indentasi Menipu**: Jangan percaya spasi/tab. Percayalah pada `{ }`. Kalau tidak ada, cuma 1 baris di bawahnya yang dikuasai.
 
 ---
 
 ### Siap Di Uji Tracing?
 
 ```cpp
 int a = 10;
 int b = 0;
 
 if (a > 5 || (b++ > 0)) {
     if (a == 10) b += 5;
 }
 printf("b = %d", b);
 ```
 
 **Diagnosis Logika:**
 1. `if (a > 5 || ...)` $\rightarrow$ `10 > 5` adalah **TRUE**.
 2. Karena konektornya `||` (OR) dan kiri sudah **TRUE**, mesin **MALAS** membaca sebelah kanan.
 3. `(b++ > 0)` **DIBUANG/DIABAIKAN**. Nilai `b` masih `0`.
 4. Masuk ke Nested If: `if (a == 10)` $\rightarrow$ `10 == 10` is **TRUE**.
 5. `b += 5` $\rightarrow$ `b` jadi `0 + 5 = 5`.
 6. Hasil akhir: **`b = 5`**.
 
 ---
 
 ### 📝 Latihan Soal Tracing
 👉 **[Bank Soal Modul 02: Percabangan (300 Soal)](./latihan/README.md)**
 
 ---
 
 ⏩ **Lanjut ke Modul Ketiga:** [Perulangan & Mesin Array (Trek Lari)](../03-perulangan-dan-manipulasi-array/materi.md)
