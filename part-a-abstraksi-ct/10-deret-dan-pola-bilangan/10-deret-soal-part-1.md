🔙 **Kembali ke Materi:** [Materi 10 Deret Dan Pola Bilangan](../10-deret-dan-pola-bilangan.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 10. Deret & Pola Bilangan - Latihan Soal Pilihan Ganda Bagian 1
## Topik: Ilmu Titen (Mengenali Pola Rahasia Dasar)

[< Kembali ke Indeks](../10-deret-dan-pola-bilangan.md) | [Bagian 2 >](./10-deret-soal-part-2.md)

---

### Soal #1: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`-1, 2, 7, 14, 23, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-8?

A. 64
B. 79
C. 47
D. 62
E. 39


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 62**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran - 2).
   - Suku 1: $1^2 - 2 = -1$
   - Suku 2: $2^2 - 2 = 2$
   - Suku 3: $3^2 - 2 = 7$
3. Pola rumus pastinya adalah: $U_n = n^2 - 2$.
4. Menghitung suku ke-8:
   $U_{8} = 8^2 - 2$
   $U_{8} = 64 - 2 = $ **62**.

</details>

### Soal #2: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`3, 9, 27, 81, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 2187
B. 729
C. 243
D. 162
E. 726


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 729**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 9 / 3 = 3
   - 27 / 9 = 3
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 3**.
3. Artinya ini adalah Deret Geometri dengan rasio 3, atau pola Pangkat dari 3.
   - Fase 1: $3^1$ = 3
   - Fase 2: $3^2$ = 9...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 3:
   $Fase_{6} = 3^6 = $ **729**.

</details>

### Soal #3: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`4, 7, 12, 19, 28, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-9?

A. 103
B. 67
C. 46
D. 84
E. 81


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 3).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 84**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **3** (mengalami pergeseran + 3).
   - Suku 1: $1^2 + 3 = 4$
   - Suku 2: $2^2 + 3 = 7$
   - Suku 3: $3^2 + 3 = 12$
3. Pola rumus pastinya adalah: $U_n = n^2 + 3$.
4. Menghitung suku ke-9:
   $U_{9} = 9^2 + 3$
   $U_{9} = 81 + 3 = $ **84**.

</details>

### Soal #4: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`2, 5, 7, 12, 19, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 38
B. 31
C. 32
D. 228
E. 26


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 31**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 5-2=3, 7-5=2. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 2 + 5 = 7 (Suku 3)
   - Suku 2 + Suku 3 = 5 + 7 = 12 (Suku 4)
   - Suku 3 + Suku 4 = 7 + 12 = 19 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 12 + 19 = **31**.

</details>

### Soal #5: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 64
B. 54
C. 62
D. 128
E. 32


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #6: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`4, 4, 8, 12, 20, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 40
B. 33
C. 32
D. 28
E. 240


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 32**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 4-4=0, 8-4=4. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 4 + 4 = 8 (Suku 3)
   - Suku 2 + Suku 3 = 4 + 8 = 12 (Suku 4)
   - Suku 3 + Suku 4 = 8 + 12 = 20 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 12 + 20 = **32**.

</details>

### Soal #7: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`0, 3, 8, 15, 24, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-7?

A. 48
B. 38
C. 35
D. 49
E. 63


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 1).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 48**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **1** (mengalami pergeseran - 1).
   - Suku 1: $1^2 - 1 = 0$
   - Suku 2: $2^2 - 1 = 3$
   - Suku 3: $3^2 - 1 = 8$
3. Pola rumus pastinya adalah: $U_n = n^2 - 1$.
4. Menghitung suku ke-7:
   $U_{7} = 7^2 - 1$
   $U_{7} = 49 - 1 = $ **48**.

</details>

### Soal #8: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`3, 9, 27, 81, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 726
B. 2187
C. 162
D. 729
E. 243


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 729**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 9 / 3 = 3
   - 27 / 9 = 3
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 3**.
3. Artinya ini adalah Deret Geometri dengan rasio 3, atau pola Pangkat dari 3.
   - Fase 1: $3^1$ = 3
   - Fase 2: $3^2$ = 9...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 3:
   $Fase_{6} = 3^6 = $ **729**.

</details>

### Soal #9: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`2, 6, 8, 14, 22, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 308
B. 37
C. 44
D. 30
E. 36


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 36**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 6-2=4, 8-6=2. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 2 + 6 = 8 (Suku 3)
   - Suku 2 + Suku 3 = 6 + 8 = 14 (Suku 4)
   - Suku 3 + Suku 4 = 8 + 14 = 22 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 14 + 22 = **36**.

