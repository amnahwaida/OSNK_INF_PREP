🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: String & Array Processing (Part 5 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **String & Array Processing**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 201**
Diberikan pita DNA mutasi string: `NXSSXXNSONS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 1 kombinasi
C. 3 kombinasi
D. 5 kombinasi
E. 0 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 7 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 202**
Diberikan pita DNA mutasi string: `SOSNOONNNOXXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 7 kombinasi
B. 5 kombinasi
C. 4 kombinasi
D. 8 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 203**
Diberikan pita DNA mutasi string: `XOSNSOSXSXXSNNN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 27 kombinasi
B. 28 kombinasi
C. 25 kombinasi
D. 26 kombinasi
E. 24 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (25 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 11 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 17)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 25)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **25 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 204**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 6, 3, 8, 7, 7, 4, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 43 Juta Rupiah
C. 46 Juta Rupiah
D. 42 Juta Rupiah
E. 44 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (44 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`6`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`3`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`7`): Max Lokal = 28, Max Global = 28
- Indeks 5 (`7`): Max Lokal = 35, Max Global = 35
- Indeks 6 (`4`): Max Lokal = 39, Max Global = 39
- Indeks 7 (`5`): Max Lokal = 44, Max Global = 44


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **44**. Opsi tervalid adalah **E**.
</details>

---
**Soal 205**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 8, 2, 5, 8, 4, 4, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 37 Juta Rupiah
C. 41 Juta Rupiah
D. 39 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (39 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`2`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`8`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`4`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`4`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`2`): Max Lokal = 39, Max Global = 39


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **39**. Opsi tervalid adalah **D**.
</details>

---
**Soal 206**
Diberikan pita DNA mutasi string: `SXSNNSXNNSONNSON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 0 kombinasi
B. 4 kombinasi
C. 2 kombinasi
D. 1 kombinasi
E. 3 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (1 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 13 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **1 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 207**
Diberikan pita DNA mutasi string: `NSONOOSONONSSNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 19 kombinasi
B. 21 kombinasi
C. 20 kombinasi
D. 22 kombinasi
E. 18 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (19 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 6 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 12 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 19)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **19 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 208**
Diberikan pita DNA mutasi string: `XOSXNXONXONSNSOXX`.
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
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 7)
- Indeks 13 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **7 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 209**
Diberikan pita DNA mutasi string: `OXNOONOOSXNSOSOO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 4 kombinasi
C. 6 kombinasi
D. 7 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (5 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 8 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 5 buah `OS`. (Total Jawaban OSN = 5)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 10)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 13 (`S`): Kawinkan dengan 6 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 16)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **5 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 210**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 8, 5, 9, 3, 7, 1, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 44 Juta Rupiah
B. 41 Juta Rupiah
C. 42 Juta Rupiah
D. 40 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`8`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`5`): Max Lokal = 17, Max Global = 17
- Indeks 3 (`9`): Max Lokal = 26, Max Global = 26
- Indeks 4 (`3`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`7`): Max Lokal = 36, Max Global = 36
- Indeks 6 (`1`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`5`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **C**.
</details>

---
**Soal 211**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 9, 9, 3, 1, 6, 7, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 49 Juta Rupiah
B. 47 Juta Rupiah
C. 46 Juta Rupiah
D. 50 Juta Rupiah
E. 48 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (48 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`9`): Max Lokal = 14, Max Global = 14
- Indeks 2 (`9`): Max Lokal = 23, Max Global = 23
- Indeks 3 (`3`): Max Lokal = 26, Max Global = 26
- Indeks 4 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 5 (`6`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`7`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`8`): Max Lokal = 48, Max Global = 48


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **48**. Opsi tervalid adalah **E**.
</details>

---
**Soal 212**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 3, 8, 9, 8, 3, 6, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 51 Juta Rupiah
B. 50 Juta Rupiah
C. 52 Juta Rupiah
D. 53 Juta Rupiah
E. 54 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (52 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`3`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`8`): Max Lokal = 18, Max Global = 18
- Indeks 3 (`9`): Max Lokal = 27, Max Global = 27
- Indeks 4 (`8`): Max Lokal = 35, Max Global = 35
- Indeks 5 (`3`): Max Lokal = 38, Max Global = 38
- Indeks 6 (`6`): Max Lokal = 44, Max Global = 44
- Indeks 7 (`8`): Max Lokal = 52, Max Global = 52


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **52**. Opsi tervalid adalah **C**.
</details>

---
**Soal 213**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 3, 7, 4, 6, 2, 5, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 41 Juta Rupiah
C. 40 Juta Rupiah
D. 43 Juta Rupiah
E. 39 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (41 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`3`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`7`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`4`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`6`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`2`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`5`): Max Lokal = 33, Max Global = 33
- Indeks 7 (`8`): Max Lokal = 41, Max Global = 41


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **41**. Opsi tervalid adalah **B**.
</details>

---
**Soal 214**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[5, 5, 6, 7, 8, 1, 3, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 44 Juta Rupiah
C. 41 Juta Rupiah
D. 45 Juta Rupiah
E. 43 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (43 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`5`): Max Lokal = 5, Max Global = 5
- Indeks 1 (`5`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`6`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`7`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 5 (`1`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`3`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`8`): Max Lokal = 43, Max Global = 43


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **43**. Opsi tervalid adalah **E**.
</details>

---
**Soal 215**
Diberikan pita DNA mutasi string: `XXOXNOSXONXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 5 kombinasi
C. 4 kombinasi
D. 1 kombinasi
E. 2 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 216**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 5, 7, 9, 8, 9, 8, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 51 Juta Rupiah
B. 52 Juta Rupiah
C. 49 Juta Rupiah
D. 48 Juta Rupiah
E. 50 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (50 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`5`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`7`): Max Lokal = 15, Max Global = 15
- Indeks 3 (`9`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`8`): Max Lokal = 32, Max Global = 32
- Indeks 5 (`9`): Max Lokal = 41, Max Global = 41
- Indeks 6 (`8`): Max Lokal = 49, Max Global = 49
- Indeks 7 (`1`): Max Lokal = 50, Max Global = 50


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **50**. Opsi tervalid adalah **E**.
</details>

---
**Soal 217**
Diberikan pita DNA mutasi string: `SSNNXNOXSNSXNXSS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 2 kombinasi
C. 6 kombinasi
D. 3 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 10 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 14 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 15 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 218**
Diberikan pita DNA mutasi string: `OONOSXXNSSONSOONNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 37 kombinasi
B. 38 kombinasi
C. 39 kombinasi
D. 40 kombinasi
E. 41 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (38 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 4 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 9 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 9 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 12 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 25)
- Indeks 16 (`N`): Panen Final! Tarik paksa rakitan array 13 buah `OS`. (Total Jawaban OSN = 38)
- Indeks 17 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **38 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 219**
Diberikan pita DNA mutasi string: `XXXSOOSXXNSOSON`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 12 kombinasi
B. 8 kombinasi
C. 10 kombinasi
D. 9 kombinasi
E. 11 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 12 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 7 buah `OS`. (Total Jawaban OSN = 9)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 220**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 2, 8, 8, 3, 7, 3, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 39 Juta Rupiah
B. 40 Juta Rupiah
C. 41 Juta Rupiah
D. 42 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`2`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`8`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`8`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`3`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`7`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`3`): Max Lokal = 35, Max Global = 35
- Indeks 7 (`5`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **B**.
</details>

---
**Soal 221**
Diberikan pita DNA mutasi string: `OSXOXSOOXXONXNO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 6 kombinasi
C. 7 kombinasi
D. 9 kombinasi
E. 8 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: B (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **B**.
</details>

---
**Soal 222**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 4, 8, 1, 1, 4, 6, 1]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 30 Juta Rupiah
B. 29 Juta Rupiah
C. 31 Juta Rupiah
D. 27 Juta Rupiah
E. 28 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (29 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`4`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`8`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`1`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`1`): Max Lokal = 18, Max Global = 18
- Indeks 5 (`4`): Max Lokal = 22, Max Global = 22
- Indeks 6 (`6`): Max Lokal = 28, Max Global = 28
- Indeks 7 (`1`): Max Lokal = 29, Max Global = 29


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **29**. Opsi tervalid adalah **B**.
</details>

---
**Soal 223**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 8, 4, 8, 5, 1, 9, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 37 Juta Rupiah
B. 36 Juta Rupiah
C. 39 Juta Rupiah
D. 40 Juta Rupiah
E. 38 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`8`): Max Lokal = 9, Max Global = 9
- Indeks 2 (`4`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`8`): Max Lokal = 21, Max Global = 21
- Indeks 4 (`5`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`9`): Max Lokal = 36, Max Global = 36
- Indeks 7 (`2`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **E**.
</details>

---
**Soal 224**
Diberikan pita DNA mutasi string: `SSXNXOONNSSOXNOSXXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 11 kombinasi
B. 13 kombinasi
C. 12 kombinasi
D. 15 kombinasi
E. 14 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 14 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 15 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 225**
Diberikan pita DNA mutasi string: `SSNNXOSSSOXOXNNOSXOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 7 kombinasi
B. 9 kombinasi
C. 8 kombinasi
D. 6 kombinasi
E. 5 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 8 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 16 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)
- Indeks 18 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 19 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 226**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 3, 6, 1, 2, 1, 6, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 28 Juta Rupiah
B. 30 Juta Rupiah
C. 29 Juta Rupiah
D. 27 Juta Rupiah
E. 31 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: C (29 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`3`): Max Lokal = 6, Max Global = 6
- Indeks 2 (`6`): Max Lokal = 12, Max Global = 12
- Indeks 3 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 4 (`2`): Max Lokal = 15, Max Global = 15
- Indeks 5 (`1`): Max Lokal = 16, Max Global = 16
- Indeks 6 (`6`): Max Lokal = 22, Max Global = 22
- Indeks 7 (`7`): Max Lokal = 29, Max Global = 29


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **29**. Opsi tervalid adalah **C**.
</details>

---
**Soal 227**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 3, 5, 7, 6, 1, 2, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 28 Juta Rupiah
B. 29 Juta Rupiah
C. 30 Juta Rupiah
D. 26 Juta Rupiah
E. 27 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (28 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`3`): Max Lokal = 5, Max Global = 5
- Indeks 2 (`5`): Max Lokal = 10, Max Global = 10
- Indeks 3 (`7`): Max Lokal = 17, Max Global = 17
- Indeks 4 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`1`): Max Lokal = 24, Max Global = 24
- Indeks 6 (`2`): Max Lokal = 26, Max Global = 26
- Indeks 7 (`2`): Max Lokal = 28, Max Global = 28


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **28**. Opsi tervalid adalah **A**.
</details>

---
**Soal 228**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 9, 6, 6, 4, 3, 8, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 43 Juta Rupiah
B. 44 Juta Rupiah
C. 47 Juta Rupiah
D. 45 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: D (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`9`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`6`): Max Lokal = 19, Max Global = 19
- Indeks 3 (`6`): Max Lokal = 25, Max Global = 25
- Indeks 4 (`4`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`3`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`8`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`5`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **D**.
</details>

---
**Soal 229**
Diberikan pita DNA mutasi string: `ONXNNOONXNOOXXXO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 0 kombinasi
B. 2 kombinasi
C. 3 kombinasi
D. 4 kombinasi
E. 1 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 230**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[7, 5, 1, 1, 3, 6, 1, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 25 Juta Rupiah
B. 24 Juta Rupiah
C. 27 Juta Rupiah
D. 28 Juta Rupiah
E. 26 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (26 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`7`): Max Lokal = 7, Max Global = 7
- Indeks 1 (`5`): Max Lokal = 12, Max Global = 12
- Indeks 2 (`1`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`1`): Max Lokal = 14, Max Global = 14
- Indeks 4 (`3`): Max Lokal = 17, Max Global = 17
- Indeks 5 (`6`): Max Lokal = 23, Max Global = 23
- Indeks 6 (`1`): Max Lokal = 24, Max Global = 24
- Indeks 7 (`2`): Max Lokal = 26, Max Global = 26


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **26**. Opsi tervalid adalah **E**.
</details>

---
**Soal 231**
Diberikan pita DNA mutasi string: `NONNXNSOOOOSSN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 14 kombinasi
B. 10 kombinasi
C. 13 kombinasi
D. 11 kombinasi
E. 12 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (11 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 11 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 12 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)
- Indeks 13 (`N`): Panen Final! Tarik paksa rakitan array 11 buah `OS`. (Total Jawaban OSN = 11)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **11 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 232**
Diberikan pita DNA mutasi string: `NSXSOSONNSSOX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 1 kombinasi
C. 2 kombinasi
D. 3 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (2 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **2 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 233**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[4, 1, 8, 3, 5, 4, 2, 2]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 29 Juta Rupiah
B. 30 Juta Rupiah
C. 27 Juta Rupiah
D. 28 Juta Rupiah
E. 31 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (29 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`4`): Max Lokal = 4, Max Global = 4
- Indeks 1 (`1`): Max Lokal = 5, Max Global = 5
- Indeks 2 (`8`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`3`): Max Lokal = 16, Max Global = 16
- Indeks 4 (`5`): Max Lokal = 21, Max Global = 21
- Indeks 5 (`4`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`2`): Max Lokal = 27, Max Global = 27
- Indeks 7 (`2`): Max Lokal = 29, Max Global = 29


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **29**. Opsi tervalid adalah **A**.
</details>

---
**Soal 234**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 6, 6, 4, 5, 8, 9, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 45 Juta Rupiah
B. 43 Juta Rupiah
C. 44 Juta Rupiah
D. 47 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (45 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`6`): Max Lokal = 8, Max Global = 8
- Indeks 2 (`6`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`4`): Max Lokal = 18, Max Global = 18
- Indeks 4 (`5`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`8`): Max Lokal = 31, Max Global = 31
- Indeks 6 (`9`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`5`): Max Lokal = 45, Max Global = 45


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **45**. Opsi tervalid adalah **A**.
</details>

---
**Soal 235**
Diberikan pita DNA mutasi string: `SNNSSXSNSNSONSSXO`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 3 kombinasi
B. 1 kombinasi
C. 0 kombinasi
D. 2 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: C (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 8 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 10 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 13 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 14 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **C**.
</details>

---
**Soal 236**
Diberikan pita DNA mutasi string: `XNNSSNSOOOONX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 4 kombinasi
B. 2 kombinasi
C. 3 kombinasi
D. 1 kombinasi
E. 0 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (0 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 4 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 6 (`S`): Kawinkan dengan 0 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 0)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **0 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 237**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[3, 7, 4, 9, 3, 7, 4, 3]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 41 Juta Rupiah
B. 39 Juta Rupiah
C. 42 Juta Rupiah
D. 38 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (40 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`3`): Max Lokal = 3, Max Global = 3
- Indeks 1 (`7`): Max Lokal = 10, Max Global = 10
- Indeks 2 (`4`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`9`): Max Lokal = 23, Max Global = 23
- Indeks 4 (`3`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`7`): Max Lokal = 33, Max Global = 33
- Indeks 6 (`4`): Max Lokal = 37, Max Global = 37
- Indeks 7 (`3`): Max Lokal = 40, Max Global = 40


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **40**. Opsi tervalid adalah **E**.
</details>

---
**Soal 238**
Diberikan pita DNA mutasi string: `XOSSNNXXXSOXXXSOSNNS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 20 kombinasi
B. 23 kombinasi
C. 22 kombinasi
D. 21 kombinasi
E. 19 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (20 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 9 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 10 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 14 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 5)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 16 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 17 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 12)
- Indeks 18 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 20)
- Indeks 19 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 11)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **20 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 239**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 5, 9, 2, 5, 3, 8, 6]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 48 Juta Rupiah
B. 44 Juta Rupiah
C. 47 Juta Rupiah
D. 45 Juta Rupiah
E. 46 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: E (46 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`5`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 3 (`2`): Max Lokal = 24, Max Global = 24
- Indeks 4 (`5`): Max Lokal = 29, Max Global = 29
- Indeks 5 (`3`): Max Lokal = 32, Max Global = 32
- Indeks 6 (`8`): Max Lokal = 40, Max Global = 40
- Indeks 7 (`6`): Max Lokal = 46, Max Global = 46


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **46**. Opsi tervalid adalah **E**.
</details>

---
**Soal 240**
Diberikan pita DNA mutasi string: `OXNXSNXONNSXXOXNOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 7 kombinasi
C. 5 kombinasi
D. 9 kombinasi
E. 6 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (6 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 2)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 10 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 13 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 6)
- Indeks 16 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 17 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **6 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 241**
Diberikan pita DNA mutasi string: `OONSSNOOOOXONXNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 15 kombinasi
B. 14 kombinasi
C. 13 kombinasi
D. 11 kombinasi
E. 12 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (12 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 4 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 5 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 6)
- Indeks 11 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 7)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)
- Indeks 14 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 12)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **12 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
**Soal 242**
Diberikan pita DNA mutasi string: `NOXNXOSSXNXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 8 kombinasi
B. 7 kombinasi
C. 9 kombinasi
D. 11 kombinasi
E. 10 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (8 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 6 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 4)
- Indeks 9 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 4)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 4 buah `OS`. (Total Jawaban OSN = 8)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **8 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 243**
Diberikan pita DNA mutasi string: `NOSXNXSOOONSOXXN`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 9 kombinasi
B. 11 kombinasi
C. 12 kombinasi
D. 8 kombinasi
E. 10 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: A (9 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 1 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 6 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 2)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 2 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 12 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 15 (`N`): Panen Final! Tarik paksa rakitan array 6 buah `OS`. (Total Jawaban OSN = 9)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **9 kombinasi ras**.
Opsi murni paling tepat adalah **A**.
</details>

