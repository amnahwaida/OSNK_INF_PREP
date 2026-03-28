# 1. Tipe Data & Operator Dasar (Loker Kelas & Pembagian Permen)
 
 Selamat datang di markas besar *Compiler Manusia*! 
 Di sini, mesin Juri OSN-K akan melempar sebaris dua baris kode berbahasa **C++** yang memanipulasi rentetan angka. Sebagai *Compiler Manusia*, kamu wajib tahu sifat-sifat kejam kodingan C++ yang sering kali **berlawanan dengan hukum matematika di sekolah**.
 
 Mari kita bedah konsep penjebak massal mulai dari aturan penulisan hingga kasta tertinggi tipe data.
 
 ---
 
 ## 📋 A. Pemanasan: Aturan Dasar Menulis Kode
 
 Sebelum kita masuk ke angka, ada 5 aturan "Sopan Santun" di C++ yang wajib muridmu tahu agar program tidak menolak untuk berjalan (*Compile Error*):
 
 1. **Titik Koma (`;`) dalah Titik**: Setiap satu perintah selesai, wajib diakhiri `;`. Tanpa ini, komputer akan menganggap perintahmu menyambung tanpa henti dan ia akan bingung!
 2. **Komentar (`//`) adalah Catatan**: Tulis apapun setelah `//` tidak akan dibaca oleh komputer. Gunakan ini untuk memberi tanda atau catatan pribadi pada kodemu.
 3. **C++ itu Beda Huruf (Case Sensitive)**: `Uang` dan `uang` adalah dua laci yang **BERBEDA**. Robot C++ sangat teliti; bagi dia, satu perbedaan huruf kapital saja sudah membuat identitasnya berubah total.
 4. **Nama Loker (Variabel)**: Tidak boleh ada **Spasi**, tidak boleh diawali **Angka**. Gunakan garis bawah (misal: `uang_jajan`) jika ingin memakai dua kata.
 5. **Petik Tunggal vs Ganda**: Satu huruf pakai petik tunggal (`'A'`), kalau teks panjang memakai petik ganda (`"Halo"`). Robot C++ menggunakan ini untuk tahu kapan sebuah teks dimulai dan berakhir.
 
 ### 🚫 Kata-Kata Terlarang (Reserved Words)
 Komputer punya "Kamus Kata Sakti" yang sudah memiliki fungsi khusus. Kamu **DILARANG KERAS** menggunakan kata-kata ini sebagai nama variabelmu karena robot akan menyangka kamu sedang memberi perintah, bukan memanggil laci.
 
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
 - `#include <iostream>`: Seperti membawa **Tas Belanja**. Di dalam tas ini ada alat "masuk" (`cin`) and "keluar" (`cout`).
 - `using namespace std;`: Izin agar kita bisa memanggil alat-alat tersebut secara langsung tanpa harus mengetik kode pendaftaran yang panjang.
 - `int main() { ... }`: Inilah **Dapur Utama**. Komputer hanya akan memasak instruksi yang kamu taruh di dalam kurung kurawal `{ }` fungsi ini.
 
 ---
 
 ## 📦 C. Rahasia Loker Ajaib (Konsep Variabel & Tipe Dasar)
 
 Sebelum bisa memberi perintah ke komputer, kamu harus menyiapkan **"Loker"** (Penyimpanan) di memori komputer agar data tidak hilang begitu saja.
 
 ### 🔍 1. Apa Itu Variabel? (Analogi Loker Sekolah)
 Bayangkan kamu punya barisan loker di sekolah. Untuk menyimpan barang, kamu harus melakukan 3 hal secara runtut:
 1.  **Pilih Ukuran Loker** (Tipe Data): Apakah kamu butuh loker kecil untuk permen, atau peti kemas raksasa?
 2.  **Beri Label Nama** (Variabel Name): Agar kamu tahu laci mana yang berisi uang jajan, dan mana yang berisi nilai ujian.
 3.  **Isi Barangnya** (Value): Masukkan angkanya ke dalamnya.
 
 Di C++, cara memesan loker adalah:
 `TipeData NamaLoker = IsiAwal;`
 
 **Contoh**: `int skor = 100;` 
 Artinya: "Robot, pesankan satu loker berlabel **Int** (ukuran standar), beri nama **skor**, dan isi dengan angka **100**."
 
 ### ✨ 2. Loker Berjamaah (Deklarasi Berantai)
 Jika kamu butuh banyak laci dengan ukuran yang sama, kamu tidak perlu mengetik berkali-kali. Cukup gunakan tanda koma:
 ```cpp
 int a, b, c; // Memesan 3 laci kosong sekaligus.
 int x = 5, y = 10; // Memesan 2 laci dan langsung mengisinya.
 ```
 
 ### 🧪 3. Macam-Macam Ukuran Loker (Tipe Data Dasar)
 Di OSN-K, pemilihan tipe data sangat krusial. Salah pilih bisa membuat angkamu "tumpah" (overflow) dan nilaimu jadi salah!
 
 - **`int`** (Loker Standar): Paling sering dipakai. Kapasitasnya pas untuk angka bulat dari -2 miliar sampai 2 miliar.
 - **`long long`** (Peti Kemas): Loker raksasa untuk angka triliunan (hingga $10^{18}$). Pakailah ini jika soal melibatkan perkalian angka besar.
 - **`bool`** (Saklar Lampu): Loker paling irit. Hanya bisa berisi dua hal: **`true`** (1) atau **`false`** (0).
 - **`double`** (Gelas Takar): Digunakan jika datanya memiliki koma atau pecahan ($3.14$ atau $0.5$).
 
 ### 🔒 4. Loker Tertutup (Konstanta `const`)
 Jika ada angka yang sifatnya permanen dan tidak boleh berubah (misal: nilai maksimal peserta), gunakan kata sakti `const`:
 ```cpp
 const int MAX_N = 100;
 MAX_N = 200; // <--- ERROR! Robot akan protes karena segel pabriknya dirusak.
 ```
 
 ---
 
 ## 🚪 D. Komunikasi Dasar (Input `cin` & Output `cout`)
 
 Bagaimana cara kita memasukkan data dari keyboard ke loker, dan menampilkannya ke layar?
 
 1. **`cin >> laci;` (Input)**: Bayangkan ini corong yang menyedot apa yang kamu ketik di keyboard ke dalam `laci`.
 2. **`cout << laci;` (Output)**: Bayangkan ini proyektor yang menembakkan isi `laci` ke layar monitormu.
 
 ### 🧱 Rantai Kereta (Chaining)
 Kamu bisa menyambungkan perintah input/output seperti gerbong kereta api:
 ```cpp
 cin >> a >> b >> c; // Sekali sedot 3 angka sekaligus!
 ```
 **Hati-hati: Jebakan Menempel!**
 Robot C++ itu sangat polos. Jika kamu mencetak dua variabel berturut-turut, ia tidak akan memberimu spasi otomatis.
 ```cpp
 cout << a << b; // Jika a=10, b=20, hasilnya: 1020 (Bisa disangka angka sepuluh ribu!)
 cout << a << " " << b; // Gunakan " " secara manual agar rapi: 10 20.
 ```
 
 ### ⚠️ Jebakan Kecepatan: `endl` vs `"\n"`
 Dalam kompetisi, kecepatan itu segalanya.
 - **`endl`**: Lambat karena ia membuat baris baru sambil "menguras" aliran data ke layar.
 - **`"\n"`**: Sangat cepat karena ia hanya fokus memindahkan kursor ke baris baru.
 
 ### ⚡ Mantra Pelicin (Fast I/O)
 Taruh baris ini di awal fungsi `main` agar `cin` dan `cout` kamu berlari secepat kilat:
 ```cpp
 ios::sync_with_stdio(0); cin.tie(0);
 ```
 
 ---
 
 ## 🚀 E. Jalur Cepat & Format Jadul (`scanf` & `printf`)
 
 Juri OSN-K kadang memberikan data jutaan angka. Cara paling aman untuk menanganinya dengan cepat adalah menggunakan gaya penulisan bahasa C (`scanf/printf`).
 
 | Tipe Data | Kode Meja | Tipe Data | Kode Meja |
 | :--- | :--- | :--- | :--- |
 | `int` | **`%d`** | `long long`| **`%lld`** |
 | `double`| **`%lf`** | `char` | **`%c`** |
 
 ### 🎯 Keajaiban Formatting
 Inilah alasan utama kita memakai `printf`. Kita bisa memesan berapa angka yang ingin ditampilkan di belakang koma:
 - **`%.2lf`**: Menampilkan 2 angka saja di belakang koma (hasil pembulatan tampilan).
 - **`%.0lf`**: Menghilangkan seluruh angka koma.
 
 ### 📝 Input dengan Scanf
 ```cpp
 scanf("%d", &uang); 
 ```
 **Pesan Penting**: Jangan lupakan simbol **`&`** (Ampersand). Robot butuh alamat GPS variabelmu agar dia tidak salah menaruh data!
 
 ---
 
 ## ⚠️ F. Aturan Main Loker (Jebakan Dasar)
 
 ### ❌ 1. Integer Division (Pembagian Tanpa Ampun)
 **Di mesin C++, `5 / 2` HASILNYA ADALAH `2`!** Lho kok bisa?
 **Analogi Loker Semen**: Karena `int` adalah loker batu yang keras, ia tidak bisa menampung "serpihan desimal".
 *Aturan Emas:* Setiap pembagian antara integer, robot akan **memotong buang semua angka koma** tanpa mempedulikan pembulatan matematika.
 
 ### 🗑️ 2. Laci Bekas Penghuni Lama (Garbage Value)
 Jika kamu membuat variabel tapi lupa memberi isi awal (Inisialisasi), robot tidak akan mengosongkannya. Ia akan membiarkan **"Sampah"** angka acak raksasa tertinggal di sana.
 - **Solusi Juara**: Biasakan mengisi nol di awal: `int poin = 0;`.
 
 ---
 
 ## 🔮 G. Sihir Sisa Bagi (Modulo `%`)
 
 Jika pembagi (`/`) membuang sisa, maka operator Modulo (`%`) justru bertugas untuk **mencari sisanya**!
 
 **Analogi Kelereng**:
 Punya 11 kelereng dibagi ke 3 kantong. Setiap kantong isi 3 utuh ($3 \times 3 = 9$). Sisanya yang tidak bisa dibagi rata adalah **2**. Maka, `11 % 3 = 2`.
 
 ### 🧪 Detektif Logika
 - **`x % 2 == 0`**: Berarti angka itu **GENAP**.
 - **`x % 2 != 0`**: Berarti angka itu **GANJIL**.
 
 ### ⚠️ Modulo Angka Kecil vs Besar
 Berapa hasil `3 % 7` (3 sisa bagi 7)? Jawabannya adalah **3**.
 *Logikanya:* Jika barangnya lebih sedikit daripada pembaginya, maka tidak ada yang bisa dibagikan satu pun, sehingga barang di tanganmu tetap utuh (semuanya sisa).
 
 ---
 
 ## ➕ H. Operator Aritmatika & Hierarki (KABATAKU)
 
 Komputer tidak menghitung dari kiri ke kanan secara membabi buta. Ia mengikuti hukum kasta:
 1. **Kasta Bangsawan `( )`**: Apa pun di dalam kurung dikerjakan paling duluan.
 2. **Kasta Prajurit `*`, `/`, `%`**: Lebih kuat daripada tambah-kurang.
 3. **Kasta Rakyat `+`, `-`**: Dikerjakan paling akhir.
 
 ---
 
 ## 🛠️ I. Alat Hitung Lanjutan (`cmath`)
 
 Untuk rumus yang lebih rumit, kita butuh "Kotak Perkakas" tambahan dari perpustakaan `#include <cmath>`:
 - **`abs(x)`**: Mengubah angka minus jadi positif (Nilai Mutlak).
 - **`sqrt(x)`**: Mencari akar kuadrat.
 - **`floor(x)` (Lantai)**: Memaksa pembulatan ke bawah.
 - **`ceil(x)` (Atap)**: Memaksa pembulatan ke atas (Sangat berguna untuk soal menghitung jumlah bus/kotak penampung).
 
 ### 🚨 Tanda Bahaya: INF & NAN
 - **`inf` (Infinity)**: Berarti hasil hitunganmu tak terhingga (misal membagi angka dengan nol).
 - **`nan` (Not a Number)**: Berarti kamu menyuruh robot melakukan hal yang tidak mungkin (misal mencari akar dari angka negatif).
 
 ---
 
 ## 🚚 J. Operator Assignment (Pindah Barang)
 
 Di kodingan, simbol **`=`** bukan berarti "Sama Dengan", melainkan perintah untuk **"Memindahkan Barang"**.
 - **`a = 5`**: Ambil angka 5, taruh ke laci `a`. (Isi laci `a` yang lama akan langsung hangus/terhapus).
 - **`a += 2`**: Perintah cepat untuk "Ambil isi `a` sekarang, tambahkan 2, lalu masukkan lagi."
 
 ### ⚠️ Jebakan Batman: Pre vs Post
 - **`++a` (Naik Dulu)**: Robot menaikkan nilai dulu, baru angkanya dipakai dalam rumus.
 - **`a++` (Pakai Dulu)**: Robot memakai angka yang sekarang dulu untuk rumus, baru setelah rumus itu selesai, nilainya naik.
 
 ---
 
 ## 🚦 K. Operator Perbandingan & Logika
 
 - `==` (Sama dengan): "Apakah isinya identik?".
 - `!=` (Tidak sama): "Apakah isinya berbeda?".
 - `&&` (DAN): **Keduanya harus Benar** agar bisa lewat.
 - `||` (ATAU): Asal **salah satu Benar**, gerbang akan terbuka.
 - `!` (TIDAK): Pemutar balik fakta (Benar jadi Salah, Salah jadi Benar).
 
 ---
 
 ## 🔢 L. Hasil Akhir Logika & Wajah Benar-Salah
 
 Di mata robot, kebenaran itu berwujud angka:
 - **Benar (True)**: Biasanya angka **1**. Namun secara teknis, **apa pun yang BUKAN 0** dianggap BENAR oleh robot.
 - **Salah (False)**: Mutlak angka **0**.
 
 ---
 
 ## 🧪 M. Tip & Trick Khas OSN-K
 
 1. **Angka Eksponen**: Gunakan `1e9` untuk menulis 1 Miliar dengan cepat.
 2. **Modulo Sakral**: Juri sering meminta jawaban dimodulo $10^9+7$ untuk mencegah angka meluap dari loker `long long`.
 
 ### ⚠️ Jebakan Overflow (Trik 1LL)
 ```cpp
 int a = 1000000;
 int b = 1000000;
 long long c = 1LL * a * b; // Sertakan 1LL agar robot mau menghitung di skala raksasa!
 ```
 Tanpa `1LL`, robot akan menghitung perkalian di area laci kecil (`int`) dan hasilnya akan meledak menjadi angka sampah sebelum masuk ke `long long c`.
 
 ---
 
 ## 🔤 N. Perang Kasta (Konversi Tipe Data)
 
 ### 1. Promosi Kasta Otomatis
 Jika `int` dan `double` bertarung dalam satu rumus, robot akan otomatis menganggap si `int` naik jabatan menjadi `double` agar rumus tersebut akurat.
 
 ### 🧠 2. Perubahan Paksa (Explicit Casting)
 Kamu bisa memaksa robot mengubah pandangannya terhadap sebuah angka:
 `(double)5 / 2` $\rightarrow$ Robot akan melihat angka 5 sebagai `5.0`. Hasilnya pun jadi **2.5**, bukan lagi 2!
 
 ### 3. Tabel Sakti ASCII
 Karakter sebenarnya adalah angka yang memakai "topeng" simbol.
 | Karakter | Kode ASCII | Trik |
 | :--- | :--- | :--- |
 | `'0' s.d '9'` | **48 s.d 57** | `c - '0'` = Mendapatkan angka aslinya. |
 | `'A' s.d 'Z'` | **65 s.d 90** | `'C' - 'A' = 2` (Urutan abjad). |
 | `'a' s.d 'z'` | **97 s.d 122**| Selisih Huruf Besar & Kecil adalah **32**. |
 
 ---
 
 ## 🌍 O. Wilayah Kekuasaan (Scope Global vs Lokal)
 
 - **Variabel GLOBAL** (Ditaruh di atas `int main`): Seperti papan pengumuman di lapangan sekolah. Semua fungsi bisa melihatnya, dan hebatnya lagi, loker ini **otomatis bersih (berisi 0)** saat program baru dimulai. Pilihan favorit delegasi OSN!
 - **Variabel LOKAL** (Ditaruh di dalam `main`): Seperti catatan pribadi di dalam kelas. Hanya yang di dalam kelas yang tahu, dan isinya berantakan (sampah) jika tidak diisi.
 
 ---
 
 ## 📜 Rangkuman & Uji Tracing
 
 ### 🏆 Ceklis Emas Penelusuran (Cek 3 Detik!)
 Sebelum menulis jawaban akhir, pastikan:
 1.  **Tipe Data**: Apakah ada pembagian antar laci `int` yang melenyapkan koma?
 2.  **Kasta Operator**: Apakah hukum KABATAKU sudah dipatuhi?
 3.  **Perubahan Nilai**: Apakah ada laci yang isinya sudah ditimpa oleh perintah baru atau increment?
 
 ---
 
 ### 🧠 Uji Tracing (Level 1 - 5)
 
 <details>
 <summary><b>Level 1: Pembagi Permen (Klik untuk Buka)</b></summary>
 
 ```cpp
 int permen = 11;
 int anak = 3;
 int bagian = permen / anak;
 int sisa = permen % anak;
 printf("Dapat %d, Sisa %d", bagian, sisa);
 ```
 **Diagnosis Logika:**
 1. **Baris 1-2**: Kita memesan dua laci `permen` (isi 11) dan `anak` (isi 3).
 2. **Baris 3 (Pembagian `int`)**: Robot menghitung $11 \div 3 = 3.666...$. Namun, karena laci `bagian` adalah tipe `int` (loker semen), robot **memotong paksa** desimalnya. Hasil akhir: **3**.
 3. **Baris 4 (Modulo)**: Robot mencari sisa bagi. $11 \pmod 3$. Perkalian terdekat adalah $3 \times 3 = 9$. Maka sisanya adalah $11 - 9 = 2$. Hasil akhir: **2**.
 4. **Output**: Mengambil isi laci `bagian` dan `sisa`. Tercetak: **Dapat 3, Sisa 2**.
 </details>
 
 <details>
 <summary><b>Level 2: Pre-Post Gaji (Klik untuk Buka)</b></summary>
 
 ```cpp
 int a = 10;
 int b = a++;
 int c = ++a;
 printf("a=%d, b=%d, c=%d", a, b, c);
 ```
 **Diagnosis Logika:**
 1. **Baris 1**: `a` berisi 10.
 2. **Baris 2 (`a++`)**: Ini adalah *Post-Increment*. Robot akan memberikan nilai `a` yang **sekarang** (10) ke laci `b`. Setelah `b` terisi 10, barulah `a` naik menjadi 11.
 3. **Baris 3 (`++a`)**: Ini adalah *Pre-Increment*. Robot harus menaikkan nilai `a` **terlebih dahulu** sebelum memakainya. Nilai `a` yang tadinya 11 naik menjadi 12. Nilai baru ini (12) kemudian diberikan ke laci `c`.
 4. **Kondisi Akhir**: `a` = 12, `b` = 10, `c` = 12.
 5. **Output**: **a=12, b=10, c=12**.
 </details>
 
 <details>
 <summary><b>Level 3: Kasta Ksatria (Klik untuk Buka)</b></summary>
 
 ```cpp
 char huruf = 'A';
 int angka = 5;
 double hasil = huruf + angka;
 printf("%.0lf", hasil);
 ```
 **Diagnosis Logika:**
 1. **Konversi ASCII**: Robot melihat `'A'`. Ia mencari di tabel kamus ASCII dan menemukan kodenya adalah **65**.
 2. **Penjumlahan**: Robot menghitung $65 + 5 = 70$.
 3. **Promosi Kasta**: Karena laci `hasil` bertipe `double` (kasta tinggi), robot menyimpan angka 70 tadi dalam bentuk desimal: **70.000000...**.
 4. **Formatting**: Perintah `%.0lf` menyuruh robot: "Cetak angka koma ini, tapi jangan tampilkan satu pun angka di belakang titiknya."
 5. **Output**: **70**.
 </details>
 
 <details>
 <summary><b>Level 4: Kiamat Eksponen (Klik untuk Buka)</b></summary>
 
 ```cpp
 long long x = 1e9;
 int y = 2000000000;
 bool cek = (x * 2 > y);
 int hasil = cek + 10;
 printf("%d", hasil);
 ```
 **Diagnosis Logika:**
 1. **Eksponen**: `1e9` adalah 1 Miliar ($1.000 .000 .000$).
 2. **Perbandingan**: Robot menghitung `x * 2` yaitu 2 Miliar. Apakah 2 Miliar **lebih besar dari** 2 Miliar? Jawabannya **TIDAK/SALAH**.
 3. **Nilai Boelan**: Karena salah, laci `cek` berisi angka **0** (False).
 4. **Matematika Logika**: Robot menghitung `hasil = 0 + 10`. Hasil akhirnya adalah **10**.
 5. **Output**: **10**.
 </details>
 
 <details>
 <summary><b>Level 5: THE ULTIMATE BOSS (Klik untuk Buka)</b></summary>
 
 ```cpp
 char c = 'C'; 
 int x = 10;
 long long y = 1e9;
 double z = 4.0;
 
 int a = c - 'A'; 
 int b = ++a + (x++ % 3); 
 int res = (b * sqrt(z)) - (y / 500000000); 
 bool final_cek = (res > 5); 
 int ans = final_cek + x; 
 
 printf("ans = %d", ans);
 ```
 **Diagnosis Logika Sang Juara:**
 1. **Step 1 (ASCII Math)**: `'C'` adalah 67, `'A'` adalah 65. Maka `a = 67 - 65 = 2`.
 2. **Step 2 (Complex Increment)**:
    - **`++a`**: `a` naik dari 2 menjadi **3**.
    - **`x++ % 3`**: Robot memakai nilai `x` yang sekarang (**10**) untuk di-modulo 3. Hasilnya adalah **1**. Setelah operasi ini selesai, barulah `x` naik menjadi **11**.
    - **`b = 3 + 1 = 4`**.
 3. **Step 3 (The Math Engine)**:
    - **`sqrt(4.0)`** adalah 2.0. Maka `b * 2.0` = $4 \times 2 = 8$.
    - **`y / 500.000.000`** $\rightarrow$ 1 Miliar / 500 Juta = **2**.
    - **`res = 8 - 2 = 6`**.
 4. **Step 4 (Final Verdict)**: 
    - **`res > 5`**: Apakah 6 > 5? **YA (BENAR/1)**. Maka laci `final_cek` berisi 1.
    - **`ans = 1 + 11 = 12`** (Ingat, `x` sudah jadi 11 di Step 2).
 5. **Output**: **ans = 12**.
 </details>
 
 ---
 
 ⏩ **Lanjut ke Modul Kedua:** [Logika Percabangan (Razia BP)](../02-percabangan/materi.md)
