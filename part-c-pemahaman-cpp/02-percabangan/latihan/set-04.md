# Latihan Soal Part C - Modul 02 - Set 04 (Hall of Fame Edition: Percabangan Terpadu)
 
 ---
 
 🏛️ **KELAS MASTER - DIAGNOSA MESIN:**
 Selamat datang di gerbang terakhir pemahaman logika. Di set ini, kamu tidak hanya menebak hasil, tapi juga harus membedah urutan pemikiran komputer bit demi bit. Hati-hati dengan efek samping (*side effects*), hierarki tipe data, dan bayangan variabel (*shadowing*).
 
 ---
 
 ### Soal 31: Tabrakan Short-Circuit (The Collision)
 ```cpp
 int x = 5, y = 10, z = 0;
 bool res = (x-- > 0 && ++z > 0) || (++y > 0 && z-- > 0);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`, `y`, dan `z`?
 2. Mengapa blok `(++y > 0 && z-- > 0)` sama sekali tidak pernah menyentuh memori?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 4.
 - `y` = 10 (Tetap).
 - `z` = 1.
 - `res = true (1)`.
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 S --> C1{"x-- > 0 (T)"}
 C1 -- Lanjut && --> C2["++z > 0 (T)"]
 C2 -- Hasil Kiri True --> End["res = true"]
 C2 -- Short-circuit OR --> C3["Blok Kanan Dilewati!"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Sisi Kiri `||`**: Robot cek `x-- > 0` ($5 > 0$) $\rightarrow$ **BENAR**. `x` turun jadi **4**.
 2. Karena syarat pertama `&&` Benar, robot lanjut ke `++z > 0`. `z` naik jadi **1**. Apakah $1 > 0$? **BENAR**.
 3. Hasil seluruh kurung kiri adalah **BENAR**.
 4. **Short-Circuit OR**: Karena sisi kiri `||` sudah Benar, robot robot malas dan langsung berhenti. Segala sesuatu di sisi kanan `||` (**termasuk `++y`**) tidak dijalankan!
 
 **Jawaban Akhir: x=4, y=10, z=1**
 </details>
 
 ---
 
 ### Soal 32: Geseran Ternary ASCII (ASCII Shift)
 ```cpp
 char c = 'B';
 int shift = 2;
 char res = (c + shift > 'Z') ? 'A' : (!!shift ? c + 1 : 'X');
 ```
 **Pertanyaan:**
 1. Berapakah nilai karakter `res`?
 2. Apa maksud dari `!!shift` di dalam ternary kedua?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek Ternary 1**: `c + shift` $\rightarrow$ `'B' + 2` = `'D'` (ASCII 68). Apakah `'D' > 'Z'`? **SALAH**.
 2. **Masuk Ternary 2**: `(!!shift ? c + 1 : 'X')`.
 3. Robot evaluasi `!!shift`: `shift` (2) adalah Benar (1) $\rightarrow$ `!2` (Salah/0) $\rightarrow$ `!!2` (**Benar/1**).
 4. Karena Benar, robot memilih `c + 1` $\rightarrow$ `'B' + 1 = 'C'`.
 
 **Jawaban Akhir: 'C'**
 </details>
 
 ---
 
 ### Soal 33: Switch Matrix Fallthrough (Triple Variable Update)
 ```cpp
 int a = 1, b = 5, c = 10;
 switch (a++) {
     case 1: b += a++; 
     case 2: c = b--; 
              break;
     default: a = 0;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `a`, `b`, dan `c`?
 2. Bagaimana `a` bertambah dua kali dalam satu jalur eksekusi?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: `switch(a++)`. Robot ambil nilai 1 untuk switch, lalu `a` naik jadi **2**.
 2. Robot masuk ke `case 1`.
 3. **Eksekusi case 1**: `b += a++`. `b = 5 + 2 = 7`. Lalu `a` naik lagi jadi **3**.
 4. **Waterfall**: Tanpa `break;`, jatuh ke `case 2`.
 5. **Eksekusi case 2**: `c = b--`. `c` diisi nilai `b` (**7**). Lalu `b` turun jadi **6**.
 6. **Selesai**: Ada `break;`, robot berhenti.
 
 **Jawaban Akhir: a=3, b=6, c=7**
 </details>
 
 ---
 
 ### Soal 34: Ranjau Penugasan Implisit (Truth Minefield)
 ```cpp
 int x = 0, y = 5;
 if (x = !y) {
     x += 10;
 } else {
     x -= 10;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`?
 2. Mengapa robot masuk ke blok `else`? Padahal ada perintah `x = !y`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi If**: `x = !y`. Robot melihat `!y` (!5) $\rightarrow$ **Salah/0**.
 2. Robot mengisi `x` dengan angka **0**.
 3. Hasil dari `if(0)` adalah **SALAH**.
 4. Robot masuk ke blok `else`.
 5. `x -= 10` $\rightarrow$ `0 - 10 = -10`.
 
 **Jawaban Akhir: -10**
 </details>
 
 ---
 
 ### Soal 35: Batas Presisi Peluru (Precision Boundary)
 ```cpp
 double d = 0.1 + 0.2;
 int x = 10;
 if (d - 0.3 > 1e-15) {
     x = 20;
 } else if (d == 0.3) {
     x = 30;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`?
 2. Mengapa `d == 0.3` bernilai SALAH bagi robot?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bencana Biner**: `0.1 + 0.2` aslinya adalah `0.300000000000000044...`. Ia sedikit lebih besar dari 0.3.
 2. **Cek If 1**: `d - 0.3` hasilnya sekitar $4.4 \times 10^{-17}$. Apakah ini lebih besar dari $10^{-15}$? **SALAH**.
 3. **Cek If 2**: `d == 0.3`. Karena ada sisa koma diujung, mereka tidak sama. **SALAH**.
 4. Karena semua Salah, `x` tetap **10**.
 
 **Jawaban Akhir: 10**
 </details>
 
 ---
 
 ### Soal 36: Scope & Global Shadowing (Else Redirection)
 ```cpp
 int k = 100;
 int main() {
     int k = 10;
     if (k < 5) {
         int k = 1;
     } else {
         ::k = k + 1;
     }
     printf("%d", ::k);
 }
 ```
 **Pertanyaan:**
 1. Angka apa yang tercetak?
 2. Nilai `k` mana yang ditambahkan ke angka 1 di dalam blok `else`?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If**: `k < 5`. `k` yang digunakan adalah lokal `main` (**10**). $10 < 5$ adalah **SALAH**.
 2. Robot masuk ke blok `else`.
 3. **Eksekusi else**: `::k = k + 1`. 
    - `k` adalah lokal `main` (10). 
    - `::k` adalah Global (100).
    - `Global = 10 + 1 = 11`.
 4. Nilai `::k` berubah jadi **11**.
 
 **Jawaban Akhir: 11**
 </details>
 
 ---
 
 ### Soal 37: 1LL Condition Overload (Product Bounds)
 ```cpp
 int n = 50000;
 int m = 50000;
 bool res = false;
 if (1LL * n * m >= 2500000000) {
     res = true;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res` (0 atau 1)?
 2. Apa yang terjadi jika `1LL *` dihapus dari kode di atas?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot hitung `n * m` ($50000 \times 50000 = 2.5 \times 10^9$).
 2. Karena ada `1LL`, robot berhitung di skala Long Long. 2.5 Miliar muat!
 3. Apakah 2.5 Miliar >= 2.5 Miliar? **BENAR**.
 4. `res = true (1)`.
 5. *Info: Jika 1LL dihapus, hasil perkalian meledak (overflow) dan bernilai negatif, sehingga res jadi 0.*
 
 **Jawaban Akhir: 1**
 </details>
 
 ---
 
 ### Soal 38: Bit-Parity Switch (Masking Logic)
 ```cpp
 int x = 15;
 int out = 0;
 switch (x & 3) {
     case 1: out = 10; break;
     case 3: out = 30; 
     default: out += (x % 2);
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `out`?
 2. Bagaimana hasil bitwise `15 & 3` ditemukan?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: `15 & 3`.
    - 15 = `1111` (Biner).
    - 3 = `0011` (Biner).
    - Hasil AND: `0011` $\rightarrow$ **3**.
 2. Robot masuk ke `case 3`.
 3. **Eksekusi case 3**: `out = 30`. 
 4. **Waterfall**: Tanpa `break;`, jatuh ke `default`.
 5. **Eksekusi default**: `out += (15 % 2)`.
    - $30 + 1 = \mathbf{31}$.
 
 **Jawaban Akhir: 31**
 </details>
 
 ---
 
 ### Soal 39: Negasi Berlapis (Logic Labyrinth)
 ```cpp
 int a = 0, b = 1;
 bool res = (!!!a != !!b) ? (a = 5) : (b = 5);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `a` dan `b`?
 2. Apakah operator `!=` dievaluasi sebelum atau sesudah ternary `?` ?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Syarat**: `(!!!a != !!b)`.
    - `!!!a` (!!!0): `0` (F) $\rightarrow$ `!0` (T) $\rightarrow$ `!!0` (F) $\rightarrow$ `!!!0` (**T/1**).
    - `!!b` (!!1): `1` (T) $\rightarrow$ `!1` (F) $\rightarrow$ `!!1` (**T/1**).
    - Apakah $1 \neq 1$? **SALAH**.
 2. Karena Salah, robot memilih jalur kedua: `(b = 5)`.
 3. Variabel `b` diisi angka **5**. Variabel `a` tetap **0**.
 
 **Jawaban Akhir: a=0, b=5**
 </details>
 
 ---
 
 ### Soal 40: THE GRAND MASTER CHAMPION (The Integrated Final)
 ```cpp
 int hp = 100, def = 50;
 char status = 'A'; // Active
 int dmg = 0;
 
 if (status == 'A' && (hp -= 20) > 0) {
     if (hp < 100 || def++ > 50) {
         dmg = (def == 51) ? (hp / 2) : (hp % 10);
     }
 } else {
     hp = 0;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `hp`, `def`, dan `dmg`?
 2. Mengapa `def` tidak pernah bertambah nilainya?
 
 <details>
 <summary><b>Diagnosis Logika SANG JUARA</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **If Luar**: `status == 'A'` (T) && `(hp -= 20) > 0`.
    - `hp` turun jadi **80**. Apakah $80 > 0$? **BENAR**.
    - Hasil kurung luar: **BENAR**. Masuk.
 2. **If Dalam**: `hp < 100 || def++ > 50`.
    - `hp < 100` ($80 < 100$) adalah **BENAR**.
    - **Short-Circuit OR**: Karena sudah Benar, robot **TIDAK MENGECEK** `def++ > 50`.
    - Berarti `def` **tetap 50**!
 3. **Ternary di dalam If**: `(def == 51) ? (hp / 2) : (hp % 10)`.
    - Apakah `50 == 51`? **SALAH**.
    - Robot memilih `hp % 10` $\rightarrow$ `80 % 10 = 0`.
 4. `dmg` menjadi **0**.
 
 **Jawaban Akhir: hp=80, def=50, dmg=0**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 🏆 **CONGRATULATIONS! Kamu telah menaklukkan Hall of Fame Percabangan!**
