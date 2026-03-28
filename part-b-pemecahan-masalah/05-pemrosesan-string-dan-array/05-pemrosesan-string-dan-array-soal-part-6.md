🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: String & Array Processing (Part 6 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 251**
Diberikan pita DNA mutasi string: `NONONXSOXNXNSOSXOSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 7 kombinasi
C. 3 kombinasi
D. 4 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 17 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 252**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 3, 1, 8, 7, 9, 7, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 45 Juta Rupiah
C. 42 Juta Rupiah
D. 44 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`3`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`1`): Max Lokal = 7, Max Global = 7
- Indeks 3 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`7`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`5`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **E**.
</details>

---
**Soal 253**
Diberikan pita DNA mutasi string: `ONSXOSONNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 6 kombinasi
C. 8 kombinasi
D. 7 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 254**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 7, 5, 9, 6, 5, 4, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 45 Juta Rupiah
C. 49 Juta Rupiah
D. 48 Juta Rupiah
E. 47 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (47 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`5`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`9`): Max Lokal = 28, Max Global = 28
- Indeks 4 (`6`): Max Lokal = 34, Max Global = 34
- Indeks 5 (`5`): Max Lokal = 39, Max Global = 39
- Indeks 6 (`4`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`4`): Max Lokal = 47, Max Global = 47


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **47**. Opsi tervalid adalah **E**.
</details>

---
**Soal 255**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 5, 6, 8, 3, 1, 2, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 37 Juta Rupiah
C. 36 Juta Rupiah
D. 35 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`5`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`3`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`1`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`2`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`8`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **D**.
</details>

---
**Soal 256**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 4, 6, 9, 6, 1, 9, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 41 Juta Rupiah
C. 43 Juta Rupiah
D. 40 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`4`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`6`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`9`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`6`): Max Lokal = 27, Max Global = 27
- Indeks 5 (`1`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`9`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`4`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **B**.
</details>

---
**Soal 257**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 4, 4, 7, 9, 6, 8, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 47 Juta Rupiah
B. 51 Juta Rupiah
C. 50 Juta Rupiah
D. 49 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`4`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`4`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`7`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`6`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`8`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`9`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **D**.
</details>

---
**Soal 258**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 5, 3, 4, 4, 9, 8, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 45 Juta Rupiah
C. 42 Juta Rupiah
D. 41 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`5`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`3`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`8`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`4`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **A**.
</details>

---
**Soal 259**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 8, 5, 1, 7, 8, 1, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 38 Juta Rupiah
C. 40 Juta Rupiah
D. 39 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`8`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`5`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`1`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`7`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`8`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`1`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`6`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **C**.
</details>

---
**Soal 260**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 1, 4, 1, 1, 6, 3, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 25 Juta Rupiah
B. 28 Juta Rupiah
C. 27 Juta Rupiah
D. 26 Juta Rupiah
E. 24 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (26 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`1`): Max Lokal = 3, Max Global = 3
- Indeks 2 (`4`): Max Lokal = 7, Max Global = 7
- Indeks 3 (`1`): Max Lokal = 8, Max Global = 8
- Indeks 4 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 5 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 6 (`3`): Max Lokal = 18, Max Global = 18
- Indeks 7 (`8`): Max Lokal = 26, Max Global = 26


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **26**. Opsi tervalid adalah **D**.
</details>

---
**Soal 261**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 7, 4, 1, 7, 3, 5, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 44 Juta Rupiah
C. 42 Juta Rupiah
D. 43 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`1`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`7`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`5`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`8`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **C**.
</details>

---
**Soal 262**
Diberikan pita DNA mutasi string: `OXOSXSNOOXXNSXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 7 kombinasi
C. 11 kombinasi
D. 8 kombinasi
E. 10 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 263**
Diberikan pita DNA mutasi string: `OXOONSNXNSSSNNOOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 30 kombinasi
B. 31 kombinasi
C. 32 kombinasi
D. 33 kombinasi
E. 29 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (30 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 30)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **30 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 264**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 7, 5, 5, 6, 3, 5, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 48 Juta Rupiah
C. 46 Juta Rupiah
D. 47 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`5`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`6`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`3`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`5`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`8`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **C**.
</details>

---
**Soal 265**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 9, 2, 5, 9, 6, 3, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 42 Juta Rupiah
D. 43 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`9`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`2`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`5`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`6`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`3`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`6`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **E**.
</details>

---
**Soal 266**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 8, 2, 4, 7, 6, 2, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 38 Juta Rupiah
C. 40 Juta Rupiah
D. 39 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`8`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`2`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`4`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`7`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`6`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`2`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`6`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **C**.
</details>

---
**Soal 267**
Diberikan pita DNA mutasi string: `ONOOXONSNOONSNOSONO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 36 kombinasi
B. 34 kombinasi
C. 37 kombinasi
D. 35 kombinasi
E. 38 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (35 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 12 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 15 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 8)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 35)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 9)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **35 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 268**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 6, 4, 3, 7, 9, 2, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 33 Juta Rupiah
B. 35 Juta Rupiah
C. 34 Juta Rupiah
D. 36 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`6`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`3`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`2`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`1`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **C**.
</details>

---
**Soal 269**
Diberikan pita DNA mutasi string: `OSSNNNXXOOXSNNONXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 23 kombinasi
B. 20 kombinasi
C. 22 kombinasi
D. 21 kombinasi
E. 24 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (21 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 11)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 16)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 21)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **21 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 270**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 5, 2, 9, 3, 8, 6, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 36 Juta Rupiah
B. 38 Juta Rupiah
C. 37 Juta Rupiah
D. 39 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`5`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`2`): Max Lokal = 8, Max Global = 8
- Indeks 3 (`9`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`3`): Max Lokal = 20, Max Global = 20
- Indeks 5 (`8`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`6`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`4`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **B**.
</details>

---
**Soal 271**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 8, 2, 1, 8, 7, 1, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 37 Juta Rupiah
C. 41 Juta Rupiah
D. 40 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`1`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`8`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`7`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`1`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`5`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **E**.
</details>

---
**Soal 272**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 6, 6, 3, 5, 6, 2, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 39 Juta Rupiah
C. 40 Juta Rupiah
D. 38 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`6`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`3`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`5`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`6`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`2`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`3`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **C**.
</details>

---
**Soal 273**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 2, 4, 5, 7, 8, 2, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 31 Juta Rupiah
C. 35 Juta Rupiah
D. 32 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (33 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`2`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`4`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`5`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`8`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`2`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`1`): Max Lokal = 33, Max Global = 33


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **33**. Opsi tervalid adalah **E**.
</details>

---
**Soal 274**
Diberikan pita DNA mutasi string: `XSNSSOSXOSNSSXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 2 kombinasi
C. 3 kombinasi
D. 5 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 12 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 275**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 3, 6, 7, 1, 9, 1, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 40 Juta Rupiah
C. 37 Juta Rupiah
D. 39 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`3`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`7`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`1`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`9`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`1`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`8`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **D**.
</details>

---
**Soal 276**
Diberikan pita DNA mutasi string: `OOXONONSNXSNSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 11 kombinasi
B. 14 kombinasi
C. 12 kombinasi
D. 13 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 10 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 277**
Diberikan pita DNA mutasi string: `SNNOONXSNOXNNOXSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 6 kombinasi
C. 7 kombinasi
D. 9 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 16 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 278**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 2, 1, 5, 5, 5, 4, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 33 Juta Rupiah
B. 35 Juta Rupiah
C. 37 Juta Rupiah
D. 36 Juta Rupiah
E. 34 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`2`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`1`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`5`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`5`): Max Lokal = 20, Max Global = 20
- Indeks 5 (`5`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`6`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **B**.
</details>

---
**Soal 279**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 7, 7, 1, 8, 5, 6, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 44 Juta Rupiah
C. 45 Juta Rupiah
D. 46 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`7`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`7`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`1`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`8`): Max Lokal = 27, Max Global = 27
- Indeks 5 (`5`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`6`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`6`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **B**.
</details>

---
**Soal 280**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 5, 5, 6, 4, 6, 8, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 49 Juta Rupiah
C. 48 Juta Rupiah
D. 47 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (47 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`5`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`5`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`6`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`6`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`8`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`4`): Max Lokal = 47, Max Global = 47


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **47**. Opsi tervalid adalah **D**.
</details>

---
**Soal 281**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 9, 4, 2, 1, 4, 4, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 31 Juta Rupiah
B. 28 Juta Rupiah
C. 30 Juta Rupiah
D. 29 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`9`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`4`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`1`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`4`): Max Lokal = 26, Max Global = 26
- Indeks 7 (`4`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **C**.
</details>

---
**Soal 282**
Diberikan pita DNA mutasi string: `NXOSOOXNSONNOOOOSXOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 9 kombinasi
C. 11 kombinasi
D. 10 kombinasi
E. 12 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 8)
- Indeks 16 (`S`): Kawinkan dengan 8 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 9)
- Indeks 19 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 283**
Diberikan pita DNA mutasi string: `OOOSSNXNSSXXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 25 kombinasi
B. 26 kombinasi
C. 24 kombinasi
D. 27 kombinasi
E. 23 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (24 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 3 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 4 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 24)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **24 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 284**
Diberikan pita DNA mutasi string: `XNOXXOSNNNOSOXXSXNXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 15 kombinasi
B. 17 kombinasi
C. 18 kombinasi
D. 16 kombinasi
E. 14 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (15 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 15)
- Indeks 19 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **15 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 285**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 4, 3, 2, 9, 1, 5, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 36 Juta Rupiah
C. 35 Juta Rupiah
D. 38 Juta Rupiah
E. 37 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`3`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`5`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`5`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **E**.
</details>