</details>

### Soal #10: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 128
B. 62
C. 32
D. 66
E. 64


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #11: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`4, 3, 7, 10, 17, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 28
B. 170
C. 24
D. 34
E. 27


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 27**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 3-4=-1, 7-3=4. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 4 + 3 = 7 (Suku 3)
   - Suku 2 + Suku 3 = 3 + 7 = 10 (Suku 4)
   - Suku 3 + Suku 4 = 7 + 10 = 17 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 10 + 17 = **27**.

</details>

### Soal #12: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`-1, 2, 7, 14, 23, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-9?

A. 98
B. 41
C. 79
D. 81
E. 62


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 79**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran - 2).
   - Suku 1: $1^2 - 2 = -1$
   - Suku 2: $2^2 - 2 = 2$
   - Suku 3: $3^2 - 2 = 7$
3. Pola rumus pastinya adalah: $U_n = n^2 - 2$.
4. Menghitung suku ke-9:
   $U_{9} = 9^2 - 2$
   $U_{9} = 81 - 2 = $ **79**.

</details>

### Soal #13: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`3, 9, 27, 81, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 2187
B. 729
C. 243
D. 726
E. 162


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 729**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 9 / 3 = 3
   - 27 / 9 = 3
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 3**.
3. Artinya ini adalah Deret Geometri dengan rasio 3, atau pola Pangkat dari 3.
   - Fase 1: $3^1$ = 3
   - Fase 2: $3^2$ = 9...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 3:
   $Fase_{6} = 3^6 = $ **729**.

</details>

### Soal #14: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`3, 5, 8, 13, 21, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 42
B. 35
C. 34
D. 29
E. 273


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 34**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 5-3=2, 8-5=3. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 3 + 5 = 8 (Suku 3)
   - Suku 2 + Suku 3 = 5 + 8 = 13 (Suku 4)
   - Suku 3 + Suku 4 = 8 + 13 = 21 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 13 + 21 = **34**.

</details>

### Soal #15: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`3, 6, 11, 18, 27, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-12?

A. 146
B. 51
C. 123
D. 144
E. 171


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 146**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran + 2).
   - Suku 1: $1^2 + 2 = 3$
   - Suku 2: $2^2 + 2 = 6$
   - Suku 3: $3^2 + 2 = 11$
3. Pola rumus pastinya adalah: $U_n = n^2 + 2$.
4. Menghitung suku ke-12:
   $U_{12} = 12^2 + 2$
   $U_{12} = 144 + 2 = $ **146**.

</details>

### Soal #16: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 64
B. 62
C. 65
D. 32
E. 128


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #17: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 32
B. 54
C. 62
D. 128
E. 64


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #18: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`3, 6, 9, 15, 24, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 33
B. 40
C. 39
D. 48
E. 360


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 39**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 6-3=3, 9-6=3. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 3 + 6 = 9 (Suku 3)
   - Suku 2 + Suku 3 = 6 + 9 = 15 (Suku 4)
   - Suku 3 + Suku 4 = 9 + 15 = 24 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 15 + 24 = **39**.

</details>

### Soal #19: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 128
B. 62
C. 64
D. 59
E. 32


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #20: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`1, 2, 3, 5, 8, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 40
B. 13
C. 16
D. 14
E. 11


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 13**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 2-1=1, 3-2=1. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 1 + 2 = 3 (Suku 3)
   - Suku 2 + Suku 3 = 2 + 3 = 5 (Suku 4)
   - Suku 3 + Suku 4 = 3 + 5 = 8 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 5 + 8 = **13**.

</details>

### Soal #21: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 32
B. 128
C. 62
D. 66
E. 64


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #22: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`2, 5, 10, 17, 26, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-10?

A. 82
B. 101
C. 46
D. 100
E. 122


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 1).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 101**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **1** (mengalami pergeseran + 1).
   - Suku 1: $1^2 + 1 = 2$
   - Suku 2: $2^2 + 1 = 5$
   - Suku 3: $3^2 + 1 = 10$
3. Pola rumus pastinya adalah: $U_n = n^2 + 1$.
4. Menghitung suku ke-10:
   $U_{10} = 10^2 + 1$
   $U_{10} = 100 + 1 = $ **101**.

</details>

### Soal #23: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`4, 7, 12, 19, 28, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-10?

