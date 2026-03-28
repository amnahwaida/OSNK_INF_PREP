# 2. Percabangan & Logika Boolean (Seni Razia Komputer)
 
 Selamat datang di gerbang logika! Di sini, kode C++ tidak lagi berjalan lurus seperti kereta api, tapi mulai bercabang seperti labirin. Sebagai *Compiler Manusia*, tugasmu adalah menentukan **jalur mana yang benar-benar dilewati** dan **jalur mana yang cuma fatamorgana**.
 
 Mesin C++ itu **Super Kaku** dan **Sangat Malas**. Mari kita pelajari sifat aslinya agar kamu tidak tersesat dalam percabangan.
 
 ---
 
 ## 📋 A. Hukum Kurung Kurawal `{ }` (Wilayah Kekuasaan)
 
 Masalah nomor satu pemula adalah mengira `if` berkuasa atas banyak baris di bawahnya. 
 - **Aturan Emas:** Jika tidak ada `{ }`, si `if` **HANYA** memimpin **satu baris** (sampai ketemu titik koma `;` pertama).
 
 **Analogi "Raja Tanpa Tembok":**
 ```cpp
 if (uang > 100)
     belanja();   // <--- Ini rakyat si Raja if.
     nabung();    // <--- Ini rakyat merdeka! Dia jalan terus, mau uangnya banyak atau sedikit.
 ```
 *Tips Tracing:* Selalu tarik garis lurus dari `if`. Jika tidak ada kurung, baris kedua dan seterusnya *selalu* dijalankan terlepas kondisinya benar atau salah.
 
 ---
 
 ## 🚦 B. Gembok Persyaratan (`if`, `else if`, `else`)
 
 Pikirkan ini sebagai **Filter Bertingkat**.
 1. **`if`**: Saringan pertama. Kalau lolos, yang lain diabaikan.
 2. **`else if`**: Saringan cadangan (Hanya dicek jika saringan di atasnya gagal).
 3. **`else`**: Jaring pengaman terakhir. Kalau semua saringan di atas gagal, secara otomatis masuk ke sini.
 
 **Analogi "Pintu VIP":**
 Begitu kamu masuk lewat pintu `if`, pengawal langsung **membakar habis** pintu `else if` dan `else`. Kamu tidak bisa (dan tidak perlu) menengok ke pintu-pintu lain lagi.
 
 ---
 
 ## ⚠️ C. Jebakan Batman: `==` vs `=`
 
 Ini adalah jebakan "Salah Ketik" yang sering disengaja oleh juri:
 - `x == 5`: "Tanda Tanya" $\rightarrow$ "Halo, apakah kamu angka 5?"
 - `x = 5`: "Tanda Seru/Perintah" $\rightarrow$ "Kamu sekarang jadi angka 5, titik!"
 
 **Efek Samping:** Jika kamu menulis `if (x = 5)`, laci `x` yang tadinya berisi 100 akan **terhapus permanen** dan diganti jadi 5. Kondisinya juga dianggap **TRUE** karena 5 bukan nol.
 
 ---
 
 ## 🧨 D. Jebakan Double-Action: Penugasan + Perbandingan
 
 Kadang juri ingin melihat apakah kamu bisa melakukan dua hal sekaligus dalam satu tarikan napas.
 ```cpp
 if ((a = 0) == 0) { ... }
 ```
 **Cara Tracingnya:**
 1. Kerjakan di dalam kurung: `a = 0`. Sekarang laci `a` resmi jadi **0**.
 2. Bandingkan hasilnya: `0 == 0`.
 3. Hasilnya **TRUE**! (Tapi ingat, isi `a` sekarang sudah jadi nol).
 
 ---
 
 ## ⛓️ E. Jebakan Rantai Palsu (`10 < 5 < 20`)
 
 Di matematika, ini salah. Di C++, ini benar. Kok bisa?
 - **Robot C++ itu Bertahap:** 
   1. Dia hitung `10 < 5`. Hasilnya **0** (False).
   2. Sekarang rumusnya jadi `0 < 20`.
   3. Apakah 0 lebih kecil dari 20? **BETUL BANGET (TRUE)**!
 
 ---
 
 ## ⚡ F. Operator Logika (`&&`, `||`, `!`)
 
 - `&&` (DAN): Harus **Kompak Benar**. Satu saja salah, semua hancur.
 - `||` (ATAU): Harus **Ada yang Benar**. Satu saja benar, semua selamat.
 - `!` (TIDAK): **Kacamata Terbalik**. (True jadi False, False jadi True).
 
 ---
 
 ## ⚖️ G. Hukum Kasta Logika (Precedence)
 
 Sama seperti perkalian dikerjakan sebelum pertambahan, operator logika juga punya kasta:
 1. `!` (Kasta Tertinggi/Diktator) $\rightarrow$ Dikerjakan paling awal.
 2. `&&` (Kasta Menengah/Geng Motor) $\rightarrow$ Sangat lengket satu sama lain.
 3. `||` (Kasta Rakyat/Geng Sepeda) $\rightarrow$ Paling longgar, dikerjakan terakhir.
 
 ---
 
 ## 💤 H. Evaluasi Sirkuit-Pendek (Robot Pemalas)
 
 Ini adalah sifat paling penting untuk menghemat waktu tracing:
 **1. Kemalasan AND (`&&`)**: Jika sisi kiri sudah **SALAH**, abaikan sisi kanan. (Gak mungkin benar kalau salah satu udah salah).
 **2. Kemalasan OR (`||`)**: Jika sisi kiri sudah **BENAR**, abaikan sisi kanan. (Hadiah udah dapet, buat apa cek syarat lain?).
 
 ---
 
 ## 🧬 I. Misteri "Angka adalah Kebenaran"
 
 Mengapa `if(5)` itu benar tapi `if(0)` itu salah?
 - **Filosofi Biner:** Di C++, angka **0** adalah kegelapan (False). Angka lainnya (1, -5, 999) adalah cahaya (True). 
 
 ---
 
 ## 🎰 J. Vending Machine (`switch - case`)
 
 Gunakan ini jika pilihannya banyak dan angkanya pasti (diskrit).
 
 ### 🛠️ Cara Kerja & Komponen:
 - **`switch (variabel)`**: Masukkan laci yang ingin diperiksa.
 - **`case 1:`**: Jika isi laci adalah 1, jalankan baris di bawahnya.
 - **`break;`**: REM darurat! Jika tidak ada ini, mesin akan "Bablas" menjalankan bawahnya.
 - **`default:`**: Jaring pengaman. Jalankan ini jika tidak ada `case` yang cocok.
 
 ### 💡 Tip Pro: Jurus "Bablas" Berjamaah
 Terkadang kita **sengaja** tidak memasang `break` untuk menangani beberapa pilihan sekaligus.
 ```cpp
 switch (hari) {
     case 1:
     case 2:
     case 3:
     case 4:
     case 5: printf("Kerja!"); break;
     case 6:
     case 7: printf("Libur!"); break;
 }
 ```
 
 ### 🛠️ Kupas Tuntas: Break & Default
 
 **1. Mengapa Perlu `break`? (Aturan Lift)**
 Bayangkan kamu naik **Lift**. Jika kamu ingin ke lantai 3, kamu menekan tombol 3. Begitu sampai di lantai 3, kamu **KELUAR** dari lift.
 - Di C++, `break;` adalah perintah untuk **"Keluar dari Lift"**.
 - Tanpa `break;`, lift tersebut akan **terus berjalan** turun ke lantai di bawahnya secara otomatis. Ia akan menjalankan semua perintah `case` berikutnya sampai ketemu `break` baru atau mentok di ujung.
 
 **2. Mengapa Perlu `default`? (Jaring Pengaman)**
 `default` adalah bagian yang akan dijalankan jika **TIDAK ADA** satupun `case` yang cocok.
 - Pikirkan ini sebagai **"Aksi Darurat"**.
 - Tanpa `default`, jika tidak ada angka yang cocok, programmu hanya akan diam saja dan melompat keluar tanpa kabar. Dengan `default`, kamu bisa memberitahu user: "Woi, pilihan kamu gak ada di menu!".
 - *Fakta Menarik:* `default` biasanya diletakkan paling bawah, sehingga ia tidak butuh `break;` lagi karena sudah berada di pintu keluar.
 
 ### 🌍 Pemanasan di Program Nyata:
 Di dunia nyata, `switch` adalah pahlawan untuk menu navigasi. Bayangkan kamu membuat **Game Petualangan**:
 ```cpp
 char input;
 cin >> input; // Misal kita ketik 'a'
 
 switch (input) {
     case 'w': y++; break; // Jalan maju
     case 's': y--; break; // Jalan mundur
     case 'a': x--; break; // Jalan kiri
     case 'd': x++; break; // Jalan kanan
     default: printf("Tombol Salah!"); // User ngaco
 }
 ```
 **Diagnosis Logika Game:**
 1. **Pencarian Label**: Begitu `input` berisi `'a'`, mesin segera mencari label `case 'a'`.
 2. **Eksekusi Lokal**: Mesin masuk ke baris `x--;` dan mengeksekusinya (koordinat x berkurang).
 3. **Rem Aktif**: Karena ada `break;`, mesin berhenti di situ dan langsung melompat keluar gerbang `switch`. Ia tidak akan peduli dengan `case 'd'` atau `default`.
 4. **Aksi Darurat**: Jika kita mengetik `'z'`, mesin tidak menemukan label yang cocok, maka ia meluncur ke dasar yaitu `default` dan mengomeli kita dengan "Tombol Salah!".
 
 ---
 
 ## ✂️ K. Cabang Kilat (Ternary Operator `? :`)
 
 Inilah cara orang sibuk menulis `if-else` dalam satu baris. Pikirkan ini sebagai **"Jalan Pintas"** untuk mengisi nilai laci berdasarkan satu syarat singkat.
 
 ### 📐 Struktur Anatomi:
 `(Kondisi) ? [Nilai Jika Benar] : [Nilai Jika Salah];`
 
 ### 🌍 Pemanasan di Program Nyata:
 
 **1. Mencari Angka Terbesar (The Boss Finder)**
 Daripada menulis 4 baris `if-else`, kamu cukup satu baris:
 ```cpp
 int max_val = (a > b) ? a : b; // Siapa yang menang, dia yang masuk ke laci.
 ```
 
 **2. Cek Lulus/Gagal (Sistem Raport)**
 ```cpp
 printf("%s", (skor >= 75) ? "LULUS" : "REMEDIAL");
 ```
 
 **3. Penentu Genap-Ganjil (Logistik)**
 ```cpp
 string label = (x % 2 == 0) ? "GENAP" : "GANJIL";
 ```
 
 **Diagnosis Logika Kilat:**
 1. **Evaluasi Cepat**: Mesin pertama-tama fokus menghitung yang di dalam kurung `()`, misal `80 >= 75`.
 2. **Pilih Jalur**:
    - Jika **BENAR (TRUE)**: Mesin melompat melewati tanda tanya `?` dan mengambil paket data pertama ("LULUS").
    - Jika **SALAH (FALSE)**: Mesin meluncur melewati titik dua `:` dan mengambil paket data kedua ("REMEDIAL").
 3. **Hasil Akhir**: Data yang terpilih itulah yang akan masuk ke laci variabel atau ditampilkan di layar.
 
 > [!WARNING]
 > **Jangan Berlebihan!** Ternary memang keren, tapi jangan menumpuk Ternary di dalam Ternary (`? ? : :`). Hal itu akan membuat kodemu terbaca seperti bahasa alien yang membingungkan bagi mata manusia (dan muridmu). Gunakan hanya untuk perbandingan **pendek dan sederhana**.
 
 ---
 
 ## 🕵️ L. Misteri "Dangling Else" (Siapa Pemilik Gembok?)
 
 Jika ada `else` nyasar tanpa `{ }`, carilah `if` terdekat tepat di atasnya yang masih jomblo (belum punya pasangan `else`).
 - Jangan tertipu tanda spasi atau tab. Juri sengaja menjauhkan `else` dari pasangannya agar kamu bingung. Berhati-hatilah!
 
 ---
 
 ## 🍜 M. Strategi Memilih Gembok (Workflow Terpercaya)
 
 - **Gunakan `if - else if`**: Jika hadiahnya cuma boleh satu (Pilih Soto atau Bakso).
 - **Gunakan Banyak `if` mandiri**: Jika hadiahnya boleh banyak (Beli baju AND beli tas).
 
 ---
 
 ## 🌀 N. Analogi Labirin Decisional (Rangkuman Visual)
 
 1. **Nested If**: Seperti masuk ke dalam brankas di dalam bank (Pintu PIN -> Sidik Jari).
 2. **Else-If Chain**: Seperti antre prasmanan (Satu lauk sudah diambil, lanjut ke meja makan).
 
 ---
 
 ## 📜 O. Rangkuman: Mantra "Compiler Manusia"
 
 Sebelum men-trace soal percabangan, ucapkan 3 mantra ini:
 1. **"Kurung mana kurung?"** (Cek batas wilayah kekuasaan `{ }`).
 2. **"Kiri dulu baru kanan!"** (Cek Short-circuit).
 3. **"Sekali benar, lupakan yang else!"** (Cek kunci `else if`).
 
 ---
 
 ### 🧠 Siap Di Uji Tracing? (Level 1: Gembok Berantai)
 
 ```cpp
 int skor = 80;
 int bonus = 0;
 
 if (skor > 50 || (bonus++ == 5)) {
     if (skor > 90) bonus += 10;
     else bonus += 5;
 }
 printf("bonus = %d", bonus);
 ```
 **Diagnosis Logika:**
 1. `skor > 50` $\rightarrow 80 > 50$ is **TRUE**.
 2. Konektor `||` (OR) mendeteksi sisi kiri sudah TRUE. Robot malas aktif!
 3. `(bonus++ == 5)` **DIABAIKAN**. Bonus tetap `0`.
 4. Masuk ke dalam: `skor > 90` adalah **FALSE**.
 5. Lari ke `else`: `bonus += 5` $\rightarrow$ bonus jadi `0 + 5 = 5`.
 6. Hasil akhir: **`bonus = 5`**.
 
 ---
 
 ### 🧗 Siap Di Uji Tracing? (Level 2: Pemburu Tanpa Tembok)
 
 ```cpp
 int a = 5;
 int b = 10;
 
 if (a > 10)
     a = a + 2;
     b = b + 5; // <--- Apakah ini rakyat Raja if?
     
 if (b > 10) {
     if (a == 5) b = 0;
     else b = 1;
 }
 printf("a = %d, b = %d", a, b);
 ```
 **Diagnosis Logika:**
 1. `a > 10` $\rightarrow 5 > 10$ is **FALSE**.
 2. Karena tidak ada kurung `{ }`, Raja `if` cuma berkuasa atas `a = a + 2`. Perintah itu **DIBATALKAN**.
 3. Namun `b = b + 5` adalah rakyat merdeka! Ia tetap jalan: `b = 10 + 5 = 15`.
 4. Pintu Berikutnya: `if (b > 10)` $\rightarrow 15 > 10$ is **TRUE**.
 5. Cek `if (a == 5)`? Karena `a` tadi tidak jadi ditambah, ia masih `5`. Hasilnya **TRUE**.
 6. `b = 0`.
 7. Hasil akhir: **`a = 5, b = 0`**.
 
 ---
 
 ### 🌋 Siap Di Uji Tracing? (Level 3: Kiamat Logika)
 
 ```cpp
 int x = 10;
 int y = 5;
 
 if (x < y < 20) {
     if (x = 2) y += x;
 }
 printf("x = %d, y = %d", x, y);
 ```
 **Diagnosis Logika:**
 1. `x < y < 20` $\rightarrow$ Robot C++ menghitung `10 < 5` dulu. Hasilnya **0** (False).
 2. Lalu `0 < 20` dihitung. Hasilnya **1** (True)! Gerbang Labirin terbuka.
 3. Masuk ke dalam: `if (x = 2)`. Ini bukan `==`. Juri mencuci otak `x` menjadi **2**. 
 4. Angka `2` dianggap **TRUE**, maka `y += x` dikerjakan.
 5. `y = 5 + 2 = 7`.
 6. Hasil akhir: **`x = 2, y = 7`**.
 
 ---
 
 ### 👹 Siap Di Uji Tracing? (MOD LEVEL: THE ULTIMATE BOSS)
 
 ```cpp
 int a = 5, b = 10, c = 0;
 
 if (a > 10 && (b++ > 0)) {
     c = 100;
 } else if (a < b < 0) {
     c = 200;
 } else {
     if (a = 2) {
         switch (b) {
             case 10: 
                 if (b > 5)
                     if (b < 10) c = 1;
                 else c = 2; // Dangling Else!
             case 5: c += 10; break;
         }
     }
     c = (c == 12) ? c + 3 : c + 1;
 }
 printf("a = %d, b = %d, c = %d", a, b, c);
 ```
 **Diagnosis Logika Sang Juara:**
 1. `if (a > 10)` ($5 > 10$) is **FALSE**. Karena konektor `&&`, mesin malas membaca sisi kanan. `b++` dibuang! Nilai `b` tetap **10**.
 2. `else if (a < b < 0)` $\rightarrow$ `5 < 10` is **1**. Lalu `1 < 0` is **FALSE**. Lari ke `else`.
 3. Di dalam `else`: `if (a = 2)`. Cuci otak! `a` sekarang **2**. Angka 2 adalah **TRUE**.
 4. `switch (b)` (Beri nilai `10`):
    - `case 10`:
      - `if (b > 5)` ($10 > 5$) is **TRUE**.
      - `if (b < 10)` ($10 < 10$) is **FALSE**.
      - `else c = 2` menempel pada `if` terdekat. Jadi `c` diisi **2**.
      - **TIDAK ADA BREAK!** Mesin kebelet lari ke `case 5`.
    - `case 5`: `c += 10` $\rightarrow 2 + 10 = 12$. Lalu `break` (pintu keluar).
 5. Perintah terakhir: `c = (c == 12) ? c + 3 : c + 1;`.
    - Karena `c` adalah 12, maka ambil jalur kiri: `12 + 3 = 15`.
 6. Hasil akhir: **`a = 2, b = 10, c = 15`**.
 
 ---
 
 ### 📝 Latihan Soal Tracing
 👉 **[Bank Soal Modul 02: Percabangan (300 Soal)](./latihan/README.md)**
 
 ---
 
 ⏩ **Lanjut ke Modul Ketiga:** [Perulangan & Mesin Array (Trek Lari)](../03-perulangan-dan-manipulasi-array/materi.md)
