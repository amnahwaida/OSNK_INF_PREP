# 10. Deret & Pola Bilangan - Latihan Soal Bagian 4
## Topik: Kode vs Sigma (Looping Pertambahan)

[< Bagian 3](./10-deret-soal-part-3.md) | [Bagian 5 >](./10-deret-soal-part-5.md)

---

### Soal #151: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #152: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (3k + 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (3 * k + 2);
}
```</details>

### Soal #153: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (3k + 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (3 * k + 2);
}
```</details>

### Soal #154: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #155: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (2k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (2 * k - 1);
}
```</details>

### Soal #156: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (3k + 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (3 * k + 1);
}
```</details>

### Soal #157: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (5k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (5 * k - 1);
}
```</details>

### Soal #158: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (3k + 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (3 * k + 1);
}
```</details>

### Soal #159: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{5} (2i - 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (0) + (2) + (4) + (6) + (8)
= **20**.</details>

### Soal #160: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (5i - 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (9) + (14) + (19)
= **46**.</details>

### Soal #161: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (5i - 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (9) + (14) + (19)
= **46**.</details>

### Soal #162: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (2i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (6) + (8) + (10) + (12) + (14)
= **54**.</details>

### Soal #163: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (6) + (8) + (10)
= **28**.</details>

### Soal #164: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i - 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (0) + (2) + (4) + (6)
= **12**.</details>

### Soal #165: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (3k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (3 * k - 2);
}
```</details>

### Soal #166: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (3i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (5) + (8) + (11) + (14) + (17) + (20)
= **75**.</details>

### Soal #167: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (3k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (3 * k - 2);
}
```</details>

### Soal #168: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (2k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (2 * k - 2);
}
```</details>

### Soal #169: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (2k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (2 * k - 1);
}
```</details>

### Soal #170: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (2k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (2 * k - 1);
}
```</details>

### Soal #171: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (3) + (5) + (7) + (9)
= **24**.</details>

### Soal #172: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i - 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (1) + (3) + (5) + (7)
= **16**.</details>

### Soal #173: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (4i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (6) + (10) + (14) + (18)
= **48**.</details>

### Soal #174: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{5} (4i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (6) + (10) + (14) + (18) + (22)
= **70**.</details>

### Soal #175: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (5k + 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (5 * k + 2);
}
```</details>

### Soal #176: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (3i - 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (1) + (4) + (7) + (10) + (13) + (16)
= **51**.</details>

### Soal #177: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (5k + 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (5 * k + 1);
}
```</details>

### Soal #178: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (3i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (7) + (10) + (13)
= **34**.</details>

### Soal #179: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i - 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (1) + (3) + (5) + (7)
= **16**.</details>

### Soal #180: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (4k + 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (4 * k + 2);
}
```</details>

### Soal #181: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #182: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (3k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (3 * k - 1);
}
```</details>

### Soal #183: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (5i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (6) + (11) + (16) + (21) + (26) + (31)
= **111**.</details>

### Soal #184: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (2i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (6) + (8) + (10)
= **28**.</details>

### Soal #185: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #186: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (2k + 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (2 * k + 1);
}
```</details>

### Soal #187: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (3i - 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (1) + (4) + (7) + (10) + (13) + (16)
= **51**.</details>

### Soal #188: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (4i - 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (2) + (6) + (10) + (14)
= **32**.</details>

### Soal #189: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (4i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (5) + (9) + (13) + (17)
= **44**.</details>

### Soal #190: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (2i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (6) + (8) + (10) + (12) + (14)
= **54**.</details>

### Soal #191: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{4} (4i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (5) + (9) + (13) + (17)
= **44**.</details>

### Soal #192: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #193: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (2k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (2 * k - 2);
}
```</details>

### Soal #194: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{6} (4k - 1)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 6; k++) {
    total += (4 * k - 1);
}
```</details>

### Soal #195: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{4} (5k - 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 4; k++) {
    total += (5 * k - 2);
}
```</details>

### Soal #196: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (5i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (6) + (11) + (16) + (21) + (26) + (31)
= **111**.</details>

### Soal #197: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{5} (2i - 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (1) + (3) + (5) + (7) + (9)
= **25**.</details>

### Soal #198: Notasi Sigma (For-Loop)
Tuliskan Pseudo-code kodingan `For-loop` yang artinya setara persis dengan Simbol Klasik ini:
$\sum_{k=1}^{5} (5k + 2)$

<details><summary>💡 Hint</summary>Total awalnya 0, counter-nya (misal K) jalan dari 1 sampai batas akhir, tiap jalan nilai total ditambah ({koef}*k {sign} {abs(offset)}).</details>
<details><summary>✅ Jawaban</summary>```cpp
int total = 0;
for (int k = 1; k <= 5; k++) {
    total += (5 * k + 2);
}
```</details>

### Soal #199: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{6} (4i + 1)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (5) + (9) + (13) + (17) + (21) + (25)
= **90**.</details>

### Soal #200: Notasi Sigma (For-Loop)
Selesaikan Notasi Sigma berikut layaknya komputer:
$\sum_{i=1}^{5} (2i + 2)$

<details><summary>💡 Hint</summary>Ganti huruf $i$ dengan angka 1, 2, 3.. sampai batas atas ({end_idx}), lalu jumlahkan semua hasilnya.</details>
<details><summary>✅ Jawaban</summary>Jabaran Loop: (4) + (6) + (8) + (10) + (12)
= **40**.</details>

---
[< Bagian 3](./10-deret-soal-part-3.md) | [Bagian 5 >](./10-deret-soal-part-5.md)
