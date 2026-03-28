# 1. Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)
 
 Selamat datang di markas besar *Compiler Manusia*! 
 Di sini, mesin Juri OSN-K akan melempar sebaris dua baris kode berbahasa **C++** yang memanipulasi rentetan angka. Sebagai *Compiler Manusia*, kamu wajib tahu sifat-sifat kejam kodingan C++ yang sering kali **berlawanan dengan hukum matematika di sekolah**.
 
 Mari kita bedah konsep penjebak massal mulai dari aturan penulisan hingga kasta tertinggi tipe data.
 
 ---
 
 ## 📋 A. Pemanasan: Aturan Dasar Menulis Kode
 
 Sebelum kita masuk ke angka, ada 5 aturan "Sopan Santun" di C++ yang wajib muridmu tahu:
 
 1. **Titik Koma (`;`) dalah Titik**: Setiap satu perintah selesai, wajib diakhiri `;`. 
 2. **Komentar (`//`) adalah Catatan**: Tulis apapun setelah `//` tidak akan dibaca oleh komputer. 
 3. **C++ itu Beda Huruf (Case Sensitive)**: `Uang` dan `uang` adalah dua laci yang **BERBEDA**. Hati-hati dengan huruf kapital!
 4. **Nama Loker (Variabel)**: Tidak boleh ada **Spasi**, tidak boleh diawali **Angka**.
 5. **Petik Tunggal vs Ganda**: Satu huruf pakai petik tunggal `'A'`, kalau teks panjang memakai petik ganda `"Halo"`.
 
 ### 🚫 Kata-Kata Terlarang (Reserved Words)
 Komputer punya "Kamus Kata Sakti" yang sudah memiliki fungsi khusus. Kamu **DILARANG KERAS** menggunakan kata-kata ini sebagai nama variabelmu.
 
 | Kategori | Kata Terlarang |
 | :--- | :--- |
 | **Tipe Data** | `bool`, `char`, `double`, `float`, `int`, `long`, `short`, `signed`, `unsigned`, `void`, `wchar_t`, `auto` |
 | **Kontrol Alur** | `break`, `case`, `continue`, `default`, `do`, `else`, `for`, `goto`, `if`, `return`, `switch`, `while` |
 | **Akses & Memori** | `class`, `const`, `delete`, `enum`, `extern`, `friend`, `inline`, `mutable`, `namespace`, `new`, `operator`, `private`, `protected`, `public`, `register`, `sizeof`, `static`, `struct`, `template`, `this`, `typedef`, `union`, `using`, `virtual`, `volatile` |
 | **Logika & Lainnya** | `and`, `and_eq`, `asm`, `bitand`, `bitor`, `compl`, `const_cast`, `dynamic_cast`, `explicit`, `export`, `false`, `not`, `not_eq`, `or`, `or_eq`, `reinterpret_cast`, `static_cast`, `throw`, `true`, `try`, `typeid`, `typename`, `xor`, `xor_eq` |
 
 **Analogi**: Jangan menamai anjing peliharaanmu "Pelayan" di dalam restoran, seisi restoran akan bingung! Begitu juga di C++, jangan menamai variabelmu `int` atau `if`.
 
 ---
 
 ## 🛠️ B. Boilerplate: Perlengkapan Wajib C++
 
 Pernah lihat baris `#include <iostream>` atau `int main()`? Jangan pusing, anggap itu **Perlengkapan Wajib**:
 - `#include <iostream>`: Seperti membawa **Tas Belanja**. Di dalam tas ini ada alat `cin` and `cout`.
 - `using namespace std;`: Izin agar kita bisa memanggil `cin` dan `cout` langsung tanpa mendaftarkannya satu-per-satu.
 - `int main() { ... }`: Inilah **Dapur Utama**. Komputer hanya akan memasak apa yang ada di dalam kurung kurawal `{ }` fungsi ini.
 
 ---
 
 ## 📦 C. Rahasia Loker Ajaib (Konsep Variabel & Tipe Dasar)
 
 Sebelum bisa memberi perintah ke komputer, kamu harus menyiapkan **"Loker"** untuk menyimpan datamu.
 
 ### 🔍 1. Apa Itu Variabel? (Analogi Loker Sekolah)
 Bayangkan kamu punya barisan loker di sekolah. Untuk menyimpan barang, kamu harus melakukan 3 hal:
 1.  **Pilih Ukuran Loker** (Tipe Data): Apakah kamu butuh loker kecil untuk permen, atau peti kemas untuk sepeda?
 2.  **Beri Label Nama** (Variabel Name): Agar kamu tidak tertukar dengan loker temanmu.
 3.  **Isi Barangnya** (Value): Masukkan angka atau huruf ke dalamnya.
 
 Di C++, cara memesan loker adalah:
 `TipeData NamaLoker = IsiAwal;`
 
 **Contoh**: `int skor = 100;` 
 Artinya: "Robot, siapkan loker ukuran **Integer** bernama **Skor**, dan langsung isi dengan angka **100**."
 
 ### ✨ 2. Loker Berjamaah (Deklarasi Berantai)
 Seringkali murid malas membuat laci satu per satu. Kamu bisa membuat banyak laci sekaligus asal ukurannya sama:
 ```cpp
 int a, b, c; // Robot membuat 3 laci kosong sekaligus!
 int x = 5, y = 10, z = 15; // Robot membuat 3 laci dan mengisinya sekaligus!
 ```
 
 ### 🧪 3. Macam-Macam Ukuran Loker (Tipe Data Dasar)
 Di OSN-K, pemilihan ukuran loker sangat menentukan apakah kamu dapat skor atau tidak.
 
 - `int` (**Loker Semen**): Cuma bisa diisi **Bilangan Bulat** (-2 miliar s.d 2 miliar).
 - `long long` (**Peti Kemas**): Loker raksasa. Untuk angka triliunan atau $10^{18}$.
 - `bool` (**Saklar Lampu**): Cuma punya dua kemungkinan: **`true`** (Benar/1) atau **`false`** (Salah/0).
 - `double` (**Gelas Takar**): Spesialis angka koma/pecahan ($3.14$).
 
 ### 🔒 4. Loker Tertutup (Konstanta `const`)
 Terkadang ada angka yang **tidak boleh diubah** (misalnya nilai Maksimal). Kita menyegelnya dengan kata sakti `const`:
 ```cpp
 const int MAX_N = 100;
 MAX_N = 200; // <--- ERROR! Robot akan marah karena segel pabrik dirusak.
 ```
 
 ---
 
 ## 🚪 D. Komunikasi Dasar (Input `cin` & Output `cout`)
 
 Setelah laci siap, bagaimana cara memasukkan barang dari keyboard dan mencetaknya ke layar?
 
 1. **`cin >> laci;` (Input)**: Corong masuk dari Keyboard.
 2. **`cout << laci;` (Output)**: Corong keluar ke Layar.
 
 ### 🧱 Rantai Kereta (Chaining cin/cout)
 Kamu bisa menyambungnya seperti gerbong kereta:
 ```cpp
 cin >> a >> b >> c; // Sekali sedot 3 angka dari keyboard!
 ```
 **Hati-hati: Jebakan Menempel!**
 Saat mencetak dua angka, robot C++ tidak otomatis memberimu spasi.
 ```cpp
 cout << a << b; // Jika a=10, b=20, hasilnya: 1020 (SALAH!)
 cout << a << " " << b; // Hasilnya: 10 20 (BENAR).
 ```
 
 ### ⚠️ Jebakan Kecepatan: `endl` vs `"\n"`
 Memakai `endl` di soal dengan ribuan data bisa membuat programmu **TLE** (Terlalu Lambat)!
 - **`endl` (Lompat Sambil Ngosongin)**: Selain membuat baris baru, ia memaksa komputer mengosongkan aliran data (*Flush*) ke layar. Ini **LAMBAT**.
 - **`"\n"` (Lompat Saja)**: Hanya pindah baris tanpa mengganggu aliran data. Ini **CEPAT**.
 
 ### ⚡ Mantra Pelicin (Fast I/O)
 Agar `cin` dan `cout` secepat kilat (setara `scanf`), taruh mantra ini di awal `int main()`:
 ```cpp
 ios::sync_with_stdio(0);
 cin.tie(0);
 ```
 
 ---
 
 ## 🚀 E. Jalur Cepat & Format Jadul (`scanf` & `printf`)
 
 Kenapa harus dipelajari? Karena lebih **CEPAT** memproses jutaan angka dan lebih **MUDAH** mengatur tampilan koma.
 
 | Tipe Data | Kode Meja | Tipe Data | Kode Meja |
 | :--- | :--- | :--- | :--- |
 | `int` | **`%d`** | `long long`| **`%lld`** |
 | `double`| **`%lf`** | `char` | **`%c`** |
 
 ### 📝 1. Cara Menulis Output (`printf`)
 ```cpp
 printf("Skor saya adalah %d poin", 100);
 ```
 
 ### 🎯 2. Keajaiban Formatting
 Kita bisa memesan berapa angka di belakang koma dengan mudah:
 - **`%.2lf`**: Angka koma, cukup **2 angka** saja di belakang titik.
 - **`%.0lf`**: Hilangkan semua angka belakang koma.
 
 ### 📝 3. Cara Menulis Input (`scanf`)
 ```cpp
 scanf("%d", &uang);
 ```
 **Hati-hati: Jebakan "&" (Alamat GPS)**
 Pada `scanf`, kamu wajib menaruh simbol **`&`** (Ampersand). Robot butuh **Alamat GPS** (`&`) untuk tahu di mana laci itu berada.
 
 ---
 
 ## ⚠️ F. Aturan Main Loker (Jebakan Dasar)
 
 ### ❌ 1. Integer Division (Pembagian Tanpa Ampun)
 **Di kodingan `int`, `5 / 2` HASILNYA ADALAH `2`!** Lho kok bisa? Kemana sisa $0.5$ nya?
 **Analogi Laci Semen keras**: Koma-nya hangus terbakar karena masuk ke laci yang tidak bisa menyimpan desimal.
 *Aturan:* Kalau tipe datanya `int`, setiap ada rumus Pembagi `/`, **buang semua angka komanya tanpa pembulatan**.
 
 ### 🗑️ 2. Laci Bekas Penghuni Lama (Garbage Value)
 Jika kamu membuat loker tapi tidak mengisinya, isinya akan berupa **"Sampah"** angka acak raksasa dari program lain!
 - **Pelajaran:** Selalu beri nilai awal, misalnya: `int saldo = 0;`. 
 
 ---
 
 ## 🔮 G. Sihir Sisa Bagi (Modulo `%`)
 
 Modulo artinya: **"Cari Sisa Baginya!"**
 `14 % 4 = 2` (Karena $3 \times 4 = 12$, sisa 2 kelereng yang gak bisa dibagi).
 
 ### 🧪 Pendeteksi Genap-Ganjil
 - **Genap**: `if (x % 2 == 0)` $\rightarrow$ "Apakah sisa bagi 2 adalah nol?"
 - **Ganjil**: `if (x % 2 != 0)` atau `if (x % 2 == 1)` $\rightarrow$ "Apakah sisa bagi 2 tidak nol?"
 
 ### ⚠️ Modulo Angka Kecil vs Besar
 Berapa hasil `3 % 7`? Jawabannya **3**.
 *Aturan:* Jika angka kiri *lebih kecil* dari angka kanan, jawabannya adalah **Angka Kiri** itu sendiri.
 
 ---
 
 ## ➕ H. Operator Aritmatika & Hierarki (KABATAKU)
 
 1. Lingkaran Kurung `( )` $\rightarrow$ **Kasta Tertinggi** (Wajib duluan!).
 2. Perkalian `*`, Pembagian `/`, and Modulo `%` $\rightarrow$ **Kasta Menengah**.
 3. Penjumlahan `+` dan Pengurangan `-` $\rightarrow$ **Kasta Rakyat**.
 
 ---
 
 ## 🛠️ I. Alat Hitung Lanjutan (`cmath`)
 
 1. **`abs(x)` (Nilai Mutlak)**: Menghilangkan tanda minus. `abs(-5)` jadi `5`.
 2. **`sqrt(x)` (Akar Kuadrat)**: `sqrt(16)` jadi `4`.
 3. **`pow(a, b)` (Pangkat)**: `pow(2, 3)` jadi `8`.
 4. **`round(x)` (Pembulatan Terdekat)**: `round(2.6)` jadi `3`.
 5. **`floor(x)` (Lantai)**: Memaksa pembulatan ke **BAWAH**. `floor(2.9)` jadi `2`. 
 6. **`ceil(x)` (Atap)**: Memaksa pembulatan ke **ATAS**. `ceil(2.1)` jadi `3`. (**Penting untuk soal bus/rak!**)
 
 ### ⚠️ Tanda Bahaya: INF & NAN
 Terkadang, robot mengeluarkan kata-kata ajaib di layarmu. Jangan panik, inilah artinya:
 - **`inf` (Infinity)**: Terjadi jika kamu membagi angka koma dengan nol (misal: `1.0 / 0.0`). Tak hingga!
 - **`nan` (Not a Number)**: Terjadi jika kamu menaruh perintah yang mustahil (misal: `sqrt(-1.0)`). Akar angka negatif itu tidak ada di dunia nyata robot!
 
 > [!TIP]
 > Hati-hati! Hasil dari `sqrt`, `pow`, `floor`, dan `ceil` otomatis berwujud **`double`** (angka koma), meskipun kamu memasukkan angka bulat.
 
 ---
 
 ## 🚚 J. Operator Assignment & Increment
 
 **1. `a = 5`**: Pindahkan barang ke laci `a`.
 **2. `a += 2`**: Ambil isi laci `a`, tambah 2, masukkan lagi.
 
 ### ⚠️ Jebakan Batman: Pre vs Post
 - **`++a` (Pre-increment)**: "Tambah dulu, baru dipakai."
 - **`a++` (Post-increment)**: "Pakai nilai sekarang dulu, baru tambah di baris berikutnya."
 
 ---
 
 ## 🚦 K. Operator Perbandingan & Logika
 
 - `==` (Sama dengan), `!=` (Tidak sama), `<`, `>`, `<=`, `>=`.
 - `&&` (DAN): Harus **Semua Benar**.
 - `||` (ATAU): Asal ada **Satu Benar**.
 - `!` (TIDAK): Kacamata kebalikan.
 
 ---
 
 ## 🔢 L. Hasil Akhir Logika & Nilai Kebenaran
 
 - **Hasil Logika**: `(10 > 5)` bernilai **1** (Benar), `(5 > 10)` bernilai **0** (Salah).
 - **Kebalikan**: Di kodingan, **HANYA angka 0** yang dianggap **FALSE**. Angka lainnya (`-1`, `1`, `999`) dianggap **TRUE**!
 
 ---
 
 ## 🧪 M. Tip & Trick Khas OSN-K
 
 1. **Angka Eksponen**: `1e9` = 1 Miliar. `2e9` = Batas maksimal `int`.
 2. **Modulo 1e9+7**: Angka sakral juri untuk mencegah luapan angka raksasa.
 
 ### ⚠️ Jebakan Overflow (1LL)
 ```cpp
 int a = 1000000;
 int b = 1000000;
 long long c = 1LL * a * b; // Pakai 1LL agar robot berhitung di skala raksasa!
 ```
 
 ---
 
 ## 🔤 N. Perang Kasta & ASCII Table
 
 ### 1. Kasta Tipe Data (Type Promotion)
 `char` $\rightarrow$ `int` $\rightarrow$ `double`. Saat dicampur, kasta tertinggi selalu menang!
 
 ### 🧠 2. Ilmu Perubahan Paksa (Explicit Casting)
 Terkadang kita ingin memaksa robot mengubah tipe data di tengah jalan. Gunakan kurung `(tipe_tujuan)` di depan angka.
 - **Trik Jitu Pembagian**: `int a = 5, b = 2; double hasil = (double)a / b;` $\rightarrow$ Hasilnya **2.5**! (Karena `a` dipaksa jadi `double` dulu).
 
 ### 3. Tabel Sakti ASCII
 | Karakter | Kode ASCII | Trik Penting |
 | :--- | :--- | :--- |
 | `'0' s.d '9'` | **48 s.d 57** | `c - '0'` = Mengubah karakter angka jadi angka asli. |
 | `'A' s.d 'Z'` | **65 s.d 90** | `'C' - 'A'` = 2 (Urutan abjad). |
 | `'a' s.d 'z'` | **97 s.d 122**| Selisih Huruf Besar & Kecil adalah **32**. |
 
 ---
 
 ## 🌍 O. Wilayah Kekuasaan (Scope Global vs Lokal)
 
 - **LOKAL**: Dibentuk di dalam `main()`. Isinya sampah jika tidak diisi.
 - **GLOBAL**: Dibentuk di ATAS `main()`. **Otomatis berisi 0** tanpa perlu diisi. (Pilihan terbaik untuk OSN-K!).
 
 ---
 
 ## 📜 Rangkuman & Uji Tracing
 
 ### 🏆 Ceklis Emas Penelusuran (Cek 3 Detik!)
 1.  **Tipe Data**: Adakah pembagian `int` yang melenyapkan koma?
 2.  **Kasta Operator**: Dahulukan KABATAKU!
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