A. 100
B. 124
C. 48
D. 84
E. 103


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 3).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 103**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **3** (mengalami pergeseran + 3).
   - Suku 1: $1^2 + 3 = 4$
   - Suku 2: $2^2 + 3 = 7$
   - Suku 3: $3^2 + 3 = 12$
3. Pola rumus pastinya adalah: $U_n = n^2 + 3$.
4. Menghitung suku ke-10:
   $U_{10} = 10^2 + 3$
   $U_{10} = 100 + 3 = $ **103**.

</details>

### Soal #24: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 128
B. 32
C. 66
D. 64
E. 62


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #25: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`1, 4, 5, 9, 14, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 126
B. 24
C. 28
D. 19
E. 23


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 23**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 4-1=3, 5-4=1. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 1 + 4 = 5 (Suku 3)
   - Suku 2 + Suku 3 = 4 + 5 = 9 (Suku 4)
   - Suku 3 + Suku 4 = 5 + 9 = 14 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 9 + 14 = **23**.

</details>

### Soal #26: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 32
B. 66
C. 62
D. 64
E. 128


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #27: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`0, 3, 8, 15, 24, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-11?

A. 46
B. 99
C. 120
D. 121
E. 143


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 1).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 120**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **1** (mengalami pergeseran - 1).
   - Suku 1: $1^2 - 1 = 0$
   - Suku 2: $2^2 - 1 = 3$
   - Suku 3: $3^2 - 1 = 8$
3. Pola rumus pastinya adalah: $U_n = n^2 - 1$.
4. Menghitung suku ke-11:
   $U_{11} = 11^2 - 1$
   $U_{11} = 121 - 1 = $ **120**.

</details>

### Soal #28: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`3, 6, 11, 18, 27, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-8?

A. 64
B. 66
C. 43
D. 51
E. 83


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 66**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran + 2).
   - Suku 1: $1^2 + 2 = 3$
   - Suku 2: $2^2 + 2 = 6$
   - Suku 3: $3^2 + 2 = 11$
3. Pola rumus pastinya adalah: $U_n = n^2 + 2$.
4. Menghitung suku ke-8:
   $U_{8} = 8^2 + 2$
   $U_{8} = 64 + 2 = $ **66**.

</details>

### Soal #29: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`3, 2, 5, 7, 12, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 17
B. 20
C. 24
D. 19
E. 84


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 19**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 2-3=-1, 5-2=3. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 3 + 2 = 5 (Suku 3)
   - Suku 2 + Suku 3 = 2 + 5 = 7 (Suku 4)
   - Suku 3 + Suku 4 = 5 + 7 = 12 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 7 + 12 = **19**.

</details>

### Soal #30: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 32
B. 59
C. 62
D. 64
E. 128


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #31: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`4, 7, 12, 19, 28, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-9?

A. 84
B. 67
C. 103
D. 46
E. 81


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 3).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 84**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **3** (mengalami pergeseran + 3).
   - Suku 1: $1^2 + 3 = 4$
   - Suku 2: $2^2 + 3 = 7$
   - Suku 3: $3^2 + 3 = 12$
3. Pola rumus pastinya adalah: $U_n = n^2 + 3$.
4. Menghitung suku ke-9:
   $U_{9} = 9^2 + 3$
   $U_{9} = 81 + 3 = $ **84**.

</details>

### Soal #32: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`3, 2, 5, 7, 12, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 19
B. 17
C. 24
D. 84
E. 20


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 19**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 2-3=-1, 5-2=3. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 3 + 2 = 5 (Suku 3)
   - Suku 2 + Suku 3 = 2 + 5 = 7 (Suku 4)
   - Suku 3 + Suku 4 = 5 + 7 = 12 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 7 + 12 = **19**.

</details>

### Soal #33: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`0, 3, 8, 15, 24, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-9?

A. 99
B. 81
C. 42
D. 63
E. 80


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 1).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 80**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **1** (mengalami pergeseran - 1).
   - Suku 1: $1^2 - 1 = 0$
   - Suku 2: $2^2 - 1 = 3$
   - Suku 3: $3^2 - 1 = 8$
3. Pola rumus pastinya adalah: $U_n = n^2 - 1$.
4. Menghitung suku ke-9:
   $U_{9} = 9^2 - 1$
   $U_{9} = 81 - 1 = $ **80**.

</details>

### Soal #34: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 32
B. 128
C. 64
D. 74
E. 62


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #35: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 128
B. 64
C. 32
D. 60
E. 62


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #36: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`-2, 1, 6, 13, 22, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-11?

