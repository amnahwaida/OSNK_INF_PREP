🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Algoritma Greedy (Part 3 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Algoritma Greedy**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 101**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[15:00-16:00, 12:00-15:00, 11:00-12:00, 18:00-20:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 1 rapat
C. 5 rapat
D. 2 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-12:00, 12:00-15:00, 15:00-16:00, 18:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (12:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (15:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (18:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 102**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[12:00-13:00, 18:00-22:00, 14:00-15:00, 18:00-20:00, 7:00-11:00, 18:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 3 rapat
C. 2 rapat
D. 5 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-11:00, 12:00-13:00, 14:00-15:00, 18:00-19:00, 18:00-20:00, 18:00-22:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (12:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (18:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (18:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (18:00 - 22:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 103**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[10:00-14:00, 10:00-11:00, 13:00-16:00, 16:00-19:00, 9:00-13:00, 17:00-18:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 1 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[10:00-11:00, 9:00-13:00, 10:00-14:00, 13:00-16:00, 17:00-18:00, 16:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (9:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (10:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (13:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (16:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 104**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[10:00-12:00, 12:00-14:00, 8:00-12:00, 13:00-17:00, 7:00-8:00, 12:00-13:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 1 rapat
C. 5 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 10:00-12:00, 8:00-12:00, 12:00-13:00, 12:00-14:00, 13:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (10:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (8:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (12:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (12:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 13:00).
- Mengecek Jadwal (13:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 105**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 5, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 4 keping koin
C. 3 keping koin
D. 5 keping koin
E. 7 keping koin

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
**Soal 106**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[9:00-10:00, 16:00-18:00, 9:00-11:00, 16:00-18:00, 17:00-21:00, 7:00-8:00, 7:00-8:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 1 rapat
C. 3 rapat
D. 2 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 7:00-8:00, 9:00-10:00, 9:00-11:00, 16:00-18:00, 16:00-18:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (7:00 - 8:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 8:00).
- Mengecek Jadwal (9:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (9:00 - 11:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (16:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 107**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 13** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 2 keping koin
B. 4 keping koin
C. 6 keping koin
D. 5 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 108**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 13** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 7 keping koin
C. 3 keping koin
D. 8 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (6 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 5
Ambil 5 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **6 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 6 adalah perilaku sistem aslinya).*
</details>

---
**Soal 109**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 2 keping koin
C. 4 keping koin
D. 6 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 6
Ambil 1 koin '5' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 110**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[13:00-16:00, 10:00-12:00, 18:00-22:00, 8:00-11:00, 11:00-14:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 1 rapat
D. 3 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-11:00, 10:00-12:00, 11:00-14:00, 13:00-16:00, 18:00-22:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (10:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (11:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (13:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (18:00 - 22:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 22:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 111**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-10:00, 17:00-20:00, 14:00-15:00, 7:00-8:00, 8:00-10:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 1 rapat
B. 5 rapat
C. 2 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 7:00-10:00, 8:00-10:00, 14:00-15:00, 17:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (7:00 - 10:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 8:00).
- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (17:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 112**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-15:00, 10:00-11:00, 7:00-8:00, 18:00-21:00, 16:00-18:00, 7:00-11:00, 17:00-21:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 2 rapat
C. 1 rapat
D. 3 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (5 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 10:00-11:00, 7:00-11:00, 11:00-15:00, 16:00-18:00, 18:00-21:00, 17:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (10:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (7:00 - 11:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (11:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (18:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 21:00).

Total rapat sukses dicentang: **5 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 113**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-18:00, 16:00-19:00, 17:00-21:00, 18:00-21:00, 8:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 3 rapat
C. 1 rapat
D. 2 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-12:00, 16:00-18:00, 16:00-19:00, 17:00-21:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (16:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (16:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (17:00 - 21:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).
- Mengecek Jadwal (18:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 114**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-14:00, 11:00-14:00, 12:00-16:00, 10:00-12:00, 16:00-20:00, 11:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 2 rapat
C. 5 rapat
D. 1 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[10:00-12:00, 11:00-12:00, 11:00-14:00, 11:00-14:00, 12:00-16:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (10:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (11:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (11:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (12:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (16:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 115**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 7, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 9 keping koin
B. 7 keping koin
C. 6 keping koin
D. 3 keping koin
E. 8 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (7 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 6
Ambil 6 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **7 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 7 adalah perilaku sistem aslinya).*
</details>

---
**Soal 116**
Kerajaan Namec memiliki pecahan uang kuno: `[9, 6, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 8 keping koin
B. 4 keping koin
C. 7 keping koin
D. 6 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (6 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '9' -> Sisa 5
Ambil 5 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **6 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 6 adalah perilaku sistem aslinya).*
</details>

---
**Soal 117**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-17:00, 14:00-17:00, 15:00-17:00, 11:00-13:00, 8:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 1 rapat
B. 2 rapat
C. 5 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-12:00, 11:00-13:00, 16:00-17:00, 14:00-17:00, 15:00-17:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 13:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (14:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (15:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 118**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[9:00-12:00, 16:00-19:00, 18:00-19:00, 14:00-18:00, 17:00-19:00, 14:00-18:00, 14:00-15:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 1 rapat
C. 3 rapat
D. 2 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[9:00-12:00, 14:00-15:00, 14:00-18:00, 14:00-18:00, 16:00-19:00, 18:00-19:00, 17:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (9:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (14:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (14:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (16:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (18:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (17:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 119**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[17:00-18:00, 8:00-9:00, 16:00-19:00, 13:00-14:00, 13:00-16:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 2 rapat
C. 5 rapat
D. 4 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-9:00, 13:00-14:00, 13:00-16:00, 17:00-18:00, 16:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 9:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 9:00).
- Mengecek Jadwal (13:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (13:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 14:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (16:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 120**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[14:00-17:00, 7:00-10:00, 17:00-19:00, 11:00-15:00, 17:00-20:00, 15:00-19:00, 16:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 3 rapat
C. 4 rapat
D. 1 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-10:00, 11:00-15:00, 14:00-17:00, 17:00-19:00, 15:00-19:00, 16:00-19:00, 17:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (11:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (17:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (15:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (16:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (17:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 121**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 5, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 7 keping koin
C. 6 keping koin
D. 5 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 7
Ambil 1 koin '5' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 122**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-18:00, 15:00-17:00, 10:00-12:00, 11:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 2 rapat
C. 1 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[10:00-12:00, 11:00-12:00, 15:00-17:00, 16:00-18:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (10:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (16:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 123**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-17:00, 18:00-21:00, 13:00-16:00, 16:00-18:00, 16:00-17:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 4 rapat
C. 3 rapat
D. 1 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[13:00-16:00, 16:00-17:00, 16:00-17:00, 16:00-18:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (13:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (16:00 - 17:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (16:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (18:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 124**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 1 keping koin
B. 5 keping koin
C. 4 keping koin
D. 3 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 125**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 6, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

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
Ambil 1 koin '11' -> Sisa 3
Ambil 3 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 126**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 6, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 6 keping koin
C. 5 keping koin
D. 3 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 7
Ambil 1 koin '6' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 127**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 7, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 8 keping koin
B. 3 keping koin
C. 7 keping koin
D. 5 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (6 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 5
Ambil 5 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **6 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 6 adalah perilaku sistem aslinya).*
</details>

---
**Soal 128**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 5, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 6 keping koin
C. 4 keping koin
D. 5 keping koin
E. 7 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 7
Ambil 1 koin '5' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 129**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[12:00-16:00, 10:00-12:00, 9:00-11:00, 7:00-8:00, 13:00-15:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 5 rapat
B. 4 rapat
C. 1 rapat
D. 2 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 9:00-11:00, 10:00-12:00, 13:00-15:00, 12:00-16:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (9:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (10:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 11:00).
- Mengecek Jadwal (13:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (12:00 - 16:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 130**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 18** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 7 keping koin
C. 4 keping koin
D. 5 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 7
Ambil 1 koin '5' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 4 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 131**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 17** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 4 keping koin
C. 6 keping koin
D. 2 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 6
Ambil 1 koin '5' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 132**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 5, 1]`.
Raja ingin membayar harga barang **sebesar 14** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 8 keping koin
C. 4 keping koin
D. 7 keping koin
E. 6 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 5 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 133**
Pak Dengklek menerima 7 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[15:00-17:00, 18:00-19:00, 14:00-18:00, 18:00-19:00, 16:00-20:00, 9:00-10:00, 8:00-12:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 3 rapat
D. 1 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: C (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[9:00-10:00, 8:00-12:00, 15:00-17:00, 14:00-18:00, 18:00-19:00, 18:00-19:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (9:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (8:00 - 12:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 10:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (14:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (18:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (18:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).
- Mengecek Jadwal (16:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **C**.
</details>

---
**Soal 134**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 7, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 2 keping koin
B. 4 keping koin
C. 5 keping koin
D. 3 keping koin
E. 1 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: A (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **A**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 135**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 5, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 3 keping koin
B. 2 keping koin
C. 5 keping koin
D. 4 keping koin
E. 1 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 5
Ambil 1 koin '5' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 136**
Pak Dengklek menerima 5 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-14:00, 8:00-10:00, 11:00-12:00, 12:00-16:00, 18:00-22:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 1 rapat
C. 5 rapat
D. 4 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[8:00-10:00, 11:00-12:00, 11:00-14:00, 12:00-16:00, 18:00-22:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (8:00 - 10:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 10:00).
- Mengecek Jadwal (11:00 - 12:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 12:00).
- Mengecek Jadwal (11:00 - 14:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 12:00).
- Mengecek Jadwal (12:00 - 16:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 16:00).
- Mengecek Jadwal (18:00 - 22:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 22:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 137**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-14:00, 18:00-19:00, 15:00-17:00, 15:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 5 rapat
C. 1 rapat
D. 2 rapat
E. 4 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-14:00, 15:00-17:00, 18:00-19:00, 15:00-19:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 14:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 14:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (18:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (15:00 - 19:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 138**
Kerajaan Namec memiliki pecahan uang kuno: `[10, 5, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 2 keping koin
B. 6 keping koin
C. 5 keping koin
D. 3 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (3 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '10' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **3 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 3 adalah perilaku sistem aslinya).*
</details>

---
**Soal 139**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 5, 1]`.
Raja ingin membayar harga barang **sebesar 18** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 4 keping koin
C. 6 keping koin
D. 7 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 2 koin '8' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 140**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-11:00, 15:00-17:00, 17:00-18:00, 15:00-18:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 4 rapat
B. 5 rapat
C. 1 rapat
D. 2 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: E (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-11:00, 15:00-17:00, 17:00-18:00, 15:00-18:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (17:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (15:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 18:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **E**.
</details>

---
**Soal 141**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-8:00, 18:00-21:00, 7:00-9:00, 16:00-17:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 5 rapat
C. 1 rapat
D. 4 rapat
E. 2 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 7:00-9:00, 16:00-17:00, 18:00-21:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (7:00 - 9:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 8:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (18:00 - 21:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 21:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 142**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 7, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 7 keping koin
B. 4 keping koin
C. 5 keping koin
D. 6 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 143**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 5 keping koin
C. 1 keping koin
D. 3 keping koin
E. 2 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (2 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 1
Ambil 1 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **2 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 2 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 2 adalah perilaku sistem aslinya).*
</details>

---
**Soal 144**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 7, 1]`.
Raja ingin membayar harga barang **sebesar 12** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 5 keping koin
C. 7 keping koin
D. 8 keping koin
E. 4 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: B (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **B**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 5 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 145**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 6, 1]`.
Raja ingin membayar harga barang **sebesar 18** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 6 keping koin
B. 7 keping koin
C. 5 keping koin
D. 4 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: D (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 2 koin '8' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **D**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
**Soal 146**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[7:00-8:00, 14:00-18:00, 18:00-20:00, 8:00-11:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 2 rapat
B. 5 rapat
C. 1 rapat
D. 4 rapat
E. 3 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: D (4 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[7:00-8:00, 8:00-11:00, 14:00-18:00, 18:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (7:00 - 8:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 8:00).
- Mengecek Jadwal (8:00 - 11:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 11:00).
- Mengecek Jadwal (14:00 - 18:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 18:00).
- Mengecek Jadwal (18:00 - 20:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 20:00).

Total rapat sukses dicentang: **4 rapat**. Opsi tervalidasi adalah **D**.
</details>

---
**Soal 147**
Kerajaan Namec memiliki pecahan uang kuno: `[11, 5, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 4 keping koin
B. 3 keping koin
C. 6 keping koin
D. 7 keping koin
E. 5 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: E (5 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '11' -> Sisa 4
Ambil 4 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **5 keping koin**! Opsi tepat: **E**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 5 adalah perilaku sistem aslinya).*
</details>

---
**Soal 148**
Pak Dengklek menerima 6 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[11:00-15:00, 14:00-18:00, 15:00-17:00, 15:00-18:00, 15:00-18:00, 14:00-15:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 2 rapat
C. 1 rapat
D. 4 rapat
E. 5 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: B (2 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-15:00, 14:00-15:00, 15:00-17:00, 14:00-18:00, 15:00-18:00, 15:00-18:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 15:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 15:00).
- Mengecek Jadwal (14:00 - 15:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 15:00).
- Mengecek Jadwal (15:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (14:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (15:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).
- Mengecek Jadwal (15:00 - 18:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 17:00).

Total rapat sukses dicentang: **2 rapat**. Opsi tervalidasi adalah **B**.
</details>

---
**Soal 149**
Pak Dengklek menerima 4 proposal permohonan peminjaman ruangan aula desa untuk hari ini berskala: `(Jam Mulai - Jam Kelar)`.
Daftar jadwal acak yang diajukan: `[16:00-20:00, 11:00-13:00, 16:00-17:00, 17:00-19:00]`.

Menerapkan pilar Algoritma Rekayasa **Greedy Activity Selection**, berapa MAKSIMAL JUMLAH proposal rapat yang sukses diadakan tanpa saling tindih jam?

A. 3 rapat
B. 5 rapat
C. 4 rapat
D. 2 rapat
E. 1 rapat

<details>
<summary><b>Klik untuk melihat kunci jawaban & hukum urut Greedy</b></summary>

**Jawaban: A (3 rapat)**

**Pembahasan (Trik Rahasia: Sorot Jam Kelar!):**
Algoritma Greedy untuk optimalisasi tata jadwal *Activity Selection* memaksakan 1 hukum egois mutlak: **JANGAN PEDULI KAPAN MULAINYA, SELALU URUTKAN & AMBIL DARI JADWAL YANG KELARNYA PALING CEPAT!**

Mari kita seret daftar jadwal yang semrawut tadi dan kita jejerkan murni berdasarkan Jam Selesainya:
`[11:00-13:00, 16:00-17:00, 17:00-19:00, 16:00-20:00]`

Simulasi penyewaan rakus Pak Dengklek:

- Mengecek Jadwal (11:00 - 13:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 13:00).
- Mengecek Jadwal (16:00 - 17:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 17:00).
- Mengecek Jadwal (17:00 - 19:00): ✅ **DITERIMA** (Tidak nabrak, ruangan kosong sejak 19:00).
- Mengecek Jadwal (16:00 - 20:00): ❌ Ditolak (Nabrak! Ruangan masih dipakai sampai 19:00).

Total rapat sukses dicentang: **3 rapat**. Opsi tervalidasi adalah **A**.
</details>

---
**Soal 150**
Kerajaan Namec memiliki pecahan uang kuno: `[8, 5, 1]`.
Raja ingin membayar harga barang **sebesar 15** menggunakan algoritma **Greedy Naif (Metode Serakah Murni)**.

Jika Raja Namec secara naif nekat bertindak murni *Greedy* layaknya perampok, berapa **Keping Koin Total** yang akan dia keluarkan dari dompetnya?
*(Hati-hati, ini pertanyaan kemahalan bot Greedy, belum tentu optimal! Lacak logikanya).*

A. 5 keping koin
B. 7 keping koin
C. 4 keping koin
D. 6 keping koin
E. 3 keping koin

<details>
<summary><b>Klik untuk melihat kunci jawaban & Fatal Error Greedy</b></summary>

**Jawaban: C (4 keping koin)**

**Pembahasan (Taktik Rakus Bodoh O(N)):**
Karena dimintai algoritma Greedy Naif, memori CPU tidak akan memikirkan optimalisasi matriks DP. State otaknya 110% mengabdi untuk "AMBIL KOIN PALING GEMUK TERSISA!".

Simulasi Rakus:
Ambil 1 koin '8' -> Sisa 7
Ambil 1 koin '5' -> Sisa 2
Ambil 2 koin '1' -> Sisa 0

Total yang dikeluarkan CPU Greedy Naif tersebut adalah **4 keping koin**! Opsi tepat: **C**.

*(Bahan Refleksi Genius: Padahal kalau dihitung pakai mata Dynamic Programming, solusi minimum sejatinya hanyalah 3 koin. Namun karena soal explicitly minta simulasi pergerakan algoritma GREEDY, maka jawaban 4 adalah perilaku sistem aslinya).*
</details>

---
