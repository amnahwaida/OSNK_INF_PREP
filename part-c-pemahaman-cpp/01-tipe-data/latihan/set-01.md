# Latihan Soal Part C - Modul 01 - Set 01 (Premium Survival Edition)
 
 ---
 
 ⚠️ **PERINGATAN KOMPILATOR MANUSIA:**
 Soal-soal di bawah ini dirancang untuk menjebakmu dengan detail terkecil. Jangan percaya pada insting matematikamu di sekolah; percayalah pada **Aturan Main Robot C++**.
 
 ---
 
 ### Soal 1: Hierarki KABATAKU & Penugasan Berantai
 ```cpp
 int a = 10, b = 3, c = 2;
 int x = a + b * c / 2 - b % c;
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `x`?
 2. Bagaimana urutan langkah robot saat menghitung rumus di atas?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `a` = 10, `b` = 3, `c` = 2.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot melihat kasta operator. Perkalian (`*`), Pembagian (`/`), dan Modulo (`%`) adalah selevel (Kasta Menengah), jadi dikerjakan dari **Kiri ke Kanan**.
 2. Langkah 1 (`b * c`): $3 \times 2 = 6$.
 3. Langkah 2 (`6 / 2`): $6 \div 2 = 3$.
 4. Langkah 3 (`b % c`): $3 \pmod 2$. Sisa baginya adalah **1**.
 5. Rumus berubah menjadi: `x = 10 + 3 - 1`.
 6. Operasi tambah-kurang (Kasta Rakyat) dikerjakan dari kiri: `13 - 1 = 12`.
 
 **Jawaban Akhir: 12**
 </details>
 
 ---
 
 ### Soal 2: Caesar Cipher & Perputaran Modulo
 ```cpp
 char huruf = 'Y'; // ASCII 89
 char hasil = 'A' + (huruf - 'A' + 3) % 26;
 ```
 **Pertanyaan:**
 1. Huruf apakah yang tersimpan di dalam variabel `hasil`?
 2. Apa fungsi dari `% 26` dalam rumus di atas?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `huruf` = 89 ('Y').
 - 'A' = 65.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Hitung Jarak Abjad**: `huruf - 'A'` $\rightarrow 89 - 65 = 24$. (Artinya 'Y' adalah huruf ke-24 setelah 'A').
 2. **Geser 3 Langkah**: $24 + 3 = 27$.
 3. **Perputaran (Modulo 26)**: $27 \pmod{26}$. Sisanya adalah **1**.
 4. **Balikkan ke Karakter**: `'A' + 1` $\rightarrow 65 + 1 = 66$.
 5. Di tabel ASCII, angka 66 adalah huruf **'B'**.
 
 **Jawaban Akhir: 'B'**
 **Penjelasan:** `% 26` berfungsi menciptakan **Siklus Putar**. Jika pergeseran melebihi 'Z', robot akan otomatis kembali ke 'A'.
 </details>
 
 ---
 
 ### Soal 3: Jebakan Maut $10^{12}$ (Overflow)
 ```cpp
 int a = 1000000; // Satu Juta
 int b = 1000000; // Satu Juta
 long long x = a * b;
 long long y = 1LL * a * b;
 ```
 **Pertanyaan:**
 1. Apakah isi variabel `x` dan `y` sama? Jika tidak, apa isinya?
 2. Mengapa keberadaan `1LL` sangat menentukan nasib skormu?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = Angka Sampah (Overflow).
 - `y` = 1,000,000,000,000 (Satu Triliun).
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Analisis `x`**: Robot melihat `a * b`. Karena keduanya tipe `int`, robot menghitung hasilnya di area memori `int` (Kapasitas cuma 2 Miliar). Hasil 1 Triliun meledak (Overflow) menjadi angka acak sebelum sempat dimasukkan ke `long long x`.
 2. **Analisis `y`**: Robot melihat `1LL`. Ini adalah pesulap kasta `long long`. Karena ada dia di paling kiri, robot dipaksa berhitung di skala raksasa sejak awal. Hasil 1 Triliun aman tersimpan di `long long y`.
 
 **Jawaban Akhir: Tidak Sama.**
 **Pesan Juara:** Di OSN-K, jika mengalikan angka yang hasilnya bisa > 2 Miliar, **Wajib** pakai `1LL` di depan!
 </details>
 
 ---
 
 ### Soal 4: Presisi Robot (Manual Casting)
 ```cpp
 int tabungan = 10;
 int dibagi = 4;
 double jatah1 = tabungan / dibagi;
 double jatah2 = (double)tabungan / dibagi;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `jatah1` dan `jatah2`?
 2. Mengapa `jatah1` tidak menghasilkan angka 2.5 meskipun ditampung di `double`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `jatah1` = 2.0.
 - `jatah2` = 2.5.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Kasus `jatah1`**: Robot menghitung `tabungan / dibagi` (10 / 4) di area `int`. Hasilnya adalah **2** (Koma 0.5 hangus dibakar). Baru setelah angkanya jadi 2, robot menaruhnya ke `double`, sehingga jadi `2.0`.
 2. **Kasus `jatah2`**: Robot melihat `(double)tabungan`. Robot mengubah pandangannya terhadap angka 10 menjadi **10.0**. Sekarang rumusnya adalah $10.0 \div 4$. Karena ada Bangsawan (`double`), hasilnya sukses jadi **2.5**.
 
 **Jawaban Akhir: 2.0 dan 2.5.**
 </details>
 
 ---
 
 ### Soal 5: Logika 0 & 1 (Boolean Math)
 ```cpp
 int a = 5, b = 10;
 int hasil = (a > b) + (b > a) * 5 + (a == 5);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `hasil`?
 2. Bagaimana robot mengubah Benar/Salah menjadi angka?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `a > b` (5 > 10) $\rightarrow$ Salah, robot menganggapnya angka **0**.
 2. `b > a` (10 > 5) $\rightarrow$ Benar, robot menganggapnya angka **1**.
 3. `a == 5` (5 == 5) $\rightarrow$ Benar, robot menganggapnya angka **1**.
 4. Rumus berubah menjadi: `0 + 1 * 5 + 1`.
 5. Robot menghitung perkalian duluan: `0 + 5 + 1`.
 6. Hasil akhir: **6**.
 
 **Jawaban Akhir: 6**
 </details>
 
 ---
 
 ### Soal 6: Paradoks Pre vs Post Increment
 ```cpp
 int x = 10;
 int y = x++;
 int z = ++x;
 int total = x + y + z;
 ```
 **Pertanyaan:**
 1. Berapakah isi masing-masing laci `x`, `y`, dan `z` di baris terakhir?
 2. Berapakah nilai `total`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Awalnya `x = 10`.
 2. **Baris 2 (`x++`)**: Laci `y` mengambil nilai `x` yang sekarang (**10**). Baru setelah itu `x` naik jadi 11.
 3. **Baris 3 (`++x`)**: `x` naik dulu dari 11 menjadi **12**. Baru setelah itu laci `z` mengambil nilai 12.
 4. Kondisi Akhir: `x` = 12, `y` = 10, `z` = 12.
 5. `total = 12 + 10 + 12 = 34`.
 
 **Jawaban Akhir: 34**
 </details>
 
 ---
 
 ### Soal 7: Modulo Sakral & Angka Eksponen
 ```cpp
 long long mod = 1e9 + 7;
 long long h = (2e9 + 5) % mod;
 ```
 **Pertanyaan:**
 1. Berapakah nilai dari `h`?
 2. Bagaimana cara menghitung modulo angka 2 Miliar terhadap 1 Miliar?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `mod` = $1.000 .000 .007$.
 2. `2e9 + 5` = $2.000 .000 .005$.
 3. Kita bagi: $2.000 .000 .005 \div 1.000 .000 .007$.
 4. Dapat **1**, dengan sisa: $2.000 .000 .005 - 1.000 .000 .007 = 999.999.998$.
 
 **Jawaban Akhir: 999.999.998**
 </details>
 
 ---
 
 ### Soal 8: Masterclass Printf & Formatting
 ```cpp
 double pi = 3.14159;
 int angka = 10;
 printf("%.2f %03d", pi, angka);
 ```
 **Pertanyaan:**
 1. Apa yang akan tercetak di layar monitormu?
 2. Apa arti dari kode `%03d`?
 
 <details>
 <summary><b>Diagnosis Visual Output</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `%.2f` $\rightarrow$ Cetak `pi` dengan 2 angka di belakang koma. Hasil: **3.14**.
 2. `%03d` $\rightarrow$ Cetak integer minimal 3 digit. Jika kurang dari 3 digit, tambahkan angka **0** di depannya (Padding). Hasil: **010**.
 3. Antara keduanya ada spasi `" "`.
 
 **Jawaban Akhir: 3.14 010**
 </details>
 
 ---
 
 ### Soal 9: Bayangan Variabel (Global Scope)
 ```cpp
 int skor = 100; // GLOBAL
 
 int main() {
     int skor = 50; // LOKAL
     {
         int skor = 10; // LOKAL DALAM
         printf("%d ", skor);
     }
     printf("%d", skor);
 }
 ```
 **Pertanyaan:**
 1. Apa yang akan tercetak di layar? (Ada dua angka).
 2. Mengapa angka `100` di baris paling atas tidak muncul?
 
 <details>
 <summary><b>Diagnosis Wilayah Kekuasaan</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot selalu memprioritaskan "Orang Dalam" yang paling dekat.
 2. Di dalam kurung kurawal `{ }` terdalam, ada `skor = 10`. Maka tercetak **10**.
 3. Setelah kurung itu tutup, `skor = 10` hancur. Robot kembali melihat wilayah `main`, di sana ada `skor = 50`. Maka tercetak **50**.
 4. Variabel Global `100` tertutup bayang-bayang variabel lokal (*Shadowing*).
 
 **Jawaban Akhir: 10 50**
 </details>
 
 ---
 
 ### Soal 10: THE FINAL BOSS - Human Compiler Simulation
 ```cpp
 char c = 'B'; // ASCII 66
 int x = 5;
 double d = 2.0;
 
 int res = (c - 'A' + 1) * (int)(x / d) + (++x % 2);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari `res`?
 2. Berapakah nilai akhir `x` sekarang?
 
 <details>
 <summary><b>Diagnosis Logika Sang Juara</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1**: `(c - 'A' + 1)` $\rightarrow (66 - 65 + 1) = 2$.
 2. **Bagian 2**: `(x / d)` $\rightarrow 5 \div 2.0 = 2.5$. Lalu di-cast ke `int` $\rightarrow$ **2**.
 3. **Bagian 3**: `(++x % 2)`. `x` naik dulu dari 5 menjadi **6**. Baru di-modulo: `6 % 2 = 0`.
 4. Gabungkan: `2 * 2 + 0` = **4**.
 
 **Jawaban Akhir:**
 1. **res = 4**
 2. **x = 6**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 ⏩ **Lanjut ke Latihan Percabangan: [Set 02](../../02-percabangan/latihan/README.md)**
