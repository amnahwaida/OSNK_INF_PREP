🔙 **Kembali ke Materi:** [Materi 10 Deret Dan Pola Bilangan](../10-deret-dan-pola-bilangan.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 10. Deret & Pola Bilangan - Latihan Soal Pilihan Ganda Bagian 4
## Topik: Sandi Komputer Sigma (Membaca Algoritma For-Loop Tersembunyi)

[< Bagian 3](./10-deret-soal-part-3.md) | [Bagian 5 >](./10-deret-soal-part-5.md)

---

### Soal #151: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (2 * k + 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 62
B. 58
C. 77
D. 120
E. 60


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 60**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 + 3) = 5
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 + 3) = 7
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 + 3) = 9
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 + 3) = 11
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 + 3) = 13
   - k=6 $\rightarrow$ ditambah (2 $\times$ 6 + 3) = 15
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **60**.

</details>

### Soal #152: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{6} (4i - 1)$$

A. 84
B. 78
C. 79
D. 82
E. 105


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 78**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (6).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 1)$.
   - Loop i=1: $(4(1) - 1) = 3$
   - Loop i=2: $(4(2) - 1) = 7$
   - Loop i=3: $(4(3) - 1) = 11$
   - Loop i=4: $(4(4) - 1) = 15$
   - Loop i=5: $(4(5) - 1) = 19$
   - Loop i=6: $(4(6) - 1) = 23$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (7) + (11) + (15) + (19) + (23) = **78**.

</details>

### Soal #153: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (2 * k + 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 72
B. 70
C. 140
D. 68
E. 88


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 70**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 + 2) = 4
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 + 2) = 6
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 + 2) = 8
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 + 2) = 10
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 + 2) = 12
   - k=6 $\rightarrow$ ditambah (2 $\times$ 6 + 2) = 14
   - k=7 $\rightarrow$ ditambah (2 $\times$ 7 + 2) = 16
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **70**.

</details>

### Soal #154: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (5i - 1)$$

A. 71
B. 72
C. 75
D. 99
E. 70


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 70**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(5i - 1)$.
   - Loop i=1: $(5(1) - 1) = 4$
   - Loop i=2: $(5(2) - 1) = 9$
   - Loop i=3: $(5(3) - 1) = 14$
   - Loop i=4: $(5(4) - 1) = 19$
   - Loop i=5: $(5(5) - 1) = 24$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (4) + (9) + (14) + (19) + (24) = **70**.

</details>

### Soal #155: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (2 * k + 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 108
B. 70
C. 52
D. 56
E. 54


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 54**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 + 2) = 4
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 + 2) = 6
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 + 2) = 8
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 + 2) = 10
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 + 2) = 12
   - k=6 $\rightarrow$ ditambah (2 $\times$ 6 + 2) = 14
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **54**.

</details>

### Soal #156: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{6} (2i + 1)$$

A. 48
B. 50
C. 47
D. 42
E. 63


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 48**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (6).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(2i + 1)$.
   - Loop i=1: $(2(1) + 1) = 3$
   - Loop i=2: $(2(2) + 1) = 5$
   - Loop i=3: $(2(3) + 1) = 7$
   - Loop i=4: $(2(4) + 1) = 9$
   - Loop i=5: $(2(5) + 1) = 11$
   - Loop i=6: $(2(6) + 1) = 13$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (5) + (7) + (9) + (11) + (13) = **48**.

</details>

### Soal #157: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (5i + 2)$$

A. 85
B. 117
C. 75
D. 83
E. 90


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 85**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(5i + 2)$.
   - Loop i=1: $(5(1) + 2) = 7$
   - Loop i=2: $(5(2) + 2) = 12$
   - Loop i=3: $(5(3) + 2) = 17$
   - Loop i=4: $(5(4) + 2) = 22$
   - Loop i=5: $(5(5) + 2) = 27$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (7) + (12) + (17) + (22) + (27) = **85**.

</details>

### Soal #158: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (5i - 2)$$

A. 131
B. 140
C. 164
D. 128
E. 126


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 126**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(5i - 2)$.
   - Loop i=1: $(5(1) - 2) = 3$
   - Loop i=2: $(5(2) - 2) = 8$
   - Loop i=3: $(5(3) - 2) = 13$
   - Loop i=4: $(5(4) - 2) = 18$
   - Loop i=5: $(5(5) - 2) = 23$
   - Loop i=6: $(5(6) - 2) = 28$
   - Loop i=7: $(5(7) - 2) = 33$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (8) + (13) + (18) + (23) + (28) + (33) = **126**.

