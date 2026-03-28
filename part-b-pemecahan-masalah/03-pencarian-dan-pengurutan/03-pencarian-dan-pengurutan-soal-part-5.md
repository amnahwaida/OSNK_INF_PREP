🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Pencarian & Pengurutan (Part 5 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 201**
Bebek-bebek di barisan bernomor dada: `[66, 39, 75, 86, 65, 83]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [39, 86, 65, 66, 75, 83]
B. [39, 83, 65, 66, 86, 75]
C. [39, 65, 75, 86, 66, 83]
D. [83, 39, 75, 66, 86, 65]
E. [83, 39, 86, 75, 65, 66]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([39, 65, 75, 86, 66, 83])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[66, 39, 75, 86, 65, 83]`
- Putaran 1: Cari anak terpecebol di area sisa [39, 66, 75, 86, 65, 83]. Ditemukan si `39`. Tukar paksa dudukan dengan `66`. Array mutasi -> `[39, 66, 75, 86, 65, 83]`
- Putaran 2: Cari anak terpecebol di area sisa [65, 75, 86, 66, 83]. Ditemukan si `65`. Tukar paksa dudukan dengan `66`. Array mutasi -> `[39, 65, 75, 86, 66, 83]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[39, 65, 75, 86, 66, 83]**. Opsi murni: **C**.
</details>

---
**Soal 202**
Bebek-bebek di barisan bernomor dada: `[59, 58, 25, 39, 60, 30]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [25, 30, 59, 39, 60, 58]
B. [58, 30, 60, 25, 59, 39]
C. [59, 39, 60, 58, 30, 25]
D. [30, 25, 59, 58, 39, 60]
E. [30, 25, 39, 58, 59, 60]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([25, 30, 59, 39, 60, 58])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[59, 58, 25, 39, 60, 30]`
- Putaran 1: Cari anak terpecebol di area sisa [25, 58, 59, 39, 60, 30]. Ditemukan si `25`. Tukar paksa dudukan dengan `59`. Array mutasi -> `[25, 58, 59, 39, 60, 30]`
- Putaran 2: Cari anak terpecebol di area sisa [30, 59, 39, 60, 58]. Ditemukan si `30`. Tukar paksa dudukan dengan `58`. Array mutasi -> `[25, 30, 59, 39, 60, 58]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[25, 30, 59, 39, 60, 58]**. Opsi murni: **A**.
</details>

---
**Soal 203**
Bebek-bebek di barisan bernomor dada: `[25, 59, 77, 30, 49, 89]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [25, 30, 77, 59, 49, 89]
B. [25, 59, 49, 30, 77, 89]
C. [59, 49, 30, 77, 25, 89]
D. [77, 25, 30, 89, 49, 59]
E. [49, 30, 89, 59, 25, 77]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([25, 30, 77, 59, 49, 89])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[25, 59, 77, 30, 49, 89]`
- Putaran 1: Cari anak terpecebol di area sisa [25, 59, 77, 30, 49, 89]. Ditemukan si `25`. Tukar paksa dudukan dengan `25`. Array mutasi -> `[25, 59, 77, 30, 49, 89]`
- Putaran 2: Cari anak terpecebol di area sisa [30, 77, 59, 49, 89]. Ditemukan si `30`. Tukar paksa dudukan dengan `59`. Array mutasi -> `[25, 30, 77, 59, 49, 89]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[25, 30, 77, 59, 49, 89]**. Opsi murni: **A**.
</details>

---
**Soal 204**
Diberikan barisan angka: `[24, 98, 28, 48, 60]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [48, 28, 24, 98, 60]
B. [98, 24, 60, 48, 28]
C. [24, 28, 48, 60, 98]
D. [98, 24, 28, 60, 48]
E. [48, 60, 28, 98, 24]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([24, 28, 48, 60, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[24, 98, 28, 48, 60]`
Cek posisi 0&1 (24 < 98) -> Aman dibiarkan. Array kini: `[24, 98, 28, 48, 60]`
Cek posisi 1&2 (98 > 28) -> Tukar! Array kini: `[24, 28, 98, 48, 60]`
Cek posisi 2&3 (98 > 48) -> Tukar! Array kini: `[24, 28, 48, 98, 60]`
Cek posisi 3&4 (98 > 60) -> Tukar! Array kini: `[24, 28, 48, 60, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[24, 28, 48, 60, 98]**.
</details>

---
**Soal 205**
Bebek-bebek di barisan bernomor dada: `[56, 51, 72, 90, 98, 15]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [98, 56, 15, 51, 72, 90]
B. [72, 51, 15, 56, 90, 98]
C. [15, 51, 72, 90, 98, 56]
D. [90, 72, 15, 56, 98, 51]
E. [72, 98, 51, 15, 56, 90]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([15, 51, 72, 90, 98, 56])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[56, 51, 72, 90, 98, 15]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 51, 72, 90, 98, 56]. Ditemukan si `15`. Tukar paksa dudukan dengan `56`. Array mutasi -> `[15, 51, 72, 90, 98, 56]`
- Putaran 2: Cari anak terpecebol di area sisa [51, 72, 90, 98, 56]. Ditemukan si `51`. Tukar paksa dudukan dengan `51`. Array mutasi -> `[15, 51, 72, 90, 98, 56]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 51, 72, 90, 98, 56]**. Opsi murni: **C**.
</details>

---
**Soal 206**
Bebek-bebek di barisan bernomor dada: `[87, 42, 60, 30, 31, 61]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [31, 42, 61, 60, 87, 30]
B. [31, 30, 61, 60, 42, 87]
C. [31, 87, 42, 30, 60, 61]
D. [30, 31, 60, 87, 42, 61]
E. [60, 87, 42, 61, 30, 31]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([30, 31, 60, 87, 42, 61])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[87, 42, 60, 30, 31, 61]`
- Putaran 1: Cari anak terpecebol di area sisa [30, 42, 60, 87, 31, 61]. Ditemukan si `30`. Tukar paksa dudukan dengan `87`. Array mutasi -> `[30, 42, 60, 87, 31, 61]`
- Putaran 2: Cari anak terpecebol di area sisa [31, 60, 87, 42, 61]. Ditemukan si `31`. Tukar paksa dudukan dengan `42`. Array mutasi -> `[30, 31, 60, 87, 42, 61]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[30, 31, 60, 87, 42, 61]**. Opsi murni: **D**.
</details>

---
**Soal 207**
Pak Dengklek memiliki daftar absensi **1427 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 13 langkah
C. 12 langkah
D. 14 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1427 elemen
- Langkah 1: Sisa populasi tebasan separuh = 714 elemen
- Langkah 2: Sisa populasi tebasan separuh = 357 elemen
- Langkah 3: Sisa populasi tebasan separuh = 179 elemen
- Langkah 4: Sisa populasi tebasan separuh = 90 elemen
- Langkah 5: Sisa populasi tebasan separuh = 45 elemen
- Langkah 6: Sisa populasi tebasan separuh = 23 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 208**
Diberikan barisan angka: `[42, 28, 45, 86, 17]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [42, 28, 45, 17, 86]
B. [28, 42, 45, 17, 86]
C. [86, 45, 28, 17, 42]
D. [45, 28, 86, 42, 17]
E. [17, 86, 42, 45, 28]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([28, 42, 45, 17, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[42, 28, 45, 86, 17]`
Cek posisi 0&1 (42 > 28) -> Tukar! Array kini: `[28, 42, 45, 86, 17]`
Cek posisi 1&2 (42 < 45) -> Aman dibiarkan. Array kini: `[28, 42, 45, 86, 17]`
Cek posisi 2&3 (45 < 86) -> Aman dibiarkan. Array kini: `[28, 42, 45, 86, 17]`
Cek posisi 3&4 (86 > 17) -> Tukar! Array kini: `[28, 42, 45, 17, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[28, 42, 45, 17, 86]**.
</details>

---
**Soal 209**
Bebek-bebek di barisan bernomor dada: `[80, 27, 75, 15, 10, 52]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [80, 27, 52, 15, 75, 10]
B. [10, 15, 75, 27, 80, 52]
C. [80, 75, 52, 10, 15, 27]
D. [15, 52, 10, 80, 27, 75]
E. [80, 27, 75, 10, 15, 52]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([10, 15, 75, 27, 80, 52])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[80, 27, 75, 15, 10, 52]`
- Putaran 1: Cari anak terpecebol di area sisa [10, 27, 75, 15, 80, 52]. Ditemukan si `10`. Tukar paksa dudukan dengan `80`. Array mutasi -> `[10, 27, 75, 15, 80, 52]`
- Putaran 2: Cari anak terpecebol di area sisa [15, 75, 27, 80, 52]. Ditemukan si `15`. Tukar paksa dudukan dengan `27`. Array mutasi -> `[10, 15, 75, 27, 80, 52]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[10, 15, 75, 27, 80, 52]**. Opsi murni: **B**.
</details>

---
**Soal 210**
Pak Dengklek memiliki daftar absensi **1208 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 11 langkah
C. 14 langkah
D. 12 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1208 elemen
- Langkah 1: Sisa populasi tebasan separuh = 604 elemen
- Langkah 2: Sisa populasi tebasan separuh = 302 elemen
- Langkah 3: Sisa populasi tebasan separuh = 151 elemen
- Langkah 4: Sisa populasi tebasan separuh = 76 elemen
- Langkah 5: Sisa populasi tebasan separuh = 38 elemen
- Langkah 6: Sisa populasi tebasan separuh = 19 elemen
- Langkah 7: Sisa populasi tebasan separuh = 10 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 211**
Diberikan barisan angka: `[82, 75, 14, 85, 77]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [75, 14, 82, 77, 85]
B. [82, 77, 14, 75, 85]
C. [85, 14, 77, 82, 75]
D. [82, 77, 85, 14, 75]
E. [75, 85, 14, 82, 77]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([75, 14, 82, 77, 85])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[82, 75, 14, 85, 77]`
Cek posisi 0&1 (82 > 75) -> Tukar! Array kini: `[75, 82, 14, 85, 77]`
Cek posisi 1&2 (82 > 14) -> Tukar! Array kini: `[75, 14, 82, 85, 77]`
Cek posisi 2&3 (82 < 85) -> Aman dibiarkan. Array kini: `[75, 14, 82, 85, 77]`
Cek posisi 3&4 (85 > 77) -> Tukar! Array kini: `[75, 14, 82, 77, 85]`


Terbukti bahwa elemen maha gemuk (`85`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[75, 14, 82, 77, 85]**.
</details>

---
**Soal 212**
Bebek-bebek di barisan bernomor dada: `[44, 74, 16, 51, 87, 70]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [16, 44, 74, 51, 87, 70]
B. [16, 70, 44, 87, 74, 51]
C. [70, 51, 16, 74, 87, 44]
D. [51, 87, 74, 44, 16, 70]
E. [44, 70, 16, 74, 51, 87]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([16, 44, 74, 51, 87, 70])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[44, 74, 16, 51, 87, 70]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 74, 44, 51, 87, 70]. Ditemukan si `16`. Tukar paksa dudukan dengan `44`. Array mutasi -> `[16, 74, 44, 51, 87, 70]`
- Putaran 2: Cari anak terpecebol di area sisa [44, 74, 51, 87, 70]. Ditemukan si `44`. Tukar paksa dudukan dengan `74`. Array mutasi -> `[16, 44, 74, 51, 87, 70]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 44, 74, 51, 87, 70]**. Opsi murni: **A**.
</details>

---
**Soal 213**
Diberikan barisan angka: `[81, 53, 27, 17, 45]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [17, 81, 53, 27, 45]
B. [27, 53, 81, 45, 17]
C. [53, 27, 17, 81, 45]
D. [53, 27, 17, 45, 81]
E. [27, 53, 17, 45, 81]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([53, 27, 17, 45, 81])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[81, 53, 27, 17, 45]`
Cek posisi 0&1 (81 > 53) -> Tukar! Array kini: `[53, 81, 27, 17, 45]`
Cek posisi 1&2 (81 > 27) -> Tukar! Array kini: `[53, 27, 81, 17, 45]`
Cek posisi 2&3 (81 > 17) -> Tukar! Array kini: `[53, 27, 17, 81, 45]`
Cek posisi 3&4 (81 > 45) -> Tukar! Array kini: `[53, 27, 17, 45, 81]`


Terbukti bahwa elemen maha gemuk (`81`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[53, 27, 17, 45, 81]**.
</details>

---
**Soal 214**
Diberikan barisan angka: `[68, 73, 29, 49, 95]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [73, 68, 95, 49, 29]
B. [68, 29, 49, 73, 95]
C. [68, 49, 73, 29, 95]
D. [73, 29, 68, 95, 49]
E. [49, 68, 29, 73, 95]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([68, 29, 49, 73, 95])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[68, 73, 29, 49, 95]`
Cek posisi 0&1 (68 < 73) -> Aman dibiarkan. Array kini: `[68, 73, 29, 49, 95]`
Cek posisi 1&2 (73 > 29) -> Tukar! Array kini: `[68, 29, 73, 49, 95]`
Cek posisi 2&3 (73 > 49) -> Tukar! Array kini: `[68, 29, 49, 73, 95]`
Cek posisi 3&4 (73 < 95) -> Aman dibiarkan. Array kini: `[68, 29, 49, 73, 95]`


Terbukti bahwa elemen maha gemuk (`95`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[68, 29, 49, 73, 95]**.
</details>

---
**Soal 215**
Bebek-bebek di barisan bernomor dada: `[37, 72, 64, 79, 34, 63]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [72, 34, 63, 37, 79, 64]
B. [72, 79, 63, 34, 64, 37]
C. [34, 79, 63, 72, 37, 64]
D. [37, 63, 79, 64, 34, 72]
E. [34, 37, 64, 79, 72, 63]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([34, 37, 64, 79, 72, 63])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[37, 72, 64, 79, 34, 63]`
- Putaran 1: Cari anak terpecebol di area sisa [34, 72, 64, 79, 37, 63]. Ditemukan si `34`. Tukar paksa dudukan dengan `37`. Array mutasi -> `[34, 72, 64, 79, 37, 63]`
- Putaran 2: Cari anak terpecebol di area sisa [37, 64, 79, 72, 63]. Ditemukan si `37`. Tukar paksa dudukan dengan `72`. Array mutasi -> `[34, 37, 64, 79, 72, 63]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[34, 37, 64, 79, 72, 63]**. Opsi murni: **E**.
</details>

---
**Soal 216**
Pak Dengklek memiliki daftar absensi **692 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 13 langkah
C. 10 langkah
D. 12 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 692 elemen
- Langkah 1: Sisa populasi tebasan separuh = 346 elemen
- Langkah 2: Sisa populasi tebasan separuh = 173 elemen
- Langkah 3: Sisa populasi tebasan separuh = 87 elemen
- Langkah 4: Sisa populasi tebasan separuh = 44 elemen
- Langkah 5: Sisa populasi tebasan separuh = 22 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 217**
Diberikan barisan angka: `[68, 86, 76, 88, 55]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [86, 88, 76, 68, 55]
B. [68, 76, 86, 55, 88]
C. [86, 68, 55, 88, 76]
D. [68, 76, 88, 55, 86]
E. [76, 55, 86, 68, 88]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([68, 76, 86, 55, 88])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[68, 86, 76, 88, 55]`
Cek posisi 0&1 (68 < 86) -> Aman dibiarkan. Array kini: `[68, 86, 76, 88, 55]`
Cek posisi 1&2 (86 > 76) -> Tukar! Array kini: `[68, 76, 86, 88, 55]`
Cek posisi 2&3 (86 < 88) -> Aman dibiarkan. Array kini: `[68, 76, 86, 88, 55]`
Cek posisi 3&4 (88 > 55) -> Tukar! Array kini: `[68, 76, 86, 55, 88]`


Terbukti bahwa elemen maha gemuk (`88`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[68, 76, 86, 55, 88]**.
</details>

---
**Soal 218**
Diberikan barisan angka: `[62, 63, 45, 98, 44]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [62, 63, 45, 44, 98]
B. [62, 45, 63, 44, 98]
C. [62, 98, 63, 44, 45]
D. [62, 44, 63, 45, 98]
E. [45, 44, 63, 98, 62]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([62, 45, 63, 44, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[62, 63, 45, 98, 44]`
Cek posisi 0&1 (62 < 63) -> Aman dibiarkan. Array kini: `[62, 63, 45, 98, 44]`
Cek posisi 1&2 (63 > 45) -> Tukar! Array kini: `[62, 45, 63, 98, 44]`
Cek posisi 2&3 (63 < 98) -> Aman dibiarkan. Array kini: `[62, 45, 63, 98, 44]`
Cek posisi 3&4 (98 > 44) -> Tukar! Array kini: `[62, 45, 63, 44, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[62, 45, 63, 44, 98]**.
</details>

---
**Soal 219**
Pak Dengklek memiliki daftar absensi **980 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 10 langkah
C. 12 langkah
D. 9 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 980 elemen
- Langkah 1: Sisa populasi tebasan separuh = 490 elemen
- Langkah 2: Sisa populasi tebasan separuh = 245 elemen
- Langkah 3: Sisa populasi tebasan separuh = 123 elemen
- Langkah 4: Sisa populasi tebasan separuh = 62 elemen
- Langkah 5: Sisa populasi tebasan separuh = 31 elemen
- Langkah 6: Sisa populasi tebasan separuh = 16 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 220**
Pak Dengklek memiliki daftar absensi **1967 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 14 langkah
C. 12 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1967 elemen
- Langkah 1: Sisa populasi tebasan separuh = 984 elemen
- Langkah 2: Sisa populasi tebasan separuh = 492 elemen
- Langkah 3: Sisa populasi tebasan separuh = 246 elemen
- Langkah 4: Sisa populasi tebasan separuh = 123 elemen
- Langkah 5: Sisa populasi tebasan separuh = 62 elemen
- Langkah 6: Sisa populasi tebasan separuh = 31 elemen
- Langkah 7: Sisa populasi tebasan separuh = 16 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 221**
Pak Dengklek memiliki daftar absensi **1946 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 14 langkah
C. 11 langkah
D. 13 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1946 elemen
- Langkah 1: Sisa populasi tebasan separuh = 973 elemen
- Langkah 2: Sisa populasi tebasan separuh = 487 elemen
- Langkah 3: Sisa populasi tebasan separuh = 244 elemen
- Langkah 4: Sisa populasi tebasan separuh = 122 elemen
- Langkah 5: Sisa populasi tebasan separuh = 61 elemen
- Langkah 6: Sisa populasi tebasan separuh = 31 elemen
- Langkah 7: Sisa populasi tebasan separuh = 16 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 222**
Pak Dengklek memiliki daftar absensi **531 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 10 langkah
D. 11 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 531 elemen
- Langkah 1: Sisa populasi tebasan separuh = 266 elemen
- Langkah 2: Sisa populasi tebasan separuh = 133 elemen
- Langkah 3: Sisa populasi tebasan separuh = 67 elemen
- Langkah 4: Sisa populasi tebasan separuh = 34 elemen
- Langkah 5: Sisa populasi tebasan separuh = 17 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 223**
Diberikan barisan angka: `[65, 36, 28, 94, 64]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [94, 36, 65, 28, 64]
B. [64, 28, 36, 65, 94]
C. [28, 65, 94, 64, 36]
D. [65, 28, 36, 94, 64]
E. [36, 28, 65, 64, 94]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([36, 28, 65, 64, 94])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[65, 36, 28, 94, 64]`
Cek posisi 0&1 (65 > 36) -> Tukar! Array kini: `[36, 65, 28, 94, 64]`
Cek posisi 1&2 (65 > 28) -> Tukar! Array kini: `[36, 28, 65, 94, 64]`
Cek posisi 2&3 (65 < 94) -> Aman dibiarkan. Array kini: `[36, 28, 65, 94, 64]`
Cek posisi 3&4 (94 > 64) -> Tukar! Array kini: `[36, 28, 65, 64, 94]`


Terbukti bahwa elemen maha gemuk (`94`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[36, 28, 65, 64, 94]**.
</details>

---
**Soal 224**
Diberikan barisan angka: `[61, 53, 58, 64, 78]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [53, 58, 61, 64, 78]
B. [58, 53, 61, 64, 78]
C. [61, 58, 64, 53, 78]
D. [64, 58, 61, 53, 78]
E. [78, 58, 53, 61, 64]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([53, 58, 61, 64, 78])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[61, 53, 58, 64, 78]`
Cek posisi 0&1 (61 > 53) -> Tukar! Array kini: `[53, 61, 58, 64, 78]`
Cek posisi 1&2 (61 > 58) -> Tukar! Array kini: `[53, 58, 61, 64, 78]`
Cek posisi 2&3 (61 < 64) -> Aman dibiarkan. Array kini: `[53, 58, 61, 64, 78]`
Cek posisi 3&4 (64 < 78) -> Aman dibiarkan. Array kini: `[53, 58, 61, 64, 78]`


Terbukti bahwa elemen maha gemuk (`78`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[53, 58, 61, 64, 78]**.
</details>

---
**Soal 225**
Diberikan barisan angka: `[40, 77, 17, 60, 85]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [40, 17, 60, 77, 85]
B. [85, 40, 60, 77, 17]
C. [85, 17, 77, 40, 60]
D. [77, 40, 60, 85, 17]
E. [17, 77, 60, 85, 40]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([40, 17, 60, 77, 85])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[40, 77, 17, 60, 85]`
Cek posisi 0&1 (40 < 77) -> Aman dibiarkan. Array kini: `[40, 77, 17, 60, 85]`
Cek posisi 1&2 (77 > 17) -> Tukar! Array kini: `[40, 17, 77, 60, 85]`
Cek posisi 2&3 (77 > 60) -> Tukar! Array kini: `[40, 17, 60, 77, 85]`
Cek posisi 3&4 (77 < 85) -> Aman dibiarkan. Array kini: `[40, 17, 60, 77, 85]`


Terbukti bahwa elemen maha gemuk (`85`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[40, 17, 60, 77, 85]**.
</details>

---
**Soal 226**
Diberikan barisan angka: `[43, 50, 65, 86, 12]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [86, 43, 65, 12, 50]
B. [50, 12, 65, 43, 86]
C. [43, 50, 65, 12, 86]
D. [65, 12, 43, 86, 50]
E. [50, 12, 65, 86, 43]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([43, 50, 65, 12, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[43, 50, 65, 86, 12]`
Cek posisi 0&1 (43 < 50) -> Aman dibiarkan. Array kini: `[43, 50, 65, 86, 12]`
Cek posisi 1&2 (50 < 65) -> Aman dibiarkan. Array kini: `[43, 50, 65, 86, 12]`
Cek posisi 2&3 (65 < 86) -> Aman dibiarkan. Array kini: `[43, 50, 65, 86, 12]`
Cek posisi 3&4 (86 > 12) -> Tukar! Array kini: `[43, 50, 65, 12, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[43, 50, 65, 12, 86]**.
</details>

---
**Soal 227**
Diberikan barisan angka: `[61, 90, 19, 84, 86]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [90, 19, 86, 61, 84]
B. [61, 19, 84, 86, 90]
C. [84, 19, 61, 86, 90]
D. [19, 84, 86, 61, 90]
E. [61, 90, 84, 19, 86]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([61, 19, 84, 86, 90])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[61, 90, 19, 84, 86]`
Cek posisi 0&1 (61 < 90) -> Aman dibiarkan. Array kini: `[61, 90, 19, 84, 86]`
Cek posisi 1&2 (90 > 19) -> Tukar! Array kini: `[61, 19, 90, 84, 86]`
Cek posisi 2&3 (90 > 84) -> Tukar! Array kini: `[61, 19, 84, 90, 86]`
Cek posisi 3&4 (90 > 86) -> Tukar! Array kini: `[61, 19, 84, 86, 90]`


Terbukti bahwa elemen maha gemuk (`90`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[61, 19, 84, 86, 90]**.
</details>

---
**Soal 228**
Pak Dengklek memiliki daftar absensi **565 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 9 langkah
C. 12 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 565 elemen
- Langkah 1: Sisa populasi tebasan separuh = 283 elemen
- Langkah 2: Sisa populasi tebasan separuh = 142 elemen
- Langkah 3: Sisa populasi tebasan separuh = 71 elemen
- Langkah 4: Sisa populasi tebasan separuh = 36 elemen
- Langkah 5: Sisa populasi tebasan separuh = 18 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 229**
Diberikan barisan angka: `[53, 86, 60, 48, 54]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [86, 53, 60, 54, 48]
B. [53, 60, 48, 54, 86]
C. [53, 48, 54, 86, 60]
D. [53, 54, 60, 48, 86]
E. [60, 86, 53, 54, 48]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([53, 60, 48, 54, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[53, 86, 60, 48, 54]`
Cek posisi 0&1 (53 < 86) -> Aman dibiarkan. Array kini: `[53, 86, 60, 48, 54]`
Cek posisi 1&2 (86 > 60) -> Tukar! Array kini: `[53, 60, 86, 48, 54]`
Cek posisi 2&3 (86 > 48) -> Tukar! Array kini: `[53, 60, 48, 86, 54]`
Cek posisi 3&4 (86 > 54) -> Tukar! Array kini: `[53, 60, 48, 54, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[53, 60, 48, 54, 86]**.
</details>

---
**Soal 230**
Diberikan barisan angka: `[87, 70, 68, 29, 38]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [29, 68, 87, 38, 70]
B. [38, 29, 68, 87, 70]
C. [87, 29, 70, 38, 68]
D. [68, 87, 70, 29, 38]
E. [70, 68, 29, 38, 87]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([70, 68, 29, 38, 87])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[87, 70, 68, 29, 38]`
Cek posisi 0&1 (87 > 70) -> Tukar! Array kini: `[70, 87, 68, 29, 38]`
Cek posisi 1&2 (87 > 68) -> Tukar! Array kini: `[70, 68, 87, 29, 38]`
Cek posisi 2&3 (87 > 29) -> Tukar! Array kini: `[70, 68, 29, 87, 38]`
Cek posisi 3&4 (87 > 38) -> Tukar! Array kini: `[70, 68, 29, 38, 87]`


Terbukti bahwa elemen maha gemuk (`87`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[70, 68, 29, 38, 87]**.
</details>

---
**Soal 231**
Diberikan barisan angka: `[39, 63, 27, 88, 40]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [40, 88, 39, 27, 63]
B. [63, 39, 27, 40, 88]
C. [39, 27, 63, 40, 88]
D. [88, 40, 27, 63, 39]
E. [27, 39, 88, 63, 40]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([39, 27, 63, 40, 88])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[39, 63, 27, 88, 40]`
Cek posisi 0&1 (39 < 63) -> Aman dibiarkan. Array kini: `[39, 63, 27, 88, 40]`
Cek posisi 1&2 (63 > 27) -> Tukar! Array kini: `[39, 27, 63, 88, 40]`
Cek posisi 2&3 (63 < 88) -> Aman dibiarkan. Array kini: `[39, 27, 63, 88, 40]`
Cek posisi 3&4 (88 > 40) -> Tukar! Array kini: `[39, 27, 63, 40, 88]`


Terbukti bahwa elemen maha gemuk (`88`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[39, 27, 63, 40, 88]**.
</details>

---
**Soal 232**
Bebek-bebek di barisan bernomor dada: `[27, 45, 69, 67, 42, 46]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [46, 45, 27, 67, 42, 69]
B. [27, 42, 69, 67, 45, 46]
C. [46, 67, 69, 27, 45, 42]
D. [46, 45, 27, 69, 42, 67]
E. [42, 45, 46, 69, 67, 27]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([27, 42, 69, 67, 45, 46])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[27, 45, 69, 67, 42, 46]`
- Putaran 1: Cari anak terpecebol di area sisa [27, 45, 69, 67, 42, 46]. Ditemukan si `27`. Tukar paksa dudukan dengan `27`. Array mutasi -> `[27, 45, 69, 67, 42, 46]`
- Putaran 2: Cari anak terpecebol di area sisa [42, 69, 67, 45, 46]. Ditemukan si `42`. Tukar paksa dudukan dengan `45`. Array mutasi -> `[27, 42, 69, 67, 45, 46]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[27, 42, 69, 67, 45, 46]**. Opsi murni: **B**.
</details>

---
**Soal 233**
Bebek-bebek di barisan bernomor dada: `[13, 30, 35, 14, 66, 26]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [30, 14, 35, 26, 13, 66]
B. [30, 13, 26, 35, 66, 14]
C. [66, 26, 14, 30, 13, 35]
D. [13, 14, 35, 30, 66, 26]
E. [66, 26, 30, 35, 14, 13]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([13, 14, 35, 30, 66, 26])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[13, 30, 35, 14, 66, 26]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 30, 35, 14, 66, 26]. Ditemukan si `13`. Tukar paksa dudukan dengan `13`. Array mutasi -> `[13, 30, 35, 14, 66, 26]`
- Putaran 2: Cari anak terpecebol di area sisa [14, 35, 30, 66, 26]. Ditemukan si `14`. Tukar paksa dudukan dengan `30`. Array mutasi -> `[13, 14, 35, 30, 66, 26]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 14, 35, 30, 66, 26]**. Opsi murni: **D**.
</details>

---
**Soal 234**
Bebek-bebek di barisan bernomor dada: `[71, 10, 53, 82, 56, 74]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [10, 53, 71, 82, 56, 74]
B. [53, 74, 56, 71, 10, 82]
C. [53, 56, 10, 71, 74, 82]
D. [56, 74, 53, 82, 10, 71]
E. [53, 10, 82, 71, 74, 56]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([10, 53, 71, 82, 56, 74])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[71, 10, 53, 82, 56, 74]`
- Putaran 1: Cari anak terpecebol di area sisa [10, 71, 53, 82, 56, 74]. Ditemukan si `10`. Tukar paksa dudukan dengan `71`. Array mutasi -> `[10, 71, 53, 82, 56, 74]`
- Putaran 2: Cari anak terpecebol di area sisa [53, 71, 82, 56, 74]. Ditemukan si `53`. Tukar paksa dudukan dengan `71`. Array mutasi -> `[10, 53, 71, 82, 56, 74]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[10, 53, 71, 82, 56, 74]**. Opsi murni: **A**.
</details>

---
**Soal 235**
Diberikan barisan angka: `[15, 50, 14, 77, 92]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [14, 15, 92, 77, 50]
B. [50, 77, 14, 15, 92]
C. [15, 14, 50, 77, 92]
D. [50, 92, 77, 15, 14]
E. [15, 50, 77, 14, 92]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([15, 14, 50, 77, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[15, 50, 14, 77, 92]`
Cek posisi 0&1 (15 < 50) -> Aman dibiarkan. Array kini: `[15, 50, 14, 77, 92]`
Cek posisi 1&2 (50 > 14) -> Tukar! Array kini: `[15, 14, 50, 77, 92]`
Cek posisi 2&3 (50 < 77) -> Aman dibiarkan. Array kini: `[15, 14, 50, 77, 92]`
Cek posisi 3&4 (77 < 92) -> Aman dibiarkan. Array kini: `[15, 14, 50, 77, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[15, 14, 50, 77, 92]**.
</details>

---
**Soal 236**
Pak Dengklek memiliki daftar absensi **1940 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 14 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1940 elemen
- Langkah 1: Sisa populasi tebasan separuh = 970 elemen
- Langkah 2: Sisa populasi tebasan separuh = 485 elemen
- Langkah 3: Sisa populasi tebasan separuh = 243 elemen
- Langkah 4: Sisa populasi tebasan separuh = 122 elemen
- Langkah 5: Sisa populasi tebasan separuh = 61 elemen
- Langkah 6: Sisa populasi tebasan separuh = 31 elemen
- Langkah 7: Sisa populasi tebasan separuh = 16 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 237**
Pak Dengklek memiliki daftar absensi **1151 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 11 langkah
D. 10 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1151 elemen
- Langkah 1: Sisa populasi tebasan separuh = 576 elemen
- Langkah 2: Sisa populasi tebasan separuh = 288 elemen
- Langkah 3: Sisa populasi tebasan separuh = 144 elemen
- Langkah 4: Sisa populasi tebasan separuh = 72 elemen
- Langkah 5: Sisa populasi tebasan separuh = 36 elemen
- Langkah 6: Sisa populasi tebasan separuh = 18 elemen
- Langkah 7: Sisa populasi tebasan separuh = 9 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 238**
Bebek-bebek di barisan bernomor dada: `[20, 94, 50, 68, 81, 73]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [20, 50, 94, 68, 81, 73]
B. [68, 94, 73, 50, 20, 81]
C. [50, 94, 73, 68, 81, 20]
D. [68, 94, 50, 20, 73, 81]
E. [20, 94, 81, 68, 50, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([20, 50, 94, 68, 81, 73])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[20, 94, 50, 68, 81, 73]`
- Putaran 1: Cari anak terpecebol di area sisa [20, 94, 50, 68, 81, 73]. Ditemukan si `20`. Tukar paksa dudukan dengan `20`. Array mutasi -> `[20, 94, 50, 68, 81, 73]`
- Putaran 2: Cari anak terpecebol di area sisa [50, 94, 68, 81, 73]. Ditemukan si `50`. Tukar paksa dudukan dengan `94`. Array mutasi -> `[20, 50, 94, 68, 81, 73]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[20, 50, 94, 68, 81, 73]**. Opsi murni: **A**.
</details>

---
**Soal 239**
Bebek-bebek di barisan bernomor dada: `[35, 47, 65, 90, 89, 27]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [89, 65, 90, 35, 47, 27]
B. [35, 65, 47, 27, 90, 89]
C. [35, 65, 90, 47, 27, 89]
D. [90, 27, 89, 65, 35, 47]
E. [27, 35, 65, 90, 89, 47]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([27, 35, 65, 90, 89, 47])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[35, 47, 65, 90, 89, 27]`
- Putaran 1: Cari anak terpecebol di area sisa [27, 47, 65, 90, 89, 35]. Ditemukan si `27`. Tukar paksa dudukan dengan `35`. Array mutasi -> `[27, 47, 65, 90, 89, 35]`
- Putaran 2: Cari anak terpecebol di area sisa [35, 65, 90, 89, 47]. Ditemukan si `35`. Tukar paksa dudukan dengan `47`. Array mutasi -> `[27, 35, 65, 90, 89, 47]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[27, 35, 65, 90, 89, 47]**. Opsi murni: **E**.
</details>

---
**Soal 240**
Bebek-bebek di barisan bernomor dada: `[69, 89, 49, 84, 51, 12]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [51, 69, 12, 49, 89, 84]
B. [12, 49, 89, 84, 51, 69]
C. [84, 89, 49, 69, 51, 12]
D. [49, 89, 69, 51, 84, 12]
E. [49, 89, 84, 51, 12, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([12, 49, 89, 84, 51, 69])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[69, 89, 49, 84, 51, 12]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 89, 49, 84, 51, 69]. Ditemukan si `12`. Tukar paksa dudukan dengan `69`. Array mutasi -> `[12, 89, 49, 84, 51, 69]`
- Putaran 2: Cari anak terpecebol di area sisa [49, 89, 84, 51, 69]. Ditemukan si `49`. Tukar paksa dudukan dengan `89`. Array mutasi -> `[12, 49, 89, 84, 51, 69]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 49, 89, 84, 51, 69]**. Opsi murni: **B**.
</details>

---
**Soal 241**
Diberikan barisan angka: `[34, 14, 30, 67, 23]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [67, 14, 30, 23, 34]
B. [14, 30, 34, 23, 67]
C. [14, 67, 30, 23, 34]
D. [23, 14, 34, 67, 30]
E. [14, 23, 67, 34, 30]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([14, 30, 34, 23, 67])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[34, 14, 30, 67, 23]`
Cek posisi 0&1 (34 > 14) -> Tukar! Array kini: `[14, 34, 30, 67, 23]`
Cek posisi 1&2 (34 > 30) -> Tukar! Array kini: `[14, 30, 34, 67, 23]`
Cek posisi 2&3 (34 < 67) -> Aman dibiarkan. Array kini: `[14, 30, 34, 67, 23]`
Cek posisi 3&4 (67 > 23) -> Tukar! Array kini: `[14, 30, 34, 23, 67]`


Terbukti bahwa elemen maha gemuk (`67`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[14, 30, 34, 23, 67]**.
</details>

---
**Soal 242**
Bebek-bebek di barisan bernomor dada: `[98, 55, 13, 42, 33, 57]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [98, 13, 33, 57, 42, 55]
B. [57, 98, 33, 42, 13, 55]
C. [42, 33, 13, 57, 98, 55]
D. [13, 33, 98, 42, 55, 57]
E. [42, 55, 33, 98, 57, 13]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([13, 33, 98, 42, 55, 57])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[98, 55, 13, 42, 33, 57]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 55, 98, 42, 33, 57]. Ditemukan si `13`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[13, 55, 98, 42, 33, 57]`
- Putaran 2: Cari anak terpecebol di area sisa [33, 98, 42, 55, 57]. Ditemukan si `33`. Tukar paksa dudukan dengan `55`. Array mutasi -> `[13, 33, 98, 42, 55, 57]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 33, 98, 42, 55, 57]**. Opsi murni: **D**.
</details>

---
**Soal 243**
Bebek-bebek di barisan bernomor dada: `[36, 27, 54, 53, 86, 56]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [53, 36, 54, 27, 86, 56]
B. [27, 36, 54, 53, 86, 56]
C. [54, 36, 53, 86, 27, 56]
D. [54, 56, 86, 27, 53, 36]
E. [54, 27, 53, 56, 86, 36]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([27, 36, 54, 53, 86, 56])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[36, 27, 54, 53, 86, 56]`
- Putaran 1: Cari anak terpecebol di area sisa [27, 36, 54, 53, 86, 56]. Ditemukan si `27`. Tukar paksa dudukan dengan `36`. Array mutasi -> `[27, 36, 54, 53, 86, 56]`
- Putaran 2: Cari anak terpecebol di area sisa [36, 54, 53, 86, 56]. Ditemukan si `36`. Tukar paksa dudukan dengan `36`. Array mutasi -> `[27, 36, 54, 53, 86, 56]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[27, 36, 54, 53, 86, 56]**. Opsi murni: **B**.
</details>

---
**Soal 244**
Bebek-bebek di barisan bernomor dada: `[47, 61, 83, 15, 98, 41]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [61, 47, 83, 15, 41, 98]
B. [15, 61, 47, 41, 98, 83]
C. [15, 41, 83, 47, 98, 61]
D. [61, 98, 83, 47, 15, 41]
E. [41, 47, 15, 98, 83, 61]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([15, 41, 83, 47, 98, 61])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[47, 61, 83, 15, 98, 41]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 61, 83, 47, 98, 41]. Ditemukan si `15`. Tukar paksa dudukan dengan `47`. Array mutasi -> `[15, 61, 83, 47, 98, 41]`
- Putaran 2: Cari anak terpecebol di area sisa [41, 83, 47, 98, 61]. Ditemukan si `41`. Tukar paksa dudukan dengan `61`. Array mutasi -> `[15, 41, 83, 47, 98, 61]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 41, 83, 47, 98, 61]**. Opsi murni: **C**.
</details>

---
**Soal 245**
Bebek-bebek di barisan bernomor dada: `[29, 40, 17, 56, 74, 15]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [15, 29, 56, 40, 74, 17]
B. [56, 17, 74, 15, 40, 29]
C. [15, 17, 40, 56, 74, 29]
D. [15, 17, 29, 74, 40, 56]
E. [56, 29, 17, 74, 15, 40]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([15, 17, 40, 56, 74, 29])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[29, 40, 17, 56, 74, 15]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 40, 17, 56, 74, 29]. Ditemukan si `15`. Tukar paksa dudukan dengan `29`. Array mutasi -> `[15, 40, 17, 56, 74, 29]`
- Putaran 2: Cari anak terpecebol di area sisa [17, 40, 56, 74, 29]. Ditemukan si `17`. Tukar paksa dudukan dengan `40`. Array mutasi -> `[15, 17, 40, 56, 74, 29]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 17, 40, 56, 74, 29]**. Opsi murni: **C**.
</details>

---
**Soal 246**
Bebek-bebek di barisan bernomor dada: `[25, 38, 82, 46, 11, 17]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [17, 11, 38, 46, 25, 82]
B. [25, 82, 17, 38, 46, 11]
C. [11, 17, 82, 46, 25, 38]
D. [11, 82, 46, 17, 38, 25]
E. [82, 46, 38, 17, 25, 11]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([11, 17, 82, 46, 25, 38])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[25, 38, 82, 46, 11, 17]`
- Putaran 1: Cari anak terpecebol di area sisa [11, 38, 82, 46, 25, 17]. Ditemukan si `11`. Tukar paksa dudukan dengan `25`. Array mutasi -> `[11, 38, 82, 46, 25, 17]`
- Putaran 2: Cari anak terpecebol di area sisa [17, 82, 46, 25, 38]. Ditemukan si `17`. Tukar paksa dudukan dengan `38`. Array mutasi -> `[11, 17, 82, 46, 25, 38]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[11, 17, 82, 46, 25, 38]**. Opsi murni: **C**.
</details>

---
**Soal 247**
Pak Dengklek memiliki daftar absensi **1161 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 13 langkah
C. 14 langkah
D. 12 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1161 elemen
- Langkah 1: Sisa populasi tebasan separuh = 581 elemen
- Langkah 2: Sisa populasi tebasan separuh = 291 elemen
- Langkah 3: Sisa populasi tebasan separuh = 146 elemen
- Langkah 4: Sisa populasi tebasan separuh = 73 elemen
- Langkah 5: Sisa populasi tebasan separuh = 37 elemen
- Langkah 6: Sisa populasi tebasan separuh = 19 elemen
- Langkah 7: Sisa populasi tebasan separuh = 10 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 248**
Pak Dengklek memiliki daftar absensi **1782 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 12 langkah
C. 11 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1782 elemen
- Langkah 1: Sisa populasi tebasan separuh = 891 elemen
- Langkah 2: Sisa populasi tebasan separuh = 446 elemen
- Langkah 3: Sisa populasi tebasan separuh = 223 elemen
- Langkah 4: Sisa populasi tebasan separuh = 112 elemen
- Langkah 5: Sisa populasi tebasan separuh = 56 elemen
- Langkah 6: Sisa populasi tebasan separuh = 28 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 249**
Diberikan barisan angka: `[62, 75, 21, 64, 49]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [75, 62, 21, 49, 64]
B. [62, 21, 64, 75, 49]
C. [62, 21, 64, 49, 75]
D. [64, 75, 49, 62, 21]
E. [49, 64, 62, 75, 21]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([62, 21, 64, 49, 75])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[62, 75, 21, 64, 49]`
Cek posisi 0&1 (62 < 75) -> Aman dibiarkan. Array kini: `[62, 75, 21, 64, 49]`
Cek posisi 1&2 (75 > 21) -> Tukar! Array kini: `[62, 21, 75, 64, 49]`
Cek posisi 2&3 (75 > 64) -> Tukar! Array kini: `[62, 21, 64, 75, 49]`
Cek posisi 3&4 (75 > 49) -> Tukar! Array kini: `[62, 21, 64, 49, 75]`


Terbukti bahwa elemen maha gemuk (`75`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[62, 21, 64, 49, 75]**.
</details>

---
**Soal 250**
Bebek-bebek di barisan bernomor dada: `[35, 86, 54, 17, 40, 73]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [17, 35, 54, 86, 40, 73]
B. [86, 40, 17, 73, 35, 54]
C. [73, 40, 86, 17, 35, 54]
D. [54, 35, 40, 73, 17, 86]
E. [40, 73, 54, 17, 35, 86]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([17, 35, 54, 86, 40, 73])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[35, 86, 54, 17, 40, 73]`
- Putaran 1: Cari anak terpecebol di area sisa [17, 86, 54, 35, 40, 73]. Ditemukan si `17`. Tukar paksa dudukan dengan `35`. Array mutasi -> `[17, 86, 54, 35, 40, 73]`
- Putaran 2: Cari anak terpecebol di area sisa [35, 54, 86, 40, 73]. Ditemukan si `35`. Tukar paksa dudukan dengan `86`. Array mutasi -> `[17, 35, 54, 86, 40, 73]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[17, 35, 54, 86, 40, 73]**. Opsi murni: **A**.
</details>

---