A. 121
B. 44
C. 97
D. 141
E. 118


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 3).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 118**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **3** (mengalami pergeseran - 3).
   - Suku 1: $1^2 - 3 = -2$
   - Suku 2: $2^2 - 3 = 1$
   - Suku 3: $3^2 - 3 = 6$
3. Pola rumus pastinya adalah: $U_n = n^2 - 3$.
4. Menghitung suku ke-11:
   $U_{11} = 11^2 - 3$
   $U_{11} = 121 - 3 = $ **118**.

</details>

### Soal #37: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`-1, 2, 7, 14, 23, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-11?

A. 142
B. 98
C. 121
D. 119
E. 45


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 119**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran - 2).
   - Suku 1: $1^2 - 2 = -1$
   - Suku 2: $2^2 - 2 = 2$
   - Suku 3: $3^2 - 2 = 7$
3. Pola rumus pastinya adalah: $U_n = n^2 - 2$.
4. Menghitung suku ke-11:
   $U_{11} = 11^2 - 2$
   $U_{11} = 121 - 2 = $ **119**.

</details>

### Soal #38: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`-1, 2, 7, 14, 23, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-8?

A. 47
B. 39
C. 79
D. 62
E. 64


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di- 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 62**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran - 2).
   - Suku 1: $1^2 - 2 = -1$
   - Suku 2: $2^2 - 2 = 2$
   - Suku 3: $3^2 - 2 = 7$
3. Pola rumus pastinya adalah: $U_n = n^2 - 2$.
4. Menghitung suku ke-8:
   $U_{8} = 8^2 - 2$
   $U_{8} = 64 - 2 = $ **62**.

</details>

### Soal #39: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`3, 5, 8, 13, 21, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 42
B. 34
C. 35
D. 273
E. 29


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 34**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 5-3=2, 8-5=3. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 3 + 5 = 8 (Suku 3)
   - Suku 2 + Suku 3 = 5 + 8 = 13 (Suku 4)
   - Suku 3 + Suku 4 = 8 + 13 = 21 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 13 + 21 = **34**.

</details>

### Soal #40: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 62
B. 66
C. 64
D. 32
E. 128


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #41: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`4, 2, 6, 8, 14, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 112
B. 23
C. 28
D. 20
E. 22


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 22**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 2-4=-2, 6-2=4. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 4 + 2 = 6 (Suku 3)
   - Suku 2 + Suku 3 = 2 + 6 = 8 (Suku 4)
   - Suku 3 + Suku 4 = 6 + 8 = 14 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 8 + 14 = **22**.

</details>

### Soal #42: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`2, 4, 6, 10, 16, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 27
B. 26
C. 32
D. 22
E. 160


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 26**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 4-2=2, 6-4=2. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 2 + 4 = 6 (Suku 3)
   - Suku 2 + Suku 3 = 4 + 6 = 10 (Suku 4)
   - Suku 3 + Suku 4 = 6 + 10 = 16 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 10 + 16 = **26**.

</details>

### Soal #43: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`4, 7, 12, 19, 28, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-8?

A. 44
B. 67
C. 52
D. 64
E. 84


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 3).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 67**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **3** (mengalami pergeseran + 3).
   - Suku 1: $1^2 + 3 = 4$
   - Suku 2: $2^2 + 3 = 7$
   - Suku 3: $3^2 + 3 = 12$
3. Pola rumus pastinya adalah: $U_n = n^2 + 3$.
4. Menghitung suku ke-8:
   $U_{8} = 8^2 + 3$
   $U_{8} = 64 + 3 = $ **67**.

</details>

### Soal #44: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`2, 5, 10, 17, 26, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-12?

A. 145
B. 170
C. 144
D. 122
E. 50


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 1).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 145**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **1** (mengalami pergeseran + 1).
   - Suku 1: $1^2 + 1 = 2$
   - Suku 2: $2^2 + 1 = 5$
   - Suku 3: $3^2 + 1 = 10$
3. Pola rumus pastinya adalah: $U_n = n^2 + 1$.
4. Menghitung suku ke-12:
   $U_{12} = 12^2 + 1$
   $U_{12} = 144 + 1 = $ **145**.

</details>

### Soal #45: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 128
B. 64
C. 62
D. 32
E. 65


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

### Soal #46: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Diberikan sebuah barisan bilangan rahasia tingkat OSN-K:
`3, 6, 11, 18, 27, ...`
Berdasarkan pola tersebut, berapakah nilai untuk suku ke-11?