---
**Soal 244**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[1, 6, 6, 6, 3, 6, 1, 5]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 36 Juta Rupiah
B. 34 Juta Rupiah
C. 35 Juta Rupiah
D. 33 Juta Rupiah
E. 32 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (34 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`1`): Max Lokal = 1, Max Global = 1
- Indeks 1 (`6`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`6`): Max Lokal = 19, Max Global = 19
- Indeks 4 (`3`): Max Lokal = 22, Max Global = 22
- Indeks 5 (`6`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`5`): Max Lokal = 34, Max Global = 34


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **34**. Opsi tervalid adalah **B**.
</details>

---
**Soal 245**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[2, 5, 6, 9, 4, 1, 4, 7]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 38 Juta Rupiah
B. 37 Juta Rupiah
C. 39 Juta Rupiah
D. 36 Juta Rupiah
E. 40 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (38 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`2`): Max Lokal = 2, Max Global = 2
- Indeks 1 (`5`): Max Lokal = 7, Max Global = 7
- Indeks 2 (`6`): Max Lokal = 13, Max Global = 13
- Indeks 3 (`9`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`4`): Max Lokal = 26, Max Global = 26
- Indeks 5 (`1`): Max Lokal = 27, Max Global = 27
- Indeks 6 (`4`): Max Lokal = 31, Max Global = 31
- Indeks 7 (`7`): Max Lokal = 38, Max Global = 38


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **38**. Opsi tervalid adalah **A**.
</details>

