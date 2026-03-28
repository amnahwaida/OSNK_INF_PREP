# Latihan Soal Part C - Modul 01 - Set 04 (Hall of Fame Edition)
 
 ---
 
 🏆 **MODUL FINAL - LEVEL ELITE:**
 Kamu telah membedah lebih dari 30 soal. Set 04 ini adalah gerbang terakhir menuju status "Master" Tipe Data & Operator. Soal-soal di sini menggabungkan hampir seluruh materi sekaligus dalam satu butir pertanyaan.
 
 ---
 
 ### Soal 31: Kasta & Overflow Gabungan
 ```cpp
 int a = 1000000;
 int b = 500000;
 long long res1 = a * b * 2;
 long long res2 = 1LL * a * b * 2;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res1` dan `res2`?
 2. Mengapa perkalian dua angka `int` yang melampaui 2 Miliar selalu berbahaya walaupun ditampung di `long long`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `a` = 1 Juta, `b` = 500 Ribu.
 - `res1` = Angka Sampah (Overflow).
 - `res2` = 1,000,000,000,000 (1 Triliun).
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Kasus `res1`**: Robot menghitung `a * b` dulu. Keduanya `int`. Hasilnya 500 Miliar. Karena batas `int` cuma 2 Miliar, meledaklah ia (Overflow). Sisa angka hancur tadi dikali 2, makin berantakan.
 2. **Kasus `res2`**: Ditemukan mantra `1LL`. Robot segera berubah kasta jadi raksasa (`long long`). Hasil perkalian 1 Triliun aman terjaga.
 
 **Jawaban Akhir: res1 = Sampah, res2 = 1 Triliun.**
 </details>
 
 ---
 
 ### Soal 32: ASCII & Logika Short-Circuit
 ```cpp
 char c = 'A'; // 65
 int x = 10;
 bool cek = (c + 32 == 'a') || (++x > 10);
 ```
 **Pertanyaan:**
 1. Berapakah isi laci `x` sekarang?
 2. Apakah syarat kedua (`++x > 10`) dijalankan oleh robot?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot cek syarat 1: `'A' + 32` $\rightarrow 65 + 32 = 97$. Angka 97 di tabel ASCII adalah benar huruf **'a'**. Hasilnya **BENAR**.
 2. Karena operatornya `||` (Atau) dan syarat pertama sudah Benar, robot berhenti memeriksa (Short-circuit).
 3. Bagian `++x` **tidak pernah disentuh**. `x` tetap di angka 10.
 
 **Jawaban Akhir: x = 10**
 </details>
 
 ---
 
 ### Soal 33: Radar Modulo & Pre-Post (Advanced Tracking)
 ```cpp
 int x = 10, y = 3;
 int a = x++ % y; 
 int b = ++x % y;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `a` dan `b`?
 2. Berapakah nilai `x` di baris terakhir?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Langkah 1 (`a = x++ % y`)**: Robot memakai nilai `x` yang sekarang (**10**) untuk di-modulo 3. $10 \pmod 3 = \mathbf{1}$. Setelah ini selesai, `x` naik jadi 11.
 2. **Langkah 2 (`b = ++x % y`)**: Robot menaikkan `x` dulu dari 11 menjadi **12**. Baru di-modulo 3. $12 \pmod 3 = \mathbf{0}$.
 3. Nilai akhir `x` adalah 12.
 
 **Jawaban Akhir: a = 1, b = 0, x = 12.**
 </details>
 
 ---
 
 ### Soal 34: Pertempuran Presisi (Mixed Types)
 ```cpp
 int a = 5, b = 2;
 double res = (a / b) + (a / (double)b);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `res`?
 2. Mengapa pembagian pertama menghasilkan 2, sedangkan pembagian kedua 2.5?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`a / b`)**: `int / int`. Koma hangus. Hasilnya **2**.
 2. **Bagian 2 (`a / (double)b`)**: `int / double`. Kasta naik. Hasilnya **2.5**.
 3. Tambahkan: `2 + 2.5 = 4.5`.
 
 **Jawaban Akhir: 4.5**
 </details>
 
 ---
 
 ### Soal 35: Paradoks Tukar Tanpa Gelas (Swap Overflow Risk)
 ```cpp
 int a = 2000000000;
 int b = 1000000000;
 a = a + b; // a = ?
 b = a - b;
 a = a - b;
 ```
 **Pertanyaan:**
 1. Apakah nilai `a` dan `b` akan berhasil tertukar?
 2. Apa risiko menggunakan teknik ini di OSN-K jika angkanya sangat besar?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mencoba `a + b` ($2 \text{ Miliar} + 1 \text{ Miliar} = 3 \text{ Miliar}$).
 2. Karena batas `int` cuma 2 Miliar, terjadi **Overflow**. Angka meledak dan jadi negatif/acak. Tahap selanjutnya tidak akan berhasil menukar angka dengan benar.
 
 **Jawaban Akhir: Gagal Menukar (Kena Overflow).**
 **Pesan Juara:** Trik ini keren, tapi **berbahaya** untuk angka besar. Pakai variabel `temp` lebih aman!
 </details>
 
 ---
 
 ### Soal 36: Global vs Local Shadowing (Expert Level)
 ```cpp
 int poin = 100;
 int main() {
     int poin = 50;
     {
         int poin = 10;
         ::poin = ::poin + poin;
     }
     printf("%d", ::poin);
 }
 ```
 **Pertanyaan:**
 1. Apa hasil cetakan perintah tersebut?
 2. Apa kegunaan simbol `::` (Scope Resolution Operator)?
 
 <details>
 <summary><b>Diagnosis Wilayah Kekuasaan</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `::poin` merujuk pada variabel **GLOBAL** (100).
 2. `poin` tanpa titik dua merujuk pada variabel terdekat, yaitu **LOKAL DALAM** (10).
 3. Rumus: `Global (100) = Global (100) + Lokal (10)`.
 4. Maka Global berubah jadi **110**.
 5. Cetak `::poin` $\rightarrow$ **110**.
 
 **Jawaban Akhir: 110**
 </details>
 
 ---
 
 ### Soal 37: Scientific Notation & Char Casting
 ```cpp
 int n = 1.5e2; 
 char c = n - 35;
 printf("%c", c);
 ```
 **Pertanyaan:**
 1. Huruf apakah yang tersimpan di dalam `c`?
 2. Berapakah nilai numerik dari `n`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `1.5e2` $\rightarrow 1.5 \times 10^2 = 150$. Jadi `n = 150`.
 2. `150 - 35 = 115`.
 3. Angka 115 di tabel ASCII adalah huruf **'s'** kecil.
 
 **Jawaban Akhir: 's'**
 </details>
 
 ---
 
 ### Soal 38: Sizeof Calculation (Memory Trap)
 ```cpp
 int x = 10;
 int res = sizeof(x) * sizeof(char) + sizeof(long long);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Sebutkan ukuran byte untuk `int`, `char`, dan `long long`!
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `sizeof(int)` = 4.
 2. `sizeof(char)` = 1.
 3. `sizeof(long long)` = 8.
 4. Rumus: $4 \times 1 + 8 = 4 + 8 = 12$.
 
 **Jawaban Akhir: 12**
 </details>
 
 ---
 
 ### Soal 39: Negative Modulo & Boolean Logic
 ```cpp
 int a = -10, b = 3;
 bool cek = (a % b == -1) && (b % -3 == 0);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `cek` (0 atau 1)?
 2. Mengapa `b % -3` hasilnya bisa 0?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`-10 % 3 == -1`)**: `10 % 3 = 1`. Tanda ikut kiri (-), jadi -1. `-1 == -1` adalah **BENAR (1)**.
 2. **Bagian 2 (`3 % -3 == 0`)**: 3 dibagi -3 habis (sisa 0). Jadi `0 == 0` adalah **BENAR (1)**.
 3. `Benar && Benar` = **Benar (1)**.
 
 **Jawaban Akhir: 1 (True)**
 </details>
 
 ---
 
 ### Soal 40: THE HALL OF FAME BOSS (Integrated)
 ```cpp
 char c = 'D'; // 68
 int x = 3;
 double d = 1.7;
 
 int out = (c - 'A') * (int)(x + d) + (1LL * 1000000000 * 3 / 1000000000) % 2;
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari `out`?
 2. Berapakah nilai `(int)(x+d)`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (ASCII)**: `'D' - 'A'` $\rightarrow 68 - 65 = 3$.
 2. **Bagian 2 (Cast)**: `(int)(3 + 1.7)` $\rightarrow (int)(4.7) = 4$.
 3. **Bagian 3 (Overflow)**: $3 \text{ Miliar} \div 1 \text{ Miliar} = 3$.
 4. **Bagian 4 (Modulo)**: $3 \pmod 2 = 1$.
 5. **Total**: $(3 \times 4) + 1 = 12 + 1 = 13$.
 
 **Jawaban Akhir: 13**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🏁 **HEBAT! Kamu telah menyelesaikan 4 Set Latihan Maut Modul 01!**
