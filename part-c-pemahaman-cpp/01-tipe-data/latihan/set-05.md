# Latihan Soal Part C - Modul 01 - Set 05 (The God-Tier Challenge)
 
 ---
 
 🌌 **DIMENSI DEWA - LEVEL TERAKHIR:**
 Selamat datang di gerbang terakhir. Jika kamu bisa melampaui 10 soal ini dengan logika yang jernih, maka kamu sudah siap untuk berdiri di jajaran elit peserta OSN-K Informatika tingkat Nasional. Robot C++ tidak akan memberi ampun di sini.
 
 ---
 
 ### Soal 41: Spiral ASCII & Modulo Tak Terhingga
 ```cpp
 char c = 'z'; // ASCII 122
 char res = 'a' + (c - 'a' + 27) % 26;
 ```
 **Pertanyaan:**
 1. Karakter apakah yang tersimpan di dalam variabel `res`?
 2. Bagaimana logika rotasi pergeseran 27 langkah untuk abjad yang hanya berjumlah 26?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `c` = 122 ('z').
 - 'a' = 97.
 - `res` = 97 ('a').
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Hitung Jarak (`c - 'a'`)**: $122 - 97 = 25$. ('z' adalah huruf ke-25 setelah 'a').
 2. **Geser 27 Langkah**: $25 + 27 = 52$.
 3. **Rotasi Siklus (`% 26`)**: $52 \pmod{26}$. Hasilnya adalah **0**.
 4. Karena sisa baginya 0, robot kembali ke titik awal: `'a' + 0 = 'a'`.
 5. Pergeseran 27 langkah sama dengan 1 putaran penuh (26) + 1 langkah (1). Jadi seolah-olah berputar dari 'z' $\rightarrow$ 'a'.
 
 **Jawaban Akhir: 'a'**
 </details>
 
 ---
 
 ### Soal 42: Ranjau Short-Circuit (Delayed Side Effects)
 ```cpp
 int x = 5, y = 10;
 bool cek = (x > 10 && ++y > 0) || (x < 10 && ++y > 10);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `y`?
 2. Berapakah nilai `cek` (0 atau 1)?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`(x > 10 && ++y > 0)`)**: Syarat pertama `5 > 10` bernilai **Salah**. Robot segera berhenti mengecek (Short-circuit). Perintah `++y` di sini **TIDAK JALAN**. `y` masih 10. Hasil kurung pertama adalah **Salah**.
 2. **Bagian 2 (`(x < 10 && ++y > 10)`)**: Karena bagian 1 Salah, robot harus cek sisi kanan `||`. Syarat pertama `5 < 10` bernilai **Benar**. Robot lanjut ke syarat kedua.
 3. **Efek Samping**: Robot menjalankan `++y`, sehingga `y` naik dari 10 menjadi **11**. Lalu dicek: `11 > 10`? Jawabannya **Benar**.
 4. `Salah || Benar` = **Benar (1)**.
 
 **Jawaban Akhir: y = 11, cek = 1**
 </details>
 
 ---
 
 ### Soal 43: Casting Inception (Stacked Casts)
 ```cpp
 int a = 7;
 double b = 2.0;
 int res = (int)((double)(a / 2) + (a / b));
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `res`?
 2. Mengapa bagian pertama menghasilkan 3.0 sedangkan bagian kedua 3.5?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`a / 2`)**: `int / int`. Hasilnya **3**. Lalu di-cast ke `double` $\rightarrow$ **3.0**.
 2. **Bagian 2 (`a / b`)**: `7 / 2.0`. Ada `double`, hasilnya presisi **3.5**.
 3. **Jumlahkan**: `3.0 + 3.5 = 6.5`.
 4. **Casting Terakhir**: Hasil 6.5 dipaksa masuk ke `int`. Koma dibuang.
 
 **Jawaban Akhir: 6**
 </details>
 
 ---
 
 ### Soal 44: Rantai Overflow 1LL (Strategic Positioning)
 ```cpp
 int a = 1000000, b = 2000, c = 1000000;
 long long res_A = a * b * 1LL * c;
 long long res_B = a * c * b * 1LL;
 ```
 **Pertanyaan:**
 1. Apakah `res_A` dan `res_B` sama?
 2. Mengapa penempatan `1LL` di akhir (`res_B`) tetap berbahaya bagi skormu?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Kasus `res_A`**: Robot menghitung `a * b` (2 Miliar). Belum overflow. Lalu dikali `1LL`, robot naik kasta jadi besar. Dikali `c` (1 Juta), aman jadi **2 Triliun**.
 2. **Kasus `res_B`**: Robot menghitung `a * c` ($10^6 \times 10^6 = 10^{12}$). Tapi robot masih berhitung di kasta `int`. Hasilnya **MELEDAK (Overflow)** jadi angka sampah sebelum sempat menemu `1LL` di akhir.
 
 **Jawaban Akhir: Tidak Sama. res_B Hancur/Overflow.**
 **Pesan Juara:** Selalu letakkan `1LL` di **awal** perkalian atau di urutan yang memastikan hasil belum melebihi 2 Miliar.
 </details>
 
 ---
 
 ### Soal 45: Scientific Double-Edged Sword (Precision Loss)
 ```cpp
 double d = 1.0e11 / 1.0e9; // 100 Billion / 1 Billion
 char c = (char)d;
 int n = d;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `c` dan `n`?
 2. Mengapa angka **100** aman di `int` tapi bisa jadi karakter aneh di `char`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `d` = 100.0.
 - `n` = 100.
 - `c` = 'd' (ASCII 100).
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Hitung d**: $100.000 .000 .000 \div 1.000 .000 .000 = 100.0$.
 2. **Isi n**: Angka 100 masuk ke `int`. Aman.
 3. **Isi c**: Angka 100 dipaksa masuk ke `char`. Di tabel ASCII, angka 100 adalah huruf **'d'** kecil.
 
 **Jawaban Akhir: c = 'd', n = 100**
 </details>
 
 ---
 
 ### Soal 46: Rotasi Koordinat Negatif (Safety Modulo)
 ```cpp
 int pos = -10;
 int gerak = (pos % 3 + 3) % 3;
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `gerak` (0, 1, atau 2)?
 2. Apa kegunaan trik `((a % b) + b) % b` di atas?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Modulo Dalam (`-10 % 3`)**: $10 \pmod 3 = 1$. Karena kiri negatif, hasilnya **-1**.
 2. **Tambah b (`-1 + 3`)**: Hasilnya **2**.
 3. **Modulo Akhir (`2 % 3`)**: Hasilnya tetap **2**.
 
 **Jawaban Akhir: 2**
 **Kegunaan:** Memastikan hasil modulo angka negatif **selalu positif**. Sangat vital untuk soal koordinat atau memutar jarum jam berlawanan arah.
 </details>
 
 ---
 
 ### Soal 47: Logika Aritmatika (Double Bang)
 ```cpp
 int x = 5;
 int hasil = (!x) + (!!x) * 10 - (!0);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `hasil`?
 2. Apa arti dari `!x` dan `!!x` jika dipandang sebagai angka?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **`!x` (!5)**: Sesuatu yang berisi dianggap Benar. Lawan dari Benar adalah **Salah (0)**.
 2. **`!!x` (!!5)**: Lawan dari Salah adalah **Benar (1)**. (Sering disebut trik *Normalize to 1*).
 3. **`!0`**: Lawan dari Nol (Salah) adalah **Benar (1)**.
 4. Rumus: `0 + 1 * 10 - 1` = **9**.
 
 **Jawaban Akhir: 9**
 </details>
 
 ---
 
 ### Soal 48: Labirin Scope Shadowing (3 Layers)
 ```cpp
 int x = 1;
 int main() {
     int x = 10;
     {
         int x = 100;
         ::x = x + ::x;
     }
     printf("%d", ::x);
 }
 ```
 **Pertanyaan:**
 1. Berapakah angka yang muncul di layar?
 2. Mengapa `x = 10` di dalam `main` tidak ikut serta dalam hitungan?
 
 <details>
 <summary><b>Diagnosis Wilayah Kekuasaan</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `::x` merujuk ke Global (**1**).
 2. Di dalam blok paling dalam `{ }`, `x` merujuk ke variabel Lokal terdalam (**100**).
 3. Rumus: `Global = 100 + 1 = 101`.
 4. Variabel `x=10` diabaikan karena ada `x=100` yang lebih dekat dan `::x` yang menunjuk spesifik ke Global.
 
 **Jawaban Akhir: 101**
 </details>
 
 ---
 
 ### Soal 49: Masterclass Formatting Terkutuk
 ```cpp
 double val = 12.34567;
 printf("%0*.*f", 10, 3, -val);
 ```
 **Pertanyaan:**
 1. Apa yang akan tercetak di layar? (Hitung secara teliti termasuk tanda minus).
 2. Apa fungsi dari tanda bintang `*` dalam format `printf`?
 
 <details>
 <summary><b>Diagnosis Visual Output</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bintang pertama (`*`)**: Diambil dari parameter kodingan, yaitu **10** (Total panjang).
 2. **Bintang kedua (`*`)**: Diambil dari parameter kodingan, yaitu **3** (Angka desimal).
 3. **Angka**: `-12.34567` dibulatkan 3 angka $\rightarrow$ **-12.346**.
 4. **Tampilan**: `-12.346` terdiri dari **7 karakter** (termasuk minus dan titik).
 5. **Padding**: Total harus 10, kurang 3 karakter. Tambahkan angka **0** di depan (karena ada format `010`).
 
 **Jawaban Akhir: -00012.346**
 </details>
 
 ---
 
 ### Soal 50: THE FINAL BOSS - THE HUMAN COMPILER DIVINE
 ```cpp
 char c = 'E'; // 69
 int k = 2;
 double p = 0.9;
 
 int res = (int)((c - 'A') / 3.0) * (int)(k + p) + (1e12 > 1LL * 1000000 * 1000000);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari `res`?
 2. Sebutkan urutan hierarki robot dalam memproses tantangan terakhir ini!
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`(c - 'A') / 3.0`)**: $(69 - 65) = 4$. Lalu $4 \div 3.0 = 1.333...$. Di-cast ke `int` jadi **1**.
 2. **Bagian 2 (`(int)(k + p)`)**: $(int)(2 + 0.9) = (int)(2.9) = \mathbf{2}$.
 3. **Bagian 3 (Logic Overflow)**: `1e12` (1 Triliun) dibandingkan dengan `1LL * 1Miliar * 1Miliar` ($10^{12}$ atau 1 Triliun). Apakah 1 Triliun **lebih besar dari** 1 Triliun? **SALAH (0)**.
 4. **Gabungkan**: $(1 \times 2) + 0 = \mathbf{2}$.
 
 **Jawaban Akhir: 2**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🏁 **Sempurna! Kamu telah menamatkan Tantangan Modul 01! Persiapkan diri untuk Modul 02: Percabangan!**
