🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: String & Array Processing (Part 1 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 1**
Diberikan pita DNA mutasi string: `OSXSXNXSXXNSOSXOSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 14 kombinasi
B. 16 kombinasi
C. 13 kombinasi
D. 15 kombinasi
E. 17 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (14 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 11 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 13 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 16 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **14 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 2**
Diberikan pita DNA mutasi string: `SXNNOOOSOXON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 2 kombinasi
C. 6 kombinasi
D. 5 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 3**
Diberikan pita DNA mutasi string: `XSXOOOSNNSXXNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 13 kombinasi
B. 11 kombinasi
C. 12 kombinasi
D. 14 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 4**
Diberikan pita DNA mutasi string: `SSSXNONNSOXOSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 7 kombinasi
C. 3 kombinasi
D. 6 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 5**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 9, 6, 8, 8, 8, 4, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 60 Juta Rupiah
B. 62 Juta Rupiah
C. 63 Juta Rupiah
D. 59 Juta Rupiah
E. 61 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (61 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 2 (`6`): Max Lokal = 24, Max Global = 24
- Indeks 3 (`8`): Max Lokal = 32, Max Global = 32
- Indeks 4 (`8`): Max Lokal = 40, Max Global = 40
- Indeks 5 (`8`): Max Lokal = 48, Max Global = 48
- Indeks 6 (`4`): Max Lokal = 52, Max Global = 52
- Indeks 7 (`9`): Max Lokal = 61, Max Global = 61


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **61**. Opsi tervalid adalah **E**.
</details>

---
**Soal 6**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 8, 2, 6, 3, 3, 7, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 40 Juta Rupiah
C. 44 Juta Rupiah
D. 41 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`3`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`7`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`6`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **E**.
</details>

---
**Soal 7**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 7, 7, 9, 1, 9, 9, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 56 Juta Rupiah
B. 54 Juta Rupiah
C. 57 Juta Rupiah
D. 53 Juta Rupiah
E. 55 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (55 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`7`): Max Lokal = 16, Max Global = 16
- Indeks 2 (`7`): Max Lokal = 23, Max Global = 23
- Indeks 3 (`9`): Max Lokal = 32, Max Global = 32
- Indeks 4 (`1`): Max Lokal = 33, Max Global = 33
- Indeks 5 (`9`): Max Lokal = 42, Max Global = 42
- Indeks 6 (`9`): Max Lokal = 51, Max Global = 51
- Indeks 7 (`4`): Max Lokal = 55, Max Global = 55


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **55**. Opsi tervalid adalah **E**.
</details>

---
**Soal 8**
Diberikan pita DNA mutasi string: `SOXXOXSNSOXOXSNNOSON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 32 kombinasi
B. 33 kombinasi
C. 30 kombinasi
D. 34 kombinasi
E. 31 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (31 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 17 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 19 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 31)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **31 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 9**
Diberikan pita DNA mutasi string: `XSOSXXONNSONSOSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 5 kombinasi
C. 8 kombinasi
D. 4 kombinasi
E. 7 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 10**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 8, 5, 8, 3, 8, 8, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 50 Juta Rupiah
B. 47 Juta Rupiah
C. 46 Juta Rupiah
D. 49 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (48 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`8`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`5`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`8`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`3`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`8`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`8`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`7`): Max Lokal = 48, Max Global = 48


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **48**. Opsi tervalid adalah **E**.
</details>

---
**Soal 11**
Diberikan pita DNA mutasi string: `OXXSOONSOSXNS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 12 kombinasi
B. 11 kombinasi
C. 9 kombinasi
D. 10 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 12**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 3, 1, 7, 5, 8, 8, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 51 Juta Rupiah
B. 49 Juta Rupiah
C. 47 Juta Rupiah
D. 50 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`3`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`1`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`7`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`8`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`8`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`9`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **B**.
</details>

---
**Soal 13**
Diberikan pita DNA mutasi string: `XSNXXSNXONNOSXOSXX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 1 kombinasi
B. 3 kombinasi
C. 0 kombinasi
D. 5 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 12 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 14**
Diberikan pita DNA mutasi string: `XOONSNSOSNSOXXSOSSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 8 kombinasi
C. 12 kombinasi
D. 11 kombinasi
E. 9 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 7 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 14)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 16 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 19)
- Indeks 17 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 24)
- Indeks 18 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 29)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 15**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 5, 8, 6, 3, 6, 7, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 36 Juta Rupiah
C. 35 Juta Rupiah
D. 38 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`5`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`6`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`3`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`6`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`7`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`1`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **A**.
</details>

---
**Soal 16**
Diberikan pita DNA mutasi string: `ONNXNSSSSNSSNNNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 21 kombinasi
B. 23 kombinasi
C. 24 kombinasi
D. 25 kombinasi
E. 22 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (22 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 11 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 16)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 22)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **22 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 17**
Diberikan pita DNA mutasi string: `XOSXXXSNNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 6 kombinasi
C. 4 kombinasi
D. 7 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 18**
Diberikan pita DNA mutasi string: `SSXSNOOXONS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 2 kombinasi
C. 0 kombinasi
D. 3 kombinasi
E. 1 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 19**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 6, 7, 3, 7, 5, 4, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 48 Juta Rupiah
C. 52 Juta Rupiah
D. 50 Juta Rupiah
E. 51 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (50 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 3 (`3`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`7`): Max Lokal = 32, Max Global = 32
- Indeks 5 (`5`): Max Lokal = 37, Max Global = 37
- Indeks 6 (`4`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`9`): Max Lokal = 50, Max Global = 50


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **50**. Opsi tervalid adalah **D**.
</details>

---
**Soal 20**
Diberikan pita DNA mutasi string: `SXXXNXOONSOSSNNXON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 25 kombinasi
B. 24 kombinasi
C. 23 kombinasi
D. 27 kombinasi
E. 26 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (24 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 16)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 24)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **24 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 21**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 3, 1, 4, 9, 8, 5, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 39 Juta Rupiah
C. 37 Juta Rupiah
D. 41 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`3`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`1`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`4`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`9`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`8`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`5`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`1`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **B**.
</details>

---
**Soal 22**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 3, 6, 2, 1, 9, 6, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 35 Juta Rupiah
C. 39 Juta Rupiah
D. 36 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`3`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`6`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`2`): Max Lokal = 12, Max Global = 12
- Indeks 4 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 5 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`6`): Max Lokal = 28, Max Global = 28
- Indeks 7 (`9`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **A**.
</details>

---
**Soal 23**
Diberikan pita DNA mutasi string: `OOSNSSXSSSNXNOSSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 43 kombinasi
B. 46 kombinasi
C. 44 kombinasi
D. 45 kombinasi
E. 47 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (44 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 14)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 12 buah `OS`. (Total Jawaban OSN = 26)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 18)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 18 buah `OS`. (Total Jawaban OSN = 44)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **44 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 24**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 4, 3, 3, 7, 3, 9, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 31 Juta Rupiah
B. 32 Juta Rupiah
C. 35 Juta Rupiah
D. 33 Juta Rupiah
E. 34 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (33 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`4`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`3`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`3`): Max Lokal = 12, Max Global = 12
- Indeks 4 (`7`): Max Lokal = 19, Max Global = 19
- Indeks 5 (`3`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`2`): Max Lokal = 33, Max Global = 33


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **33**. Opsi tervalid adalah **D**.
</details>

---
**Soal 25**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 8, 9, 8, 8, 3, 7, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 56 Juta Rupiah
B. 54 Juta Rupiah
C. 57 Juta Rupiah
D. 55 Juta Rupiah
E. 58 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (56 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`9`): Max Lokal = 23, Max Global = 23
- Indeks 3 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 4 (`8`): Max Lokal = 39, Max Global = 39
- Indeks 5 (`3`): Max Lokal = 42, Max Global = 42
- Indeks 6 (`7`): Max Lokal = 49, Max Global = 49
- Indeks 7 (`7`): Max Lokal = 56, Max Global = 56


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **56**. Opsi tervalid adalah **A**.
</details>

---
**Soal 26**
Diberikan pita DNA mutasi string: `SSSOXOOSNONONSSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 24 kombinasi
B. 21 kombinasi
C. 22 kombinasi
D. 23 kombinasi
E. 25 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (22 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 13 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 14 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 22)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **22 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 27**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 9, 5, 9, 8, 4, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 48 Juta Rupiah
B. 50 Juta Rupiah
C. 47 Juta Rupiah
D. 51 Juta Rupiah
E. 49 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 3 (`5`): Max Lokal = 27, Max Global = 27
- Indeks 4 (`9`): Max Lokal = 36, Max Global = 36
- Indeks 5 (`8`): Max Lokal = 44, Max Global = 44
- Indeks 6 (`4`): Max Lokal = 48, Max Global = 48
- Indeks 7 (`1`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **E**.
</details>

---
**Soal 28**
Diberikan pita DNA mutasi string: `SNOOXNNSSXNNOSO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 7 kombinasi
C. 11 kombinasi
D. 10 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 29**
Diberikan pita DNA mutasi string: `NOSOONXOSONO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 7 kombinasi
B. 9 kombinasi
C. 6 kombinasi
D. 5 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 30**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 2, 9, 7, 3, 3, 4, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 39 Juta Rupiah
C. 42 Juta Rupiah
D. 38 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`2`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`9`): Max Lokal = 20, Max Global = 20
- Indeks 3 (`7`): Max Lokal = 27, Max Global = 27
- Indeks 4 (`3`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`3`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`4`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`3`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **A**.
</details>

---
**Soal 31**
Diberikan pita DNA mutasi string: `ONXXNSSOOXNSXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 8 kombinasi
C. 9 kombinasi
D. 7 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (7 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 32**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 9, 2, 5, 8, 6, 5, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 44 Juta Rupiah
B. 47 Juta Rupiah
C. 45 Juta Rupiah
D. 46 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`9`): Max Lokal = 17, Max Global = 17
- Indeks 2 (`2`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`8`): Max Lokal = 32, Max Global = 32
- Indeks 5 (`6`): Max Lokal = 38, Max Global = 38
- Indeks 6 (`5`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`3`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **D**.
</details>

---
**Soal 33**
Diberikan pita DNA mutasi string: `XSNXNNSXNNSOOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 1 kombinasi
C. 0 kombinasi
D. 3 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 13 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 34**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 2, 7, 9, 1, 7, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 40 Juta Rupiah
C. 38 Juta Rupiah
D. 39 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`2`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`9`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`1`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`7`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`1`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **B**.
</details>

---
**Soal 35**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 4, 4, 5, 7, 7, 4, 3]`.
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
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`4`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`4`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`5`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`7`): Max Lokal = 24, Max Global = 24
- Indeks 5 (`7`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`4`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`3`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **B**.
</details>

---
**Soal 36**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 7, 6, 8, 4, 4, 7, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 48 Juta Rupiah
C. 50 Juta Rupiah
D. 47 Juta Rupiah
E. 51 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (49 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`7`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`6`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`8`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`7`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`9`): Max Lokal = 49, Max Global = 49


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **49**. Opsi tervalid adalah **A**.
</details>

---
**Soal 37**
Diberikan pita DNA mutasi string: `NNONSSSNNNNSSSOSXSNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 25 kombinasi
B. 24 kombinasi
C. 21 kombinasi
D. 22 kombinasi
E. 23 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (22 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 11 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 12 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 13 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 15 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 17 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 22)
- Indeks 19 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **22 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 38**
Diberikan pita DNA mutasi string: `ONXSSOXSOXOOSNNS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 19 kombinasi
B. 17 kombinasi
C. 18 kombinasi
D. 21 kombinasi
E. 20 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (18 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 12 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 15 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 14)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **18 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 39**
Diberikan pita DNA mutasi string: `XOSSNSSOXXNXNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 9 kombinasi
C. 12 kombinasi
D. 11 kombinasi
E. 13 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (10 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **10 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 40**
Diberikan pita DNA mutasi string: `ONXXONXOSONSOSO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 6 kombinasi
B. 3 kombinasi
C. 5 kombinasi
D. 4 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 41**
Diberikan pita DNA mutasi string: `ONONNOXNXSOXOOSOSO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 1 kombinasi
C. 2 kombinasi
D. 0 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 14 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 16 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 16)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 42**
Diberikan pita DNA mutasi string: `OSXNNSXNSNONSNXO`.
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
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 12 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 15)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **15 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 43**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 6, 1, 1, 6, 9, 1, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 29 Juta Rupiah
B. 30 Juta Rupiah
C. 28 Juta Rupiah
D. 27 Juta Rupiah
E. 26 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (28 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`6`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`1`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`1`): Max Lokal = 11, Max Global = 11
- Indeks 4 (`6`): Max Lokal = 17, Max Global = 17
- Indeks 5 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`1`): Max Lokal = 28, Max Global = 28


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **28**. Opsi tervalid adalah **C**.
</details>

---
**Soal 44**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 9, 9, 4, 1, 9, 1, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 44 Juta Rupiah
C. 42 Juta Rupiah
D. 41 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`9`): Max Lokal = 15, Max Global = 15
- Indeks 2 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 3 (`4`): Max Lokal = 28, Max Global = 28
- Indeks 4 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`9`): Max Lokal = 38, Max Global = 38
- Indeks 6 (`1`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`4`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **E**.
</details>

---
**Soal 45**
Diberikan pita DNA mutasi string: `OOXONSNSNSOSOSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 26 kombinasi
B. 29 kombinasi
C. 27 kombinasi
D. 30 kombinasi
E. 28 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (27 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 13 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 18)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 18 buah `OS`. (Total Jawaban OSN = 27)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **27 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 46**
Diberikan pita DNA mutasi string: `SSNOSSXSOSOOSO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 1 kombinasi
C. 2 kombinasi
D. 3 kombinasi
E. 0 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 47**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 8, 2, 7, 2, 9, 4, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 35 Juta Rupiah
B. 36 Juta Rupiah
C. 37 Juta Rupiah
D. 33 Juta Rupiah
E. 34 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`8`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`2`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`7`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`2`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`9`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`4`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`1`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **A**.
</details>

---
**Soal 48**
Diberikan pita DNA mutasi string: `SSSOOXOSOXOOSSXSXXNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 22 kombinasi
B. 23 kombinasi
C. 24 kombinasi
D. 21 kombinasi
E. 20 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (21 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 12 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 13 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)
- Indeks 15 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 21)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 21 buah `OS`. (Total Jawaban OSN = 21)
- Indeks 19 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **21 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 49**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 1, 7, 7, 4, 3, 2, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 35 Juta Rupiah
B. 34 Juta Rupiah
C. 33 Juta Rupiah
D. 37 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (35 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`1`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`7`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`4`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`3`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`2`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`5`): Max Lokal = 35, Max Global = 35


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **35**. Opsi tervalid adalah **A**.
</details>

---
**Soal 50**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 5, 9, 8, 3, 7, 9, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 47 Juta Rupiah
B. 48 Juta Rupiah
C. 49 Juta Rupiah
D. 46 Juta Rupiah
E. 45 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (47 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`5`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`9`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`8`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`3`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`7`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`9`): Max Lokal = 42, Max Global = 42
- Indeks 7 (`5`): Max Lokal = 47, Max Global = 47


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **47**. Opsi tervalid adalah **A**.
</details>

---