---
**Soal 286**
Diberikan pita DNA mutasi string: `XXONOONNXSNXXXNS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 5 kombinasi
C. 6 kombinasi
D. 9 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 287**
Diberikan pita DNA mutasi string: `SSSOSOOXSOXXSXNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 17 kombinasi
B. 16 kombinasi
C. 18 kombinasi
D. 15 kombinasi
E. 19 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (16 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 16)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **16 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 288**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 5, 1, 9, 4, 5, 6, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 32 Juta Rupiah
B. 35 Juta Rupiah
C. 34 Juta Rupiah
D. 36 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`5`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`5`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`6`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`1`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **C**.
</details>

---
**Soal 289**
Diberikan pita DNA mutasi string: `XOSOXONOSSXXNXSSNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 43 kombinasi
B. 46 kombinasi
C. 45 kombinasi
D. 44 kombinasi
E. 47 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (44 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 27)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 44)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **44 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 290**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 1, 9, 5, 7, 4, 3, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 43 Juta Rupiah
C. 44 Juta Rupiah
D. 42 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`1`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`5`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`7`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`4`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`3`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`7`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **C**.
</details>

---
**Soal 291**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 1, 8, 3, 6, 2, 7, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 34 Juta Rupiah
C. 37 Juta Rupiah
D. 35 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (36 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`1`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`3`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`2`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`7`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`4`): Max Lokal = 36, Max Global = 36


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **36**. Opsi tervalid adalah **E**.
</details>

---
**Soal 292**
Diberikan pita DNA mutasi string: `SNSNONNOXSNNOSNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 17 kombinasi
B. 13 kombinasi
C. 16 kombinasi
D. 15 kombinasi
E. 14 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (14 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **14 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 293**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 8, 5, 1, 9, 3, 4, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 41 Juta Rupiah
C. 40 Juta Rupiah
D. 38 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`8`): Max Lokal = 16, Max Global = 16
- Indeks 2 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`1`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`3`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`4`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`2`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **C**.
</details>

