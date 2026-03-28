🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: String & Array Processing (Part 3 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 101**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 4, 9, 6, 6, 2, 7, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 46 Juta Rupiah
C. 45 Juta Rupiah
D. 43 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`4`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`9`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`6`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`6`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`2`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`7`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`7`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **E**.
</details>

---
**Soal 102**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 7, 7, 2, 9, 4, 5, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 45 Juta Rupiah
C. 43 Juta Rupiah
D. 42 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`7`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`2`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`9`): Max Lokal = 32, Max Global = 32
- Indeks 5 (`4`): Max Lokal = 36, Max Global = 36
- Indeks 6 (`5`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`2`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **C**.
</details>

---
**Soal 103**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 2, 9, 3, 8, 2, 1, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 43 Juta Rupiah
D. 42 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`2`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`3`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`8`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`2`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`1`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`9`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **E**.
</details>

---
**Soal 104**
Diberikan pita DNA mutasi string: `XXSSOONOOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 1 kombinasi
B. 2 kombinasi
C. 0 kombinasi
D. 5 kombinasi
E. 3 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 105**
Diberikan pita DNA mutasi string: `NOSSSXXOXXONNSNXNXO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 20 kombinasi
B. 21 kombinasi
C. 18 kombinasi
D. 19 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (18 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **18 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 106**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 4, 3, 1, 9, 4, 5, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 38 Juta Rupiah
D. 36 Juta Rupiah
E. 37 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`4`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`3`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`1`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`4`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`5`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`5`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **C**.
</details>

---
**Soal 107**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 4, 8, 7, 4, 5, 6, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 51 Juta Rupiah
C. 48 Juta Rupiah
D. 47 Juta Rupiah
E. 50 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`4`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`8`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`7`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`5`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`6`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`9`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **A**.
</details>

---
**Soal 108**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 2, 5, 4, 6, 3, 2, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 32 Juta Rupiah
B. 33 Juta Rupiah
C. 34 Juta Rupiah
D. 30 Juta Rupiah
E. 31 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`2`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`5`): Max Lokal = 11, Max Global = 11
- Indeks 3 (`4`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`6`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`3`): Max Lokal = 24, Max Global = 24
- Indeks 6 (`2`): Max Lokal = 26, Max Global = 26
- Indeks 7 (`6`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **A**.
</details>

---
**Soal 109**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 4, 8, 3, 9, 1, 4, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 40 Juta Rupiah
C. 44 Juta Rupiah
D. 43 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`4`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`8`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`3`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`9`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`9`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **E**.
</details>

---
**Soal 110**
Diberikan pita DNA mutasi string: `NNNXSSXSSSOOXNNOSOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 0 kombinasi
C. 1 kombinasi
D. 3 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 8 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 9 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 16 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 111**
Diberikan pita DNA mutasi string: `SSONONSSNNSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 8 kombinasi
C. 10 kombinasi
D. 11 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 112**
Diberikan pita DNA mutasi string: `SOSOXONNSXXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 4 kombinasi
C. 1 kombinasi
D. 3 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 113**
Diberikan pita DNA mutasi string: `ONSSSSONNSXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 16 kombinasi
B. 15 kombinasi
C. 13 kombinasi
D. 14 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (14 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **14 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 114**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 6, 4, 4, 8, 7, 6, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 42 Juta Rupiah
C. 40 Juta Rupiah
D. 41 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`6`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`4`): Max Lokal = 11, Max Global = 11
- Indeks 3 (`4`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`8`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`7`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`6`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`6`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **B**.
</details>

---
**Soal 115**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 6, 3, 9, 9, 2, 9, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 52 Juta Rupiah
B. 49 Juta Rupiah
C. 53 Juta Rupiah
D. 50 Juta Rupiah
E. 51 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (51 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`3`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`9`): Max Lokal = 27, Max Global = 27
- Indeks 4 (`9`): Max Lokal = 36, Max Global = 36
- Indeks 5 (`2`): Max Lokal = 38, Max Global = 38
- Indeks 6 (`9`): Max Lokal = 47, Max Global = 47
- Indeks 7 (`4`): Max Lokal = 51, Max Global = 51


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **51**. Opsi tervalid adalah **E**.
</details>

---
**Soal 116**
Diberikan pita DNA mutasi string: `OSXNNNONON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 5 kombinasi
C. 8 kombinasi
D. 7 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 117**
Diberikan pita DNA mutasi string: `XONXSOSOSXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 1 kombinasi
C. 5 kombinasi
D. 0 kombinasi
E. 3 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 118**
Diberikan pita DNA mutasi string: `NOSNOONNSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 6 kombinasi
C. 9 kombinasi
D. 8 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (7 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 119**
Diberikan pita DNA mutasi string: `XSSSNSSOSNXOONOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 1 kombinasi
B. 2 kombinasi
C. 3 kombinasi
D. 5 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 120**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 3, 4, 3, 5, 6, 9, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 38 Juta Rupiah
C. 42 Juta Rupiah
D. 41 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`3`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`4`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`3`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`6`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`9`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`1`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **A**.
</details>

---
**Soal 121**
Diberikan pita DNA mutasi string: `OONXOOSSNXSXNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 22 kombinasi
B. 19 kombinasi
C. 21 kombinasi
D. 23 kombinasi
E. 20 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (20 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 6 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 7 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 10 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 20)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **20 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 122**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 4, 6, 6, 9, 6, 4, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 45 Juta Rupiah
C. 48 Juta Rupiah
D. 44 Juta Rupiah
E. 47 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`4`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`6`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`9`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`6`): Max Lokal = 36, Max Global = 36
- Indeks 6 (`4`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`6`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **A**.
</details>

---
**Soal 123**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 4, 4, 8, 6, 2, 1, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 36 Juta Rupiah
C. 39 Juta Rupiah
D. 38 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`4`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`8`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`2`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`8`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **A**.
</details>

---
**Soal 124**
Diberikan pita DNA mutasi string: `SNSXXONOXNONSSSONOSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 25 kombinasi
B. 22 kombinasi
C. 24 kombinasi
D. 26 kombinasi
E. 23 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (23 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 18 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 14)
- Indeks 19 (`N`): Panen Final! Tarik paksa rakitan array 14 buah `OS`. (Total Jawaban OSN = 23)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **23 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 125**
Diberikan pita DNA mutasi string: `OOSNXOSOXSNXNOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 20 kombinasi
B. 22 kombinasi
C. 21 kombinasi
D. 19 kombinasi
E. 23 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (20 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 11)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 20)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 14 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **20 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 126**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 9, 6, 2, 3, 8, 8, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 45 Juta Rupiah
C. 44 Juta Rupiah
D. 47 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`9`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`6`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`2`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`3`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`8`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`6`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **B**.
</details>

---
**Soal 127**
Diberikan pita DNA mutasi string: `ONONXSOXNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 4 kombinasi
C. 7 kombinasi
D. 5 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 128**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 4, 1, 7, 3, 7, 1, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 37 Juta Rupiah
D. 38 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`7`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`3`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`7`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`1`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`7`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **D**.
</details>

---
**Soal 129**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 9, 4, 6, 2, 7, 2, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 43 Juta Rupiah
C. 45 Juta Rupiah
D. 44 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`9`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`6`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`2`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`7`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`2`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`9`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **D**.
</details>

---
**Soal 130**
Diberikan pita DNA mutasi string: `XONOSNONNOOSSSOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 7 kombinasi
C. 9 kombinasi
D. 8 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 12 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 13 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 131**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 6, 4, 7, 2, 4, 4, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 38 Juta Rupiah
C. 37 Juta Rupiah
D. 36 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`6`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`4`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`7`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`2`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`4`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`4`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`6`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **C**.
</details>

---
**Soal 132**
Diberikan pita DNA mutasi string: `SXOXSOSOXNOXOSOOXSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 5 kombinasi
C. 3 kombinasi
D. 4 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 17 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)
- Indeks 18 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 22)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 133**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 1, 9, 3, 9, 4, 5, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 37 Juta Rupiah
C. 39 Juta Rupiah
D. 40 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`1`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`9`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`3`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`9`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`5`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`1`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **C**.
</details>

---
**Soal 134**
Diberikan pita DNA mutasi string: `SOOSOSNSOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 6 kombinasi
C. 4 kombinasi
D. 7 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 135**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 3, 2, 8, 9, 2, 4, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 43 Juta Rupiah
C. 41 Juta Rupiah
D. 40 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`3`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`2`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`8`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`9`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`2`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`4`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`7`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **A**.
</details>

---
**Soal 136**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 3, 3, 3, 2, 8, 9, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 39 Juta Rupiah
C. 37 Juta Rupiah
D. 38 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`3`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`3`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`3`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`2`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`8`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`9`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`4`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **B**.
</details>

---
**Soal 137**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 6, 4, 2, 2, 6, 9, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 35 Juta Rupiah
B. 37 Juta Rupiah
C. 38 Juta Rupiah
D. 39 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`6`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`4`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`2`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`2`): Max Lokal = 20, Max Global = 20
- Indeks 5 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`9`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`2`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **B**.
</details>

---
**Soal 138**
Diberikan pita DNA mutasi string: `XXSSXSONXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 0 kombinasi
C. 1 kombinasi
D. 5 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 139**
Diberikan pita DNA mutasi string: `OSXOXONSOONSNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 25 kombinasi
B. 26 kombinasi
C. 23 kombinasi
D. 24 kombinasi
E. 22 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (23 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 14)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 23)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **23 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 140**
Diberikan pita DNA mutasi string: `NNXNSOSSONOOSSXNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 21 kombinasi
B. 24 kombinasi
C. 25 kombinasi
D. 23 kombinasi
E. 22 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (22 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 22)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **22 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 141**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 5, 2, 1, 2, 5, 2, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 33 Juta Rupiah
B. 31 Juta Rupiah
C. 34 Juta Rupiah
D. 32 Juta Rupiah
E. 30 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`5`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`2`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`1`): Max Lokal = 14, Max Global = 14
- Indeks 4 (`2`): Max Lokal = 16, Max Global = 16
- Indeks 5 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 6 (`2`): Max Lokal = 23, Max Global = 23
- Indeks 7 (`9`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **D**.
</details>

---
**Soal 142**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 2, 5, 7, 9, 3, 3, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 36 Juta Rupiah
B. 32 Juta Rupiah
C. 34 Juta Rupiah
D. 35 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`2`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`5`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`7`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`9`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`3`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`3`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`3`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **C**.
</details>

---
**Soal 143**
Diberikan pita DNA mutasi string: `NOOONSNSSSSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 6 kombinasi
C. 5 kombinasi
D. 3 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 144**
Diberikan pita DNA mutasi string: `NSSONNNOSNSONXXSNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 15 kombinasi
B. 13 kombinasi
C. 14 kombinasi
D. 12 kombinasi
E. 16 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (13 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 7 buah `OS`. (Total Jawaban OSN = 13)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **13 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 145**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 5, 3, 1, 5, 6, 1, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 32 Juta Rupiah
C. 30 Juta Rupiah
D. 31 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`5`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`3`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`1`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`5`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`6`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`1`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`2`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **B**.
</details>

---
**Soal 146**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 5, 7, 5, 4, 2, 6, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 35 Juta Rupiah
C. 36 Juta Rupiah
D. 39 Juta Rupiah
E. 37 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`5`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`7`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`5`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`4`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`2`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`6`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`5`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **E**.
</details>

---
**Soal 147**
Diberikan pita DNA mutasi string: `SONNXSNNSOSXXNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 5 kombinasi
C. 9 kombinasi
D. 8 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 148**
Diberikan pita DNA mutasi string: `NXXONXSSOONOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 1 kombinasi
C. 3 kombinasi
D. 2 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 149**
Diberikan pita DNA mutasi string: `SSNOSOXSNNNXNONSOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 16 kombinasi
B. 18 kombinasi
C. 17 kombinasi
D. 14 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (15 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 15)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 17 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **15 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 150**
Diberikan pita DNA mutasi string: `OXNSNNXXNXXONNOOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 7 kombinasi
B. 6 kombinasi
C. 8 kombinasi
D. 4 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
