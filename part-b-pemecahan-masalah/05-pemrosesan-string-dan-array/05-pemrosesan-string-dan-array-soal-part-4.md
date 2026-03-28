# Latihan Soal: String & Array Processing (Part 4 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 151**
Diberikan pita DNA mutasi string: `OXOSSSNXXXNOXOONSNNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 41 kombinasi
B. 42 kombinasi
C. 43 kombinasi
D. 40 kombinasi
E. 39 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (40 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 18)
- Indeks 16 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 29)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 40)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **40 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 152**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 6, 2, 5, 6, 6, 4, 3]`.
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
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`6`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`2`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`5`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`6`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`6`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`4`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`3`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **D**.
</details>

---
**Soal 153**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 4, 7, 8, 9, 5, 3, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 39 Juta Rupiah
C. 38 Juta Rupiah
D. 37 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`4`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`9`): Max Lokal = 30, Max Global = 30
- Indeks 5 (`5`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`3`): Max Lokal = 38, Max Global = 38
- Indeks 7 (`1`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **B**.
</details>

---
**Soal 154**
Diberikan pita DNA mutasi string: `OSXOSNSXSOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 4 kombinasi
C. 6 kombinasi
D. 2 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 155**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 5, 3, 1, 2, 6, 4, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 29 Juta Rupiah
B. 31 Juta Rupiah
C. 28 Juta Rupiah
D. 30 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`5`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`3`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`1`): Max Lokal = 15, Max Global = 15
- Indeks 4 (`2`): Max Lokal = 17, Max Global = 17
- Indeks 5 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 6 (`4`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`3`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **D**.
</details>

---
**Soal 156**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 3, 5, 5, 2, 5, 9, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 32 Juta Rupiah
B. 33 Juta Rupiah
C. 29 Juta Rupiah
D. 30 Juta Rupiah
E. 31 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (31 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`3`): Max Lokal = 4, Max Global = 4
- Indeks 2 (`5`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`5`): Max Lokal = 14, Max Global = 14
- Indeks 4 (`2`): Max Lokal = 16, Max Global = 16
- Indeks 5 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 6 (`9`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`1`): Max Lokal = 31, Max Global = 31


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **31**. Opsi tervalid adalah **E**.
</details>

---
**Soal 157**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 4, 6, 9, 6, 3, 1, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 32 Juta Rupiah
B. 30 Juta Rupiah
C. 34 Juta Rupiah
D. 31 Juta Rupiah
E. 33 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (32 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`4`): Max Lokal = 5, Max Global = 5
- Indeks 2 (`6`): Max Lokal = 11, Max Global = 11
- Indeks 3 (`9`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`1`): Max Lokal = 30, Max Global = 30
- Indeks 7 (`2`): Max Lokal = 32, Max Global = 32


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **32**. Opsi tervalid adalah **A**.
</details>

---
**Soal 158**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 5, 2, 3, 9, 3, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 41 Juta Rupiah
C. 38 Juta Rupiah
D. 39 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`5`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`2`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`3`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`9`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`3`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`4`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **D**.
</details>

---
**Soal 159**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 5, 8, 1, 7, 8, 1, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 36 Juta Rupiah
B. 35 Juta Rupiah
C. 38 Juta Rupiah
D. 39 Juta Rupiah
E. 37 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`5`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`8`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`7`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`1`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`5`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **E**.
</details>

---
**Soal 160**
Diberikan pita DNA mutasi string: `XXSOSSNOXNSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 11 kombinasi
C. 7 kombinasi
D. 10 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 161**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 5, 4, 8, 8, 4, 7, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 48 Juta Rupiah
C. 52 Juta Rupiah
D. 51 Juta Rupiah
E. 50 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (50 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`5`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`4`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`8`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`8`): Max Lokal = 32, Max Global = 32
- Indeks 5 (`4`): Max Lokal = 36, Max Global = 36
- Indeks 6 (`7`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`7`): Max Lokal = 50, Max Global = 50


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **50**. Opsi tervalid adalah **E**.
</details>

---
**Soal 162**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 4, 7, 3, 8, 1, 6, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 41 Juta Rupiah
D. 38 Juta Rupiah
E. 42 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`4`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`7`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`3`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`8`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`1`): Max Lokal = 30, Max Global = 30
- Indeks 6 (`6`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`4`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **B**.
</details>

---
**Soal 163**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 4, 8, 3, 7, 3, 7, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 46 Juta Rupiah
B. 45 Juta Rupiah
C. 42 Juta Rupiah
D. 44 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`4`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`3`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`7`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`3`): Max Lokal = 34, Max Global = 34
- Indeks 6 (`7`): Max Lokal = 41, Max Global = 41
- Indeks 7 (`3`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **D**.
</details>

---
**Soal 164**
Diberikan pita DNA mutasi string: `OSNONXSSOSXSXNXNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 23 kombinasi
B. 26 kombinasi
C. 27 kombinasi
D. 24 kombinasi
E. 25 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (24 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 13)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 24)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **24 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 165**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 8, 8, 5, 2, 4, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 43 Juta Rupiah
C. 45 Juta Rupiah
D. 44 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 3 (`8`): Max Lokal = 29, Max Global = 29
- Indeks 4 (`5`): Max Lokal = 34, Max Global = 34
- Indeks 5 (`2`): Max Lokal = 36, Max Global = 36
- Indeks 6 (`4`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`4`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **D**.
</details>

---
**Soal 166**
Diberikan pita DNA mutasi string: `SSSNSOSOXNONS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 1 kombinasi
B. 2 kombinasi
C. 5 kombinasi
D. 4 kombinasi
E. 3 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 167**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 7, 4, 5, 4, 5, 7, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 38 Juta Rupiah
C. 40 Juta Rupiah
D. 39 Juta Rupiah
E. 36 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`7`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`4`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`5`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`5`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`7`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`4`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **B**.
</details>

---
**Soal 168**
Diberikan pita DNA mutasi string: `OOSOSNOONX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 12 kombinasi
B. 11 kombinasi
C. 10 kombinasi
D. 13 kombinasi
E. 9 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (10 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 10)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **10 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 169**
Diberikan pita DNA mutasi string: `XNNSSSONOSONSNXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 7 kombinasi
C. 9 kombinasi
D. 8 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (7 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 170**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 1, 4, 5, 3, 2, 3, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 24 Juta Rupiah
B. 26 Juta Rupiah
C. 27 Juta Rupiah
D. 25 Juta Rupiah
E. 28 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (26 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`1`): Max Lokal = 5, Max Global = 5
- Indeks 2 (`4`): Max Lokal = 9, Max Global = 9
- Indeks 3 (`5`): Max Lokal = 14, Max Global = 14
- Indeks 4 (`3`): Max Lokal = 17, Max Global = 17
- Indeks 5 (`2`): Max Lokal = 19, Max Global = 19
- Indeks 6 (`3`): Max Lokal = 22, Max Global = 22
- Indeks 7 (`4`): Max Lokal = 26, Max Global = 26


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **26**. Opsi tervalid adalah **B**.
</details>

---
**Soal 171**
Diberikan pita DNA mutasi string: `XNNSNSSOOOOSOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 2 kombinasi
C. 1 kombinasi
D. 5 kombinasi
E. 0 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 172**
Diberikan pita DNA mutasi string: `SONNXSSNXXSOOOOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 2 kombinasi
C. 5 kombinasi
D. 1 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 173**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 9, 6, 8, 2, 6, 8, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 47 Juta Rupiah
C. 45 Juta Rupiah
D. 48 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (47 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`9`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`6`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`8`): Max Lokal = 27, Max Global = 27
- Indeks 4 (`2`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`6`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`8`): Max Lokal = 43, Max Global = 43
- Indeks 7 (`4`): Max Lokal = 47, Max Global = 47


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **47**. Opsi tervalid adalah **B**.
</details>

---
**Soal 174**
Diberikan pita DNA mutasi string: `OOSONSNOOSXSOSNNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 48 kombinasi
B. 52 kombinasi
C. 51 kombinasi
D. 50 kombinasi
E. 49 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (49 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 9 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 15)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 13 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 21)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 21 buah `OS`. (Total Jawaban OSN = 28)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 21 buah `OS`. (Total Jawaban OSN = 49)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **49 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 175**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 6, 6, 4, 6, 3, 3, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 30 Juta Rupiah
B. 28 Juta Rupiah
C. 31 Juta Rupiah
D. 29 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`6`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`4`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`3`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`1`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **A**.
</details>

---
**Soal 176**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 6, 7, 4, 8, 1, 1, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 30 Juta Rupiah
B. 29 Juta Rupiah
C. 28 Juta Rupiah
D. 31 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (30 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`6`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`7`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`8`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`1`): Max Lokal = 28, Max Global = 28
- Indeks 7 (`2`): Max Lokal = 30, Max Global = 30


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **30**. Opsi tervalid adalah **A**.
</details>

---
**Soal 177**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 4, 2, 6, 8, 4, 7, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 41 Juta Rupiah
C. 42 Juta Rupiah
D. 40 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`4`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`2`): Max Lokal = 11, Max Global = 11
- Indeks 3 (`6`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`8`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 6 (`7`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`4`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **D**.
</details>

---
**Soal 178**
Diberikan pita DNA mutasi string: `ONXXONNSXNNNXNNXONNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 17 kombinasi
B. 14 kombinasi
C. 16 kombinasi
D. 13 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (14 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 10)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 14)
- Indeks 19 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **14 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 179**
Diberikan pita DNA mutasi string: `XOXONXXNSSSNXNOSNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 29 kombinasi
B. 31 kombinasi
C. 32 kombinasi
D. 33 kombinasi
E. 30 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (30 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 15 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 21)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 30)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **30 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 180**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 1, 5, 1, 6, 5, 7, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 42 Juta Rupiah
C. 38 Juta Rupiah
D. 40 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`1`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`5`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 4 (`6`): Max Lokal = 19, Max Global = 19
- Indeks 5 (`5`): Max Lokal = 24, Max Global = 24
- Indeks 6 (`7`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`9`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **D**.
</details>

---
**Soal 181**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 9, 8, 4, 8, 9, 3, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 54 Juta Rupiah
B. 53 Juta Rupiah
C. 56 Juta Rupiah
D. 57 Juta Rupiah
E. 55 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (55 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`9`): Max Lokal = 18, Max Global = 18
- Indeks 2 (`8`): Max Lokal = 26, Max Global = 26
- Indeks 3 (`4`): Max Lokal = 30, Max Global = 30
- Indeks 4 (`8`): Max Lokal = 38, Max Global = 38
- Indeks 5 (`9`): Max Lokal = 47, Max Global = 47
- Indeks 6 (`3`): Max Lokal = 50, Max Global = 50
- Indeks 7 (`5`): Max Lokal = 55, Max Global = 55


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **55**. Opsi tervalid adalah **E**.
</details>

---
**Soal 182**
Diberikan pita DNA mutasi string: `OSONXONSNXSSNONOOOSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 43 kombinasi
B. 45 kombinasi
C. 44 kombinasi
D. 46 kombinasi
E. 42 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (43 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 10 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 16)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 10 buah `OS`. (Total Jawaban OSN = 26)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 18 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 19 (`N`): Panen Final! Tarik paksa rakitan array 17 buah `OS`. (Total Jawaban OSN = 43)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **43 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 183**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 8, 9, 6, 9, 4, 7, 9]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 57 Juta Rupiah
B. 58 Juta Rupiah
C. 60 Juta Rupiah
D. 59 Juta Rupiah
E. 56 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (58 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`9`): Max Lokal = 23, Max Global = 23
- Indeks 3 (`6`): Max Lokal = 29, Max Global = 29
- Indeks 4 (`9`): Max Lokal = 38, Max Global = 38
- Indeks 5 (`4`): Max Lokal = 42, Max Global = 42
- Indeks 6 (`7`): Max Lokal = 49, Max Global = 49
- Indeks 7 (`9`): Max Lokal = 58, Max Global = 58


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **58**. Opsi tervalid adalah **B**.
</details>