</details>

### Soal #159: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{4} (3i + 1)$$

A. 50
B. 34
C. 33
D. 37
E. 30


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 34**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (4).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(3i + 1)$.
   - Loop i=1: $(3(1) + 1) = 4$
   - Loop i=2: $(3(2) + 1) = 7$
   - Loop i=3: $(3(3) + 1) = 10$
   - Loop i=4: $(3(4) + 1) = 13$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (4) + (7) + (10) + (13) = **34**.

</details>

### Soal #160: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (4i - 3)$$

A. 94
B. 95
C. 120
D. 91
E. 112


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 91**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 3)$.
   - Loop i=1: $(4(1) - 3) = 1$
   - Loop i=2: $(4(2) - 3) = 5$
   - Loop i=3: $(4(3) - 3) = 9$
   - Loop i=4: $(4(4) - 3) = 13$
   - Loop i=5: $(4(5) - 3) = 17$
   - Loop i=6: $(4(6) - 3) = 21$
   - Loop i=7: $(4(7) - 3) = 25$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (1) + (5) + (9) + (13) + (17) + (21) + (25) = **91**.

</details>

### Soal #161: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (3i - 2)$$

A. 35
B. 45
C. 38
D. 37
E. 51


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 35**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(3i - 2)$.
   - Loop i=1: $(3(1) - 2) = 1$
   - Loop i=2: $(3(2) - 2) = 4$
   - Loop i=3: $(3(3) - 2) = 7$
   - Loop i=4: $(3(4) - 2) = 10$
   - Loop i=5: $(3(5) - 2) = 13$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (1) + (4) + (7) + (10) + (13) = **35**.

</details>

### Soal #162: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{6} (4i - 2)$$

A. 84
B. 76
C. 72
D. 98
E. 74


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 72**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (6).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 2)$.
   - Loop i=1: $(4(1) - 2) = 2$
   - Loop i=2: $(4(2) - 2) = 6$
   - Loop i=3: $(4(3) - 2) = 10$
   - Loop i=4: $(4(4) - 2) = 14$
   - Loop i=5: $(4(5) - 2) = 18$
   - Loop i=6: $(4(6) - 2) = 22$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (2) + (6) + (10) + (14) + (18) + (22) = **72**.

</details>

### Soal #163: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (3 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 74
B. 77
C. 100
D. 154
E. 80


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 77**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 - 1) = 2
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 - 1) = 5
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 - 1) = 8
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 - 1) = 11
   - k=5 $\rightarrow$ ditambah (3 $\times$ 5 - 1) = 14
   - k=6 $\rightarrow$ ditambah (3 $\times$ 6 - 1) = 17
   - k=7 $\rightarrow$ ditambah (3 $\times$ 7 - 1) = 20
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **77**.

</details>

### Soal #164: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total = total + (6 * k - 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 104
B. 80
C. 58
D. 52
E. 46


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 52**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (6 $\times$ 1 - 2) = 4
   - k=2 $\rightarrow$ ditambah (6 $\times$ 2 - 2) = 10
   - k=3 $\rightarrow$ ditambah (6 $\times$ 3 - 2) = 16
   - k=4 $\rightarrow$ ditambah (6 $\times$ 4 - 2) = 22
3. Iterasi (Loop) berhenti saat $k=4$ menabrak tembok syarat kondisinya `k <= 4`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **52**.

</details>

### Soal #165: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{4} (4i - 1)$$

A. 36
B. 37
C. 26
D. 55
E. 40


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 36**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (4).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 1)$.
   - Loop i=1: $(4(1) - 1) = 3$
   - Loop i=2: $(4(2) - 1) = 7$
   - Loop i=3: $(4(3) - 1) = 11$
   - Loop i=4: $(4(4) - 1) = 15$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (7) + (11) + (15) = **36**.

</details>

### Soal #166: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (4i - 3)$$

