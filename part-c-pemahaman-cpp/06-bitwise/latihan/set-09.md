🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal Part C - Modul 06 - Set 09

### Soal 201
```cpp
int status_lampu = 5;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=5"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 202
```cpp
int status_lampu = 2;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=2"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 203
```cpp
int status_lampu = 2;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=2"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 204
```cpp
int sensor_angka = 4;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=4 (0b100)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 4 (0b100) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 205
```cpp
int sensor_angka = 2;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=2 (0b10)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 2 (0b10) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 206
```cpp
int sensor_angka = 1;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **1**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=1 (0b1)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 1"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 1 (0b1) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **1**.

---
### Soal 207
```cpp
int status_lampu = 2;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=2"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 208
```cpp
int sensor_angka = 5;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **1**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=5 (0b101)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 1"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 5 (0b101) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **1**.

---
### Soal 209
```cpp
int sensor_angka = 4;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=4 (0b100)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 4 (0b100) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 210
```cpp
int sensor_angka = 2;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=2 (0b10)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 2 (0b10) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 211
```cpp
int sensor_angka = 1;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **1**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=1 (0b1)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 1"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 1 (0b1) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **1**.

---
### Soal 212
```cpp
int power_up = 2;
int hasil_shift = power_up << 2;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **8**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=2"] --> B["Geser Kiri 2x"]
B --> C["Hasil: 8"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 2 dengan 2 pangkat 2.
3. **Hasil**: 2 * 4 = **8**.

---
### Soal 213
```cpp
int sensor_angka = 2;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=2 (0b10)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 2 (0b10) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 214
```cpp
int power_up = 5;
int hasil_shift = power_up << 2;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **20**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=5"] --> B["Geser Kiri 2x"]
B --> C["Hasil: 20"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 5 dengan 2 pangkat 2.
3. **Hasil**: 5 * 4 = **20**.

---
### Soal 215
```cpp
int status_lampu = 2;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=2"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 216
```cpp
int power_up = 5;
int hasil_shift = power_up << 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **10**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=5"] --> B["Geser Kiri 1x"]
B --> C["Hasil: 10"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 5 dengan 2 pangkat 1.
3. **Hasil**: 5 * 2 = **10**.

---
### Soal 217
```cpp
int sensor_angka = 4;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=4 (0b100)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 0"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 4 (0b100) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **0**.

---
### Soal 218
```cpp
int power_up = 5;
int hasil_shift = power_up << 2;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **20**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=5"] --> B["Geser Kiri 2x"]
B --> C["Hasil: 20"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 5 dengan 2 pangkat 2.
3. **Hasil**: 5 * 4 = **20**.

---
### Soal 219
```cpp
int power_up = 3;
int hasil_shift = power_up << 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **6**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=3"] --> B["Geser Kiri 1x"]
B --> C["Hasil: 6"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 3 dengan 2 pangkat 1.
3. **Hasil**: 3 * 2 = **6**.

---
### Soal 220
```cpp
int status_lampu = 2;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=2"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
### Soal 221
```cpp
int sensor_angka = 3;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **1**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=3 (0b11)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 1"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 3 (0b11) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **1**.

---
### Soal 222
```cpp
int sensor_angka = 1;
int cek_ganjil = sensor_angka & 1;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **1**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph TD
A["angka=1 (0b1)"] --> B["Lampu Terakhir & 1"]
B --> C["Hasil: 1"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Bit Ganjil**: Bit paling kanan menentukan ganjil atau genap. 
2. **Tracing**: 1 (0b1) di-AND-kan dengan 1 (0b1).
3. **Logika**: Hanya jika bit terakhir 1, hasilnya 1 (Artinya Ganjil).
4. **Hasil**: `cek_ganjil` bernilai **1**.

---
### Soal 223
```cpp
int power_up = 5;
int hasil_shift = power_up << 2;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **20**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=5"] --> B["Geser Kiri 2x"]
B --> C["Hasil: 20"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 5 dengan 2 pangkat 2.
3. **Hasil**: 5 * 4 = **20**.

---
### Soal 224
```cpp
int power_up = 3;
int hasil_shift = power_up << 2;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **12**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["angka=3"] --> B["Geser Kiri 2x"]
B --> C["Hasil: 12"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **Shift Kiri**: Menggeser bit ke kiri dan menambah nol di belakang.
2. **Ekuivalen**: Sama dengan mengali 3 dengan 2 pangkat 2.
3. **Hasil**: 3 * 4 = **12**.

---
### Soal 225
```cpp
int status_lampu = 4;
int toggle = status_lampu ^ status_lampu;
```
**Pertanyaan:**
1. Berapakah hasil akhirnya?
2. Deskripsikan langkah robot compiler saat memproses kode ini!

**Jawaban & Diagnosis:**
1. **0**
2. Baca bagian 'Analisis Mendalam' di bawah.

**Mermaid Flowchart:**
```mermaid
graph LR
A["lampu=4"] --> B["XOR Diri Sendiri"]
B --> C["Hasil: 0 (Padam)"]
```

**📖 Penjelasan Komprehensif:**
**Analisis Mendalam (Compiler Manusia):**
1. **XOR Self**: Angka apa pun jika di-XOR dengan dirinya sendiri akan saling meniadakan.
2. **Magic Logic**: Bit yang sama menghasilkan 0.
3. **Hasil**: `toggle` mutlak bernilai **0**.

---
