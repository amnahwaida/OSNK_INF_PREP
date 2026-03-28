# Latihan Modul 08: Advanced Vector & Algos (Set 02)
 
 [< Kembali ke Materi](../materi.md)
 
 ## 📋 Petunjuk:
 - Set ini berisi soal-soal tingkat lanjut yang muncul di OSN-K 2022-2024.
 - Gunakan intuisi algoritme (Binary Search, Two-Pointers) untuk mempercepat tracing.
 
 ---
 
 ### Soal 1 (Binary Search Tracing)
 ```cpp
 vector<int> A = {2, 4, 6, 8, 10, 12, 14};
 int L = 0, R = 6, X = 10;
 int mid;
 while (L <= R) {
     mid = (L + R) / 2;
     if (A[mid] == X) break;
     if (A[mid] < X) L = mid + 1;
     else R = mid - 1;
 }
 cout << mid;
 ```
 **Pertanyaan:** Berapa nilai `mid` saat loop berhenti?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **4**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. **Data:** `A = {2, 4, 6, 8, 10, 12, 14}`, Target `X = 10`.
 2. **Iterasi 1:** `L=0, R=6`. `mid = (0+6)/2 = 3`. 
    - `A[3]` adalah 8. Karena 8 < 10, maka `L = 3 + 1 = 4`.
 3. **Iterasi 2:** `L=4, R=6`. `mid = (4+6)/2 = 5`.
    - `A[5]` adalah 12. Karena 12 > 10, maka `R = 5 - 1 = 4`.
 4. **Iterasi 3:** `L=4, R=4`. `mid = (4+4)/2 = 4`.
    - `A[4]` adalah 10. **Cocok!** Loop berhenti (`break`).
 5. **Hasil Akhir:** **4**.
 </details>
 
 ---
 
 ### Soal 2 (Complexity Scaling - OSNK 2024 Style)
 Sebuah fungsi Binary Search membutuhkan waktu **10 detik** untuk memproses $N=1000$ data. Untuk $N=2000$, waktunya menjadi **11 detik**. Berapa estimasi waktu yang dibutuhkan untuk $N=8000$?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **13**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Ini adalah pola **Logaritma**. Setiap kali $N$ dikali 2, waktu bertambah secara konstan (dalam hal ini +1 detik).
 2. $N=1000 \rightarrow 10s$
 3. $N=2000 \rightarrow 11s$ (+1 detik)
 4. $N=4000 \rightarrow 12s$ (+1 detik)
 5. $N=8000 \rightarrow 13s$ (+1 detik)
 6. **Hasil Akhir:** **13**.
 </details>
 
 ---
 
 ### Soal 3 (Two-Pointers Merge)
 ```cpp
 vector<int> A = {1, 5}, B = {2, 4};
 vector<int> C;
 int i = 0, j = 0;
 while (i < 2 && j < 2) {
     if (A[i] < B[j]) { C.push_back(A[i]); i++; }
     else { C.push_back(B[j]); j++; }
 }
 cout << C[1];
 ```
 **Pertanyaan:** Apa isi `C[1]`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **2**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `i=0 (1), j=0 (2)`: 1 < 2 $\rightarrow$ `C = [1]`, `i=1`.
 2. `i=1 (5), j=0 (2)`: 5 > 2 $\rightarrow$ `C = [1, 2]`, `j=1`.
 3. `C[1]` adalah elemen kedua, yaitu **2**.
 4. **Hasil Akhir:** **2**.
 </details>
 
 ---
 
 ### Soal 4 (Number Theory: Digit Sum)
 ```cpp
 int n = 2024, res = 0;
 while (n > 0) {
     if ((n % 10) % 2 == 0) res += (n % 10);
     n /= 10;
 }
 cout << res;
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **6**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Program menjumlahkan digit yang **genap**.
 2. Digit dari 2024 adalah 2, 0, 2, 4.
 3. Semuanya genap: `4 + 2 + 0 + 2 = 8`.
 4. **Tunggu!** Mari kita telusuri urutannya:
    - Step 1: `n%10 = 4`. Genap? Ya. `res = 4`. `n = 202`.
    - Step 2: `n%10 = 2`. Genap? Ya. `res = 4 + 2 = 6`. `n = 20`.
    - Step 3: `n%10 = 0`. Genap? Ya. `res = 6 + 0 = 6`. `n = 2`.
    - Step 4: `n%10 = 2`. Genap? Ya. `res = 6 + 2 = 8`. `n = 0`.
 5. **Hasil Akhir:** **8**. (Koreksi: 2+0+2+4 = 8).
 </details>
 
 ---
 
 ### Soal 5 (Josephus Pattern - $K=2$)
 ```cpp
 int f(int n) {
     if (n == 1) return 1;
     return (f(n-1) + 2 - 1) % n + 1;
 }
 ```
 **Pertanyaan:** Berapa hasil `f(5)`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **3**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Ini pola Josephus $K=2$.
 2. Rumus praktis untuk $K=2$: Cari pangkat 2 terbesar ($2^m$) yang $\le n$. Hasilnya adalah $2(n - 2^m) + 1$.
 3. Untuk $n=5$, pangkat 2 terbesarnya adalah $4$ ($2^2$).
 4. Hasil $= 2(5 - 4) + 1 = 2(1) + 1 = 3$.
 5. **Hasil Akhir:** **3**.
 </details>
 
 ---
 
 ### Soal 6 (Nested 2D Vector)
 ```cpp
 vector<vector<int>> M = {{1, 2, 3}, {4, 5, 6}};
 int ans = 0;
 for (int i = 0; i < M.size(); i++) {
     ans += M[i][M[i].size() - 1];
 }
 cout << ans;
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **9**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Loop menjumlahkan elemen paling belakang dari setiap baris.
 2. Baris 0: Elemen terakhir adalah 3.
 3. Baris 1: Elemen terakhir adalah 6.
 4. `3 + 6 = 9`.
 5. **Hasil Akhir:** **9**.
 </details>
 
 ---
 
 ### Soal 7 (Two-Pointers Competition)
 ```cpp
 vector<int> A = {1, 10, 100}, B = {5, 50, 500};
 int i = 0, j = 0, count = 0;
 while (i < 3 && j < 3) {
     if (A[i] < B[j]) i++;
     else j++;
     count++;
 }
 cout << count;
 ```
 **Pertanyaan:** Berapa kali loop berputar (`count`)?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **5**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. `i=0(1), j=0(5)`: 1 < 5 $\rightarrow$ `i=1, count=1`.
 2. `i=1(10), j=0(5)`: 10 > 5 $\rightarrow$ `j=1, count=2`.
 3. `i=1(10), j=1(50)`: 10 < 50 $\rightarrow$ `i=2, count=3`.
 4. `i=2(100), j=1(50)`: 100 > 50 $\rightarrow$ `j=2, count=4`.
 5. `i=2(100), j=2(500)`: 100 < 500 $\rightarrow$ `i=3, count=5`.
 6. Loop berhenti karena `i` sudah mencapai 3.
 7. **Hasil Akhir:** **5**.
 </details>
 
 ---
 
 ### Soal 8 (Vector Back and Push)
 ```cpp
 vector<int> v = {10};
 for (int i = 0; i < 3; i++) {
     v.push_back(v.back() + 5);
 }
 cout << v[3];
 ```
 **Pertanyaan:** Apa outputnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **25**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. Start: `[10]`
 2. `i=0`: `push(10+5)` $\rightarrow$ `[10, 15]`
 3. `i=1`: `push(15+5)` $\rightarrow$ `[10, 15, 20]`
 4. `i=2`: `push(20+5)` $\rightarrow$ `[10, 15, 20, 25]`
 5. `v[3]` (indeks 3) adalah **25**.
 6. **Hasil Akhir:** **25**.
 </details>
 
 ---
 
 ### Soal 9 (Binary Search Boundary)
 ```cpp
 vector<int> v = {10, 20, 30, 40, 50};
 int L = 0, R = 4, target = 25, ans = -1;
 while (L <= R) {
     int mid = (L + R) / 2;
     if (v[mid] >= target) { ans = v[mid]; R = mid - 1; }
     else L = mid + 1;
 }
 cout << ans;
 ```
 **Pertanyaan:** Mencari angka terkecil yang $\ge 25$. Apa hasilnya?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **30**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. **Iterasi 1:** `L=0, R=4, mid=2`. `v[2]=30`. Karena 30 $\ge$ 25, `ans=30` dan `R=1`.
 2. **Iterasi 2:** `L=0, R=1, mid=0`. `v[0]=10`. Karena 10 < 25, `L=1`.
 3. **Iterasi 3:** `L=1, R=1, mid=1`. `v[1]=20`. Karena 20 < 25, `L=2`.
 4. Loop berhenti (`L > R`).
 5. **Hasil Akhir:** **30**. (Ini adalah logika `lower_bound`).
 </details>
 
 ---
 
 ### Soal 10 (Final Combination)
 ```cpp
 vector<int> v = {1, 2, 3};
 int n = v.size();
 for (int i = 0; i < n; i++) {
     int temp = v[i];
     while (temp > 0) {
         if (temp % 2 == 1) v.push_back(temp);
         temp /= 2;
     }
 }
 cout << v.size();
 ```
 **Pertanyaan:** Berapa ukuran akhir vector `v`?
 <details>
 <summary>✅ Jawaban & Pembahasan</summary>
 
 **Jawaban:** **7**
 
 **📖 Analisis Mendalam (Step-by-Step):**
 1. **i=0 (temp=1):** 1 % 2 == 1 $\rightarrow$ `push(1)`. `temp=0`. (v = [1, 2, 3, 1])
 2. **i=1 (temp=2):** 
    - 2 % 2 == 0 $\rightarrow$ No. `temp=1`.
    - 1 % 2 == 1 $\rightarrow$ `push(1)`. `temp=0`. (v = [1, 2, 3, 1, 1])
 3. **i=2 (temp=3):** 
    - 3 % 2 == 1 $\rightarrow$ `push(3)`. `temp=1`.
    - 1 % 2 == 1 $\rightarrow$ `push(1)`. `temp=0`. (v = [1, 2, 3, 1, 1, 3, 1])
 4. Loop berhenti karena `i` sudah mencapai `n=3`.
 5. Ukuran akhir `v` adalah **7**.
 6. **Hasil Akhir:** **7**.
 </details>