A. 120
B. 91
C. 94
D. 95
E. 112


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 91**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 3)$.
   - Loop i=1: $(4(1) - 3) = 1$
   - Loop i=2: $(4(2) - 3) = 5$
   - Loop i=3: $(4(3) - 3) = 9$
   - Loop i=4: $(4(4) - 3) = 13$
   - Loop i=5: $(4(5) - 3) = 17$
   - Loop i=6: $(4(6) - 3) = 21$
   - Loop i=7: $(4(7) - 3) = 25$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (1) + (5) + (9) + (13) + (17) + (21) + (25) = **91**.

</details>

### Soal #167: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (6 * k - 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 228
B. 154
C. 108
D. 120
E. 114


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 114**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (6 $\times$ 1 - 2) = 4
   - k=2 $\rightarrow$ ditambah (6 $\times$ 2 - 2) = 10
   - k=3 $\rightarrow$ ditambah (6 $\times$ 3 - 2) = 16
   - k=4 $\rightarrow$ ditambah (6 $\times$ 4 - 2) = 22
   - k=5 $\rightarrow$ ditambah (6 $\times$ 5 - 2) = 28
   - k=6 $\rightarrow$ ditambah (6 $\times$ 6 - 2) = 34
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **114**.

</details>

### Soal #168: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total = total + (3 * k - 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 19
B. 22
C. 25
D. 44
E. 35


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 22**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 - 2) = 1
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 - 2) = 4
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 - 2) = 7
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 - 2) = 10
3. Iterasi (Loop) berhenti saat $k=4$ menabrak tembok syarat kondisinya `k <= 4`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **22**.

</details>

### Soal #169: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (2i + 1)$$

A. 34
B. 35
C. 30
D. 37
E. 48


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 35**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(2i + 1)$.
   - Loop i=1: $(2(1) + 1) = 3$
   - Loop i=2: $(2(2) + 1) = 5$
   - Loop i=3: $(2(3) + 1) = 7$
   - Loop i=4: $(2(4) + 1) = 9$
   - Loop i=5: $(2(5) + 1) = 11$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (5) + (7) + (9) + (11) = **35**.

</details>

### Soal #170: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (3 * k + 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 116
B. 91
C. 88
D. 182
E. 94


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 91**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 + 1) = 4
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 + 1) = 7
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 + 1) = 10
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 + 1) = 13
   - k=5 $\rightarrow$ ditambah (3 $\times$ 5 + 1) = 16
   - k=6 $\rightarrow$ ditambah (3 $\times$ 6 + 1) = 19
   - k=7 $\rightarrow$ ditambah (3 $\times$ 7 + 1) = 22
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **91**.

</details>

### Soal #171: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total = total + (5 * k - 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 65
B. 120
C. 60
D. 55
E. 87


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 60**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 - 3) = 2
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 - 3) = 7
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 - 3) = 12
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 - 3) = 17
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 - 3) = 22
3. Iterasi (Loop) berhenti saat $k=5$ menabrak tembok syarat kondisinya `k <= 5`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **60**.

</details>

### Soal #172: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (4i + 2)$$

A. 70
B. 60
C. 74
D. 96
E. 68


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 70**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i + 2)$.
   - Loop i=1: $(4(1) + 2) = 6$
   - Loop i=2: $(4(2) + 2) = 10$
   - Loop i=3: $(4(3) + 2) = 14$
   - Loop i=4: $(4(4) + 2) = 18$
   - Loop i=5: $(4(5) + 2) = 22$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (6) + (10) + (14) + (18) + (22) = **70**.

</details>

### Soal #173: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (4i - 3)$$

A. 49
B. 66
C. 45
D. 48
E. 60


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 45**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i - 3)$.
   - Loop i=1: $(4(1) - 3) = 1$
   - Loop i=2: $(4(2) - 3) = 5$
   - Loop i=3: $(4(3) - 3) = 9$
   - Loop i=4: $(4(4) - 3) = 13$
   - Loop i=5: $(4(5) - 3) = 17$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (1) + (5) + (9) + (13) + (17) = **45**.

</details>

### Soal #174: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (5 * k + 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 166
B. 204
C. 322
D. 161
E. 156


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 161**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 + 3) = 8
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 + 3) = 13
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 + 3) = 18
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 + 3) = 23
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 + 3) = 28
   - k=6 $\rightarrow$ ditambah (5 $\times$ 6 + 3) = 33
   - k=7 $\rightarrow$ ditambah (5 $\times$ 7 + 3) = 38
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **161**.

</details>

