# Latihan Soal Part C - Modul 02 - Set 05 (God-Tier Challenge: Percabangan + Tipe Data)
 
 ---
 
 🌌 **LEVEL DEWA - KEPUTUSAN AKHIR:**
 Selamat! Kamu telah sampai di puncak tertinggi. Di set ini, robot (compiler) akan mencoba menipumu dengan tumpukan logika yang saling bertabrakan. Kamu harus tetap tenang, memegang teguh prinsip **Hierarki Operator**, **Short-circuit**, dan **Overflow Control**. Inilah ujian untuk menjadi "Human Compiler" sejati.
 
 ---
 
 ### Soal 41: Normalisasi Biner (The !! Logic Switch)
 ```cpp
 int x = 5, y = 0;
 int hasil = 0;
 switch (!!x + !!y) {
     case 1: hasil = 10;
     case 2: hasil = 20; break;
     default: hasil = 30;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `hasil`?
 2. Bagaimana robot mengevaluasi rumus `!!x + !!y` di dalam switch?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 5 $\rightarrow$ `!!5` = **1** (True).
 - `y` = 0 $\rightarrow$ `!!0` = **0** (False).
 - `Switch Value` = $1 + 0 = \mathbf{1}$.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: Robot menghitung `!!x` (Double Negation). `5` (Benar) jadi `!5` (Salah/0) jadi `!!5` (**1**).
 2. Robot menghitung `!!y`. `0` (Salah) jadi `!0` (Benar/1) jadi `!!0` (**0**).
 3. Hasil Switch: $1 + 0 = \mathbf{1}$. Robot lompat ke `case 1`.
 4. **Eksekusi case 1**: `hasil = 10`.
 5. **Waterfall (No Break)**: Robot terjun bebas ke `case 2`.
 6. **Eksekusi case 2**: `hasil = 20`.
 7. **Selesai**: Ketemu `break;`, robot berhenti.
 
 **Jawaban Akhir: 20**
 </details>
 
 ---
 
 ### Soal 42: Matriks Short-Circuit (The Double Minefield)
 ```cpp
 int a = 0, b = 5, c = 10, d = 0;
 bool res = (a++ || b--) && (c++ || d--);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `a`, `b`, `c`, dan `d`?
 2. Jelaskan mengapa `d` tetap bernilai 0!
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 S --> L1{"a++ || b--"}
 L1 -- a=0(F) --> L2{"b-- (T)"}
 L1 -- Result T --> R2{"c++ || d--"}
 R2 -- c=10(T) --> End["res = true"]
 R2 -- Short-circuit OR --> Skip["d-- Dilewati!"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Kurung Kiri (`a++ || b--`)**:
    - Robot cek `a++`. Nilai 0 dibandingkan $\rightarrow$ **SALAH**. `a` naik jadi **1**.
    - Karena Salah, robot cek sisi kanan `||`. Robot ambil `b` (5) untuk dibandingan $\rightarrow$ **BENAR**. Setelah itu `b` turun jadi **4**.
    - Kurung kiri bernilai **BENAR**.
 2. **Kurung Kanan (`c++ || d--`)**:
    - Karena kurung kiri Benar (operator `&&`), robot WAJIB cek kurung kanan.
    - Robot cek `c++`. Nilai 10 dibandingkan $\rightarrow$ **BENAR**. `c` naik jadi **11**.
    - **Short-circuit OR**: Karena sisi kiri `||` sudah Benar, robot **mengabaikan** sisi kanan `||`. Perintah `d--` **tidak pernah dieksekusi**.
 
 **Jawaban Akhir: a=1, b=4, c=11, d=0**
 </details>
 
 ---
 
 ### Soal 43: Jebakan Rentang Palsu (Chained Comparison)
 ```cpp
 int x = 50;
 int hasil = 0;
 if (10 < x < 20) {
     hasil = 1;
 } else {
     hasil = 2;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `hasil`? (Hati-hati, ini jebakan maut C++!)
 2. Bagaimana robot mengevaluasi `10 < x < 20`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi If**: `10 < x < 20` tidak dibaca sekaligus oleh robot. Robot membacanya dari kiri ke kanan.
 2. **Tahap 1**: `(10 < 50)` $\rightarrow$ **BENAR (1)**.
 3. **Tahap 2**: Sekarang robot mengevaluasi `(Hasil_Tahap1 < 20)` $\rightarrow$ `(1 < 20)`.
 4. Apakah 1 < 20? **BENAR (1)**.
 5. Robot masuk ke blok `if` $\rightarrow$ `hasil = 1`.
 6. *Catatan: Walaupun 50 aslinya tidak diantara 10 dan 20, kode ini tetap bernilai True!*
 
 **Jawaban Akhir: 1**
 </details>
 
 ---
 
 ### Soal 44: Shadow Redirect Switch (Global Assignment)
 ```cpp
 int p = 100;
 int main() {
     int p = 5;
     int out = 0;
     switch (::p = p + 1) {
         case 6: out = 1; break;
         case 101: out = 2; break;
     }
     printf("%d", out);
 }
 ```
 **Pertanyaan:**
 1. Angka apa yang tercetak?
 2. Variabel `p` mana yang digunakan di sisi kanan penugasan `p + 1`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: Robot melihat perintah `::p = p + 1`.
    - `p` (Lokal `main`) adalah **5**.
    - `::p` (Global) adalah **100**.
    - `Global = 5 + 1 = 6`.
 2. Hasil evaluasi switch tersebut adalah nilai baru yang dimasukkan, yaitu **6**.
 3. Robot mencari `case 6`. Ketemu!
 4. `out = 1`.
 
 **Jawaban Akhir: 1**
 </details>
 
 ---
 
 ### Soal 45: Overflow Ternary Inception (1LL Power)
 ```cpp
 int a = 1000000, b = 2000;
 int x = (1LL * a * b > 1500000000) ? (a / 10) : (b * 2);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `x`?
 2. Bagaimana hasil perbandingan berubah jika `1LL *` dihilangkan?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Ekskusi Kondisi**: `1LL * a * b`. Karena ada `1LL`, robot berhitung di skala Long Long.
 2. $1.000.000 \times 2.000 = 2.000 .000 .000$ (2 Miliar).
 3. Apakah 2 Miliar > 1.5 Miliar? **BENAR (1)**.
 4. Robot mengambil jalur pertama: `a / 10` $\rightarrow$ $1.000.000 / 10 = \mathbf{100.000}$.
 
 **Jawaban Akhir: 100000**
 </details>
 
 ---
 
 ### Soal 46: Floating Point Precision War (Epsilon Match)
 ```cpp
 double a = 0.1, b = 0.2;
 bool match = (a + b == 0.3);
 bool safe_match = (a + b > 0.3 - 1e-9 && a + b < 0.3 + 1e-9);
 int res = (match ? 1 : (safe_match ? 2 : 3));
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Mengapa `match` bernilai `false` sedangkan `safe_match` bernilai `true`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot hitung `a + b`. Karena presisi biner, hasilnya sekitar `0.3000...004`.
 2. **`match`**: `0.300...4 == 0.3` $\rightarrow$ **SALAH (0)**.
 3. **`safe_match`**: Mengecek apakah hasil ada di rentang $0.3 \pm 10^{-9}$. Karena masuk rentang, hasilnya **BENAR (1)**.
 4. **Ternary Bertingkat**: `(match ? 1 : (true ? 2 : 3))`. Robot memilih **2**.
 
 **Jawaban Akhir: 2**
 </details>
 
 ---
 
 ### Soal 47: Triple-Nested Ternary Architect (The Pointer logic)
 ```cpp
 int a = 5, b = 10, c = 15;
 int res = (a > b) ? (c++) : (++b > a ? (a--) : (c--));
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `a`, `b`, `c`, dan `res`?
 2. Perintah mana saja yang diabaikan (Short-circuit) oleh robot?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Ternary Luar**: `a > b` ($5 > 10$) $\rightarrow$ **SALAH**. Segmen `(c++)` dilewati.
 2. **Masuk Ternary Dalam**: `(++b > a ? (a--) : (c--))`.
 3. Robot naikkan `b` dulu jadi **11**. Apakah $11 > 5$? **BENAR**.
 4. Robot ambil segmen benar: `(a--)`.
 5. Nilai `res` diisi nilai `a` semula (**5**), lalu `a` turun jadi **4**.
 6. Segmen `(c--)` dilewati.
 
 **Jawaban Akhir: a=4, b=11, c=15, res=5**
 </details>
 
 ---
 
 ### Soal 48: Bitwise Logic Parity Integration (Mixed Parity)
 ```cpp
 int x = 11, y = 14;
 int flag = 0;
 if ((x & 1) && !(y & 1)) {
     flag = 100;
 } else {
     flag = 200;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `flag`?
 2. Apa yang sedang diperiksa oleh kode `(x & 1) && !(y & 1)` dalam bahasa manusia?
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bahasa Manusia**: "Apakah `x` GANJIL dan `y` GENAP?"
 2. **Evaluasi `x & 1`**: 11 (Biner `1011`) & 1 $\rightarrow$ **1** (Benar).
 3. **Evaluasi `!(y & 1)`**: 14 (Biner `1110`) & 1 $\rightarrow$ **0**. Lalu dinegasikan `!0` $\rightarrow$ **1** (Benar).
 4. Hasil: `Benar && Benar` $\rightarrow$ **BENAR**.
 5. `flag = 100`.
 
 **Jawaban Akhir: 100**
 </details>
 
 ---
 
 ### Soal 49: De Morgan Negation Minefield (The Double Bang)
 ```cpp
 bool A = true, B = false;
 bool res = !(!A || !B) == (A && B);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res` (0 atau 1)?
 2. Sebutkan Hukum Logika yang membuktikan bahwa sisi kiri dan sisi kanan pasti selalu sama!
 
 <details>
 <summary><b>Diagnosis Logika Sang Dewa (Human Compiler)</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Sisi Kiri**: `!(!T || !F)` $\rightarrow$ `!(F || T)` $\rightarrow$ `!(T)` $\rightarrow$ **SALAH/0**.
 2. **Sisi Kanan**: `A && B` $\rightarrow$ `T && F` $\rightarrow$ **SALAH/0**.
 3. Apakah $0 == 0$? **BENAR (1)**.
 4. *Hukum De Morgan: Negasi dari (Bukan A ATAU Bukan B) adalah setara dengan (A DAN B).*
 
 **Jawaban Akhir: 1 (True)**
 </details>
 
 ---
 
 ### Soal 50: THE FINAL BOSS - THE GOD COMPILER
 ```cpp
 char c = 'B';
 int n = 5;
 int out = 0;
 
 if ((c - 'A' == 1 && ++n > 5) || (n / 2 > 0)) {
     n += 10;
     switch (n % 4) {
         case 0: out = n / 2;
         case 2: out += 5; break;
         default: out = -1;
     }
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari `n` dan `out`?
 2. Mengapa robot tidak melakukan `short-circuit` pada bagian `(n / 2 > 0)`?
 
 <details>
 <summary><b>Diagnosis Logika SANG DEWA</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If (Kurung Kiri)**: `(c - 'A' == 1 && ++n > 5)`.
    - `'B' - 'A'` = 1. Apakah $1 == 1$? **BENAR**.
    - Robot lanjut ke `++n > 5`. `n` naik jadi **6**. Apakah $6 > 5$? **BENAR**.
    - Kurung Kiri bernilai **BENAR**.
 2. **Short-Circuit OR**: Karena kurung kiri sudah Benar dan operatornya `||`, robot **TIDAK MENGECEK** `(n / 2 > 0)`.
 3. **Masuk Blok If**: `n += 10`. Nilai `n` sekarang **16**.
 4. **Switch**: `n % 4` $\rightarrow$ `16 % 4` = **0**.
 5. **Masuk case 0**: `out = n / 2` $\rightarrow$ $16 / 2 = \mathbf{8}$.
 6. **Waterfall (No Break)**: Robot jatuh ke `case 2`.
 7. **Eksekusi case 2**: `out += 5` $\rightarrow$ $8 + 5 = \mathbf{13}$.
 8. **Selesai**: Ada `break;`, robot berhenti.
 
 **Jawaban Akhir: n = 16, out = 13**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🎓 **SELAMAT! Kamu telah menyelesaikan Kurikulum Percabangan (Part C - Modul 02). Dunia koding kini ada di genggamanmu!**
