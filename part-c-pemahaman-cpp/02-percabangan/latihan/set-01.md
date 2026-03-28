# Latihan Soal Part C - Modul 02 - Set 01 (Elite/God-Tier Challenge: Percabangan)
 
 ---
 
 ⚠️ **PERINGATAN LEVEL ELITE:**
 Percabangan bukan hanya soal `if` dan `else`. Ini adalah soal **Pengambilan Keputusan Robot**. Robot bisa menjadi sangat "malas" (*short-circuit*) atau sangat "patuh" (*waterfall*). Di set ini, kamu akan diuji apakah kamu bisa menebak isi pikiran sang robot secara presisi 100%.
 
 ---
 
 ### Soal 1: Ranjau Short-Circuit Profundal
 ```cpp
 int x = 5, y = 10, z = 0;
 if ((x > 10 && ++y > 0) || (z++ == 0)) {
     x = x + y + z;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `x`, `y`, dan `z`?
 2. Syarat mana yang dijalankan oleh robot dan mana yang dilewati?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 16.
 - `y` = 10 (Tetap).
 - `z` = 1.
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 Start --> A{"x > 10 (F)"}
 A -- Next --> B{"z++ == 0 (T)"}
 A -- Skip --> C["++y (Short-circuit &&)"]
 B -- Go --> D["x = 5 + 10 + 1"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`x > 10 && ++y > 0`)**: Robot cek `5 > 10` $\rightarrow$ **SALAH**. Karena operatornya `&&`, robot malas mengecek lanjutannya. Perintah `++y` **DILEWATI**. (`y` tetap 10).
 2. **Bagian 2 (`(Saluran 1) || (z++ == 0)`)**: Karena bagian kiri `||` Salah, robot harus cek sisi kanan.
 3. **Eksekusi Kanan**: `z++ == 0`. Robot memakai nilai `z` yang sekarang (**0**) untuk dicek apakah sama dengan 0. Jawabannya **BENAR (1)**.
 4. **Side Effect**: Sesuai hukum `z++`, setelah dicek, nilai `z` naik jadi **1**.
 5. **Masuk Blok If**: Karena hasil akhirnya Benar, `x = 5 + 10 + 1 = 16`.
 
 **Jawaban Akhir: x=16, y=10, z=1**
 </details>
 
 ---
 
 ### Soal 2: Labirin Switch-Case Waterfall (Tanpa Break)
 ```cpp
 int poin = 2;
 int hukuman = 0;
 switch (poin) {
     case 3: hukuman += 100;
     case 2: hukuman += 50;
     case 1: hukuman += 10;
     default: hukuman += 5;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `hukuman`?
 2. Apa yang terjadi jika kata kunci `break` tidak ada dalam `switch`?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **Mermaid Flowchart:**
 ```mermaid
 graph TD
 Start --> A{"poin = 2?"}
 A -- Yes --> B["hukuman += 50"]
 B --> C["hukuman += 10 (Waterfall)"]
 C --> D["hukuman += 5 (Waterfall)"]
 ```
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mencari `case 2`. Ketemu! `hukuman` jadi **50**.
 2. **Bencana Waterfall**: Karena tidak ada perintah `break;`, robot tidak tahu kalau ia harus berhenti. Ia terus "terjun bebas" ke baris-baris di bawahnya tanpa peduli apakah `case`-nya cocok atau tidak.
 3. Robot melibas `case 1`: `hukuman = 50 + 10 = 60`.
 4. Robot melibas `default`: `hukuman = 60 + 5 = 65`.
 
 **Jawaban Akhir: 65**
 **Pesan Juara:** `switch` tanpa `break` adalah cara robot melakukan eksekusi bertingkat. Jangan sampai terjebak!
 </details>
 
 ---
 
 ### Soal 3: Pernikahan Ternary (Nested Ternary)
 ```cpp
 int jam = 14;
 string status = (jam < 12) ? "Pagi" : (jam < 18) ? "Sore" : "Malam";
 ```
 **Pertanyaan:**
 1. Apa isi dari variabel `status`?
 2. Bagaimana urutan evaluasi dari ternary operator di atas?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot cek syarat 1: `jam < 12` (14 < 12) $\rightarrow$ **SALAH**.
 2. Karena Salah, robot mengarah ke pilihan setelah tanda titik dua `:` yang pertama.
 3. Di pilihan ke-2, robot menemukan teka-teki baru: `(jam < 18) ? "Sore" : "Malam"`.
 4. Robot cek syarat 2: `jam < 18` (14 < 18) $\rightarrow$ **BENAR**.
 5. Robot mengambil kata **"Sore"**.
 
 **Jawaban Akhir: "Sore"**
 </details>
 
 ---
 
 ### Soal 4: Jebakan Penugasan Siluman (Assignment Trap)
 ```cpp
 int skor = 0;
 if (skor = 10) {
     skor += 5;
 } else {
     skor -= 5;
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `skor`?
 2. Mengapa robot masuk ke blok `if` padahal sebelumnya `skor = 0`?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Mata Kompilator**: Perhatikan kode di dalam `if`. Bukan `skor == 10` (perbandingan), tapi `skor = 10` (pengisian nilai).
 2. Robot mengisi loker `skor` dengan angka **10**.
 3. **Hasil Evaluasi**: Karena angka 10 di C++ dianggap sebagai **BENAR** (semua angka selain 0 adalah Benar), maka robot masuk ke blok `if`.
 4. Operasi: `skor = 10 + 5 = 15`.
 
 **Jawaban Akhir: 15**
 </details>
 
 ---
 
 ### Soal 5: Hierarki Logika (&& > ||)
 ```cpp
 bool a = true, b = false, c = false;
 bool hasil = a || b && c;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `hasil` (0 atau 1)?
 2. Antara `||` dan `&&`, mana yang memiliki kasta (prioritas) lebih tinggi?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Di C++, kasta operator `&&` (DAN) lebih tinggi dibandingkan `||` (ATAU).
 2. Robot mengerjakan `b && c` dulu: `false && false` $\rightarrow$ **false**.
 3. Baru robot mengerjakan sisanya: `true || false`.
 4. Hasil akhir: **true (1)**.
 
 **Jawaban Akhir: 1 (True)**
 </details>
 
 ---
 
 ### Soal 6: Razia ASCII & Paritas
 ```cpp
 char huruf = 'A'; // ASCII 65
 int jenis = 0;
 if (huruf % 2 == 0) {
     jenis = 1; // Genap
 } else {
     jenis = 2; // Ganjil
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai `jenis`?
 2. Bagaimana robot bisa mengoperasikan modulo `%` pada sebuah huruf?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mengubah huruf `'A'` menjadi angka aslinya di tabel ASCII, yaitu **65**.
 2. Robot menghitung: $65 \pmod 2$.
 3. Karena 65 adalah angka ganjil, sisanya adalah **1**.
 4. Maka kondisi `if` bernilai Salah ($1 == 0$ adalah Salah).
 5. Robot masuk ke blok `else` dan menjalankan `jenis = 2`.
 
 **Jawaban Akhir: 2**
 </details>
 
 ---
 
 ### Soal 7: Pintu Gerbang Overflow (LL Condition)
 ```cpp
 int x = 2000000;
 int y = 2000000;
 bool bahaya = false;
 if (x * y > 1000000000) {
     bahaya = true;
 }
 ```
 **Pertanyaan:**
 1. Apakah `bahaya` bernilai true?
 2. Mengapa perkalian di dalam `if` bisa menghasilkan nilai negatif (overflow)?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot menghitung `x * y` ($2 \times 10^6 \times 2 \times 10^6 = 4 \times 10^{12}$).
 2. **Jebakan Overflow**: Karena `x` dan `y` adalah `int`, perkaliannya dihitung di area `int` (limit 2 Miliar). Hasil 4 Triliun meledak (overflow) dan diinterpretasikan sebagai angka negatif raksasa.
 3. Apakah (Angka Negatif) > 1 Miliar? Jawabannya **SALAH**.
 4. `bahaya` tetap bernilai **false**.
 
 **Jawaban Akhir: false (0)**
 </details>
 
 ---
 
 ### Soal 8: Negasi Berlapis (Triple Bang Logic)
 ```cpp
 int a = 10;
 bool hasil = !!!(a > 5);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `hasil`?
 2. Bagaimana cara paling cepat membaca operator negasi `!` yang berkali-kali?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `10 > 5` $\rightarrow$ **Benar**.
 2. `!Benar` $\rightarrow$ Salah.
 3. `!Salah` $\rightarrow$ Benar.
 4. `!Benar` $\rightarrow$ **Salah (0)**.
 
 **Jawaban Akhir: 0 (False)**
 **Trik Juara:** Jika jumlah tanda `!` ganjil, hasilnya dibalik. Jika genap, hasilnya tetap.
 </details>
 
 ---
 
 ### Soal 9: Bayangan Lokal dalam Percabangan (Variable Shadowing)
 ```cpp
 int x = 100;
 if (x > 50) {
     int x = 10;
     x += 5;
 }
 printf("%d", x);
 ```
 **Pertanyaan:**
 1. Angka apakah yang tercetak di layar monitor?
 2. Mengapa perintah `x += 5` tidak memengaruhi angka 100?
 
 <details>
 <summary><b>Diagnosis Logika & Mermaid Flowchart</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mulai dengan `x = 100`.
 2. Masuk blok `if`. Di sana robot menemukan deklarasi baru: `int x = 10`.
 3. **Shadowing**: Laci `x` yang baru (isi 10) menutupi laci `x` yang lama (isi 100). Operasi `x += 5` hanya mengubah laci baru menjadi **15**.
 4. Begitu keluar blok `if`, laci baru dihancurkan. Robot kembali melihat laci lama yang isinya masih **100**.
 
 **Jawaban Akhir: 100**
 </details>
 
 ---
 
 ### Soal 10: THE FINAL BOSS - Simulasi Razia BP
 ```cpp
 char grade = 'B';
 int poin = 10, rambut = 15;
 int hasil = 0;
 
 if ((rambut > 10 && ++poin > 10) || grade == 'A') {
     switch (poin) {
         case 11: hasil += 100;
         case 10: hasil += 50; 
                  break;
         default: hasil += 10;
     }
 }
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `hasil`?
 2. Berapakah nilai `poin` sekarang?
 
 <details>
 <summary><b>Diagnosis Logika Sang Maestro</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Cek If**: `(15 > 10 && ++poin > 10)`. Karena `15 > 10` (Benar), robot lanjut menjalankan `++poin`.
 2. **Poin Naik**: `poin` jadi **11**. Lalu dicek `11 > 10`? Jawabannya **Benar**.
 3. **Switch Case**: `poin` sekarang 11. Robot masuk ke `case 11`.
 4. **Waterfall**: `hasil` jadi 100. Karena di `case 11` tidak ada `break;`, robot jatuh ke `case 10`.
 5. **Case 10**: `hasil = 100 + 50 = 150`. Di sini ada `break;`, robot berhenti.
 
 **Jawaban Akhir: hasil = 150, poin = 11**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 ⏩ **Lanjut ke Latihan Set 02: [Set 02](./set-02.md)**