---
**Soal 246**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[8, 5, 3, 4, 3, 2, 9, 8]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 42 Juta Rupiah
B. 40 Juta Rupiah
C. 43 Juta Rupiah
D. 44 Juta Rupiah
E. 41 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: A (42 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`8`): Max Lokal = 8, Max Global = 8
- Indeks 1 (`5`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`3`): Max Lokal = 16, Max Global = 16
- Indeks 3 (`4`): Max Lokal = 20, Max Global = 20
- Indeks 4 (`3`): Max Lokal = 23, Max Global = 23
- Indeks 5 (`2`): Max Lokal = 25, Max Global = 25
- Indeks 6 (`9`): Max Lokal = 34, Max Global = 34
- Indeks 7 (`8`): Max Lokal = 42, Max Global = 42


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **42**. Opsi tervalid adalah **A**.
</details>

---
**Soal 247**
Pak Dengklek memiliki catatan kas warung berjejer murni: `[6, 7, 1, 8, 3, 3, 1, 4]`.
Jika ia menugaskan robotnya menjalankan operasi Algoritma **Sub-array Kotak Berkelanjutan dengan Nilai Terbesar (Kadane's Algorithm / Brute Force Rentang)**, berapakah rekor keuntungan bersih paling maksimal yang bisa dikantonginya dalam sekali rentang tarik utuh?
*(Catatan: Array ini hanya boleh "di-Substring-kan" utuh, gak bisa diloncat)*.

A. 34 Juta Rupiah
B. 33 Juta Rupiah
C. 31 Juta Rupiah
D. 32 Juta Rupiah
E. 35 Juta Rupiah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Rentang Optimal</b></summary>

**Jawaban: B (33 Juta)**

**Pembahasan (Menggusur Max Lokal dan Global):**
Jejak rekam simulasi memori memakan rentang 1D Linear O(N):
- Indeks 0 (`6`): Max Lokal = 6, Max Global = 6
- Indeks 1 (`7`): Max Lokal = 13, Max Global = 13
- Indeks 2 (`1`): Max Lokal = 14, Max Global = 14
- Indeks 3 (`8`): Max Lokal = 22, Max Global = 22
- Indeks 4 (`3`): Max Lokal = 25, Max Global = 25
- Indeks 5 (`3`): Max Lokal = 28, Max Global = 28
- Indeks 6 (`1`): Max Lokal = 29, Max Global = 29
- Indeks 7 (`4`): Max Lokal = 33, Max Global = 33


Rekor Mutlak (Max Global) berhenti dikunci secara agung pada angka **33**. Opsi tervalid adalah **B**.
</details>

---
**Soal 248**
Diberikan pita DNA mutasi string: `OSXNOSOOOSNNNX`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 24 kombinasi
B. 26 kombinasi
C. 27 kombinasi
D. 25 kombinasi
E. 28 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (25 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 1 buah `OS`. (Total Jawaban OSN = 1)
- Indeks 4 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 5 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 7 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 5)
- Indeks 9 (`S`): Kawinkan dengan 5 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 8)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 9)
- Indeks 11 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 17)
- Indeks 12 (`N`): Panen Final! Tarik paksa rakitan array 8 buah `OS`. (Total Jawaban OSN = 25)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **25 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 249**
Diberikan pita DNA mutasi string: `OXNNNSOXSONSXXSOS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 2 kombinasi
B. 5 kombinasi
C. 6 kombinasi
D. 3 kombinasi
E. 4 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: D (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 2 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 3 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 4 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 5 (`S`): Kawinkan dengan 1 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 1)
- Indeks 6 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 8 (`S`): Kawinkan dengan 2 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 9 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 10 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 11 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 6)
- Indeks 14 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 9)
- Indeks 15 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 16 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 13)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **D**.
</details>

---
**Soal 250**
Diberikan pita DNA mutasi string: `ONOOXSXNOXS`.
Seorang ilmuwan OSN-K menugaskanmu mencari kemunculan struktur Genetik "OSN"! 
Tentu saja secara **Subsekuens** (Huruf O, S, dan N boleh melompat melangkahi huruf rongsokan lainnya, namun posisinya pantang dibalik wajib Lurus Kiri ke Kanan).

Ada berapa total Kombinasi Subsekuens kemunculan kata `OSN` secara absolut di dalam pita teks tersebut?

A. 5 kombinasi
B. 2 kombinasi
C. 4 kombinasi
D. 6 kombinasi
E. 3 kombinasi

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Simulasi Array OSN</b></summary>

**Jawaban: E (3 kombinasi)**

**Pembahasan (Tabel Tabungan Linear O(N)):**
Sangat bunuh diri jika dicacah dihubungkan lidi pakai pulpen manual. Murni kita telusuri per huruf dari kiri ke kanan:
- Indeks 0 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 1)
- Indeks 1 (`N`): Panen Final! Tarik paksa rakitan array 0 buah `OS`. (Total Jawaban OSN = 0)
- Indeks 2 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 2)
- Indeks 3 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 3)
- Indeks 5 (`S`): Kawinkan dengan 3 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 3)
- Indeks 7 (`N`): Panen Final! Tarik paksa rakitan array 3 buah `OS`. (Total Jawaban OSN = 3)
- Indeks 8 (`O`): Kantongi Sejarah `O` baru. (Total Kantong `O` = 4)
- Indeks 10 (`S`): Kawinkan dengan 4 kantong `O` masa lalu. (Total Kantong `OS` nambah murni jadi 7)


Pita habis dieksekusi! Laporan Final Saldo Subsekuens `OSN` yang sah di mata mesin pencetak adalah **3 kombinasi ras**.
Opsi murni paling tepat adalah **E**.
</details>

---