---
**Soal 184**
Diberikan pita DNA mutasi string: `XXSSSOSSNOSSS`.
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
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 12 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 185**
Diberikan pita DNA mutasi string: `OSOSNSONOSNNNNXNSSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 53 kombinasi
B. 52 kombinasi
C. 55 kombinasi
D. 54 kombinasi
E. 56 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (53 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 17)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 26)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 35)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 44)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 53)
- Indeks 16 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 17 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **53 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 186**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[9, 7, 6, 2, 9, 5, 6, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 53 Juta Rupiah
B. 49 Juta Rupiah
C. 52 Juta Rupiah
D. 50 Juta Rupiah
E. 51 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (51 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`9`): Max Lokal = 9, Max Global = 9
- Indeks 1 (`7`): Max Lokal = 16, Max Global = 16
- Indeks 2 (`6`): Max Lokal = 22, Max Global = 22
- Indeks 3 (`2`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`9`): Max Lokal = 33, Max Global = 33
- Indeks 5 (`5`): Max Lokal = 38, Max Global = 38
- Indeks 6 (`6`): Max Lokal = 44, Max Global = 44
- Indeks 7 (`7`): Max Lokal = 51, Max Global = 51


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **51**. Opsi tervalid adalah **E**.
</details>

---
**Soal 187**
Diberikan pita DNA mutasi string: `OONSNOXNOOOXOSOXSSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 7 kombinasi
B. 3 kombinasi
C. 4 kombinasi
D. 5 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (4 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 13 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 8)
- Indeks 16 (`S`): Kawinkan dengan 8 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 17 (`S`): Kawinkan dengan 8 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 25)
- Indeks 18 (`S`): Kawinkan dengan 8 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 33)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **4 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 188**
Diberikan pita DNA mutasi string: `XNSOSNNOSXOOXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 5 kombinasi
C. 3 kombinasi
D. 4 kombinasi
E. 1 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 189**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 1, 4, 3, 6, 5, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 36 Juta Rupiah
C. 40 Juta Rupiah
D. 39 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`1`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`3`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`6`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`5`): Max Lokal = 32, Max Global = 32
- Indeks 7 (`6`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **E**.
</details>

---
**Soal 190**
Diberikan pita DNA mutasi string: `SOSOXSSSSSNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 10 kombinasi
B. 12 kombinasi
C. 13 kombinasi
D. 11 kombinasi
E. 14 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (11 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 11)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **11 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 191**
Diberikan pita DNA mutasi string: `XXXOSSSOOSNOXNOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 15 kombinasi
B. 13 kombinasi
C. 14 kombinasi
D. 11 kombinasi
E. 12 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 192**
Diberikan pita DNA mutasi string: `OSSSNXONXOXXNXON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 11 kombinasi
B. 13 kombinasi
C. 14 kombinasi
D. 12 kombinasi
E. 15 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 193**
Diberikan pita DNA mutasi string: `OSNXSOOSSXXONSSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 12 kombinasi
B. 9 kombinasi
C. 8 kombinasi
D. 10 kombinasi
E. 11 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 13 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)
- Indeks 14 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 16)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 20)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 194**
Diberikan pita DNA mutasi string: `OXSNSOOONSOSXO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 5 kombinasi
C. 4 kombinasi
D. 2 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 9 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 195**
Diberikan pita DNA mutasi string: `XXNXNNSOXNSSX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 4 kombinasi
C. 1 kombinasi
D. 3 kombinasi
E. 0 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 11 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 196**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 8, 1, 8, 1, 7, 8, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 36 Juta Rupiah
C. 39 Juta Rupiah
D. 37 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (37 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`8`): Max Lokal = 11, Max Global = 11
- Indeks 2 (`1`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`8`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`1`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`7`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`8`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`1`): Max Lokal = 37, Max Global = 37


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **37**. Opsi tervalid adalah **D**.
</details>

---
**Soal 197**
Diberikan pita DNA mutasi string: `OOOXNXNSXO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 1 kombinasi
B. 0 kombinasi
C. 2 kombinasi
D. 3 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 198**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 4, 3, 7, 3, 6, 8, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 40 Juta Rupiah
B. 39 Juta Rupiah
C. 42 Juta Rupiah
D. 43 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`4`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`3`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`7`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`3`): Max Lokal = 20, Max Global = 20
- Indeks 5 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 6 (`8`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`7`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **E**.
</details>

---
**Soal 199**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 8, 6, 7, 3, 2, 9, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 42 Juta Rupiah
C. 41 Juta Rupiah
D. 40 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`8`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`6`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`7`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`3`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`2`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`9`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`4`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **D**.
</details>

---
**Soal 200**
Diberikan pita DNA mutasi string: `SOSOSXOONOOONNSSSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 12 kombinasi
C. 11 kombinasi
D. 10 kombinasi
E. 9 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 14 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 15 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 17)
- Indeks 16 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 24)
- Indeks 17 (`S`): Kawinkan dengan 7 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 31)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
