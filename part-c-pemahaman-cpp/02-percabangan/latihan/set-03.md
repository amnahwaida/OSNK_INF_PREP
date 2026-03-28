# Latihan Soal Part C - Modul 02 - Set 03 (Legendary Architect: Percabangan + Tipe Data)
 
 ---
 
 🏛️ **ARSITEK LEGENDA - UJIAN PAMUNGKAS:**
 Ini adalah puncak dari pemahaman Logika Percabangan. Soal-soal di sini tidak hanya menguji `if` dan `else`, tapi juga bagaimana percabangan berinteraksi dengan **Overflow**, **Presisi Double**, **ASCII Math**, dan **Bitwise Parity**. Jika kamu lulus di sini, kamu resmi menjadi "Arsitek Logika" di dunia C++.
 
 ---
 
 ### Soal 21: The 1LL Condition Crisis (Overflow in If)
 ```cpp
 int a = 1000000;
 int b = 2000;
 bool Aman = false;
 if (a * b > 1500000000) {
     Aman = true;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `Aman` (0 atau 1)?
 2. Mengapa angka 2 Miliar (`a*b`) dianggap **tidak lebih besar** dari 1.5 Miliar dalam kondisi `if` di atas?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📦 Isi Laci Memori:**
 - `a * b` = -2,147,483,648 (Overflow).
 - `Aman` = 0 (false).
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 Start --> A["Hitung a * b (int)"]
 A --> B["Hasil: -2.1 Miliar (Overflow)"]
 B --> C{"-2.1 Miliar > 1.5 Miliar? (F)"}
 C -- F --> End["Aman = false"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot menghitung `a * b` ($10^6 \times 2000 = 2 \times 10^9$). Tapi robot berhitung di kasta `int`.
 2. Karena batas `int` cuma 2.14 Miliar, perkalian tersebut nyaris meledak. Hasil aslinya di C++ (bergantung mesin) seringkali berputar menjadi angka negatif terkecil karena **Integer Overflow**.
 3. Apakah (Angka Negatif) > 1.5 Miliar? Jawabannya **SALAH (0)**.
 4. Maka `Aman` tetap bernilai `false`.
 
 **Jawaban Akhir: 0**
 </details>
 
 ---
 
 ### Soal 22: ASCII Switch Cascade (Math in Case)
 ```cpp
 char grade = 'B';
 int poin = 0;
 switch (grade - 'A' + 1) {
     case 1: poin += 10;
     case 2: poin += 20;
     case 3: poin += 30; break;
     default: poin = -1;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `poin`?
 2. Bagaimana robot mengevaluasi rumus di dalam kurung `switch()`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: `'B' - 'A'` adalah $66 - 65 = 1$. Lalu $1 + 1 = \mathbf{2}$.
 2. Robot lompat ke `case 2`.
 3. **Eksekusi `case 2`**: `poin += 20` (Poin sekarang 20).
 4. **Waterfall**: Karena tidak ada `break;`, robot jatuh ke `case 3`.
 5. **Eksekusi `case 3`**: `poin += 30` ($20 + 30 = 50$).
 6. **Keluar**: Ada `break;`, robot berhenti.
 
 **Jawaban Akhir: 50**
 </details>
 
 ---
 
 ### Soal 23: Ranjau Short-Circuit Berlapis (Field Matrix)
 ```cpp
 int x = 5, y = 10;
 bool res = (x < 0 && ++y > 0) || (y < 20 && --x > 0);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x` dan `y`?
 2. Jelaskan urutan pemblokiran eksekusi yang terjadi!
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 4.
 - `y` = 10.
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 S --> C1{"x < 0 (F)"}
 C1 -- Skip --> C2["++y (Short-circuit &&)"]
 C1 -- Logic OR --> C3{"y < 20 (T)"}
 C3 -- Proceed --> C4["--x > 0 (T)"]
 C4 -- Result --> R["res = true"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian Kiri `||`**: `(5 < 0) && ...`. Syarat pertama Salah, robot malas. `++y` **diabaikan**. (`y` tetap 10).
 2. **Bagian Kanan `||`**: Karena kiri Salah, robot wajib cek kanan.
 3. Robot cek `y < 20` ($10 < 20$) $\rightarrow$ **BENAR**. Lanjut cek sisi `&&`.
 4. Robot kurangi `x` jadi **4**. Apakah $4 > 0$? **BENAR**.
 5. Hasil akhir: **true (1)**.
 
 **Jawaban Akhir: x = 4, y = 10**
 </details>
 
 ---
 
 ### Soal 24: Shadow Redirect (Global Condition)
 ```cpp
 int p = 100;
 int main() {
     int p = 50;
     if (p > 10) {
         int p = 1;
         ::p = ::p + p;
     }
     printf("%d %d", p, ::p);
 }
 ```
 **Pertanyaan:**
 1. Angka apa saja yang tercetak di layar monitor?
 2. Variabel `p` mana yang digunakan di dalam kondisi `if (p > 10)`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If**: `p > 10`. Robot menggunakan `p` lokal milik `main` (**50**). Hasilnya **Benar**.
 2. **Di dalam If**: Muncul `p = 1`. Robot mengeksekusi `::p = ::p + p`.
 3. Artinya: `Global = Global (100) + Lokal_Dalam (1)`. Global menjadi **101**.
 4. **Print**: Cetak `p` (Lokal `main` = 50) dan `::p` (Global = 101).
 
 **Jawaban Akhir: 50 101**
 </details>
 
 ---
 
 ### Soal 25: Scientific Ternary Battle (Double Bounds)
 ```cpp
 int x = 1e6; // 1 Juta
 int y = 2e3; // 2 Ribu
 int res = (1LL * x * y > 1500000000) ? 1 : 0;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Apa kegunaan `1LL` dalam kondisi ternary di atas?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot hitung `1LL * x * y`. Karena ada `1LL`, robot berhitung di skala raksasa.
 2. $1.000 .000 \times 2.000 = 2.000 .000 .000$ (2 Miliar).
 3. Apakah 2 Miliar > 1.5 Miliar? Jawabannya **BENAR (1)**.
 4. Maka `res` mengambil nilai **1**.
 
 **Jawaban Akhir: 1**
 </details>
 
 ---
 
 ### Soal 26: Floating Point Epsilon Branch (Precision Trap)
 ```cpp
 double a = 0.1, b = 0.2;
 int status = 0;
 if (a + b == 0.3) {
     status = 1;
 } else if (a + b > 0.3 - 1e-9 && a + b < 0.3 + 1e-9) {
     status = 2;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `status` akhir?
 2. Mengapa robot seringkali gagal di `if` pertama namun sukses di `else if` kedua?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If 1**: `0.1 + 0.2 == 0.3`. Karena ketidaktelitian biner, $0.1+0.2$ seringkali bernilai $0.3000...004$. Maka syarat ini **SALAH**.
 2. **Cek If 2 (Epsilon)**: Robot mengecek apakah hasil jumlahnya berada di rentang sangat dekat dengan 0.3 (toleransi $10^{-9}$). Karena $0.3000...004$ masuk dalam rentang aman itu, maka syarat ini **BENAR**.
 3. `status` menjadi **2**.
 
 **Jawaban Akhir: 2**
 </details>
 
 ---
 
 ### Soal 27: The Compound Switch Shadow (Side Effect Switch)
 ```cpp
 int n = 5, m = 2;
 switch (n += m) {
     case 7: n *= 2;
     case 5: n += 1; break;
     default: n = 0;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `n`?
 2. Apakah nilai `n` berubah di memori sebelum robot mengevaluasi `case`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: `n += m` $\rightarrow$ `n = 5 + 2 = 7`. Sekarang di memori `n` sudah bernilai **7**.
 2. Robot mencari `case 7`. Ketemu!
 3. **Eksekusi case 7**: `n *= 2` $\rightarrow$ `n = 7 * 2 = 14`.
 4. **Waterfall**: Karena tidak ada `break;`, jatuh ke `case 5`.
 5. **Eksekusi case 5**: `n += 1` $\rightarrow$ `n = 14 + 1 = 15`.
 6. **Selesai**: Ada `break;`, robot berhenti.
 
 **Jawaban Akhir: 15**
 </details>
 
 ---
 
 ### Soal 28: Bit-Parity Branching (Odd/Even Logic)
 ```cpp
 int x = 11;
 int hasil = 0;
 if (x & 1) { // Same as x % 2 != 0
     hasil = 10;
 } else {
     hasil = 20;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `hasil`?
 2. Bagaimana cara robot membaca `x & 1` sebagai kondisi Benar/Salah?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `x = 11` dalam biner adalah `1011`.
 2. `x & 1` $\rightarrow$ `1011 & 0001`. Hasilnya adalah **1**.
 3. Di C++, angka **1** dianggap sebagai **BENAR**.
 4. Maka robot masuk ke blok `if` $\rightarrow$ `hasil = 10`.
 
 **Jawaban Akhir: 10**
 </details>
 
 ---
 
 ### Soal 29: Logical Negation Inception (Triple Bang Battle)
 ```cpp
 int a = 5, b = 10;
 bool res = !!!(a < b) == (!!(a - 5));
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res` (0 atau 1)?
 2. Jelaskan proses perombakan tanda `!` tersebut!
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Sisi Kiri**: `5 < 10` (T) $\rightarrow$ `!T` (F) $\rightarrow$ `!!T` (T) $\rightarrow$ `!!!T` (**F/0**).
 2. **Sisi Kanan**: `5 - 5` = 0. `0` adalah Salah (F) $\rightarrow$ `!F` (T) $\rightarrow$ `!!F` (**F/0**).
 3. **Bandingkan**: Apakah $0 == 0$? **BENAR (1)**.
 
 **Jawaban Akhir: 1 (True)**
 </details>
 
 ---
 
 ### Soal 30: THE ULTIMATE LEGEND - THE COMPILER'S NIGHTMARE
 ```cpp
 char c = 'C'; 
 int n = 10;
 double p = 2.5;
 int out = 0;
 
 if ((c - 'A' > 1 && ++n > 10) || (n / 2 < 5)) {
     out = (int)(p * n);
 } else {
     switch (n % 2) {
         case 1: out = 99; break;
         default: out = (1LL * 2000000000 * 2 > 1e12) ? 77 : 88;
     }
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari `out` dan `n`?
 2. Mengapa robot tidak pernah menyentuh blok `else`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Arsitek</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If (Kurung Kiri)**: `(c - 'A' > 1 && ++n > 10)`.
    - `'C' - 'A'` = 2. Apakah $2 > 1$? **BENAR**.
    - Robot lanjut ke `++n > 10`. `n` naik jadi **11**. Apakah $11 > 10$? **BENAR**.
    - Hasil seluruh Kurung Kiri adalah **BENAR**.
 2. **Short-Circuit OR**: Karena kurung kiri Benar dan operatornya `||`, robot **tidak mengecek** kurung kanan `(n / 2 < 5)`.
 3. **Masuk Blok If**: `out = (int)(2.5 * 11)`.
    - $2.5 \times 11 = 27.5$.
    - Cast ke `int` membuang koma $\rightarrow$ **27**.
 
 **Jawaban Akhir: out = 27, n = 11**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🏆 **SELAMAT! Kamu telah menamatkan seluruh tantangan Percabangan! Kamu siap melaju ke Modul 03: Perulangan!**