---
**Soal 294**
Diberikan pita DNA mutasi string: `OONOSOSOSNSNNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 47 kombinasi
B. 49 kombinasi
C. 45 kombinasi
D. 46 kombinasi
E. 48 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (46 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 6 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 8 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 10 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 29)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 46)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **46 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 295**
Diberikan pita DNA mutasi string: `OSNSOSXONXOSXOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 7 kombinasi
C. 6 kombinasi
D. 4 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 296**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 3, 6, 6, 8, 4, 7, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 41 Juta Rupiah
C. 42 Juta Rupiah
D. 44 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`3`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`6`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`6`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`8`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`4`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`7`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`4`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **A**.
</details>

---
**Soal 297**
Diberikan pita DNA mutasi string: `XNNOXSNSOSNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 6 kombinasi
C. 5 kombinasi
D. 8 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 298**
Diberikan pita DNA mutasi string: `NXSOXNXXSOONONOSOXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 7 kombinasi
C. 8 kombinasi
D. 10 kombinasi
E. 11 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 299**
Diberikan pita DNA mutasi string: `OXOOSNOXSSXXNSSSOSNS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 41 kombinasi
B. 43 kombinasi
C. 42 kombinasi
D. 45 kombinasi
E. 44 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (42 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 14)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 19)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 23)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 17 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 28)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 28 buah `OS`. (Total Jawaban OSN = 42)
- Indeks 19 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 33)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **42 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 300**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 2, 4, 1, 3, 2, 1, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 23 Juta Rupiah
B. 22 Juta Rupiah
C. 21 Juta Rupiah
D. 19 Juta Rupiah
E. 20 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (21 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`2`): Max Lokal = 3, Max Global = 3
- Indeks 2 (`4`): Max Lokal = 7, Max Global = 7
- Indeks 3 (`1`): Max Lokal = 8, Max Global = 8
- Indeks 4 (`3`): Max Lokal = 11, Max Global = 11
- Indeks 5 (`2`): Max Lokal = 13, Max Global = 13
- Indeks 6 (`1`): Max Lokal = 14, Max Global = 14
- Indeks 7 (`7`): Max Lokal = 21, Max Global = 21


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **21**. Opsi tervalid adalah **C**.
</details>

---