### Soal #175: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (6 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 208
B. 322
C. 161
D. 155
E. 167


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 161**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (6 $\times$ 1 - 1) = 5
   - k=2 $\rightarrow$ ditambah (6 $\times$ 2 - 1) = 11
   - k=3 $\rightarrow$ ditambah (6 $\times$ 3 - 1) = 17
   - k=4 $\rightarrow$ ditambah (6 $\times$ 4 - 1) = 23
   - k=5 $\rightarrow$ ditambah (6 $\times$ 5 - 1) = 29
   - k=6 $\rightarrow$ ditambah (6 $\times$ 6 - 1) = 35
   - k=7 $\rightarrow$ ditambah (6 $\times$ 7 - 1) = 41
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **161**.

</details>

### Soal #176: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total = total + (3 * k - 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 38
B. 35
C. 51
D. 32
E. 70


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 35**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 - 2) = 1
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 - 2) = 4
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 - 2) = 7
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 - 2) = 10
   - k=5 $\rightarrow$ ditambah (3 $\times$ 5 - 2) = 13
3. Iterasi (Loop) berhenti saat $k=5$ menabrak tembok syarat kondisinya `k <= 5`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **35**.

</details>

### Soal #177: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (5 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 94
B. 104
C. 198
D. 133
E. 99


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 99**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 - 1) = 4
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 - 1) = 9
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 - 1) = 14
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 - 1) = 19
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 - 1) = 24
   - k=6 $\rightarrow$ ditambah (5 $\times$ 6 - 1) = 29
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **99**.

</details>

### Soal #178: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (5 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 266
B. 172
C. 138
D. 133
E. 128


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 133**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 - 1) = 4
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 - 1) = 9
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 - 1) = 14
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 - 1) = 19
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 - 1) = 24
   - k=6 $\rightarrow$ ditambah (5 $\times$ 6 - 1) = 29
   - k=7 $\rightarrow$ ditambah (5 $\times$ 7 - 1) = 34
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **133**.

</details>

### Soal #179: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (2i + 1)$$

A. 63
B. 62
C. 56
D. 80
E. 65


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 63**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(2i + 1)$.
   - Loop i=1: $(2(1) + 1) = 3$
   - Loop i=2: $(2(2) + 1) = 5$
   - Loop i=3: $(2(3) + 1) = 7$
   - Loop i=4: $(2(4) + 1) = 9$
   - Loop i=5: $(2(5) + 1) = 11$
   - Loop i=6: $(2(6) + 1) = 13$
   - Loop i=7: $(2(7) + 1) = 15$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (3) + (5) + (7) + (9) + (11) + (13) + (15) = **63**.

</details>

### Soal #180: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total = total + (2 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 14
B. 18
C. 16
D. 32
E. 25


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 16**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 - 1) = 1
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 - 1) = 3
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 - 1) = 5
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 - 1) = 7
3. Iterasi (Loop) berhenti saat $k=4$ menabrak tembok syarat kondisinya `k <= 4`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **16**.

</details>

### Soal #181: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (6 * k + 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 182
B. 232
C. 364
D. 188
E. 176


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 182**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (6 $\times$ 1 + 2) = 8
   - k=2 $\rightarrow$ ditambah (6 $\times$ 2 + 2) = 14
   - k=3 $\rightarrow$ ditambah (6 $\times$ 3 + 2) = 20
   - k=4 $\rightarrow$ ditambah (6 $\times$ 4 + 2) = 26
   - k=5 $\rightarrow$ ditambah (6 $\times$ 5 + 2) = 32
   - k=6 $\rightarrow$ ditambah (6 $\times$ 6 + 2) = 38
   - k=7 $\rightarrow$ ditambah (6 $\times$ 7 + 2) = 44
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **182**.

</details>

### Soal #182: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total = total + (2 * k + 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 70
B. 33
C. 37
D. 48
E. 35


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 35**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 + 1) = 3
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 + 1) = 5
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 + 1) = 7
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 + 1) = 9
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 + 1) = 11
3. Iterasi (Loop) berhenti saat $k=5$ menabrak tembok syarat kondisinya `k <= 5`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **35**.

</details>