A. 123
B. 102
C. 49
D. 146
E. 121


<details><summary>💡 Hint</summary>

Sandingkan deret di atas dengan deret Kuadrat Normal murni (1, 4, 9, 16, 25). Pasti kamu melihat pola selisih yang konsisten pada tiap sukunya! (Semuanya selalu di+ 2).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 123**

**Pembahasan Langkah Demi Langkah:**
1. Ingat kembali deret kuadrat dasar ($n^2$):
   $1^2$=1, $2^2$=4, $3^2$=9, $4^2$=16, $5^2$=25.
2. Jika kita bandingkan deret kuadrat dasar ini dengan deret soal, terdapat selisih persis sebesar **2** (mengalami pergeseran + 2).
   - Suku 1: $1^2 + 2 = 3$
   - Suku 2: $2^2 + 2 = 6$
   - Suku 3: $3^2 + 2 = 11$
3. Pola rumus pastinya adalah: $U_n = n^2 + 2$.
4. Menghitung suku ke-11:
   $U_{11} = 11^2 + 2$
   $U_{11} = 121 + 2 = $ **123**.

</details>

### Soal #47: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`4, 2, 6, 8, 14, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 28
B. 22
C. 20
D. 112
E. 23


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 22**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 2-4=-2, 6-2=4. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 4 + 2 = 6 (Suku 3)
   - Suku 2 + Suku 3 = 2 + 6 = 8 (Suku 4)
   - Suku 3 + Suku 4 = 6 + 8 = 14 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 8 + 14 = **22**.

</details>

### Soal #48: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Perhatikan deret bilangan berikut:
`2, 6, 8, 14, 22, ...`
Berapakah angka selanjutnya pada deret tersebut?

A. 36
B. 30
C. 308
D. 37
E. 44


<details><summary>💡 Hint</summary>

Ilmu Titen Fibonacci: Pola ini terbentuk bukan dari perkalian, melainkan menjumlahkan dua angka terakhirnya secara beruntun.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 36**

**Pembahasan Langkah Demi Langkah:**
1. Kita cek selisihnya: 6-2=4, 8-6=2. Selisih tidak konstan.
2. Coba kita jumlahkan dua bilangan berturut-turut:
   - Suku 1 + Suku 2 = 2 + 6 = 8 (Suku 3)
   - Suku 2 + Suku 3 = 6 + 8 = 14 (Suku 4)
   - Suku 3 + Suku 4 = 8 + 14 = 22 (Suku 5)
3. Ketemu polanya! (Ini adalah Logika Fibonacci).
4. Maka Angka ke-6 = Suku 4 + Suku 5 = 14 + 22 = **36**.

</details>

### Soal #49: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`3, 9, 27, 81, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 2187
B. 729
C. 162
D. 726
E. 243


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 729**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 9 / 3 = 3
   - 27 / 9 = 3
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 3**.
3. Artinya ini adalah Deret Geometri dengan rasio 3, atau pola Pangkat dari 3.
   - Fase 1: $3^1$ = 3
   - Fase 2: $3^2$ = 9...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 3:
   $Fase_{6} = 3^6 = $ **729**.

</details>

### Soal #50: Pilihan Ganda - Ilmu Titen (Pola Bilangan)
Sebuah virus komputer menginfeksi jaringan dengan pola pembelahan:
`2, 4, 8, 16, ...`
Jika pola ini tidak dihentikan, berapakah jumlah virus pada Fase ke-6?

A. 65
B. 62
C. 64
D. 128
E. 32


<details><summary>💡 Hint</summary>

Deret ini bukan ditambah, melainkan SELALU DIKALI dengan bilangan yang sama setiap angkanya maju satu langkah (Pola Pangkat/Eksponensial).

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 64**

**Pembahasan Langkah Demi Langkah:**
1. Temukan polanya dengan membagi angka belakang dan depan:
   - 4 / 2 = 2
   - 8 / 4 = 2
2. Ternyata setiap kali berpindah, angkanya **selalu dikali 2**.
3. Artinya ini adalah Deret Geometri dengan rasio 2, atau pola Pangkat dari 2.
   - Fase 1: $2^1$ = 2
   - Fase 2: $2^2$ = 4...
4. Menghitung Fase ke-6 berarti mencari pangkat 6 dari basis 2:
   $Fase_{6} = 2^6 = $ **64**.

</details>

---
[< Kembali ke Indeks](../10-deret-dan-pola-bilangan.md) | [Bagian 2 >](./10-deret-soal-part-2.md)
