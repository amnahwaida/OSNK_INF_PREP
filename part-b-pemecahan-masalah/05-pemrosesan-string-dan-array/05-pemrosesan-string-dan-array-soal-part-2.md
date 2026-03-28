🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: String & Array Processing (Part 2 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 51**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 5, 8, 4, 1, 1, 3, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 31 Juta Rupiah
B. 34 Juta Rupiah
C. 33 Juta Rupiah
D. 30 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`5`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`4`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`1`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`3`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`2`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **E**.
</details>

---
**Soal 52**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 9, 9, 1, 9, 3, 8, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 58 Juta Rupiah
B. 55 Juta Rupiah
C. 57 Juta Rupiah
D. 56 Juta Rupiah
E. 59 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (57 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 2 (`9`): Max Lokal = 27, Max Global = 27
- Indeks 3 (`1`): Max Lokal = 28, Max Global = 28
- Indeks 4 (`9`): Max Lokal = 37, Max Global = 37
- Indeks 5 (`3`): Max Lokal = 40, Max Global = 40
- Indeks 6 (`8`): Max Lokal = 48, Max Global = 48
- Indeks 7 (`9`): Max Lokal = 57, Max Global = 57


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **57**. Opsi tervalid adalah **C**.
</details>

---
**Soal 53**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 3, 2, 7, 7, 5, 2, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 26 Juta Rupiah
B. 27 Juta Rupiah
C. 29 Juta Rupiah
D. 28 Juta Rupiah
E. 30 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (28 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`3`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`2`): Max Lokal = 6, Max Global = 6
- Indeks 3 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 4 (`7`): Max Lokal = 20, Max Global = 20
- Indeks 5 (`5`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`2`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`1`): Max Lokal = 28, Max Global = 28


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **28**. Opsi tervalid adalah **D**.
</details>

---
**Soal 54**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 2, 5, 8, 8, 9, 5, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 42 Juta Rupiah
C. 43 Juta Rupiah
D. 44 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`2`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`5`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`8`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`8`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`9`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`5`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`4`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **C**.
</details>

---
**Soal 55**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 5, 1, 4, 3, 7, 2, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 28 Juta Rupiah
B. 27 Juta Rupiah
C. 29 Juta Rupiah
D. 26 Juta Rupiah
E. 30 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (28 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`5`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`4`): Max Lokal = 13, Max Global = 13
- Indeks 4 (`3`): Max Lokal = 16, Max Global = 16
- Indeks 5 (`7`): Max Lokal = 23, Max Global = 23
- Indeks 6 (`2`): Max Lokal = 25, Max Global = 25
- Indeks 7 (`3`): Max Lokal = 28, Max Global = 28


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **28**. Opsi tervalid adalah **A**.
</details>

---
**Soal 56**
Diberikan pita DNA mutasi string: `NXSXOOXONSSONSOXXOXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 16 kombinasi
B. 19 kombinasi
C. 15 kombinasi
D. 18 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (16 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 19 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 16)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **16 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 57**
Diberikan pita DNA mutasi string: `OOSNONSNOOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 12 kombinasi
B. 10 kombinasi
C. 11 kombinasi
D. 9 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 6 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 58**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 3, 7, 1, 3, 1, 6, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 29 Juta Rupiah
B. 31 Juta Rupiah
C. 32 Juta Rupiah
D. 33 Juta Rupiah
E. 30 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (31 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`3`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`7`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`3`): Max Lokal = 19, Max Global = 19
- Indeks 5 (`1`): Max Lokal = 20, Max Global = 20
- Indeks 6 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 7 (`5`): Max Lokal = 31, Max Global = 31


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **31**. Opsi tervalid adalah **B**.
</details>

---
**Soal 59**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 4, 6, 1, 5, 5, 5, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 36 Juta Rupiah
B. 32 Juta Rupiah
C. 34 Juta Rupiah
D. 33 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`4`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`5`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`5`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`3`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **C**.
</details>

---
**Soal 60**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 8, 5, 5, 5, 1, 6, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 42 Juta Rupiah
C. 44 Juta Rupiah
D. 46 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`8`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`5`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`5`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`5`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`6`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`9`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **C**.
</details>

---
**Soal 61**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 7, 6, 9, 5, 4, 2, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 41 Juta Rupiah
C. 40 Juta Rupiah
D. 42 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`7`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`6`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 4 (`5`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`4`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`2`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`3`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **C**.
</details>

---
**Soal 62**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 6, 5, 2, 3, 3, 1, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 26 Juta Rupiah
B. 24 Juta Rupiah
C. 23 Juta Rupiah
D. 25 Juta Rupiah
E. 27 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (25 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`6`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`5`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`2`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`3`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`3`): Max Lokal = 21, Max Global = 21
- Indeks 6 (`1`): Max Lokal = 22, Max Global = 22
- Indeks 7 (`3`): Max Lokal = 25, Max Global = 25


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **25**. Opsi tervalid adalah **D**.
</details>

---
**Soal 63**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 8, 4, 2, 1, 8, 7, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 44 Juta Rupiah
B. 42 Juta Rupiah
C. 43 Juta Rupiah
D. 46 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`8`): Max Lokal = 16, Max Global = 16
- Indeks 2 (`4`): Max Lokal = 20, Max Global = 20
- Indeks 3 (`2`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`1`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`7`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`6`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **A**.
</details>

---
**Soal 64**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 5, 4, 8, 2, 8, 8, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 47 Juta Rupiah
B. 48 Juta Rupiah
C. 46 Juta Rupiah
D. 45 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`5`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`4`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`8`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`2`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`8`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`8`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`5`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **C**.
</details>

---
**Soal 65**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 6, 1, 5, 1, 7, 4, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 37 Juta Rupiah
C. 38 Juta Rupiah
D. 39 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`1`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`7`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`6`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **D**.
</details>

---
**Soal 66**
Diberikan pita DNA mutasi string: `SNSSSXONXNSNOXNXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 2 kombinasi
C. 1 kombinasi
D. 4 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 16 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 67**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 7, 5, 7, 1, 2, 2, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 29 Juta Rupiah
B. 31 Juta Rupiah
C. 30 Juta Rupiah
D. 28 Juta Rupiah
E. 27 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (29 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`7`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`5`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`1`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`2`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`2`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`2`): Max Lokal = 29, Max Global = 29


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **29**. Opsi tervalid adalah **A**.
</details>

---
**Soal 68**
Diberikan pita DNA mutasi string: `SXNNXOXNSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 2 kombinasi
C. 4 kombinasi
D. 0 kombinasi
E. 1 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 69**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 1, 6, 9, 4, 7, 7, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 48 Juta Rupiah
B. 49 Juta Rupiah
C. 50 Juta Rupiah
D. 47 Juta Rupiah
E. 51 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`1`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`4`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`7`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`7`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`9`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **B**.
</details>

---
**Soal 70**
Diberikan pita DNA mutasi string: `NNXXNNOSNSSONNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 9 kombinasi
C. 10 kombinasi
D. 8 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (7 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 9 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 71**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 3, 8, 1, 7, 9, 8, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 43 Juta Rupiah
C. 41 Juta Rupiah
D. 40 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`3`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`1`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`8`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`2`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **C**.
</details>

---
**Soal 72**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 4, 5, 7, 3, 2, 5, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 38 Juta Rupiah
C. 39 Juta Rupiah
D. 37 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`5`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`7`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`3`): Max Lokal = 27, Max Global = 27
- Indeks 5 (`2`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`5`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`5`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **C**.
</details>

---
**Soal 73**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 1, 8, 1, 9, 5, 5, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 35 Juta Rupiah
C. 38 Juta Rupiah
D. 37 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (36 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`1`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`9`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`5`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`5`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`1`): Max Lokal = 36, Max Global = 36


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **36**. Opsi tervalid adalah **E**.
</details>

---
**Soal 74**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 2, 7, 2, 6, 4, 5, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 31 Juta Rupiah
B. 32 Juta Rupiah
C. 30 Juta Rupiah
D. 28 Juta Rupiah
E. 29 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`2`): Max Lokal = 3, Max Global = 3
- Indeks 2 (`7`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`2`): Max Lokal = 12, Max Global = 12
- Indeks 4 (`6`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`5`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`3`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **C**.
</details>

---
**Soal 75**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 1, 4, 3, 7, 1, 6, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 36 Juta Rupiah
C. 37 Juta Rupiah
D. 38 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`4`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`3`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`7`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`1`): Max Lokal = 24, Max Global = 24
- Indeks 6 (`6`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`8`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **D**.
</details>

---
**Soal 76**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 7, 3, 9, 3, 7, 6, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 47 Juta Rupiah
C. 44 Juta Rupiah
D. 43 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`7`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`3`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`3`): Max Lokal = 27, Max Global = 27
- Indeks 5 (`7`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`6`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`5`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **A**.
</details>

---
**Soal 77**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 9, 1, 2, 9, 9, 9, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 43 Juta Rupiah
C. 45 Juta Rupiah
D. 47 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`9`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`2`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`9`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`9`): Max Lokal = 42, Max Global = 42
- Indeks 7 (`3`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **C**.
</details>

---
**Soal 78**
Diberikan pita DNA mutasi string: `XSOSOXSNSXSXOSSNSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 17 kombinasi
B. 19 kombinasi
C. 18 kombinasi
D. 16 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (16 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 16)
- Indeks 16 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 16)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **16 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 79**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 3, 6, 8, 1, 3, 2, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 34 Juta Rupiah
C. 35 Juta Rupiah
D. 36 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (36 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`3`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`6`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`8`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`1`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`2`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`5`): Max Lokal = 36, Max Global = 36


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **36**. Opsi tervalid adalah **D**.
</details>

---
**Soal 80**
Diberikan pita DNA mutasi string: `ONOSXNSOXXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 2 kombinasi
C. 1 kombinasi
D. 3 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 81**
Diberikan pita DNA mutasi string: `SSSNOSONNNXNOXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 5 kombinasi
C. 3 kombinasi
D. 6 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 82**
Diberikan pita DNA mutasi string: `NNXOOSXOSXSSNNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 24 kombinasi
B. 21 kombinasi
C. 23 kombinasi
D. 22 kombinasi
E. 25 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (22 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 11)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 22)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **22 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 83**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 5, 5, 9, 5, 8, 6, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 49 Juta Rupiah
C. 50 Juta Rupiah
D. 47 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (48 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`5`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`5`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`5`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`8`): Max Lokal = 37, Max Global = 37
- Indeks 6 (`6`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`5`): Max Lokal = 48, Max Global = 48


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **48**. Opsi tervalid adalah **E**.
</details>

---
**Soal 84**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 9, 9, 2, 7, 2, 1, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 34 Juta Rupiah
C. 36 Juta Rupiah
D. 33 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`9`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`9`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`2`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`7`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`2`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`1`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`2`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **E**.
</details>

---
**Soal 85**
Diberikan pita DNA mutasi string: `XNSXOXSNSSSNONXNNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 18 kombinasi
B. 19 kombinasi
C. 16 kombinasi
D. 20 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (17 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 13)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 17)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **17 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 86**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 3, 6, 7, 2, 1, 6, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 35 Juta Rupiah
C. 32 Juta Rupiah
D. 33 Juta Rupiah
E. 31 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (33 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`3`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`7`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`2`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`1`): Max Lokal = 23, Max Global = 23
- Indeks 6 (`6`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`4`): Max Lokal = 33, Max Global = 33


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **33**. Opsi tervalid adalah **D**.
</details>

---
**Soal 87**
Diberikan pita DNA mutasi string: `ONONXSOXOSSON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 11 kombinasi
B. 12 kombinasi
C. 10 kombinasi
D. 9 kombinasi
E. 13 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (10 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 10 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **10 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 88**
Diberikan pita DNA mutasi string: `NSXSXOOSONNOONOXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 6 kombinasi
C. 7 kombinasi
D. 5 kombinasi
E. 9 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 16 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 89**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 8, 1, 1, 5, 1, 5, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 30 Juta Rupiah
B. 33 Juta Rupiah
C. 32 Juta Rupiah
D. 31 Juta Rupiah
E. 34 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`8`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`1`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 4 (`5`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`1`): Max Lokal = 19, Max Global = 19
- Indeks 6 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 7 (`8`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **C**.
</details>

---
**Soal 90**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 1, 9, 1, 2, 1, 5, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 32 Juta Rupiah
B. 33 Juta Rupiah
C. 34 Juta Rupiah
D. 36 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`1`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`2`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`1`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`5`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`7`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **C**.
</details>

---
**Soal 91**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 9, 7, 3, 1, 4, 6, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 47 Juta Rupiah
C. 48 Juta Rupiah
D. 45 Juta Rupiah
E. 49 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (47 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 2 (`7`): Max Lokal = 25, Max Global = 25
- Indeks 3 (`3`): Max Lokal = 28, Max Global = 28
- Indeks 4 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`6`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`8`): Max Lokal = 47, Max Global = 47


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **47**. Opsi tervalid adalah **B**.
</details>

---
**Soal 92**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 3, 9, 9, 6, 2, 3, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 35 Juta Rupiah
C. 37 Juta Rupiah
D. 36 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`3`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`9`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`6`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`2`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`3`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`2`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **B**.
</details>

---
**Soal 93**
Diberikan pita DNA mutasi string: `XSNXONNNOXSONO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 1 kombinasi
C. 3 kombinasi
D. 5 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 94**
Diberikan pita DNA mutasi string: `NXSXXNOXSONNONSNXSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 7 kombinasi
C. 8 kombinasi
D. 10 kombinasi
E. 9 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (7 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 17 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 18 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 95**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 8, 2, 8, 3, 4, 4, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 43 Juta Rupiah
C. 42 Juta Rupiah
D. 41 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`8`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`3`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`4`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`4`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`6`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **C**.
</details>

---
**Soal 96**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 1, 4, 8, 7, 5, 8, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 44 Juta Rupiah
B. 45 Juta Rupiah
C. 47 Juta Rupiah
D. 48 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`1`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`4`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`8`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`7`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`5`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`8`): Max Lokal = 42, Max Global = 42
- Indeks 7 (`4`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **E**.
</details>

---
**Soal 97**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 8, 5, 9, 6, 6, 4, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 47 Juta Rupiah
C. 43 Juta Rupiah
D. 44 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`8`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`5`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`9`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`6`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`6`): Max Lokal = 37, Max Global = 37
- Indeks 6 (`4`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`4`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **E**.
</details>

---
**Soal 98**
Diberikan pita DNA mutasi string: `OSXNSNNOXNOSNNXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 16 kombinasi
B. 19 kombinasi
C. 20 kombinasi
D. 18 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (17 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 17)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **17 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 99**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 7, 1, 2, 5, 1, 4, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 30 Juta Rupiah
B. 28 Juta Rupiah
C. 31 Juta Rupiah
D. 32 Juta Rupiah
E. 29 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`7`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`2`): Max Lokal = 11, Max Global = 11
- Indeks 4 (`5`): Max Lokal = 16, Max Global = 16
- Indeks 5 (`1`): Max Lokal = 17, Max Global = 17
- Indeks 6 (`4`): Max Lokal = 21, Max Global = 21
- Indeks 7 (`9`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **A**.
</details>

---
**Soal 100**
Diberikan pita DNA mutasi string: `SNSONOXONXSXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 0 kombinasi
C. 5 kombinasi
D. 3 kombinasi
E. 1 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