### Soal #183: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (3 * k - 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 42
B. 63
C. 48
D. 90
E. 45


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 45**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 - 3) = 0
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 - 3) = 3
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 - 3) = 6
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 - 3) = 9
   - k=5 $\rightarrow$ ditambah (3 $\times$ 5 - 3) = 12
   - k=6 $\rightarrow$ ditambah (3 $\times$ 6 - 3) = 15
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **45**.

</details>

### Soal #184: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total = total + (3 * k + 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 50
B. 69
C. 100
D. 47
E. 53


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 50**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (3 $\times$ 1 + 1) = 4
   - k=2 $\rightarrow$ ditambah (3 $\times$ 2 + 1) = 7
   - k=3 $\rightarrow$ ditambah (3 $\times$ 3 + 1) = 10
   - k=4 $\rightarrow$ ditambah (3 $\times$ 4 + 1) = 13
   - k=5 $\rightarrow$ ditambah (3 $\times$ 5 + 1) = 16
3. Iterasi (Loop) berhenti saat $k=5$ menabrak tembok syarat kondisinya `k <= 5`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **50**.

</details>

### Soal #185: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (6 * k - 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 153
B. 294
C. 192
D. 147
E. 141


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 147**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (6 $\times$ 1 - 3) = 3
   - k=2 $\rightarrow$ ditambah (6 $\times$ 2 - 3) = 9
   - k=3 $\rightarrow$ ditambah (6 $\times$ 3 - 3) = 15
   - k=4 $\rightarrow$ ditambah (6 $\times$ 4 - 3) = 21
   - k=5 $\rightarrow$ ditambah (6 $\times$ 5 - 3) = 27
   - k=6 $\rightarrow$ ditambah (6 $\times$ 6 - 3) = 33
   - k=7 $\rightarrow$ ditambah (6 $\times$ 7 - 3) = 39
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **147**.

</details>

### Soal #186: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total = total + (2 * k + 3);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 45
B. 60
C. 47
D. 90
E. 43


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 45**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 + 3) = 5
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 + 3) = 7
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 + 3) = 9
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 + 3) = 11
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 + 3) = 13
3. Iterasi (Loop) berhenti saat $k=5$ menabrak tembok syarat kondisinya `k <= 5`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **45**.

</details>

### Soal #187: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{6} (4i + 2)$$

A. 96
B. 126
C. 84
D. 100
E. 94


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**A. 96**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (6).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(4i + 2)$.
   - Loop i=1: $(4(1) + 2) = 6$
   - Loop i=2: $(4(2) + 2) = 10$
   - Loop i=3: $(4(3) + 2) = 14$
   - Loop i=4: $(4(4) + 2) = 18$
   - Loop i=5: $(4(5) + 2) = 22$
   - Loop i=6: $(4(6) + 2) = 26$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (6) + (10) + (14) + (18) + (22) + (26) = **96**.

</details>

### Soal #188: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (5i + 1)$$

A. 140
B. 152
C. 146
D. 188
E. 147


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 147**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(5i + 1)$.
   - Loop i=1: $(5(1) + 1) = 6$
   - Loop i=2: $(5(2) + 1) = 11$
   - Loop i=3: $(5(3) + 1) = 16$
   - Loop i=4: $(5(4) + 1) = 21$
   - Loop i=5: $(5(5) + 1) = 26$
   - Loop i=6: $(5(6) + 1) = 31$
   - Loop i=7: $(5(7) + 1) = 36$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (6) + (11) + (16) + (21) + (26) + (31) + (36) = **147**.

</details>

### Soal #189: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (3i - 2)$$

A. 73
B. 72
C. 92
D. 84
E. 70


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 70**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(3i - 2)$.
   - Loop i=1: $(3(1) - 2) = 1$
   - Loop i=2: $(3(2) - 2) = 4$
   - Loop i=3: $(3(3) - 2) = 7$
   - Loop i=4: $(3(4) - 2) = 10$
   - Loop i=5: $(3(5) - 2) = 13$
   - Loop i=6: $(3(6) - 2) = 16$
   - Loop i=7: $(3(7) - 2) = 19$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (1) + (4) + (7) + (10) + (13) + (16) + (19) = **70**.

</details>

### Soal #190: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total = total + (5 * k + 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 154
B. 112
C. 234
D. 117
E. 122


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 117**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 + 2) = 7
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 + 2) = 12
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 + 2) = 17
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 + 2) = 22
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 + 2) = 27
   - k=6 $\rightarrow$ ditambah (5 $\times$ 6 + 2) = 32
