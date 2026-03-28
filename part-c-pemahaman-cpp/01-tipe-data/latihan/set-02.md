# Latihan Soal Part C - Modul 01 - Set 02 (The Legend Challenge)
 
 ---
 
 ⚠️ **PERINGATAN LEVEL LEGENDA:**
 Jika Set 01 adalah pemanasan, Set 02 ini adalah **Ujian Ketelitian**. Di sini, robot C++ akan menunjukkan sifat aslinya yang "cuek" tapi mematikan jika kau salah satu langkah saja.
 
 ---
 
 ### Soal 11: Radar Modulo Simetris
 ```cpp
 int a = 3, b = 7;
 int res = (a % b) + (b % a);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir dari variabel `res`?
 2. Bagaimana logika robot saat memproses `3 % 7` (Angka Kecil % Angka Besar)?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `a` = 3, `b` = 7.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Bagian 1 (`a % b`)**: Robot menghitung `3 % 7`. Karena 3 tidak bisa dibagi 7, robot tidak bisa mengurangi angka 3 sama sekali. Hasilnya, angka **3** tetap utuh sebagai sisa bagi.
 2. **Bagian 2 (`b % a`)**: Robot menghitung `7 % 3`. Kelipatan 3 terdekat adalah 6 ($3 \times 2 = 6$). Sisa baginya adalah $7 - 6 = 1$.
 3. Tambahkan: `3 + 1 = 4`.
 
 **Jawaban Akhir: 4**
 </details>
 
 ---
 
 ### Soal 12: Paradoks Kasta Campuran
 ```cpp
 int x = 10;
 double d = 3.0;
 int res = x / d + (int)(x / d);
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`? (Hati-hati dengan tipe sasarannya).
 2. Mengapa di langkah pertama hasilnya tampak pecah tapi di akhir tetap bulat?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 10.0 (Karena promosi kasta).
 - `res` = 6.
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Operasi 1 (`x / d`)**: `10 / 3.0`. Karena ada `double`, robot menghitung secara presisi: **3.333333...**.
 2. **Operasi 2 (`(int)(x / d)`)**: Hasil `3.333...` tadi dipaksa masuk ke loker `int`. Koma dipotong paksa. Hasilnya: **3**.
 3. **Penjumlahan**: `3.333... + 3` = **6.333333...**.
 4. **Penyimpanan Akhir**: Hasil `6.333...` dipaksa masuk ke loker `int res`. Koma kembali dipangkas. Hasil akhir: **6**.
 
 **Jawaban Akhir: 6**
 </details>
 
 ---
 
 ### Soal 13: Logika Peluru (Short-Circuit)
 ```cpp
 int x = 5;
 bool cek = (x < 10) || (++x > 10);
 ```
 **Pertanyaan:**
 1. Berapakah isi laci `x` sekarang? (Apakah jadi 6 atau tetap 5?)
 2. Apa yang dimaksud dengan "Short-Circuit" dalam logika robot?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `x` = 5.
 - `cek` = 1 (True).
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mulai memeriksa syarat pertama: `x < 10` (5 < 10). Hasilnya **BENAR / TRUE**.
 2. Robot melihat operator `||` (Atau). Sifat `||` adalah: "Asal ada satu yang Benar, maka semuanya dianggap Benar."
 3. Karena syarat pertama sudah Benar, robot menjadi **MALAS**. Ia merasa tidak perlu lagi mengecek syarat kedua (`++x > 10`).
 4. Perintah `++x` **TIDAK PERNAH DIJALANKAN**. Nilai `x` tetap di angka **5**.
 
 **Jawaban Akhir: x = 5**
 </details>
 
 ---
 
 ### Soal 14: Labirin ASCII (Cipher Offset)
 ```cpp
 char c = 'a'; // ASCII 97
 int offset = 32;
 char res = c - offset;
 ```
 **Pertanyaan:**
 1. Karakter apakah yang tersimpan di dalam `res`?
 2. Mengapa angka **32** disebut angka "Pintu Gerbang" antara huruf besar dan kecil?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `c` = 97 ('a').
 - `res` = 65 ('A').
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Robot mengambil nilai ASCII `'a'` (97).
 2. Dikurangi 32: $97 - 32 = 65$.
 3. Di dalam tabel C++, angka 65 adalah kode sakral untuk huruf besar **'A'**.
 
 **Jawaban Akhir: 'A'**
 **Penjelasan:** Jarak antara `'a'` dan `'A'` adalah tepat 32 sel. Trik ini sering dipakai untuk mengubah huruf besar-kecil secara manual tanpa `toupper()`.
 </details>
 
 ---
 
 ### Soal 15: Peti Kemas Bocor (Overflow Multiplication)
 ```cpp
 int n = 1000000;
 long long luas = n * n;
 ```
 **Pertanyaan:**
 1. Berapakah nilai dari `luas`? (Harusnya satu triliun, tapi apakah benar?)
 2. Bagaimana cara paling "Expert" untuk memperbaikinya?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📦 Isi Laci Memori:**
 - `luas` = -727379968 (Angka Sampah/Overflow).
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `n` dan `n` adalah tipe `int`. Robot menghitung perkalian $10^6 \times 10^6 = 10^{12}$ (1 Triliun).
 2. Namun, robot menghitungnya di area "Loker Semen" (`int`) yang cuma muat 2 Miliar. Akibatnya, angkanya meluap berantakan.
 3. Setelah hancur (overflow), baru robot menaruhnya ke `long long luas`. Robot hanya melihat rongsokan angka sisa overflow tadi.
 
 **Jawaban Akhir: -727379968 (Atau angka sampah lainnya)**
 **Solusi Expert:** `long long luas = 1LL * n * n;` (Gunakan `1LL` agar robot berhitung di skala raksasa sejak detik pertama).
 </details>
 
 ---
 
 ### Soal 16: Pre vs Post Level Up (State Change)
 ```cpp
 int skor = 10;
 int hasil = (skor++) + (++skor) + skor;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `hasil`?
 2. Berapakah nilai `skor` di garis garis akhir? (Waspadai pemanggilan variabel yang sama berkali-kali).
 
 <details>
 <summary><b>Diagnosis Logika Sang Juara</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Awalnya `skor = 10`.
 2. **Bagian 1 (`skor++`)**: Robot mengambil angka **10**. Baru setelah ini `skor` naik jadi 11.
 3. **Bagian 2 (`++skor`)**: Robot menaikkan `skor` dulu dari 11 menjadi **12**. Baru setelah ini angka 12 diambil.
 4. **Bagian 3 (`skor`)**: Nilai `skor` sekarang sudah resmi **12**.
 5. Total: `10 + 12 + 12 = 34`.
 
 **Jawaban Akhir: 34**
 </details>
 
 ---
 
 ### Soal 17: Keajaiban Kompresi (Shift Right)
 ```cpp
 int x = 100;
 int hasil = x >> 2;
 ```
 **Pertanyaan:**
 1. Berapakah isi laci `hasil`?
 2. Apa ekuivalen matematika sederhana dari `x >> 2`?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. `x >> 1` artinya dibagi 2 sekali.
 2. `x >> 2` artinya dibagi 2 sebanyak **Dua Kali**.
 3. Langkah 1: $100 \div 2 = 50$.
 4. Langkah 2: $50 \div 2 = 25$.
 
 **Jawaban Akhir: 25**
 </details>
 
 ---
 
 ### Soal 18: Bayangan Global & Init 0
 ```cpp
 int poin; // GLOBAL
 
 int main() {
     poin++;
     int poin = 10; // LOKAL
     poin++;
     printf("%d ", poin);
 }
 ```
 **Pertanyaan:**
 1. Apa yang tercetak di layar?
 2. Mengapa tidak ada error meskipun nama variabelnya sama?
 
 <details>
 <summary><b>Diagnosis Wilayah Kekuasaan</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Laci Global `poin` otomatis berisi **0**.
 2. Perintah `poin++` pertama beraksi pada variabel Global (0 naik jadi 1).
 3. Lalu dibentuk variabel Lokal `poin = 10`. Robot terdekat lebih berkuasa!
 4. Perintah `poin++` kedua beraksi pada variabel Lokal (10 naik jadi 11).
 5. Cetak: **11**.
 
 **Jawaban Akhir: 11**
 </details>
 
 ---
 
 ### Soal 19: Teka-Teki Modulo Negatif
 ```cpp
 int a = -7;
 int b = 3;
 int res = a % b;
 ```
 **Pertanyaan:**
 1. Berapakah nilai `res`? (Apakah 2 atau -1?)
 2. Mengapa di C++ tanda modulo mengikuti angka di sebelah kiri?
 
 <details>
 <summary><b>Isi Laci Memori & Diagnosis Logika</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. Di kodingan C++, tanda dari hasil modulo **SELALU** mengikuti tanda dari angka puncaknya (sebelah kiri).
 2. Abaikan tanda minus dulu: `7 % 3 = 1`.
 3. Kembalikan tanda minusnya: **-1**.
 
 **Jawaban Akhir: -1**
 </details>
 
 ---
 
 ### Soal 20: THE LEGEND - The Human Compiler Boss
 ```cpp
 char huruf = 'B'; 
 int x = 1LL * 1000000 * 1000000 / 1e11; 
 double d = 0.5;
 int out = (huruf - 'A') * (x + d) + (5 % 2);
 ```
 **Pertanyaan:**
 1. Berapakah nilai akhir `out`?
 2. Berapakah nilai `x` yang sebenarnya?
 
 <details>
 <summary><b>Diagnosis Logika Legenda</b></summary>
 
 **📖 Diagnosis Logika (Step-by-Step):**
 1. **Hitung x**: $10^{12}$ (1 Triliun) dibagi $10^{11}$ (100 Miliar) = **10**.
 2. **Hitung out**:
    - `(huruf - 'A')` $\rightarrow (66 - 65) = 1$.
    - `(x + d)` $\rightarrow (10 + 0.5) = 10.5$.
    - `(5 % 2)` $\rightarrow$ sisa bagi 5 oleh 2 adalah **1**.
    - Rumus: `1 * 10.5 + 1` = **11.5**.
 3. **Penyimpanan**: Dimasukkan ke `int out`, maka koma hangus. Hasil akhir **11**.
 
 **Jawaban Akhir: 11 (x = 10)**
 </details>
 
 ---
 
 🔙 **[Kembali ke Daftar Latihan](../README.md)**
 ⏩ **Lanjut ke Latihan Percabangan: [Set 02](../../02-percabangan/latihan/README.md)**
