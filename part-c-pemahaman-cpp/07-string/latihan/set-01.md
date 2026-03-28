# Latihan Modul 07: Manipulasi String (Set 01)
 
 [< Kembali ke Materi](../materi.md)
 
 ## 📋 Petunjuk:
 - Gunakan kertas buram untuk menulis indeks (0, 1, 2, ...) di atas setiap huruf.
 - Lacak perubahan karakter satu per satu.
 - Jawablah pertanyaan sebelum membuka kolom jawaban.
 
 ---
 
 ### Soal 1
 ```cpp
 string S = "KOMPUTER";
 cout << S[3] << S[0] << S[7];
 ```
 **Pertanyaan:** Apa output yang dihasilkan?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **PKR**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. **Pemetaan Indeks S:** 
    - `0:K, 1:O, 2:M, 3:P, 4:U, 5:T, 6:E, 7:R`
 2. **Ekstraksi Karakter:**
    - `S[3]` $\rightarrow$ 'P'
    - `S[0]` $\rightarrow$ 'K'
    - `S[7]` $\rightarrow$ 'R'
 3. **Hasil Akhir:** Digabungkan menjadi **PKR**.
 </details>
 
 ---
 
 ### Soal 2
 ```cpp
 string T = "OSN-K";
 for (int i = 0; i < T.length(); i++) {
     if (T[i] == '-') T[i] = '2';
 }
 cout << T;
 ```
 **Pertanyaan:** Apa nilai akhir dari string `T`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **OSN2K**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Loop berjalan dari `i=0` ke `i=4` (panjang "OSN-K" adalah 5).
 2. `i=0, 1, 2`: Karakter 'O', 'S', 'N' tidak sama dengan '-'.
 3. `i=3`: `T[3]` adalah '-'. Syarat `if` terpenuhi. `T[3]` diubah menjadi '2'.
 4. `i=4`: `T[4]` adalah 'K'. Tidak berubah.
 5. **Hasil Akhir:** **OSN2K**.
 </details>
 
 ---
 
 ### Soal 3
 ```cpp
 string S = "MATA";
 string R = "";
 for (int i = S.length() - 1; i >= 0; i--) {
     R += S[i];
 }
 cout << R;
 ```
 **Pertanyaan:** Apa output dari program tersebut?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **ATAM**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `S = "MATA"`, `length = 4`.
 2. Loop berjalan mundur dari `i=3` ke `i=0`.
 3. `i=3`: `R += S[3]` ('A') $\rightarrow$ `R = "A"`
 4. `i=2`: `R += S[2]` ('T') $\rightarrow$ `R = "AT"`
 5. `i=1`: `R += S[1]` ('A') $\rightarrow$ `R = "ATA"`
 6. `i=0`: `R += S[0]` ('M') $\rightarrow$ `R = "ATAM"`
 7. **Hasil Akhir:** **ATAM**.
 </details>
 
 ---
 
 ### Soal 4
 ```cpp
 string S = "INFORMATIKA";
 int counter = 0;
 for (int i = 0; i < S.length(); i++) {
     if (S[i] == 'A' || S[i] == 'I') counter++;
 }
 cout << counter;
 ```
 **Pertanyaan:** Berapa nilai `counter` terakhir?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **4**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Program ini menghitung jumlah huruf 'A' dan 'I' dalam kata "INFORMATIKA".
 2. Penelusuran karakter:
    - `I` (Ya), `N` (No), `F` (No), `O` (No), `R` (No), `M` (No), `A` (Ya), `T` (No), `I` (Ya), `K` (No), `A` (Ya).
 3. Total yang ditemukan: 2 huruf 'A' dan 2 huruf 'I'.
 4. **Hasil Akhir:** **4**.
 </details>
 
 ---
 
 ### Soal 5 (Jebakan OSNK 2025)
 ```cpp
 string S = "BANANA";
 for (int i = 0; i < S.length() - 1; i++) {
     if (S[i] == 'A') S[i+1] = 'O';
 }
 cout << S;
 ```
 **Pertanyaan:** Apa isi string `S` di akhir?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **BAOONO**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `i=0`: `S[0]` ('B') bukan 'A'.
 2. `i=1`: `S[1]` ('A'). Syarat terpenuhi! `S[2]` diubah jadi 'O'. (S menjadi "BAOANA")
 3. `i=2`: `S[2]` sekarang 'O', bukan 'A'.
 4. `i=3`: `S[3]` ('A'). Syarat terpenuhi! `S[4]` diubah jadi 'O'. (S menjadi "BAOANO")
 5. `i=4`: `S[4]` sekarang 'O', bukan 'A'.
 6. **Tunggu!** Mari kita cek ulang dengan teliti:
    - `i=0`: 'B' $\rightarrow$ No.
    - `i=1`: 'A' $\rightarrow$ Yes. `S[2]` jadi 'O'. Kata: `BAOANA`
    - `i=2`: 'O' $\rightarrow$ No.
    - `i=3`: 'A' $\rightarrow$ Yes. `S[4]` jadi 'O'. Kata: `BAOANO`
    - `i=4`: 'N' $\rightarrow$ No. 
 7. **Hasil Akhir:** **BAOANO**. (Catatan: Hati-hati, jika soalnya `S[i] == 'N'`, maka perubahannya akan berantai!).
 </details>
 
 ---
 
 ### Soal 6
 ```cpp
 string S = "ABC";
 string T = "123";
 string res = "";
 for (int i = 0; i < 3; i++) {
     res = res + S[i] + T[2-i];
 }
 cout << res;
 ```
 **Pertanyaan:** Apa output yang dihasilkan?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **A3B2C1**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `i=0`: `res + S[0] + T[2]` $\rightarrow$ `"" + 'A' + '3'` = `"A3"`
 2. `i=1`: `res + S[1] + T[1]` $\rightarrow$ `"A3" + 'B' + '2'` = `"A3B2"`
 3. `i=2`: `res + S[2] + T[0]` $\rightarrow$ `"A3B2" + 'C' + '1'` = `"A3B2C1"`
 4. **Hasil Akhir:** **A3B2C1**.
 </details>
 
 ---
 
 ### Soal 7 (Advanced Pattern)
 ```cpp
 string S = "AAAAA";
 int count = 0;
 for (int i = 0; i < S.length() - 1; i++) {
     if (S[i] == 'A' && S[i+1] == 'A') count++;
 }
 cout << count;
 ```
 **Pertanyaan:** Apa nilai `count` terakhir?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **4**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Loop berjalan dari `i=0` ke `i=3` (length-2).
 2. `i=0`: `S[0]`('A') & `S[1]`('A') $\rightarrow$ `count=1`
 3. `i=1`: `S[1]`('A') & `S[2]`('A') $\rightarrow$ `count=2`
 4. `i=2`: `S[2]`('A') & `S[3]`('A') $\rightarrow$ `count=3`
 5. `i=3`: `S[3]`('A') & `S[4]`('A') $\rightarrow$ `count=4`
 6. **Hasil Akhir:** **4**. 
 </details>
 
 ---
 
 ### Soal 8
 ```cpp
 string S = "toki";
 S[0] = S[0] - 32;
 cout << S;
 ```
 **Pertanyaan:** Apa outputnya? (Hint: 'a' = 97, 'A' = 65)
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **Toki**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Dalam C++, karakter adalah angka. Huruf kecil 't' dikurangi 32 akan menghasilkan padanan huruf besarnya 'T' (karena jarak ASCII antara huruf kecil dan besar adalah konstan 32).
 2. `S[0]` diubah dari 't' menjadi 'T'.
 3. Sisa string tidak berubah.
 4. **Hasil Akhir:** **Toki**.
 </details>
 
 ---
 
 ### Soal 9
 ```cpp
 string S = "12345";
 int sum = 0;
 for (int i = 0; i < S.length(); i++) {
     sum += (S[i] - '0');
 }
 cout << sum;
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **15**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `S[i] - '0'` adalah trik klasik untuk mengubah karakter angka menjadi nilai integer murni.
 2. Loop menjumlahkan: `1 + 2 + 3 + 4 + 5`.
 3. **Hasil Akhir:** **15**.
 </details>
 
 ---
 
 ### Soal 10 (Nested String)
 ```cpp
 string S = "ABC";
 string res = "";
 for (int i = 0; i < S.length(); i++) {
     for (int j = 0; j <= i; j++) {
         res += S[i];
     }
 }
 cout << res;
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **ABBCCC**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `i=0` (A): `j` jalan 1x $\rightarrow$ `res = "A"`
 2. `i=1` (B): `j` jalan 2x (0 dan 1) $\rightarrow$ `res = "ABB"`
 3. `i=2` (C): `j` jalan 3x (0, 1, 2) $\rightarrow$ `res = "ABBCCC"`
 4. **Hasil Akhir:** **ABBCCC**.
 </details>