3. Iterasi (Loop) berhenti saat $k=6$ menabrak tembok syarat kondisinya `k <= 6`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **117**.

</details>

### Soal #191: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (2i + 3)$$

A. 74
B. 56
C. 77
D. 96
E. 79


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 77**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(2i + 3)$.
   - Loop i=1: $(2(1) + 3) = 5$
   - Loop i=2: $(2(2) + 3) = 7$
   - Loop i=3: $(2(3) + 3) = 9$
   - Loop i=4: $(2(4) + 3) = 11$
   - Loop i=5: $(2(5) + 3) = 13$
   - Loop i=6: $(2(6) + 3) = 15$
   - Loop i=7: $(2(7) + 3) = 17$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (5) + (7) + (9) + (11) + (13) + (15) + (17) = **77**.

</details>

### Soal #192: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total = total + (4 * k + 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 96
B. 52
C. 70
D. 48
E. 44


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 48**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (4 $\times$ 1 + 2) = 6
   - k=2 $\rightarrow$ ditambah (4 $\times$ 2 + 2) = 10
   - k=3 $\rightarrow$ ditambah (4 $\times$ 3 + 2) = 14
   - k=4 $\rightarrow$ ditambah (4 $\times$ 4 + 2) = 18
3. Iterasi (Loop) berhenti saat $k=4$ menabrak tembok syarat kondisinya `k <= 4`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **48**.

</details>

### Soal #193: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (3i + 1)$$

A. 69
B. 49
C. 53
D. 50
E. 45


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 50**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(3i + 1)$.
   - Loop i=1: $(3(1) + 1) = 4$
   - Loop i=2: $(3(2) + 1) = 7$
   - Loop i=3: $(3(3) + 1) = 10$
   - Loop i=4: $(3(4) + 1) = 13$
   - Loop i=5: $(3(5) + 1) = 16$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (4) + (7) + (10) + (13) + (16) = **50**.

</details>

### Soal #194: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{7} (3i + 1)$$

A. 116
B. 84
C. 90
D. 94
E. 91


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**E. 91**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (7).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(3i + 1)$.
   - Loop i=1: $(3(1) + 1) = 4$
   - Loop i=2: $(3(2) + 1) = 7$
   - Loop i=3: $(3(3) + 1) = 10$
   - Loop i=4: $(3(4) + 1) = 13$
   - Loop i=5: $(3(5) + 1) = 16$
   - Loop i=6: $(3(6) + 1) = 19$
   - Loop i=7: $(3(7) + 1) = 22$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (4) + (7) + (10) + (13) + (16) + (19) + (22) = **91**.

</details>

### Soal #195: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (6i + 1)$$

A. 101
B. 95
C. 94
D. 90
E. 132


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 95**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(6i + 1)$.
   - Loop i=1: $(6(1) + 1) = 7$
   - Loop i=2: $(6(2) + 1) = 13$
   - Loop i=3: $(6(3) + 1) = 19$
   - Loop i=4: $(6(4) + 1) = 25$
   - Loop i=5: $(6(5) + 1) = 31$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (7) + (13) + (19) + (25) + (31) = **95**.

</details>

### Soal #196: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{4} (6i + 3)$$

A. 60
B. 69
C. 105
D. 72
E. 78


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 72**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (4).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(6i + 3)$.
   - Loop i=1: $(6(1) + 3) = 9$
   - Loop i=2: $(6(2) + 3) = 15$
   - Loop i=3: $(6(3) + 3) = 21$
   - Loop i=4: $(6(4) + 3) = 27$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (9) + (15) + (21) + (27) = **72**.

</details>

### Soal #197: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (5 * k - 2);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 164
B. 252
C. 121
D. 126
E. 131


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 126**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (5 $\times$ 1 - 2) = 3
   - k=2 $\rightarrow$ ditambah (5 $\times$ 2 - 2) = 8
   - k=3 $\rightarrow$ ditambah (5 $\times$ 3 - 2) = 13
   - k=4 $\rightarrow$ ditambah (5 $\times$ 4 - 2) = 18
   - k=5 $\rightarrow$ ditambah (5 $\times$ 5 - 2) = 23
   - k=6 $\rightarrow$ ditambah (5 $\times$ 6 - 2) = 28
   - k=7 $\rightarrow$ ditambah (5 $\times$ 7 - 2) = 33
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **126**.

