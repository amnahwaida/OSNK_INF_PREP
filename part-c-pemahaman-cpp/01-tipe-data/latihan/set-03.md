# Latihan Soal Part C - Modul 01 - Set 03 (Expert Masterclass)
 
 ---
 
 ⚠️ **PANGGILAN UNTUK PARA JUARA:**
 Ini adalah rintangan terakhir di Modul 01. Jika kamu bisa menyelesaikan 10 soal ini tanpa melihat jawaban, artinya kamu sudah memiliki mentalitas seorang Kompilator Manusia tingkat Dewa.
 
 ---
 
 ### Soal 21: Rantai Casting Terlarang
 ```cpp
 int x = 10, y = 4;
 double res = (int)((double)x / y) + 0.75;
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `res`?
 2. Apa yang terjadi saat `2.5` diubah paksa menjadi `(int)`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 10, `y` = 4.
 - `res` = 2.75.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian Dalam (`(double)x / y`)**: Robot mengubah `x` jadi 10.0, lalu dibagi 4. Hasilnya **2.5**.
 2. **Casting Tengah (`(int)(2.5)`)**: Hasil 2.5 dipaksa menjadi integer. Koma dibuang tanpa ampun. Hasilnya menjadi **2**.
 3. **Operasi Luar**: `2 + 0.75` = **2.75**.
 4. **Penyimpanan**: Variabel `res` adalah `double`, jadi ia bisa menampung 2.75 dengan sempurna.
 
 **Jawaban Akhir: 2.75**
 </details>
 
 ---
 
 ### Soal 22: ASCII & Logika Abjad
 ```cpp
 char huruf = 'A'; 
 bool cek = (huruf + 32 == 'a') && (huruf + 1 > 'B');
 ```
 **Pertanyaan:**
 1. Berapakah nilai dari `cek` (0 atau 1)?
 2. Mengapa syarat kedua bernilai Salah?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Syarat 1 (`'A' + 32 == 'a'`)**: Nilai 'A' adalah 65. $65 + 32 = 97$. Angka 97 di tabel ASCII adalah benar huruf **'a'**. Syarat ini **BENAR (1)**.
 2. **Syarat 2 (`'A' + 1 > 'B'`)**: Nilai 'A' + 1 adalah **66**. Kode ASCII huruf 'B' juga **66**. Apakah 66 > 66? **TIDAK (0)**. Syarat ini **SALAH (0)**.
 3. **Logika `&&` (DAN)**: `Benar && Salah` hasilnya adalah **Salah (0)**.
 
 **Jawaban Akhir: 0 (False)**
 </details>
 
 ---
 
 ### Soal 23: Sang Penjaga 1e9+7 (Overflow Pro)
 ```cpp
 int a = 2000000000; // 2 Miliar
 int b = 2000000000; // 2 Miliar
 int mod = 1e9 + 7;
 int ans = (1LL * a + b) % mod;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `ans`?
 2. Mengapa kita tidak bisa menulis `(a + b) % mod` saja?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Ekskusi Bruto**: Robot menghitung `1LL * a + b`. Berkat `1LL`, robot berhitung di skala raksasa. $2 \text{ Miliar} + 2 \text{ Miliar} = 4 \text{ Miliar}$.
 2. **Modulo**: $4.000 .000 .000 \pmod{1.000 .000 .007}$.
 3. Kita bagi: $4.000 .000 .000 \div 1.000 .000 .007 \approx 3,99...$. Robot mengambil angka bulat **3**.
 4. Sisanya: $4.000 .000 .000 - (3 \times 1.000 .000 .007) = 4.000 .000 .000 - 3.000 .000 .021 = 999.999.979$.
 
 **Jawaban Akhir: 999.999.979**
 **Pesan Juara:** Jika pakai `(a+b)`, hasilnya meledak (overflow) dulu jadi angka negatif sebelum sempat dimodulo. Selalu sertakan `1LL`!
 </details>
 
 ---
 
 ### Soal 24: Short-Circuit Pintu Ganda
 ```cpp
 int g = 5;
 bool x = (g > 10) && (++g > 0);
 bool y = (g < 10) || (++g > 0);
 ```
 **Pertanyaan:**
 1. Berapakah isi variabel `g` di akhir kodingan?
 2. Syarat mana saja yang "dilewati" oleh robot?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Operasi x**: Syarat pertama `(g > 10)` adalah **SALAH**. Karena operatornya `&&` (DAN), jika satu saja sudah salah, robot tidak perlu mengecek sisanya. `++g` dilewati. (`g` tetap 5).
 2. **Operasi y**: Syarat pertama `(g < 10)` adalah **BENAR**. Karena operatornya `||` (ATAU), jika satu saja sudah benar, robot tidak perlu mengecek sisanya. `++g` dilewati lagi! (`g` tetap 5).
 
 **Jawaban Akhir: g = 5**
 </details>
 
 ---
 
 ### Soal 25: Master Padding & Presisi
 ```cpp
 double val = 12.3456;
 printf("%07.2f", val);
 ```
 **Pertanyaan:**
 1. Apa yang akan muncul di layar monitor? (Hitung jumlah karakter secara teliti).
 2. Apa arti dari angka `07` di depan titik pada `%07.2f`?
 
 <details>
 <summary><b>Diagnosis Tampilan</b></summary>
 
 **📖 Diagnosis Visual:**
 1. **`.2f`**: Bulatkan angka ke 2 desimal. `12.3456` jadi `12.35`.
 2. **`7`**: Pastikan panjang TOTAL tampilan adalah **7 karakter** (termasuk titik).
 3. **`0`**: Jika panjangnya kurang dari 7, tambahkan angka **0** di depan (bukan spasi).
 4. `12.35` terdiri dari 5 karakter. Masih kurang 2 karakter.
 5. Tambahkan dua nol di depan: **0012.35**.
 
 **Jawaban Akhir: 0012.35**
 </details>
 
 ---
 
 ### Soal 26: Pertempuran Pre-Post Akhir
 ```cpp
 int a = 5;
 int b = ++a; // a=6, b=6
 a = b++;     // a=6, b=7
 b = ++a;     // a=7, b=7
 printf("%d %d", a, b);
 ```
 **Pertanyaan:**
 1. Angka apa saja yang tercetak di layar?
 2. Mengapa status `a` dan `b` selalu berkejaran?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Mula-mula**: `a = 5`.
 2. **Langkah 1 (`b = ++a`)**: `a` naik jadi **6**, lalu `b` mengambil nilai 6.
 3. **Langkah 2 (`a = b++`)**: `a` mengambil nilai `b` yang sekarang (**6**). Baru setelah itu `b` naik jadi 7.
 4. **Langkah 3 (`b = ++a`)**: `a` naik dulu dari 6 jadi **7**. Lalu `b` mengambil nilai 7.
 5. Cetak: **7 7**.
 
 **Jawaban Akhir: 7 7**
 </details>
 
 ---
 
 ### Soal 27: Siklus Modulo Negatif
 ```cpp
 int p = -5;
 int res = (p % 3) + 3;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Trik di atas biasanya dipakai juri untuk menangani apa?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Hitung Modulo**: `-5 % 3`. Kerjakan `5 % 3 = 2`. Karena angka kirinya negatif, hasilnya **-2**.
 2. **Hitung res**: `-2 + 3` = **1**.
 
 **Jawaban Akhir: 1**
 **Kegunaan:** Trik `(a % b + b) % b` sering dipakai untuk memastikan hasil modulo **selalu positif** walaupun inputnya negatif (sangat penting untuk soal perputaran arah/koordinat).
 </details>
 
 ---
 
 ### Soal 28: Bayangan Global & Ruang
 ```cpp
 int x = 10;
 int main() {
     int x = x + 5;
     {
         int x = 2;
         x = x * 10;
     }
     printf("%d", x);
 }
 ```
 **Pertanyaan:**
 1. Apa hasil cetakan perintah di atas?
 2. Mengapa variabel di dalam `{ }` tidak memengaruhi hasil akhir?
 
 <details>
 <summary><b>Diagnosis Wilayah Kekuasaan</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Baris 3**: `int x = x + 5`. `x` di sisi kanan mengambil dari variabel GLOBAL (10). Jadi `x` lokal di `main` berisi **15**.
 2. **Blok Dalam (`{ }`)**: Dibuat variabel `x` baru lagi (berisi 2). Lalu dikali 10 jadi **20**.
 3. **Selesai Blok**: Begitu keluar `{ }`, variabel `x=20` dihancurkan. Robot kembali hanya melihat `x` milik `main`.
 4. Cetak: **15**.
 
 **Jawaban Akhir: 15**
 </details>
 
 ---
 
 ### Soal 29: Jebakan Double & Integer Gabungan
 ```cpp
 int a = 5;
 double b = 2.0;
 int res = (a / b) + (a / (int)b);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Mengapa sisi kanan menghasilkan angka 2, sedangkan sisi kiri menyumbang nilai lebih banyak?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Sisi Kiri (`a / b`)**: `5 / 2.0`. Ada `double`, hasilnya presisi **2.5**.
 2. **Sisi Kanan (`a / (int)b`)**: `5 / 2`. Keduanya `int`, hasilnya dipangkas jadi **2**.
 3. **Total**: `2.5 + 2 = 4.5`.
 4. **Penyimpanan**: `res` adalah `int`. Hasil 4.5 dipaksa masuk, koma dibuang. Hasil akhir **4**.
 
 **Jawaban Akhir: 4**
 </details>
 
 ---
 
 ### Soal 30: THE GRAND FINALE - The Compiler's Nightmare
 ```cpp
 char k = 'C'; 
 int n = 2;
 double p = 1.6;
 
 int out = (k - 'A') * (int)(n + p) + (1LL * 2000000000 * 2 / 1000000000) % 3;
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `out`?
 2. Sebutkan setidaknya 4 konsep C++ yang digunakan dalam soal ini!
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (ASCII)**: `'C' - 'A'` = $67 - 65 = 2$.
 2. **Bagian 2 (Cast)**: `(int)(2 + 1.6)` $\rightarrow (int)(3.6) = 3$.
 3. **Bagian 3 (Overflow Fix)**: `1LL * 2Miliar * 2` = 4 Miliar. Lalu dibagi 1 Miliar = **4**.
 4. **Bagian 4 (Modulo)**: $4 \pmod 3 = 1$.
 5. **Gabungkan**: $(2 \times 3) + 1 = 6 + 1 = 7$.
 
 **Jawaban Akhir: 7**
 **Konsep Terpakai:** ASCII Math, Explicit Casting, 1LL Overflow Protection, Modulo.
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🏁 **Selamat! Kamu telah menyelesaikan seluruh rangkaian latihan Modul 01!**
