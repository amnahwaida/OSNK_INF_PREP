# Latihan Soal Part C - Modul 02 - Set 02 (Elite/God-Tier Challenge: Percabangan)
 
 ---
 
 🏆 **MODUL LANJUTAN - LEVEL MASTER:**
 Jangan terkecoh dengan penampilan kode yang pendek. Di level ini, setiap karakter (seperti tanda seru `!`, tanda kurung `()`, atau tanda sama dengan `=`) memiliki kekuatan untuk memutarbalikkan seluruh logika program. Gunakan ketelitian seorang auditor kode untuk menjawabnya.
 
 ---
 
 ### Soal 11: Radar Keamanan Ganda (Compound Short-circuit)
 ```cpp
 int x = 0, y = 5, z = 10;
 bool res = (x++ > 0 || ++y > 5) && (z-- > 10 || ++x > 0);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`, `y`, dan `z`?
 2. Bagaimana urutan evaluasi robot pada operator `&&` dan `||` di atas?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 2.
 - `y` = 6.
 - `z` = 9.
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 Start --> A{"x++ > 0 (F)"}
 A -- Next Path --> B{"++y > 5 (T)"}
 B -- Left Side T --> C{"z-- > 10 (F)"}
 C -- Next Path --> D{"++x > 0 (T)"}
 D -- Right Side T --> End["res = True"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Kurung Kiri (`x++ > 0 || ++y > 5`)**:
    - Robot cek `x++ > 0`. Nilai `x` (0) dibandingkan dengan 0 $\rightarrow$ **SALAH**. Setelah itu `x` naik jadi **1**.
    - Karena Salah, robot cek sisi kanan `||`. Robot naikkan `y` jadi **6**. Apakah $6 > 5$? **BENAR**. Kurung kiri bernilai **BENAR**.
 2. **Kurung Kanan (`z-- > 10 || ++x > 0`)**:
    - Karena kurung kiri Benar dan operatornya `&&`, robot WAJIB cek kurung kanan.
    - Robot cek `z-- > 10`. Nilai `z` (10) dibandingkan dengan 10 $\rightarrow$ **SALAH**. Setelah itu `z` turun jadi **9**.
    - Karena Salah, robot cek sisi kanan `||`. Robot naikkan `x` dari 1 menjadi **2**. Apakah $2 > 0$? **BENAR**. Kurung kanan bernilai **BENAR**.
 3. `Benar && Benar` = **Benar (1)**.
 
 **Jawaban Akhir: x=2, y=6, z=9**
 </details>
 
 ---
 
 ### Soal 12: Labirin Switch Waterfall (Variable Update Trap)
 ```cpp
 int k = 1;
 int m = 5;
 switch (k + 1) {
     case 1: m += 10;
     case 2: k = m++; 
     case 3: m += k;
              break;
     default: m = 0;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `k` dan `m`?
 2. Mengapa robot mengeksekusi `case 3` padahal hasil `k+1` adalah 2?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: `k + 1` = `1 + 1` = **2**. Robot lompat ke `case 2`.
 2. **Eksekusi `case 2`**: `k = m++`. Robot mengisi `k` dengan nilai `m` yang sekarang (**5**). Baru setelah itu `m` naik jadi 6. (Sekarang `k=5, m=6`).
 3. **Waterfall**: Karena tidak ada `break;`, robot jatuh ke `case 3`.
 4. **Eksekusi `case 3`**: `m += k`. Maka `m = 6 + 5 = 11`.
 5. **Selesai**: Ada `break;`, robot keluar dari switch.
 
 **Jawaban Akhir: k=5, m=11**
 </details>
 
 ---
 
 ### Soal 13: Pernikahan Ternary Rumit (Nested Ternary Logic)
 ```cpp
 int a = 5, b = 10;
 int res = (a > b) ? (a++) : (b > a) ? (++b) : (a + b);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `res`, `a`, dan `b`?
 2. Mengapa bagian `a++` dan `a + b` tidak pernah dieksekusi?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot cek `a > b` ($5 > 10$) $\rightarrow$ **SALAH**. Segmen `(a++)` dilewati.
 2. Robot cek segmen setelah titik dua pertama: `(b > a) ? (++b) : (a+b)`.
 3. Robot cek `b > a` ($10 > 5$) $\rightarrow$ **BENAR**.
 4. Robot mengeksekusi `++b`. Nilai `b` naik jadi **11**.
 5. Nilai 11 tersebut diberikan ke variabel `res`. Segmen `(a+b)` dilewati.
 
 **Jawaban Akhir: res=11, a=5, b=11**
 </details>
 
 ---
 
 ### Soal 14: Kebenaran Irasional (Non-Zero Evaluation)
 ```cpp
 double d = -0.5;
 int x = 0;
 if (d) {
     x = 1;
 }
 if (d + 0.5) {
     x = 2;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`?
 2. Apa syarat sebuah nilai dianggap "Salah" (False) di dalam `if` C++?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek `if(d)`**: Nilai `d` adalah -0.5. Di C++, angka berapapun selain NOL (0) dianggap **BENAR**. Maka `x` jadi **1**.
 2. **Cek `if(d + 0.5)`**: Robot hitung $-0.5 + 0.5 = 0.0$. Karena hasilnya tepat NOL, maka dianggap **SALAH**. Blok ini dilewati.
 3. Nilai akhir `x` tetap 1.
 
 **Jawaban Akhir: x = 1**
 </details>
 
 ---
 
 ### Soal 15: Penugasan dalam Switch (Switch Assignment Trap)
 ```cpp
 int n = 0;
 switch (n = 2) {
     case 0: n += 10; break;
     case 2: n += 5; break;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `n`?
 2. Apakah diperbolehkan melakukan penugasan `=` di dalam kurung `switch()`?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Evaluasi Switch**: Robot melihat `n = 2`. Robot mengisi laci `n` dengan angka 2.
 2. Hasil evaluasi switch tersebut adalah nilai yang dimasukkan, yaitu **2**.
 3. Robot mencari `case 2`. Ketemu!
 4. `n += 5` $\rightarrow$ `n = 2 + 5 = 7`.
 
 **Jawaban Akhir: 7**
 </details>
 
 ---
 
 ### Soal 16: Gerbang ASCII Bersyarat
 ```cpp
 char c = 'b'; // ASCII 98
 int res = 0;
 if (c >= 'a' && c <= 'z' && c % 2 != 0) {
     res = 1;
 } else {
     res = 2;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Mengapa syarat terakhir `c % 2 != 0` mematikan seluruh kondisi `if`?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Syarat 1 & 2**: `'b'` berada di antara `'a'` dan `'z'`. **BENAR**.
 2. **Syarat 3**: `c % 2 != 0`. Nilai 'b' adalah **98**. $98 \pmod 2 = 0$. Apakah $0 \neq 0$? **SALAH**.
 3. Karena satu syarat Salah (operator `&&`), seluruh kondisi `if` menjadi Salah.
 4. Robot masuk ke `else` $\rightarrow$ `res = 2`.
 
 **Jawaban Akhir: 2**
 </details>
 
 ---
 
 ### Soal 17: Overflow Boundary (Int Comparison Fallacy)
 ```cpp
 int a = 1000000;
 int b = 3000;
 bool cek = false;
 if (a * b > 2000000000) {
     cek = true;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `cek` (0 atau 1)?
 2. Hasil asli perkalian adalah 3 Miliar. Mengapa robot menganggapnya lebih kecil dari 2 Miliar?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot hitung `a * b` ($10^6 \times 3000 = 3 \times 10^9$).
 2. **Overflow**: Karena batas `int` cuma 2.1 Miliar, hasil 3 Miliar meluap (overflow) menjadi angka negatif raksasa.
 3. Robot cek: Apakah (Angka Negatif) > 2 Miliar? **SALAH**.
 4. `cek` tetap **false (0)**.
 
 **Jawaban Akhir: 0**
 </details>
 
 ---
 
 ### Soal 18: Shadowing & Global Access (:: Operator)
 ```cpp
 int x = 10;
 int main() {
     int x = 5;
     if (x > 0) {
         int x = 1;
         ::x = x + ::x;
     }
     printf("%d", x);
 }
 ```
 **Pertanyaan:**
 1. Angka apakah yang akan tercetak di layar monitor?
 2. Berapakah nilai variabel `x` yang berada di luar `main` (Global) sekarang?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Di dalam `if`, robot melihat `int x = 1`. Ini variabel **Lokal Terdalam**.
 2. Perintah `::x = x + ::x` berarti: `Global = Lokal + Global`.
 3. `Global = 1 + 10 = 11`.
 4. Perintah `printf` berada di luar blok `if` (tapi masih di dalam `main`). Robot melihat variabel `x` milik `main`, yaitu **5**.
 
 **Jawaban Akhir: 5**
 </details>
 
 ---
 
 ### Soal 19: Double Not (!! Logic)
 ```cpp
 int x = 5, y = 0;
 int res = 0;
 if (!!x + !y == 2) {
     res = 100;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`?
 2. Apa hasil numerik dari `!!5` dan `!0`?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **`!!x` (!!5)**: `5` (Benar) $\rightarrow$ `!5` (Salah/0) $\rightarrow$ `!!5` (Benar/1).
 2. **`!y` (!0)**: `0` (Salah) $\rightarrow$ `!0` (Benar/1).
 3. Hitungan: $1 + 1 = 2$.
 4. Apakah $2 == 2$? **BENAR**.
 5. `res = 100`.
 
 **Jawaban Akhir: 100**
 </details>
 
 ---
 
 ### Soal 20: THE MASTER - SIMULASI RAZIA BP PARALEL
 ```cpp
 int poin = 10, rambut = 15;
 char kasta = 'C';
 int hasil = 0;
 
 if (rambut > 10) {
     if (++poin > 10 && kasta == 'B') hasil = 1;
     else if (poin-- > 10 || kasta == 'C') {
         switch (kasta) {
             case 'C': hasil = poin++; break;
             case 'B': hasil = --poin; break;
         }
     }
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `hasil`, `poin`, dan `rambut`?
 2. Jelaskan mengapa `poin--` di dalam `else if` tetap memengaruhi nilai akhir walaupun ada operator `||`.
 
 <details>
 <summary><b>Diagnosis Logika Sang GURU</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **If Luar**: `rambut > 10` (15 > 10) $\rightarrow$ **BENAR**. Masuk.
 2. **If Dalam 1**: `++poin > 10 && kasta == 'B'`. `poin` naik jadi **11**. Syarat pertama Benar, tapi `kasta == 'B'` **SALAH**. Jadi seluruh If ini Gagal.
 3. **Else If**: `poin-- > 10 || kasta == 'C'`.
    - Robot cek `poin-- > 10`. Nilai `poin` (11) dibandingkan dengan 10 $\rightarrow$ **BENAR**.
    - **PENTING**: Setelah dicek, nilai `poin` turun jadi **10**.
    - Karena syarat pertama Benar, robot **Short-Circuit** (tidak cek `kasta == 'C'`). Namun kondisi sudah dianggap Benar.
 4. **Switch**: `case 'C'`. `hasil = poin++`.
    - Robot mengisi `hasil` dengan nilai `poin` yang sekarang (**10**).
    - Setelah itu `poin` naik lagi jadi **11**.
 
 **Jawaban Akhir: hasil = 10, poin = 11, rambut = 15**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 ⏩ **Lanjut ke Latihan Set 03: [Set 03](./set-03.md)**