</details>

### Soal #198: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (2 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 47
B. 64
C. 51
D. 49
E. 98


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**D. 49**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 - 1) = 1
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 - 1) = 3
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 - 1) = 5
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 - 1) = 7
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 - 1) = 9
   - k=6 $\rightarrow$ ditambah (2 $\times$ 6 - 1) = 11
   - k=7 $\rightarrow$ ditambah (2 $\times$ 7 - 1) = 13
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **49**.

</details>

### Soal #199: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Berapakah hasil hitung manual dari operasi bersimbol mengerikan (Sigma) OSN-K Informatika ini:

$$\sum_{i=1}^{5} (5i + 1)$$

A. 79
B. 111
C. 80
D. 75
E. 85


<details><summary>💡 Hint</summary>

Jangan takut, itu simbol Sigma (Huruf Yunani). Di dunia komputer dia sekadar lambang untuk `For-Loop`. Masukkan nilai $i$ dari 1 secara bertahap sampai angka ujung atas ({batas_atas}), lalu jumlahkan persis seperti numpuk koin celengan.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**C. 80**

**Pembahasan Langkah Demi Langkah:**
1. Sigma meminta kita me-looping dan mensubstitusi variabel $i$, mulai dari angka di perut bawahnya (1), berjejer sampai ke batas topi atasnya (5).
2. Setiap Loop, masukkan nilai $i$ ke pabrik perhitungan $(5i + 1)$.
   - Loop i=1: $(5(1) + 1) = 6$
   - Loop i=2: $(5(2) + 1) = 11$
   - Loop i=3: $(5(3) + 1) = 16$
   - Loop i=4: $(5(4) + 1) = 21$
   - Loop i=5: $(5(5) + 1) = 26$
3. Jika Loop sudah selesai berjalan, instruksi terakhir Sigma adalah 'Lakukan PENGGABUNGAN (SUM)' atas semua angka koin celengan itu.
   Total Jumlahan = (6) + (11) + (16) + (21) + (26) = **80**.

</details>

### Soal #200: Pilihan Ganda - Notasi Sigma (For-Loop & Kodingan)
Di layar monitormu terdapat potongan *source code* dalam instruksi C++/Java kuno:

```cpp
int total = 0;
for (int k = 1; k <= 7; k++) {
    total = total + (2 * k - 1);
}
print(total);
```

Berapakah angka yang muncul (`print`) pasca kodingan tersebut selesai dieksekusi? (Psst, ubahlah *mental model* bacamu jadi Simbol Sigma!).

A. 47
B. 49
C. 98
D. 51
E. 64


<details><summary>💡 Hint</summary>

Kodingan for-loop tersebut persis ekuivalen dengan notasi matematika Sigma $\Sigma$. Dia berjalan memasukkan nilai $k$ dari 1 sampai batas akhir {batas_atas} dan terus menambah kantong variabel `total`.

</details>
<details><summary>✅ Jawaban & Bahas</summary>

**B. 49**

**Pembahasan Langkah Demi Langkah:**
1. Kita terjemahkan balik secara mental: Fungsi di atas meminta `Looping penjumlahan berkali-kali`.
2. Polanya: Masukkan angka K iterasi secara konstan.
   - k=1 $\rightarrow$ tabungan diisi (2 $\times$ 1 - 1) = 1
   - k=2 $\rightarrow$ ditambah (2 $\times$ 2 - 1) = 3
   - k=3 $\rightarrow$ ditambah (2 $\times$ 3 - 1) = 5
   - k=4 $\rightarrow$ ditambah (2 $\times$ 4 - 1) = 7
   - k=5 $\rightarrow$ ditambah (2 $\times$ 5 - 1) = 9
   - k=6 $\rightarrow$ ditambah (2 $\times$ 6 - 1) = 11
   - k=7 $\rightarrow$ ditambah (2 $\times$ 7 - 1) = 13
3. Iterasi (Loop) berhenti saat $k=7$ menabrak tembok syarat kondisinya `k <= 7`.
4. Kodingan tersebut total mengeksekusi penjumlahan: **49**.

</details>

---
[< Bagian 3](./10-deret-soal-part-3.md) | [Bagian 5 >](./10-deret-soal-part-5.md)
