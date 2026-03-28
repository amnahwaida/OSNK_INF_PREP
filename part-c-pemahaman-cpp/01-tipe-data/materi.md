# 1. Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)
 
 Selamat datang di markas besar *Compiler Manusia*! 
 Di sini, mesin Juri OSN-K akan melempar sebaris dua baris kode berbahasa **C++** yang memanipulasi rentetan angka. Sebagai *Compiler Manusia*, kamu wajib tahu sifat-sifat kejam kodingan C++ yang sering kali **berlawanan dengan hukum matematika di sekolah**.
 
 Mari kita bedah konsep penjebak massal mulai dari aturan penulisan hingga kasta tertinggi tipe data.
 
 ---
 
 ## 📋 A. Pemanasan: Aturan Dasar Menulis Kode
 
 Sebelum kita masuk ke angka, ada 5 aturan "Sopan Santun" di C++ yang wajib muridmu tahu:
 
 1. **Titik Koma (`;`) adalah Titik**: Setiap satu perintah selesai, wajib diakhiri `;`. 
 2. **Komentar (`//`) adalah Catatan**: Tulis apapun setelah `//` tidak akan dibaca oleh komputer. 
 3. **C++ itu Beda Huruf (Case Sensitive)**: `Uang` and `uang` adalah dua laci yang **BERBEDA**. Hati-hati dengan huruf kapital!
 4. **Nama Loker (Variabel)**: Tidak boleh ada **Spasi**, tidak boleh diawali **Angka**.
 5. **Petik Tunggal vs Ganda**: Satu huruf pakai petik tunggal `'A'`, kalau teks panjang memakai petik ganda `"Halo"`.
 
 > [!TIP]
 > **Mantra Hafalan 5 Jari:**
 > "Satu Titik, Dua Catatan, Tiga Huruf, Empat Nama, Lima Petik!"
 
 ### 🚫 Kata-Kata Terlarang (Reserved Words)
 Komputer punya "Kamus Kata Sakti" yang sudah memiliki fungsi khusus. Kamu **DILARANG KERAS** menggunakan kata-kata ini sebagai nama variabelmu.
 
 | Kategori | Kata Terlarang | Penjelasan Mudah |
 | :--- | :--- | :--- |
 | **Tipe Data** | `int`, `long`, `bool`, `double`, `void` | "Ini nama ukuran loker, jangan buat jadi nama loker!" |
 | **Kontrol Alur** | `if`, `else`, `while`, `for`, `return` | "Ini kata perintah robot, jangan dipakai jadi nama!" |
 | **Akses & Memori** | `public`, `private`, `static`, `using` | "Ini izin akses robot, dilarang dipinjam!" |
 | **Logika** | `and`, `or`, `not`, `true`, `false` | "Ini jawaban Benar/Salah, jangan dipakai jadi nama boks!" |
 
 **Analogi**: Jangan menamai anjing peliharaanmu "Pelayan" di dalam restoran, seisi restoran akan bingung! Begitu juga di C++, jangan menamai variabelmu `int` atau `if`.
 
 ---
 
 ## 🛠️ B. Boilerplate: Perlengkapan Wajib C++
 
 Pernah lihat baris `#include <iostream>` atau `int main()`? Jangan pusing, anggap itu **Perlengkapan Wajib**:
 - `#include <iostream>`: Seperti membawa **Tas Belanja**. Di dalam tas ini ada alat `cin` and `cout`.
 - `using namespace std;`: Izin agar kita bisa memanggil `cin` dan `cout` langsung tanpa mendaftarkannya satu-per-satu.
 - `int main() { ... }`: Inilah **Dapur Utama**. Komputer hanya akan memasak apa yang ada di dalam kurung kurawal `{ }` fungsi ini.
 
 > [!TIP]
 > **Pesan Penting:** Tanpa "Tas Belanja" (`iostream`), robotmu tidak akan bisa melihat keyboard (`cin`) maupun layar (`cout`)!
 
 ---
 
 ## 📦 C. Rahasia Loker Ajaib (Konsep Variabel & Tipe Dasar)
 
 Sebelum bisa memberi perintah ke komputer, kamu harus menyiapkan **"Loker"** untuk menyimpan datamu.
 
 ### 🔍 1. Apa Itu Variabel? (Analogi Loker Sekolah)
 Bayangkan kamu punya barisan loker di sekolah. Untuk menyimpan barang, kamu harus melakukan 3 hal:
 1.  **Pilih Ukuran Loker** (Tipe Data): Apakah kamu butuh loker kecil untuk permen, atau peti kemas untuk sepeda?
 2.  **Beri Label Nama** (Variabel Name): Agar kamu tidak tertukar dengan loker temanmu.
 3.  **Isi Barangnya** (Value): Masukkan angka atau huruf ke dalamnya.
 
 **Contoh**: `int skor = 100;` 
 Artinya: "Robot, siapkan loker ukuran **Integer** bernama **Skor**, dan langsung isi dengan angka **100**."
 
 ### ✨ 2. Loker Berjamaah (Deklarasi Berantai)
 Seringkali murid malas membuat laci satu per satu. Kamu bisa membuat banyak laci sekaligus asal ukurannya sama:
 ```cpp
 int a, b, c; // Robot membuat 3 laci kosong sekaligus!
 ```
 
 ### 🧪 3. Macam-Macam Ukuran Loker (Tipe Data Dasar)
 
 | Tipe Data | Nama Mudah | Kapan Dipakai? |
 | :--- | :--- | :--- |
 | **`int`** | **Loker Semen** | Untuk angka bulat standar (-2M s.d 2M). |
 | **`long long`**| **Peti Kemas** | Untuk angka raksasa (Triliunan/$10^{18}$). |
 | **`bool`** | **Saklar Lampu** | Untuk jawaban Benar/Salah (`true`/`false`). |
 | **`double`** | **Gelas Takar** | Untuk angka koma/pecahan ($3.14$). |
 
 ### 🔒 4. Loker Tertutup (Konstanta `const`)
 Terkadang ada angka yang **tidak boleh diubah**. Kita menyegelnya dengan kata sakti `const`:
 ```cpp
 const int MAX_N = 100; // Segel Pabrik! Tidak bisa diganti nilainya.
 ```
 
 ---
 
 ## 🚪 D. Komunikasi Dasar (Input `cin` & Output `cout`)
 
 Sering kita sebut sebagai **"Ayo Ngobrol dengan Robot"**.
 
 1. **`cin >> laci;` (Input)**: Corong masuk dari Keyboard.
 2. **`cout << laci;` (Output)**: Corong keluar ke Layar.
 
 ### 🧱 Rantai Kereta (Chaining cin/cout)
 Kamu bisa menyambungnya seperti gerbong kereta:
 ```cpp
 cin >> a >> b >> c; // Sekali sedot 3 gerbong data!
 ```
 
 > [!IMPORTANT]
 > **Pesan Spasi:** Robot tidak otomatis memberi spasi saat cetak angka. Gunakan `" "` secara manual agar angkamu tidak menempel!
 
 ### ⚠️ Jebakan Kecepatan: `endl` vs `"\n"`
 - **`endl` (Lompat Sambil Nguras)**: Lambat karena robot harus membersihkan aliran data ke layar setiap saat.
 - **`"\n"` (Lompat Aja)**: Cepat karena robot cuma pindah baris tanpa ganggu aliran data.
 
 ### ⚡ Mantra Pelicin (Fast I/O)
 Taruh mantra ini di awal `int main()` agar programmu melesat secepat cahaya!
 ```cpp
 ios::sync_with_stdio(0); cin.tie(0);
 ```
 
 ---
 
 ## 🚀 E. Jalur Cepat & Format Jadul (`scanf` & `printf`)
 
 Diibaratkan sebagai **"Robot Pelayan Restoran"**. Kamu tidak bisa asal lempar barang, harus sebutkan **Kode Meja (Format Specifier)**.
 
 | Tipe Data | Kode Meja | Arti Mudah |
 | :--- | :--- | :--- |
 | `int` | **`%d`** | "Robot, ambilkan Bilangan Bulat!" |
 | `long long`| **`%lld`** | "Robot, ambilkan Angka Besar!" |
 | `double`| **`%lf`** | "Robot, ambilkan Angka Koma!" |
 | `char` | **`%c`** | "Robot, ambilkan Satu Huruf!" |
 
 ### 🎯 1. Keajaiban Formatting
 Inilah kehebatan `printf`. Kamu bisa mengatur jumlah nol di belakang koma:
 - **`%.2lf`**: Cetak angka, sisakan **2 angka** saja di belakang titik.
 - **`%.0lf`**: Buang semua komanya!
 
 ### 📝 2. Cara Menulis Input (`scanf`)
 ```cpp
 scanf("%d", &uang); // Jangan lupa & (Alamat GPS laci kamu!)
 ```
 
 ---
 
 ## ⚠️ F. Aturan Main Loker (Jebakan Dasar)
 
 ### ❌ 1. Integer Division (Pembagian Tanpa Ampun)
 **Analogi Loker Semen Kerah Tanpa Celah**:
 Di dunia `int`, `5 / 2` hasilnya adalah **2**. Angka `0.5` nya hangus terbakar karena tidak muat masuk ke laci semen (`int`).
 *Pelajaran:* Di kodingan, angka koma dalam pembagian integer tidak dibulatkan, tapi **DIPOTONG PAKSA**.
 
 ### 🗑️ 2. Laci Bekas (Garbage Value)
 Jika loker kamu tidak diisi angka awal, robot akan mengisinya dengan **"Sampah"** angka acak besar dari program lain. 
 - **Solusi**: Selalu isi nol di awal! `int skor = 0;` 
 
 ---
 
 ## 🔮 G. Sihir Sisa Bagi (Modulo `%`)
 
 Modulo artinya: **"Cari Paksa Sisanya!"**
 
 **Analogi Kelereng Harian**:
 Kamu punya 11 kelereng, mau dibagi ke 3 orang. 
 - Setiap anak dapet 3 biji utuh (`11 / 3 = 3`).
 - Di tanganmu sisa **2 biji** yang nggak bisa dibagi rata. Itulah hasil Modulonya! (`11 % 3 = 2`).
 
 ### 🧪 Detektif Angka
 - **`x % 2 == 0`**: "Robot, apakah angka ini GENAP?"
 - **`x % 2 != 0`**: "Robot, apakah angka ini GANJIL?"
 
 ---
 
 ## ➕ H. Operator Aritmatika & Hierarki (KABATAKU)
 
 Inilah **"Siapa yang Menang Duluan?"**:
 1. **Kasta Bangsawan `( )`**: Wajib dikerjakan paling pertama!
 2. **Kasta Menengah `*`, `/`, `%`**: Lebih kuat dari penambahan.
 3. **Kasta Rakyat `+`, `-`**: Paling buncit dikerjakan.
 
 ---
 
 ## 🛠️ I. Alat Hitung Lanjutan (`cmath`)
 
 Diibaratkan sebagai **"Kamus Perkakas Robot"**:
 - **`abs(x)`**: Buang tanda minusnya! (Pasti Positif).
 - **`sqrt(x)`**: Cari akar kuadratnya.
 - **`floor(x)` (Lantai)**: Tarik paksa ke bawah. (`2.9` jadi `2`).
 - **`ceil(x)` (Atap)**: Dorong paksa ke atas. (`2.1` jadi `3`).
 
 ---
 
 ## 🚚 J. Operator Assignment & Increment
 
 **Analogi Pindah Barang**:
 - **`a = 5`**: Ambil angka 5, masukkan ke laci `a`. (Lama dibuang, Baru masuk).
 - **`a += 2`**: "Isi laci `a` sekarang tolong ditambahkan 2 ya."
 
 ### ⚠️ Jebakan Batman: Pre vs Post
 - **`++a` (Gaji Awal)**: Robot tambahkan angkamu dulu, baru kamu pakai.
 - **`a++` (Komisi Akhir)**: Kamu pakai dulu angka lamanya, baru robot tambahkan di baris besok.
 
 ---
 
 ## 🚦 K. Operator Perbandingan (Timbangan Benar-Salah)
 
 Hasil dari timbangan ini cuma ada dua: **True (1)** atau **False (0)**.
 - `==`: "Apakah isinya kembar?"
 - `!=`: "Apakah isinya beda?"
 
 > [!IMPORTANT]
 > **Jebakan Maut:** Jangan tertukar antara `=` (Pindah barang) dengan `==` (Tanya kabar/Perbandingan). 
 
 ---
 
 ## 🚦 L. Operator Logika (Pintu Berlapis)
 
 - **`&&` (DAN)**: Seperti pintu berkunci ganda. **Semua kunci** harus benar baru bisa lewat.
 - **`||` (ATAU)**: Seperti pintu dengan banyak kunci cadangan. Asal ada **satu kunci** yang benar, langsung lewat!
 
 ---
 
 ## 🔢 M. Hasil Akhir Logika & Wajah Benar-Salah
 
 Di mata robot C++, Benar dan Salah itu punya **"Wajah Angka"**:
 - **False** = Mutlak angka **0**.
 - **True** = Apa pun yang **BUKAN 0**. (Angka `1`, `-1`, atau `999` semuanya dianggap BENAR).
 
 ---
 
 ## 🧪 N. Tip & Trick Khas OSN-K
 
 1. **`1e9`**: Cara cepat nulis 1 Miliar.
 2. **`1e9+7`**: "Angka Sakral" juri agar hasil hitunganmu tidak jebol/overflow.
 
 ### ⚠️ Jebakan Overflow (1LL)
 ```cpp
 long long c = 1LL * a * b; // Sertakan 1LL agar robot mau berhitung di skala Peti Kemas!
 ```
 
 ---
 
 ## 🔤 O. Perang Kasta & ASCII Table
 
 ### 1. Siapa yang Lebih Suci? (Promosi Kasta)
 `char` (Rakyat) < `int` (Prajurit) < `double` (Bangsawan).
 Jika rakyat dan bangsawan bertarung dalam satu rumus, robot akan mengubah semuanya menjadi kasta tertinggi (**Bangsawan/Double**) agar adil!
 
 ### 🧠 2. Ilmu Perubahan Paksa (Casting)
 Kamu bisa memaksa robot mengubah kasta angka pakai kurung:
 `(double)10 / 4` $\rightarrow$ Robot dipaksa melihat angka 10 sebagai bangsawan, sehingga hasilnya **2.5** (Bukan 2).
 
 ---
 
 ## 🌍 P. Wilayah Kekuasaan (Scope)
 
 **Analogi Ketua OSIS vs Ketua Kelas**:
 - **Global** (Luar main): Ketua OSIS. Dikenal semua orang, otomatis berisi 0 (Loker Bersih).
 - **Lokal** (Dalam main): Ketua Kelas. Cuma dikenal di kelas itu saja, lokernya berantakan (Garbage).
 
 ---
 
 ## 📜 Rangkuman & Uji Tracing
 
 ### 🏆 Ceklis Emas Penelusuran (Cek 3 Detik!)
 1.  **Tipe Data**: Adakah pembagian `int` yang melenyapkan koma?
 2.  **Kasta Operator**: Dahulukan Bangsawan (KABATAKU)!
 3.  **Perubahan Loker**: Cek apakah nilai variabel sudah ditimpa perintah baru?
 
 ---
 
 ### 🧠 Uji Tracing (Level 5: THE ULTIMATE BOSS)
 
 ```cpp
 char c = 'C'; 
 int x = 10;
 long long y = 1e9;
 double z = 4.0;
 
 int a = c - 'A'; // 67 - 65 = 2
 int b = ++a + (x++ % 3); // 3 + (1) = 4. (x jadi 11)
 int res = (b * sqrt(z)) - (y / 500000000); // 8 - 2 = 6
 bool final_cek = (res > 5); // True (1)
 int ans = final_cek + x; // 1 + 11 = 12
 
 printf("ans = %d", ans);
 ```
 **Output: ans = 12**
 
 ---
 
 ⏩ **Lanjut ke Modul Kedua:** [Logika Percabangan (Razia BP)](../02-percabangan/materi.md)
