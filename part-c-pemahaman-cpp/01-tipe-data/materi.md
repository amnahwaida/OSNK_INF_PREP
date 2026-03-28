# 1. Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)
 
 Selamat datang di markas besar *Compiler Manusia*! 
 Di sini, mesin Juri OSN-K akan melempar sebaris dua baris kode berbahasa **C++** yang memanipulasi rentetan angka. Sebagai *Compiler Manusia*, kamu wajib tahu sifat-sifat kejam kodingan C++ yang sering kali **berlawanan dengan hukum matematika di sekolah**.
 
 Mari kita bedah konsep penjebak massal mulai dari aturan penulisan hingga kasta tertinggi tipe data.
 
 ---
 
 ## 📋 A. Pemanasan: Aturan Dasar Menulis Kode
 
 Sebelum kita masuk ke angka, ada 5 aturan "Sopan Santun" di C++ yang wajib muridmu tahu:
 
 1. **Titik Koma (`;`) adalah Titik**: Setiap satu perintah selesai, wajib diakhiri `;`. 
 2. **Komentar (`//`) adalah Catatan**: Tulis apapun setelah `//` tidak akan dibaca oleh komputer. 
 3. **C++ itu Beda Huruf (Case Sensitive)**: `Uang` dan `uang` adalah dua laci yang **BERBEDA**. Hati-hati dengan huruf kapital!
 4. **Nama Loker (Variabel)**: Tidak boleh ada **Spasi**, tidak boleh diawali **Angka**.
 5. **Petik Tunggal vs Ganda**: Satu huruf pakai petik tunggal `'A'`, kalau teks panjang memakai petik ganda `"Halo"`.
 
 ### 🚫 Kata-Kata Terlarang (Reserved Words)
 Komputer punya "Kamus Kata Sakti" yang sudah memiliki fungsi khusus. Kamu **DILARANG KERAS** menggunakan kata-kata ini sebagai nama variabelmu.
 
 **Daftar Lengkap Kata Terlarang (Wajib Hindari):**
 
 | Kategori | Kata Terlarang |
 | :--- | :--- |
 | **Tipe Data** | `bool`, `char`, `double`, `float`, `int`, `long`, `short`, `signed`, `unsigned`, `void`, `wchar_t`, `auto` |
 | **Kontrol Alur** | `break`, `case`, `continue`, `default`, `do`, `else`, `for`, `goto`, `if`, `return`, `switch`, `while` |
 | **Akses & Memori** | `class`, `const`, `delete`, `enum`, `extern`, `friend`, `inline`, `mutable`, `namespace`, `new`, `operator`, `private`, `protected`, `public`, `register`, `sizeof`, `static`, `struct`, `template`, `this`, `typedef`, `union`, `using`, `virtual`, `volatile` |
 | **Logika & Lainnya** | `and`, `and_eq`, `asm`, `bitand`, `bitor`, `compl`, `const_cast`, `dynamic_cast`, `explicit`, `export`, `false`, `not`, `not_eq`, `or`, `or_eq`, `reinterpret_cast`, `static_cast`, `throw`, `true`, `try`, `typeid`, `typename`, `xor`, `xor_eq` |
 
 **Analogi**: Bayangkan kamu sedang di restoran. Kamu tidak boleh menamai anjing peliharaanmu "Menu", "Meja", atau "Pelayan", karena saat kamu memanggil mereka, seisi restoran akan bingung dan kacau! Begitu juga dengan robot C++.
 
 ---
 
 ## 🛠️ B. Boilerplate: Perlengkapan Wajib C++
 
 Pernah lihat baris `#include <iostream>` atau `int main()`? Jangan pusing, anggap itu **Perlengkapan Wajib**:
 - `#include <iostream>`: Seperti membawa **Tas Belanja**. Di dalam tas ini ada alat `cin` dan `cout`.
 - `using namespace std;`: Izin agar kita bisa memanggil `cin` dan `cout` langsung tanpa mendaftarkannya satu-per-satu.
 - `int main() { ... }`: Inilah **Dapur Utama**. Komputer hanya akan memasak apa yang ada di dalam kurung kurawal `{ }` fungsi ini.
 
 ---
 
 ## 🚪 C. Pintu Masuk & Keluar (Input `cin` & Output `cout`)
 
 Variabel adalah laci, tapi bagaimana cara memasukkan barang ke dalamnya? 
 
 1. **`cin >> laci;` (Input)**: Corong masuk dari Keyboard.
 2. **`cout << laci;` (Output)**: Corong keluar ke Layar.
 3. **`endl` atau `"\n"` (Tombol Enter)**: Berfungsi untuk pindah ke baris baru.
 
 ### 🧱 Rantai Kereta (Chaining cin/cout)
 Kamu tidak harus menulis `cin` satu per satu. Kamu bisa menyambungnya seperti gerbong kereta:
 ```cpp
 int a, b, c;
 cin >> a >> b >> c; // Sekali sedot 3 angka!
 ```
 **Hati-hati: Jebakan Menempel!**
 Saat mencetak dua angka, robot C++ tidak otomatis memberimu spasi.
 ```cpp
 cout << a << b; // Jika a=10, b=20, hasilnya: 1020 (Satu angka baru yang aneh!)
 cout << a << " " << b; // Hasilnya: 10 20 (Rapi dan Benar).
 ```
 
 ### ⚠️ Jebakan Kecepatan: `endl` vs `"\n"`
 Muridmu mungkin sering melihat `endl` di sekolah. Hati-hati! Di kodingan OSN-K yang datanya sangat banyak, memakai `endl` bisa membuat programmu **TLE** (Terlalu Lambat)!
 - **`endl` (Lompat Sambil Ngosongin)**: Selain membuat baris baru, ia memaksa komputer mengosongkan aliran data (*Flush*) ke layar setiap saat. Ini **LAMBAT SEKALI**.
 - **`"\n"` (Lompat Saja)**: Ia hanya menyuruh kursor pindah ke baris baru tanpa mengganggu sisa aliran data. Ini **SANGAT CEPAT**.
 
 **Analogi "Kurir Paket"**: 
 - `endl` itu seperti kurir yang setelah mengantar 1 paket langsung pulang ke gudang dulu baru berangkat lagi.
 - `"\n"` itu seperti kurir yang membawa semua paket dalam satu mobil, mengantarnya ke baris-baris alamat yang berbeda tanpa harus pulang ke gudang setiap saat.
 
 ### ⚡ Mantra Pelicin (Fast I/O)
 Di soal OSN-K yang datanya sangat besar (ratusan ribu baris), `cin` dan `cout` seringkali terasa "lelet". Agar secepat kilat, kita butuh mantra sakti di awal fungsi `main`:
 ```cpp
 ios::sync_with_stdio(0);
 cin.tie(0);
 ```
 **Analogi "Lampu Hijau Terus"**: Secara bawaan, C++ selalu mengecek apakah bahasa C juga mau mengirim data (antrean bareng). Mantra ini seperti membuat jalur khusus TransJakarta; `cin` dan `cout` langsung melesat tanpa peduli kendaraan lain!
 
 ---
 
 ## 🚀 D. Jalur Cepat & Format Jadul (`scanf` & `printf`)
 
 Selain `cin/cout`, terkadang juri OSN-K menggunakan gaya penulisan "Jadul" warisan bahasa C. Kenapa harus dipelajari? Karena lebih **CEPAT** memproses data jutaan angka dan lebih **MUDAH** mengatur tampilan angka (seperti jumlah nol di belakang koma).
 
 ### 🛠️ 1. Analogi "Robot Pelayan Restoran"
 Jika `cin/cout` itu seperti corong bebas, maka `scanf/printf` adalah **Robot Pelayan**. Kamu tidak bisa asal lempar barang; kamu harus memesan dengan **Kode Meja (Format Specifier)** yang spesifik.
 
 **Kamus Kode Meja (Format Specifier):**
 | Tipe Data | Kode Meja | Arti |
 | :--- | :--- | :--- |
 | `int` | **`%d`** | Bilangan Bulat biasa. |
 | `long long` | **`%lld`** | Bilangan Bulat raksasa. |
 | `float` | **`%f`** | Angka Koma. |
 | `double` | **`%lf`** | Angka Koma Presisi (Long Float).|
 | `char` | **`%c`** | Satu Huruf Tunggal. |
 
 ### 📝 2. Cara Menulis Output (`printf`)
 ```cpp
 printf("Uang saya ada %d rupiah", 5000);
 ```
 **Diagnosis Logika:** Robot membaca teks. Begitu ketemu `%d`, ia menengok ke luar tanda petik, mengambil angka `5000`, lalu menaruhnya di posisi ganjalan `%d` tersebut.
 
 ### 📝 3. Cara Menulis Input (`scanf`)
 ```cpp
 scanf("%d", &uang);
 ```
 **Hati-hati: Jebakan "&" (Alamat GPS)**
 Pada `scanf`, kamu wajib menaruh simbol **`&`** (Ampersand) sebelum nama variabel. 
 - **Analoginya**: `scanf` butuh **Alamat GPS** (`&`) untuk tahu di mana laci `uang` berada. Kalau tidak ada `&`, robot akan nyasar dan programmu *crash* (mati mendadak)!
 
 ### 🎯 4. Keajaiban Formatting (Mengatur Comma)
 Ini adalah alasan utama orang memakai `printf`. Kita bisa memesan berapa angka di belakang koma dengan sangat mudah!
 - **`%.2f`**: Cetak angka koma, tapi **cukup 2 angka** saja di belakang titik.
 - **`%.0f`**: Hilangkan semua angka belakang koma (pembulatan tampilan).
 
 ```cpp
 double pi = 3.14159;
 printf("%.2lf", pi); // Hasil di layar: 3.14
 ```
 
 ---
 
 ## 📦 E. Rahasia Loker Ajaib (Konsep Variabel & Tipe Dasar)
 
 Selamat! Kamu akan belajar tentang jantung dari segala program komputer: **Variabel**.
 
 ### 🔍 1. Apa Itu Variabel? (Analogi Loker Sekolah)
 Bayangkan kamu punya barisan loker di sekolah. Untuk menyimpan barang, kamu harus melakukan 3 hal:
 1.  **Pilih Ukuran Loker** (Tipe Data): Apakah kamu butuh loker kecil untuk permen, atau peti kemas untuk sepeda?
 2.  **Beri Label Nama** (Variabel Name): Agar kamu tidak tertukar dengan loker temanmu.
 3.  **Isi Barangnya** (Value): Masukkan angka atau huruf ke dalamnya.
 
 Di C++, cara memesan loker adalah:
 `TipeData NamaLoker = IsiAwal;`
 
 **Contoh**: `int skor = 100;` 
 Artinya: "Robot, siapkan loker ukuran **Integer** bernama **Skor**, dan langsung isi dengan angka **100**."
 
 ### 🧪 2. Macam-Macam Ukuran Loker (Tipe Data Dasar)
 Di OSN-K, pemilihan ukuran loker sangat menentukan apakah kamu dapat skor atau tidak.
 
 - `int` (**Loker Semen**): Loker standar. Cuma bisa diisi **Bilangan Bulat** (-2 miliar s.d 2 miliar).
 - `long long` (**Peti Kemas**): Loker raksasa. Untuk angka yang sangat besar (triliunan atau $10^{18}$).
 - `bool` (**Saklar Lampu**): Loker kecil yang cuma punya dua kondisi: **`true`** (Benar/1) atau **`false`** (Salah/0).
 - `double` (**Gelas Takar**): Loker khusus untuk angka koma/pecahan ($3.14$).
 
 ### 🔒 Loker Tertutup (Konstanta `const`)
 Terkadang ada angka yang **tidak boleh diubah** apa pun yang terjadi (misalnya nilai Maksimal atau nilai Modulo). Kita menyegelnya dengan kata sakti `const`:
 ```cpp
 const int MAX_N = 100;
 MAX_N = 200; // <--- ERROR! Robot akan marah karena segelnya dirusak.
 ```
 **Analogi "Segel Pabrik"**: Memakai `const` seperti memberi segel di pintu loker. Siapapun bisa melihat isi angkanya, tapi tidak ada yang bisa mengganti isinya.
 
 ### ⚠️ Jebakan Batman #1: Integer Division (Membagi Tanpa Ampun)
 
 Guru Matematika di sekolah mengajarkan: $5 \div 2 = 2.5$. Benar kan?
 **Di dunia C++, `5 / 2` HASILNYA ADALAH `2`!** Lho kok bisa? Kemana sisa $0.5$ nya?
 
 **Analogi Laci Semen keras tanpa celah karet (desimal)**:
 Kalau tipe datanya `int`, sisa serpihannya **DIBUANG KE TONG SAMPAH, DIABAIKAN, DIBAKAR!**
 
 *Aturan Emas Tracing C++:* Kalau tipe datanya `int`, setiap ada rumus Pembagian `/`, **potong buang semua angka koma di belakangnya tanpa pembulatan**.
 
 ---
 
 ## 🗑️ F. Jebakan Laci Bekas (Garbage Value)
 
 Apa yang terjadi jika kamu membuat laci tapi tidak menaruh angka apa-apa?
 ```cpp
 int saldo;
 cout << saldo;
 ```
 **Analogi Laci Bekas Penghuni Lama:**
 Bayangkan kamu menyewa loker di sekolah, tapi tidak mengisinya. Saat kamu buka laci itu besok, eh ternyata di dalamnya ada **"Sampah"** berupa angka acak yang sangat besar (misal: `-858993460`).
 
 Komputer tidak otomatis mengosongkan laci. Ia membiarkan angka sisa dari program lain tertinggal di sana.
 - **Pelajaran:** Selalu biasakan memberi nilai awal (**Inisialisasi**) saat membuat variabel, misalnya: `int saldo = 0;`. 
 
 ---
 
 ## 🔮 G. Sihir Sisa Bagi (Modulo `%`)
 
 Nah, tadi kan sisa 1 permennya dibuang tuh sama operator pembagi `/`. Terus kalau kita mau cari tahu permen sisa yang gak bisa dibagi rata itu berapa, ke mana kita mencarinya?
 Jawabannya adalah **Operator Modulo (Simbolnya `%`)**.
 
 Modulo artinya: **"Cari Sisa Baginya!"**
 
 **Analogi Kelereng Harian:**
 Kamu punya 14 kelereng. Kamu ingin membagikannya adil ke 4 temanmu.
 - Bagi Rata ($14 \div 4$): Setiap anak dapet 3 biji utuh (`14 / 4 = 3`).
 - Sisa Kelereng ($14 \pmod 4$): Total yang dibagikan $3 \times 4 = 12$ biji. Tanganmu sisa $14 - 12 = 2$ biji kelereng yang gak bisa dibagi. Inilah hasil Modulonya! (`14 % 4 = 2`).
 
 ### ⚠️ Jebakan Batman #2: Sifat Modulo Bikin Pusing
 **1. Modulo Angka Kecil terhadap Angka Besar**
 Coba jawab cepat! Berapa hasil `3 % 7` (3 sisa bagi 7)?
 - **Analogi Logis:** Pak Dengklek punya 3 kelereng. Disuruh membagikan merata ke 7 anak. Apa yang terjadi? Ya nggak mungkin! Kelerengnya kurang dari jumlah anak, nggak bisa dibagi satu pun ke siapa-siapa. Kesimpulannya: Kelereng di tangan Pak Dengklek utuh tidak berkurang. 
 - Hasilnya: **`3 % 7 = 3`**.
 *Aturan Emas Modulo OSN-K:* Jika angka kiri *lebih kecil* dari angka kanan ($A \pmod B$ dimana $A < B$), **jawabannya adalah Angka Kiri itu sendiri ($A$)**.
 
 **2. Pendeteksi Genap-Ganjil Instant**
 Di soal operasi *looping* array panjang, Modulo `2` seringkali nongol mendadak.
 - **Genap**: `if (x % 2 == 0)` $\rightarrow$ "Apakah `x` genap?"
 - **Ganjil**: `if (x % 2 != 0)` atau `if (x % 2 == 1)` $\rightarrow$ "Apakah `x` ganjil?"
 
 Jangan panik ngitung sisa bagi angka gila! `% 2` terjemahan bahasa Indonesianya murni: **"Apa golongan angka ini?"**.
 
 ---
 
 ## ➕ H. Operator Aritmatika & Hierarki (KABATAKU)
 
 Karena kamu belajar dari 0, ingatlah bahwa komputer itu seperti kalkulator super cepat. Namun, ia punya aturan "Siapa yang dikerjakan duluan?".
 
 **1. Anggota Keluarga Aritmatika:**
 - `+` (Tambah), `-` (Kurang), `*` (Kali), `/` (Bagi), `%` (Modulo).
 
 **2. Hukum KABATAKU (Kali, Bagi, Tambah, Kurang):**
 Komputer tidak mengerjakan dari kiri ke kanan saja. Ia punya kasta:
 1. Lingkaran Kurung `( )` $\rightarrow$ **Kasta Tertinggi** (Wajib duluan!).
 2. Perkalian `*`, Pembagian `/`, and Modulo `%` $\rightarrow$ **Kasta Menengah**.
 3. Penjumlahan `+` dan Pengurangan `-` $\rightarrow$ **Kasta Rakyat**.
 
 > [!TIP]
 > Jika ada `2 + 3 * 4`, hasilnya adalah **14** (karena $3 \times 4$ dikerjakan duluan), bukan 20!
 
 ---
 
 ## 🛠️ I. Alat Hitung Lanjutan (`cmath`)
 
 Selain tambah-kurang-kali-bagi, C++ menyediakan "Kotak Perkakas" tambahan bernama **`cmath`**. 
 - Untuk memakainya, di baris paling atas (Boilerplate) harus tertulis: `#include <cmath>`.
 
 **Alat Hitung Paling Sering Muncul:**
 1. **`abs(x)` (Nilai Mutlak)**: Menghilangkan tanda minus. `abs(-5)` jadi `5`. (Ingat: **Abs**olut).
 2. **`sqrt(x)` (Akar Kuadrat)**: Mencari lari akar. `sqrt(16)` jadi `4`. (**S**quare **R**oo**T**).
 3. **`pow(a, b)` (Pangkat)**: Menghitung $a$ pangkat $b$. `pow(2, 3)` jadi `8`. (**Pow**er).
 4. **`round(x)` (Pembulatan Terdekat)**: Membulatkan ke angka terdekat. `round(2.6)` jadi `3`.
 5. **`floor(x)` (Lantai)**: Memaksa pembulatan ke **BAWAH** (Lantai). `floor(2.9)` tetap jadi `2`. 
 6. **`ceil(x)` (Atap)**: Memaksa pembulatan ke **ATAS** (Atap/Ceiling). `ceil(2.1)` langsung naik jadi `3`.
 
 **Analogi "Bus Sekolah" (Kapan Memakai Ceil?)**:
 Kamu punya 10 anak dan 1 bus kapasitasnya cuma 3 orang. Secara matematika $10 \div 3 = 3.33$.
 - Kalau pakai `round`, hasilnya 3 bus (Satu anak tertinggal di lobi!).
 - Kalau pakai **`ceil`**, hasilnya **4 bus** (Semua anak terangkut, meski bus ke-4 agak kosong). **Ingat: `ceil` sangat penting untuk soal-soal logistik di OSN-K!**
 
 > [!TIP]
 > Hati-hati! Hasil dari `sqrt`, `pow`, `floor`, dan `ceil` otomatis berwujud **`double`** (angka koma), meskipun kamu memasukkan angka bulat.
 
 ---
 
 ## 🚚 J. Operator Assignment (Pindah Barang)
 
 Di matematika, `=` artinya "Sama Dengan". Di kodingan, `=` artinya **"Pindah Barang!"**.
 
 **1. `a = 5` (Assignment Dasar)**
 - **Analogi:** Ambil angka 5, lalu **masukkan** ke dalam laci bernama `a`.
 - Isi laci `a` yang lama akan **dibuang** dan diganti total dengan angka 5 yang baru.
 
 **2. Shortcut Penjumlahan (`+=`, `-=`, `*=`)**
 Seringkali kita ingin menambah isi laci yang sudah ada.
 - `a += 2` $\rightarrow$ Artinya: "Ambil isi laci `a` sekarang, tambahkan 2, lalu masukkan lagi ke laci `a`."
 
 **3. Increment & Decrement (`++`, `--`)**
 - `a++` $\rightarrow$ "Tambah isi laci `a` sebanyak 1 biji." (Sama dengan `a = a + 1`).
 - `a--` $\rightarrow$ "Kurangi isi laci `a` sebanyak 1 biji." (Sama dengan `a = a - 1`).
 
 ### ⚠️ Jebakan Batman #3: Pre vs Post (Kapan Nilainya Berubah?)
 Juri OSN-K **SANGAT SUKA** menggunakan jebakan ini:
 - **`++a` (Pre-increment)**: "Tambah dulu, baru dipakai."
 - **`a++` (Post-increment)**: "Pakai nilai sekarang dulu, baru tambah di baris berikutnya."
 
 **Analogi Gaji vs Komisi:**
 - `++a` (Gaji Awal): Bos kasih kamu uang dulu, baru kamu disuruh belanja.
 - `a++` (Komisi Akhir): Kamu belanja dulu pakai uang lama, baru pas pulang Bos kasih bonus uang tambahan.
 
 ```cpp
 int a = 5;
 int b = a++; // b jadi 5 (a ditaruh ke b dulu, baru a naik jadi 6)
 int c = ++a; // c jadi 7 (a naik jadi 7 dulu, baru a ditaruh ke c)
 ```
 
 ---
 
 ## ⚖️ K. Operator Perbandingan (Timbangan Benar-Salah)
 
 Setelah pandai menghitung, kamu akan sering disuruh membandingkan dua angka. Di sini, hasilnya bukan lagi angka, tapi **Benar (`true`)** atau **Salah (`false`)**.
 
 - `==` (Sama dengan): `"Apakah dia kembaran?"`. (Ingat: `=` pindah barang, `==` tanya kabar).
 - `!=` (Tidak sama dengan): `"Apakah mereka musuhan?"`.
 - `<`, `>`, `<=`, `>=`: Seperti di sekolah, tapi di kodingan hasilnya berubah jadi sinyal Logika.
 
 > [!IMPORTANT]
 > Di OSN-K, Hati-hati dengan `if (a = 5)`. Juri jahat suka sengaja menghilangkan satu tanda `=`. Jika tertulis `=`, itu artinya laci `a` **dipaksa** jadi 5, dan kondisinya dianggap **Benar**! Selalu cari `==` untuk perbandingan murni.
 
 ---
 
 ## 🚦 L. Operator Logika (Filter Berlapis)
 
 Jika perbandingan di atas adalah satu pintu, maka operator logika adalah **Pintu Berlapis**.
 
 - `&&` (DAN / AND): Harus **Semua Benar** baru lolos.
 - `||` (ATAU / OR): Asal ada **Satu Benar** langsung lolos.
 - `!` (TIDAK / NOT): Kacamata kebalikan (Benar jadi Salah, Salah jadi Benar).
 
 **Kamus Kebenaran (Truth Table):**
 | Syarat A | Syarat B | A && B | A \|\| B |
 | :--- | :--- | :--- | :--- |
 | ✅ True | ✅ True | **✅ True** | **✅ True** |
 | ✅ True | ❌ False | **❌ False** | **✅ True** |
 | ❌ False | ✅ True | **❌ False** | **✅ True** |
 | ❌ False | ❌ False | **❌ False** | **❌ False** |
 
 ---
 
 ## 🔢 M. Hasil Akhir Logika (Ujung dari Segalanya: 0 & 1)
 
 Di kodingan OSN-K, kamu terkadang melihat logika dicampur dengan matematika. Bagaimana robot C++ menghadapinya?
 - **Robot Matematika Logika:** Di matanya, semua hasil perbandingan `(> < == !=)` AND/OR/NOT itu **SELALU** berakhir menjadi angka **0** (Jika Salah) atau **1** (Jika Benar).
 
 **Contoh Real Code:**
 ```cpp
 int x = (10 > 5) + (5 > 2); // 1 + 1
 printf("x = %d", x); // x jadi 2!
 ```
 **Diagnosis Logika:**
 - `(10 > 5)` adalah Benar, maka robot mengubahnya jadi angka **1**.
 - `(5 > 2)` adalah Benar, maka robot mengubahnya jadi angka **1**.
 - `1 + 1` hasilnya **2**.
 
 > [!IMPORTANT]
 > **Minus pun Dianggap Benar!** Di mata C++, **HANYA angka 0** yang dianggap **FALSE**. Angka lainnya, baik itu `1`, `-1`, `-999`, atau `0.0001`, semuanya dianggap **TRUE**! Hati-hati jika juri menaruh angka negatif di dalam syarat `if`.
 
 ---
 
 ## 🧪 N. Tip & Trick Khas OSN-K (Angka Dewa & Jebakan Maut)
 
 Di soal-soal tingkat nasional, kamu akan sering melihat cara penulisan angka yang "aneh". Mari kita bedah rahasianya:
 
 **1. Angka Eksponen (`1e9`)**
 - `1e9` $\rightarrow$ Artinya $1 \times 10^9$ atau **1 Miliar**.
 - `2e9` $\rightarrow$ 2 Miliar (Ini adalah **Batas Maksimal `int`**).
 - `1e18` $\rightarrow$ Artinya $1 \times 10^{18}$ (Sering dipakai untuk nilai tak hingga di `long long`).
 
 **2. Rahasia Modulo $10^9+7$**
 Seringkali juri meminta jawaban kamu dalam bentuk: `"Keluarkan sisa bagi dengan 1.000.000.007"`. Mengapa angka ini?
 - **Mencegah Ledakan**: Agar hasil hitunganmu tidak melebihi kapasitas `long long`.
 - **Angka Prima**: $1.000.000 .007$ adalah bilangan prima besar, sehingga sangat aman untuk perhitungan matematis tingkat lanjut.
 
 ### ⚠️ 3. Jebakan Overflow Meski Pakai Long Long!
 Ini adalah jebakan nomor 1 yang mematikan banyak peserta. Perhatikan kode ini:
 ```cpp
 int a = 1000000; // Satu juta
 int b = 1000000; // Satu juta
 long long c = a * b; // HARUSNYA satu triliun kan?
 ```
 **Hasilnya: SALAH BESAR!** Robot menghitung `a * b` di area `int` dulu, sehingga meledak (Overflow) sebelum sempat ditampung di `long long`.
 
 **Solusi Sakti (1LL)**: Paksa robot menghitung dalam skala besar sejak awal:
 ```cpp
 long long c = 1LL * a * b; // Berhasil!
 ```
 
 ---
 
 ## 🔤 O. Perang Kasta Tipe Data (Char, Int, Float, Double)
 
 Selain loker semen (`int`), kamu akan berhadapan dengan tipe data lain yang punya hukum kasta yang sangat aneh di dalam mesin C++. 
 
 ```mermaid
 graph LR
     A["char <br> (1 byte)"] -->|"Promosi Otomatis"| B["int <br> (4 bytes)"]
     B -->|"Promosi Otomatis"| C["float <br> (4 bytes, 7 digit)"]
     C -->|"Promosi Otomatis"| D["double <br> (8 bytes, 15 digit)"]
     
     D -.->|"Demosi Paksa (bahaya!)"| B
     B -.->|"Demosi Paksa (bahaya!)"| A
     
     style A fill:#ffe0b2,stroke:#333
     style B fill:#c8e6c9,stroke:#333
     style C fill:#b3e5fc,stroke:#333
     style D fill:#e1bee7,stroke:#333
 ```
 **📖 Cara Membaca Diagram Hierarki Kasta:**
 - Semakin ke kanan = Semakin "Suci" kastanya. Saat dua tipe berbeda bertarung dalam satu rumus, **kasta tertinggi selalu menang** dan memaksa semua anggota lainnya naik level (*Type Promotion*).
 
 ### 1. `char` vs `int` (Karakter adalah Angka yang Bersembunyi!)
 `char` dikhususkan untuk **Satu Huruf Tunggal** (misal `'A'`). 
 Untuk menerjemahkan angka menjadi huruf, C++ menggunakan buku kamus rahasia bernama **Tabel ASCII**.
 
 **Tabel Sakti ASCII (Wajib Ingat Rentang):**
 | Kelompok Karakter | Karakter | Kode ASCII (Desimal) | Jarak/Keterangan |
 | :--- | :--- | :--- | :--- |
 | **Simbol Angka** | `'0'` s.d. `'9'` | **48 s.d. 57** | Ingat: `'0'` bukan 0 murni! |
 | **Huruf Besar** | `'A'` s.d. `'Z'` | **65 s.d. 90** | `'A'` = 65 |
 | **Huruf Kecil** | `'a'` s.d. `'z'` | **97 s.d. 122** | `'a'` = 97 |
 | **Spasi** | `' '` | **32** | Sering terlupa saat tracing. |
 
 **Kenapa Harus Sequential (Berurutan)?**
 Robot C++ menaruh huruf demi huruf secara rapi berurutan. Ini memungkinkan kita memakai trik **"Matematika Huruf"**:
 1. **Mencari Urutan Abjad**: `char c = 'C'; int urutan = c - 'A';` $\rightarrow 67 - 65 = 2$. (Artinya 'C' adalah orang ke-2 setelah 'A').
 2. **Konversi Angka Teks**: `char c = '5'; int asli = c - '0';` $\rightarrow 53 - 48 = 5$.
 3. **The Magic 32**: Jarak antara Huruf Kecil dan Huruf Besar SELALU **32**. 
    - `'a' - 32` = `'A'`.
    - `'B' + 32` = `'b'`.
 
 ---
 
 ## 🌍 P. Wilayah Kekuasaan Variabel (Scope Global vs Lokal)
 
 Di kodingan OSN-K, juri suka menamai **Dua Variabel Berbeda dengan NAMA YANG SAMA PERSIS** untuk mengecoh otakmu!
 
 **Analogi Ketua OSIS (Global) vs Ketua Kelas (Lokal):**
 ```cpp
 int uang = 100; // GLOBAL (Ketua OSIS, semua murid kenal dia)
 
 void cek_dompet() {
     int uang = 5; // LOKAL (Ketua Kelas 12A)
     printf("%d", uang);
 }
 ```
 **Hukum Kesopanan C++:** "Orang Dalam Lebih Berkuasa". Jika ada dua orang bernama sama, robot akan memanggil orang yang berada di dalam ruangan yang sama terlebih dahulu (*Shadowing*).
 
 ### ⛲ Kesaktian Loker Global (Otomatis Bersih)
 Seringkali murid bingung: *"Kenapa variabel ini tiba-tiba bernilai 0, padahal tidak saya isi?"*. Inilah rahasianya:
 - **Variabel GLOBAL**: Secara otomatis dibersihkan oleh sistem. Isinya **PASTI 0** jika tidak diisi apa-apa.
 - **Variabel LOKAL**: Seperti laci bekas berantakan. Isinya **ACAK/SAMPAH**.
 
 > [!TIP]
 > **Tips Hemat Waktu**: Jika soal OSN-K menaruh variabel di atas `int main()`, kamu tidak perlu repot melakukan inisialisasi `= 0`. Hemat 3 detik di setiap soal!
 
 ---
 
 ## 📦 Q. Intipan Masa Depan: Tipe Data Borongan
 
 Di tingkat olimpiade, data yang kamu olah tidak cuma satu permen, tapi sebungkus besar! Di sini kita akan mengintip dua tipe data yang akan dijelaskan di modul selanjutnya:
 
 ### 🧵 1. `string` (Kalimat / Rangkaian Huruf)
 Digunakan untuk menyimpan kata, kalimat, atau sandi rahasia.
 - **Analoginya**: Kereta Api Huruf. Setiap gerbong berisi satu karakter.
 - **Cara Tulis**: `string nama = "Pak Dengklek";`.
 > [!NOTE]
 > Pembahasan mendalam mengenai cara membedah kalimat ada di **Modul 07: Manipulasi String**.
 
 ### 📚 2. `array` (Loker Berderet / Daftar Angka)
 Digunakan saat kamu punya banyak angka tapi malas memberi nama laci satu per satu.
 - **Analoginya**: Lemari Loker Berderet. Satu pintu besar berjudul `nilai`, tapi di dalamnya ada laci nomor 0, 1, 2, dst.
 - **Cara Tulis**: `int nilai[5] = {90, 85, 80, 70, 100};`.
 > [!NOTE]
 > Pembahasan mengenai cara membongkar isi loker ini secara otomatis dapat kamu temukan di **Modul 03: Perulangan & Array**.
 
 ---
 
 ## 🛁 R. Analogi Tambahan: Gudang Rahasia Komputer
 
 ### 1. Long Long vs Int: Gayung vs Bak Mandi
 Kamu butuh **Bak Mandi** (`long long`) saat hasil hitunganmu sangat banyak (misal hasil perkalian `100.000 * 100.000`) agar airnya tidak tumpah lari ke mana-mana (*Overflow*).
 
 ### 2. Type Casting: Mainan Balok Anak-anak
 Memasukkan `double` (angka koma) ke dalam `int` (angka bulat) seperti memaksa **Balok Bintang** masuk ke **Lubang Kotak**. Kamu harus memotong/mengamplas semua sudut komanya sampai rata menjadi kotak polos.
 
 ---
 
 ## 📜 S. Rangkuman: Mantra "Compiler Manusia"
 
 1. **Aturan Resep**: Kode dijalankan baris demi baris dari **ATAS ke BAWAH**. 
 2. **Aturan Timpa**: Laci variabel hanya bisa menyimpan **SATU** angka. Jika diisi baru, yang lama terhapus.
 3. **Aturan Persiapan**: Kamu tidak bisa memakai bahan (variabel) sebelum menyiapkannya (deklarasi).
 
 ### 🏆 Ceklis Emas Penelusuran (Final Check)
 Sebelum kamu menulis jawaban akhir di lembar soal, lakukan 3 pengecekan ini:
 1.  **Cek Tipe Data**: Apakah ada pembagian `int` yang "koma-nya" harus hangus dibakar?
 2.  **Cek Kasta Operator**: Apakah ada perkalian/modulo yang harus didahulukan daripada penjumlahan?
 3.  **Cek Perubahan Nilai**: Apakah ada variabel yang isinya terhapus/ditimpa oleh perintah baru (seperti `a = 5` atau `a++`)?
 
 ---
 
 ### 🧠 Uji Tracing (Level 1-5)
 *(Lihat bagian bawah dokumen untuk detail diagnosis logika per level)*
 
 ---
 
 ### 📝 Latihan Soal Tracing
 👉 **[Bank Soal Modul 01: Tipe Data & Operator (300 Soal)](./latihan/README.md)**
 
 ---
 
 ⏩ **Lanjut ke Modul Kedua:** [Logika Percabangan (Razia BP)](../02-percabangan/materi.md)
