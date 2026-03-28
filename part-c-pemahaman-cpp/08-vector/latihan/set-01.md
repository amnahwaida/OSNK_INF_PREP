# Latihan Modul 08: Vector & Matrix 2D (Set 01)
 
 [< Kembali ke Materi](../materi.md)
 
 ## 📋 Petunjuk:
 - Bayangkan `vector` sebagai deretan kotak yang bisa bertambah atau berkurang.
 - Untuk Matriks 2D, bayangkan Baris sebagai 'Lantai' dan Kolom sebagai 'Kamar'.
 - Lacak ukuran `.size()` setiap kali ada perubahan.
 
 ---
 
 ### Soal 1
 ```cpp
 vector<int> v;
 v.push_back(5);
 v.push_back(10);
 v.push_back(15);
 cout << v.size() << " " << v[1];
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **3 10**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `push_back(5)` $\rightarrow$ `v = [5]`, size=1
 2. `push_back(10)` $\rightarrow$ `v = [5, 10]`, size=2
 3. `push_back(15)` $\rightarrow$ `v = [5, 10, 15]`, size=3
 4. `v.size()` bernilai 3. `v[1]` (indeks 1) bernilai 10.
 5. **Hasil Akhir:** **3 10**.
 </details> 
 
 ---
 
 ### Soal 2
 ```cpp
 vector<int> v = {1, 2, 3};
 v.pop_back();
 v.push_back(4);
 v.push_back(5);
 cout << v[2];
 ```
 **Pertanyaan:** Apa isi `v[2]` terakhir?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **4**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Start: `[1, 2, 3]`
 2. `pop_back()` $\rightarrow$ `[1, 2]` (3 dibuang)
 3. `push_back(4)` $\rightarrow$ `[1, 2, 4]`
 4. `push_back(5)` $\rightarrow$ `[1, 2, 4, 5]`
 5. Indeks 2 berisi angka **4** (ingat: 0, 1, 2).
 6. **Hasil Akhir:** **4**.
 </details>
 
 ---
 
 ### Soal 3
 ```cpp
 vector<int> v;
 for (int i = 1; i <= 4; i++) {
     v.push_back(i * 2);
 }
 cout << v[0] + v[3];
 ```
 **Pertanyaan:** Berapa hasil penjumlahannya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **10**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Loop `i=1`: `push_back(2)` $\rightarrow$ `v = [2]`
 2. `i=2`: `push_back(4)` $\rightarrow$ `v = [2, 4]`
 3. `i=3`: `push_back(6)` $\rightarrow$ `v = [2, 4, 6]`
 4. `i=4`: `push_back(8)` $\rightarrow$ `v = [2, 4, 6, 8]`
 5. `v[0]` = 2, `v[3]` = 8.
 6. `2 + 8 = 10`.
 7. **Hasil Akhir:** **10**.
 </details>
 
 ---
 
 ### Soal 4 (Matrix Indexing)
 ```cpp
 vector<vector<int>> B = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
 cout << B[2][1];
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **8**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `B[2]` $\rightarrow$ Baris indeks 2 (Baris ketiga): `{7, 8, 9}`
 2. `B[2][1]` $\rightarrow$ Kolom indeks 1 dari baris tersebut: **8**.
 3. **Hasil Akhir:** **8**.
 </details>
 
 ---
 
 ### Soal 5
 ```cpp
 vector<int> A = {10, 20};
 vector<int> B = A; // Copy vector
 B.push_back(30);
 cout << A.size() << " " << B.size();
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **2 3**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `B = A` menyalin seluruh isi A ke B. Sekarang mereka punya isi yang sama tapi di lemari berbeda.
 2. `B.push_back(30)` hanya menambah isi di lemari B.
 3. `A` tetap berisi 2 elemen, `B` sekarang berisi 3 elemen.
 4. **Hasil Akhir:** **2 3**. (Kecuali jika pakai referensi `&`, tapi di sini tidak).
 </details>
 
 ---
 
 ### Soal 6 (2D Matrix Traversal)
 ```cpp
 vector<vector<int>> M = {{1, 1}, {2, 2}};
 int sum = 0;
 for (int i = 0; i < 2; i++) {
     for (int j = 0; j < 2; j++) {
         if (i == j) sum += M[i][j];
     }
 }
 cout << sum;
 ```
 **Pertanyaan:** Apa hasil `sum`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **3**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Program ini menjumlahkan elemen diagonal (di mana baris == kolom).
 2. `i=0, j=0`: `M[0][0]` = 1. `sum = 1`
 3. `i=0, j=1`: `i != j`. No.
 4. `i=1, j=0`: `i != j`. No.
 5. `i=1, j=1`: `M[1][1]` = 2. `sum = 1 + 2 = 3`
 6. **Hasil Akhir:** **3**.
 </details>
 
 ---
 
 ### Soal 7 (OSNK 2025 Style)
 ```cpp
 vector<int> v = {10, 5, 20};
 int n = v.size();
 for (int i = 0; i < n; i++) {
     if (v[i] < 15) v.push_back(100);
 }
 cout << v.size();
 ```
 **Pertanyaan:** Berapa ukuran akhir vector `v`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **5**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. **Penting:** Variabel `n` dikunci di awal (`n = v.size()` = 3). Loop hanya akan berputar 3 kali, meskipun isi `v` bertambah.
 2. `i=0`: `v[0]` (10) < 15? **Ya**. `push_back(100)`. (v = [10, 5, 20, 100])
 3. `i=1`: `v[1]` (5) < 15? **Ya**. `push_back(100)`. (v = [10, 5, 20, 100, 100])
 4. `i=2`: `v[2]` (20) < 15? **Tidak**. 
 5. Loop berhenti karena batasnya adalah `n=3`.
 6. Ukuran akhir `v` adalah **5**.
 </details>
 
 ---
 
 ### Soal 8
 ```cpp
 vector<vector<int>> v2d;
 v2d.push_back({1, 2});
 v2d.push_back({3, 4, 5});
 cout << v2d[1].size();
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **3**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `v2d[0]` berisi `{1, 2}`.
 2. `v2d[1]` berisi `{3, 4, 5}`.
 3. Ukuran dari `v2d[1]` adalah 3.
 4. **Hasil Akhir:** **3**. (Vector dalam 2D tidak harus sama ukurannya!).
 </details>
 
 ---
 
 ### Soal 9
 ```cpp
 vector<int> v = {1, 2, 3, 4, 5};
 int res = 0;
 for (int i = 0; i < v.size(); i++) {
     if (i % 2 == 1) res += v[i];
 }
 cout << res;
 ```
 **Pertanyaan:** Apa hasil `res`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **6**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Program ini menjumlahkan elemen dengan **indeks ganjil**.
 2. Indeks ganjil adalah `i=1` (angka 2) dan `i=3` (angka 4).
 3. `2 + 4 = 6`.
 4. **Hasil Akhir:** **6**.
 </details>
 
 ---
 
 ### Soal 10 (Final Boss Tracing)
 ```cpp
 vector<int> v = {1, 2, 3};
 for (int i = 0; i < 2; i++) {
     int x = v.back(); // ambil elemen paling belakang
     v.pop_back();
     v.insert(v.begin(), x); // taruh di paling depan (geser semu)
 }
 cout << v[0];
 ```
 **Pertanyaan:** Apa isi `v[0]` di akhir?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **2**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Operasi ini memindahkan elemen belakang ke depan sebanyak 2 kali.
 2. **Start:** `[1, 2, 3]`
 3. **Putaran 1:** 
    - `x = 3`. 
    - `pop_back` $\rightarrow$ `[1, 2]`.
    - `insert(begin, 3)` $\rightarrow$ `[3, 1, 2]`.
 4. **Putaran 2:** 
    - `x = 2`.
    - `pop_back` $\rightarrow$ `[3, 1]`.
    - `insert(begin, 2)` $\rightarrow$ `[2, 3, 1]`.
 5. `v[0]` sekarang adalah **2**.
 6. **Hasil Akhir:** **2**.
 </details>
