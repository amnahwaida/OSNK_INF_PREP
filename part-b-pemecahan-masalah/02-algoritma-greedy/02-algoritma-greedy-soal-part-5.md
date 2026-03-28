# Latian Soal: Algoritma Greedy (Part 5 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Algoritma Greedy**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 201**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 7, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 3 keping koin
C. 4 keping koin
D. 2 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 3
Ambil 3 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 202**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[12:00-15:00, 15:00-18:00, 11:00-14:00, 17:00-19:00, 12:00-15:00, 16:00-20:00, 7:00-11:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 1 rapat
C. 5 rapat
D. 2 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-11:00, 11:00-14:00, 12:00-15:00, 12:00-15:00, 15:00-18:00, 17:00-19:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (11:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (15:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (17:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (16:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 203**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-19:00, 17:00-21:00, 13:00-16:00, 8:00-11:00, 15:00-16:00, 10:00-11:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 3 rapat
C. 5 rapat
D. 2 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-11:00, 10:00-11:00, 13:00-16:00, 15:00-16:00, 16:00-19:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (10:00 - 11:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (13:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (15:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 16:00).
- Mengecek Jadwal (16:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 204**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[18:00-20:00, 10:00-14:00, 8:00-9:00, 10:00-11:00, 16:00-18:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 3 rapat
C. 2 rapat
D. 1 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-9:00, 10:00-11:00, 10:00-14:00, 16:00-18:00, 18:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 9:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 9:00).
- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (10:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (18:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 205**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-18:00, 9:00-10:00, 8:00-12:00, 8:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 3 rapat
D. 1 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[9:00-10:00, 8:00-12:00, 8:00-12:00, 16:00-18:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (9:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (8:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (8:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 206**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-12:00, 11:00-14:00, 13:00-14:00, 17:00-21:00, 18:00-21:00, 9:00-10:00, 14:00-16:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 1 rapat
D. 3 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (5 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[9:00-10:00, 11:00-12:00, 11:00-14:00, 13:00-14:00, 14:00-16:00, 17:00-21:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (9:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (13:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (14:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (17:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).
- Mengecek Jadwal (18:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 21:00).

Total rapat sukses dicentang: **5 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 207**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 7, 1]`.
Raja ingin membayar harga barang **sebesar 16** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 8 keping koin
B. 6 keping koin
C. 5 keping koin
D. 4 keping koin
E. 7 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (6 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 5
Ambil 5 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **6 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 6 adalah perilaku sistem aslinya).*
</details>

---
**Soal 208**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 5, 1]`.
Raja ingin membayar harga barang **sebesar 16** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 4 keping koin
C. 5 keping koin
D. 2 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 6
Ambil 1 koin '5' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 209**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 6, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 1 keping koin
C. 2 keping koin
D. 5 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 6
Ambil 1 koin '6' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 210**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-15:00, 13:00-17:00, 18:00-22:00, 17:00-19:00, 8:00-12:00, 11:00-15:00, 15:00-18:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 1 rapat
C. 5 rapat
D. 3 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-12:00, 11:00-15:00, 11:00-15:00, 13:00-17:00, 15:00-18:00, 17:00-19:00, 18:00-22:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (11:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (13:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (15:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (17:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (18:00 - 22:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 211**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[9:00-13:00, 16:00-19:00, 10:00-11:00, 8:00-10:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 1 rapat
C. 5 rapat
D. 3 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-10:00, 10:00-11:00, 9:00-13:00, 16:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (9:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (16:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 212**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 4 keping koin
C. 1 keping koin
D. 2 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 6
Ambil 1 koin '6' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 213**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 1 keping koin
B. 3 keping koin
C. 2 keping koin
D. 5 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 6
Ambil 1 koin '6' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 214**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 6, 1]`.
Raja ingin membayar harga barang **sebesar 18** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 3 keping koin
C. 6 keping koin
D. 4 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 7
Ambil 1 koin '6' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 215**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 7, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 7 keping koin
B. 4 keping koin
C. 6 keping koin
D. 3 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 3
Ambil 3 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 216**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 5, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 5 keping koin
C. 2 keping koin
D. 3 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 2 koin '8' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 217**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[10:00-12:00, 10:00-14:00, 17:00-21:00, 18:00-20:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 1 rapat
C. 2 rapat
D. 5 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[10:00-12:00, 10:00-14:00, 18:00-20:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (10:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (10:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (18:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 20:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 218**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-20:00, 11:00-15:00, 9:00-11:00, 8:00-10:00, 15:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 4 rapat
C. 5 rapat
D. 1 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-10:00, 9:00-11:00, 11:00-15:00, 15:00-19:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (9:00 - 11:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (11:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (15:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (16:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 219**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 7, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 4 keping koin
C. 5 keping koin
D. 7 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 220**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[14:00-15:00, 15:00-17:00, 14:00-16:00, 12:00-16:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 3 rapat
C. 1 rapat
D. 5 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[14:00-15:00, 14:00-16:00, 12:00-16:00, 15:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (12:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 221**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 6, 1]`.
Raja ingin membayar harga barang **sebesar 13** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 5 keping koin
C. 3 keping koin
D. 6 keping koin
E. 7 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 3
Ambil 3 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 222**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[17:00-19:00, 18:00-19:00, 10:00-14:00, 8:00-12:00, 12:00-15:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 1 rapat
D. 5 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-12:00, 10:00-14:00, 12:00-15:00, 17:00-19:00, 18:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (10:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (12:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (17:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (18:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 223**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-20:00, 7:00-8:00, 8:00-11:00, 11:00-12:00, 9:00-13:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 1 rapat
C. 4 rapat
D. 5 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 8:00-11:00, 11:00-12:00, 9:00-13:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (8:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (9:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (16:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 224**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-14:00, 10:00-14:00, 7:00-8:00, 16:00-20:00, 10:00-13:00, 18:00-21:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 4 rapat
D. 1 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 10:00-13:00, 11:00-14:00, 10:00-14:00, 16:00-20:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (10:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (11:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (10:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (16:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).
- Mengecek Jadwal (18:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 20:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 225**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 2 keping koin
B. 3 keping koin
C. 4 keping koin
D. 5 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 2 koin '8' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 226**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[17:00-18:00, 17:00-21:00, 10:00-13:00, 11:00-13:00, 7:00-8:00, 17:00-20:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 3 rapat
C. 1 rapat
D. 2 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 10:00-13:00, 11:00-13:00, 17:00-18:00, 17:00-20:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (10:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (11:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (17:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 227**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 6, 1]`.
Raja ingin membayar harga barang **sebesar 16** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 6 keping koin
C. 3 keping koin
D. 2 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 7
Ambil 1 koin '6' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 228**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 2 keping koin
C. 7 keping koin
D. 6 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 229**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 5, 1]`.
Raja ingin membayar harga barang **sebesar 16** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 6 keping koin
C. 3 keping koin
D. 5 keping koin
E. 7 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 7
Ambil 1 koin '5' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 230**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 7, 1]`.
Raja ingin membayar harga barang **sebesar 18** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 3 keping koin
C. 5 keping koin
D. 7 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 2 koin '8' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 231**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[17:00-18:00, 9:00-10:00, 7:00-8:00, 13:00-17:00, 15:00-16:00, 9:00-10:00, 15:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 3 rapat
D. 1 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 9:00-10:00, 9:00-10:00, 15:00-16:00, 13:00-17:00, 17:00-18:00, 15:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (9:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (9:00 - 10:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (15:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (13:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 16:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (15:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 232**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[13:00-16:00, 17:00-18:00, 9:00-11:00, 11:00-14:00, 14:00-16:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 3 rapat
C. 4 rapat
D. 2 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[9:00-11:00, 11:00-14:00, 13:00-16:00, 14:00-16:00, 17:00-18:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (9:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (11:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (13:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (14:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 233**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[13:00-14:00, 7:00-8:00, 14:00-16:00, 16:00-17:00, 13:00-15:00, 10:00-11:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 4 rapat
C. 1 rapat
D. 3 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (5 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 10:00-11:00, 13:00-14:00, 13:00-15:00, 14:00-16:00, 16:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (13:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (13:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (14:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).

Total rapat sukses dicentang: **5 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 234**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-11:00, 18:00-19:00, 12:00-15:00, 18:00-21:00, 11:00-14:00, 17:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 5 rapat
C. 2 rapat
D. 1 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-11:00, 11:00-14:00, 12:00-15:00, 18:00-19:00, 17:00-19:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (11:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (18:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (17:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (18:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 235**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 5, 1]`.
Raja ingin membayar harga barang **sebesar 13** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 8 keping koin
C. 5 keping koin
D. 6 keping koin
E. 7 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 5 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 236**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-9:00, 15:00-16:00, 7:00-8:00, 14:00-15:00, 8:00-10:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 4 rapat
C. 5 rapat
D. 3 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 7:00-9:00, 8:00-10:00, 14:00-15:00, 15:00-16:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (7:00 - 9:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 8:00).
- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (15:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 237**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 7, 1]`.
Raja ingin membayar harga barang **sebesar 13** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 4 keping koin
C. 3 keping koin
D. 7 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 3
Ambil 3 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 238**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[14:00-17:00, 16:00-20:00, 12:00-15:00, 15:00-17:00, 11:00-13:00, 15:00-16:00, 8:00-9:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 1 rapat
C. 5 rapat
D. 3 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-9:00, 11:00-13:00, 12:00-15:00, 15:00-16:00, 14:00-17:00, 15:00-17:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 9:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 9:00).
- Mengecek Jadwal (11:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (15:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (14:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 16:00).
- Mengecek Jadwal (15:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 16:00).
- Mengecek Jadwal (16:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 239**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[14:00-15:00, 14:00-17:00, 8:00-12:00, 8:00-10:00, 10:00-11:00, 9:00-12:00, 7:00-8:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 3 rapat
D. 1 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 8:00-10:00, 10:00-11:00, 8:00-12:00, 9:00-12:00, 14:00-15:00, 14:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (8:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (9:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 240**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 7, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 8 keping koin
B. 6 keping koin
C. 2 keping koin
D. 7 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (6 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 5
Ambil 5 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **6 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 6 adalah perilaku sistem aslinya).*
</details>

---
**Soal 241**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 5, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 2 keping koin
C. 5 keping koin
D. 3 keping koin
E. 1 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 5
Ambil 1 koin '5' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 242**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-13:00, 12:00-16:00, 18:00-20:00, 11:00-15:00, 16:00-17:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 4 rapat
C. 1 rapat
D. 3 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-13:00, 11:00-15:00, 12:00-16:00, 16:00-17:00, 18:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (11:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (12:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (18:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 243**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[14:00-15:00, 12:00-15:00, 15:00-16:00, 14:00-16:00, 17:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 2 rapat
C. 1 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[14:00-15:00, 12:00-15:00, 15:00-16:00, 14:00-16:00, 17:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (15:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (14:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 16:00).
- Mengecek Jadwal (17:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 244**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-19:00, 14:00-15:00, 12:00-15:00, 13:00-15:00, 16:00-18:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 4 rapat
C. 2 rapat
D. 3 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[14:00-15:00, 12:00-15:00, 13:00-15:00, 16:00-18:00, 16:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (13:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (16:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 245**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[18:00-21:00, 16:00-19:00, 16:00-20:00, 11:00-13:00, 17:00-21:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 3 rapat
C. 1 rapat
D. 5 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-13:00, 16:00-19:00, 16:00-20:00, 18:00-21:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (16:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (16:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (18:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 246**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[10:00-12:00, 11:00-12:00, 14:00-17:00, 13:00-15:00, 18:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 1 rapat
D. 5 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[10:00-12:00, 11:00-12:00, 13:00-15:00, 14:00-17:00, 18:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (10:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (13:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (18:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 247**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[17:00-18:00, 8:00-9:00, 18:00-21:00, 11:00-12:00, 17:00-19:00, 7:00-8:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 1 rapat
B. 5 rapat
C. 3 rapat
D. 4 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (5 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 8:00-9:00, 11:00-12:00, 17:00-18:00, 17:00-19:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (8:00 - 9:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 9:00).
- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (17:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (18:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).

Total rapat sukses dicentang: **5 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 248**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[8:00-10:00, 14:00-17:00, 11:00-12:00, 7:00-8:00, 9:00-13:00, 10:00-12:00, 15:00-17:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 1 rapat
D. 3 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 8:00-10:00, 11:00-12:00, 10:00-12:00, 9:00-13:00, 14:00-17:00, 15:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (10:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (9:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (14:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (15:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 249**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 7 keping koin
B. 5 keping koin
C. 6 keping koin
D. 4 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 250**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-13:00, 17:00-20:00, 12:00-15:00, 16:00-19:00, 9:00-13:00, 13:00-14:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 1 rapat
C. 4 rapat
D. 3 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-13:00, 9:00-13:00, 13:00-14:00, 12:00-15:00, 16:00-19:00, 17:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (9:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (13:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (12:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (16:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (17:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
