# Latian Soal: Pencarian & Pengurutan (Part 1 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 1**
Diberikan barisan angka: `[92, 27, 26, 24, 48]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [26, 27, 92, 24, 48]
B. [26, 24, 92, 27, 48]
C. [24, 27, 48, 26, 92]
D. [27, 26, 24, 48, 92]
E. [48, 24, 27, 92, 26]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([27, 26, 24, 48, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[92, 27, 26, 24, 48]`
Cek posisi 0&1 (92 > 27) -> Tukar! Array kini: `[27, 92, 26, 24, 48]`
Cek posisi 1&2 (92 > 26) -> Tukar! Array kini: `[27, 26, 92, 24, 48]`
Cek posisi 2&3 (92 > 24) -> Tukar! Array kini: `[27, 26, 24, 92, 48]`
Cek posisi 3&4 (92 > 48) -> Tukar! Array kini: `[27, 26, 24, 48, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[27, 26, 24, 48, 92]**.
</details>

---
**Soal 2**
Diberikan barisan angka: `[20, 95, 75, 47, 64]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [64, 47, 75, 20, 95]
B. [64, 47, 95, 20, 75]
C. [95, 20, 75, 64, 47]
D. [20, 75, 47, 64, 95]
E. [64, 75, 47, 20, 95]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([20, 75, 47, 64, 95])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[20, 95, 75, 47, 64]`
Cek posisi 0&1 (20 < 95) -> Aman dibiarkan. Array kini: `[20, 95, 75, 47, 64]`
Cek posisi 1&2 (95 > 75) -> Tukar! Array kini: `[20, 75, 95, 47, 64]`
Cek posisi 2&3 (95 > 47) -> Tukar! Array kini: `[20, 75, 47, 95, 64]`
Cek posisi 3&4 (95 > 64) -> Tukar! Array kini: `[20, 75, 47, 64, 95]`


Terbukti bahwa elemen maha gemuk (`95`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[20, 75, 47, 64, 95]**.
</details>

---
**Soal 3**
Bebek-bebek di barisan bernomor dada: `[69, 87, 32, 14, 11, 26]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [14, 32, 69, 11, 87, 26]
B. [11, 14, 32, 87, 69, 26]
C. [11, 87, 32, 69, 26, 14]
D. [69, 11, 26, 32, 87, 14]
E. [32, 87, 26, 11, 14, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([11, 14, 32, 87, 69, 26])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[69, 87, 32, 14, 11, 26]`
- Putaran 1: Cari anak terpecebol di area sisa [11, 87, 32, 14, 69, 26]. Ditemukan si `11`. Tukar paksa dudukan dengan `69`. Array mutasi -> `[11, 87, 32, 14, 69, 26]`
- Putaran 2: Cari anak terpecebol di area sisa [14, 32, 87, 69, 26]. Ditemukan si `14`. Tukar paksa dudukan dengan `87`. Array mutasi -> `[11, 14, 32, 87, 69, 26]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[11, 14, 32, 87, 69, 26]**. Opsi murni: **B**.
</details>

---
**Soal 4**
Bebek-bebek di barisan bernomor dada: `[77, 79, 21, 49, 42, 37]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [77, 21, 37, 49, 42, 79]
B. [21, 37, 77, 49, 42, 79]
C. [42, 21, 37, 77, 49, 79]
D. [49, 21, 77, 42, 37, 79]
E. [21, 49, 42, 37, 77, 79]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([21, 37, 77, 49, 42, 79])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[77, 79, 21, 49, 42, 37]`
- Putaran 1: Cari anak terpecebol di area sisa [21, 79, 77, 49, 42, 37]. Ditemukan si `21`. Tukar paksa dudukan dengan `77`. Array mutasi -> `[21, 79, 77, 49, 42, 37]`
- Putaran 2: Cari anak terpecebol di area sisa [37, 77, 49, 42, 79]. Ditemukan si `37`. Tukar paksa dudukan dengan `79`. Array mutasi -> `[21, 37, 77, 49, 42, 79]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[21, 37, 77, 49, 42, 79]**. Opsi murni: **B**.
</details>

---
**Soal 5**
Bebek-bebek di barisan bernomor dada: `[51, 83, 87, 90, 94, 52]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [51, 94, 87, 90, 52, 83]
B. [83, 52, 90, 87, 51, 94]
C. [90, 87, 83, 52, 51, 94]
D. [51, 52, 87, 90, 94, 83]
E. [90, 94, 83, 87, 52, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([51, 52, 87, 90, 94, 83])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[51, 83, 87, 90, 94, 52]`
- Putaran 1: Cari anak terpecebol di area sisa [51, 83, 87, 90, 94, 52]. Ditemukan si `51`. Tukar paksa dudukan dengan `51`. Array mutasi -> `[51, 83, 87, 90, 94, 52]`
- Putaran 2: Cari anak terpecebol di area sisa [52, 87, 90, 94, 83]. Ditemukan si `52`. Tukar paksa dudukan dengan `83`. Array mutasi -> `[51, 52, 87, 90, 94, 83]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[51, 52, 87, 90, 94, 83]**. Opsi murni: **D**.
</details>

---
**Soal 6**
Bebek-bebek di barisan bernomor dada: `[62, 44, 76, 96, 31, 18]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [76, 62, 96, 44, 31, 18]
B. [44, 96, 76, 18, 31, 62]
C. [18, 31, 76, 96, 44, 62]
D. [18, 96, 44, 62, 31, 76]
E. [31, 76, 96, 44, 18, 62]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([18, 31, 76, 96, 44, 62])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[62, 44, 76, 96, 31, 18]`
- Putaran 1: Cari anak terpecebol di area sisa [18, 44, 76, 96, 31, 62]. Ditemukan si `18`. Tukar paksa dudukan dengan `62`. Array mutasi -> `[18, 44, 76, 96, 31, 62]`
- Putaran 2: Cari anak terpecebol di area sisa [31, 76, 96, 44, 62]. Ditemukan si `31`. Tukar paksa dudukan dengan `44`. Array mutasi -> `[18, 31, 76, 96, 44, 62]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[18, 31, 76, 96, 44, 62]**. Opsi murni: **C**.
</details>

---
**Soal 7**
Diberikan barisan angka: `[40, 51, 12, 69, 86]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [12, 51, 40, 86, 69]
B. [40, 12, 51, 69, 86]
C. [40, 86, 12, 51, 69]
D. [86, 12, 40, 51, 69]
E. [69, 51, 86, 12, 40]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([40, 12, 51, 69, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[40, 51, 12, 69, 86]`
Cek posisi 0&1 (40 < 51) -> Aman dibiarkan. Array kini: `[40, 51, 12, 69, 86]`
Cek posisi 1&2 (51 > 12) -> Tukar! Array kini: `[40, 12, 51, 69, 86]`
Cek posisi 2&3 (51 < 69) -> Aman dibiarkan. Array kini: `[40, 12, 51, 69, 86]`
Cek posisi 3&4 (69 < 86) -> Aman dibiarkan. Array kini: `[40, 12, 51, 69, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[40, 12, 51, 69, 86]**.
</details>

---
**Soal 8**
Pak Dengklek memiliki daftar absensi **743 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 9 langkah
C. 11 langkah
D. 10 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 743 elemen
- Langkah 1: Sisa populasi tebasan separuh = 372 elemen
- Langkah 2: Sisa populasi tebasan separuh = 186 elemen
- Langkah 3: Sisa populasi tebasan separuh = 93 elemen
- Langkah 4: Sisa populasi tebasan separuh = 47 elemen
- Langkah 5: Sisa populasi tebasan separuh = 24 elemen
- Langkah 6: Sisa populasi tebasan separuh = 12 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 9**
Pak Dengklek memiliki daftar absensi **1766 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 13 langkah
C. 11 langkah
D. 10 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1766 elemen
- Langkah 1: Sisa populasi tebasan separuh = 883 elemen
- Langkah 2: Sisa populasi tebasan separuh = 442 elemen
- Langkah 3: Sisa populasi tebasan separuh = 221 elemen
- Langkah 4: Sisa populasi tebasan separuh = 111 elemen
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
**Soal 10**
Diberikan barisan angka: `[39, 94, 28, 67, 98]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [39, 28, 67, 94, 98]
B. [67, 98, 28, 94, 39]
C. [28, 39, 67, 94, 98]
D. [67, 39, 28, 94, 98]
E. [28, 98, 67, 94, 39]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([39, 28, 67, 94, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[39, 94, 28, 67, 98]`
Cek posisi 0&1 (39 < 94) -> Aman dibiarkan. Array kini: `[39, 94, 28, 67, 98]`
Cek posisi 1&2 (94 > 28) -> Tukar! Array kini: `[39, 28, 94, 67, 98]`
Cek posisi 2&3 (94 > 67) -> Tukar! Array kini: `[39, 28, 67, 94, 98]`
Cek posisi 3&4 (94 < 98) -> Aman dibiarkan. Array kini: `[39, 28, 67, 94, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[39, 28, 67, 94, 98]**.
</details>

---
**Soal 11**
Pak Dengklek memiliki daftar absensi **1077 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 14 langkah
C. 13 langkah
D. 12 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1077 elemen
- Langkah 1: Sisa populasi tebasan separuh = 539 elemen
- Langkah 2: Sisa populasi tebasan separuh = 270 elemen
- Langkah 3: Sisa populasi tebasan separuh = 135 elemen
- Langkah 4: Sisa populasi tebasan separuh = 68 elemen
- Langkah 5: Sisa populasi tebasan separuh = 34 elemen
- Langkah 6: Sisa populasi tebasan separuh = 17 elemen
- Langkah 7: Sisa populasi tebasan separuh = 9 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 12**
Pak Dengklek memiliki daftar absensi **1561 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 11 langkah
D. 13 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1561 elemen
- Langkah 1: Sisa populasi tebasan separuh = 781 elemen
- Langkah 2: Sisa populasi tebasan separuh = 391 elemen
- Langkah 3: Sisa populasi tebasan separuh = 196 elemen
- Langkah 4: Sisa populasi tebasan separuh = 98 elemen
- Langkah 5: Sisa populasi tebasan separuh = 49 elemen
- Langkah 6: Sisa populasi tebasan separuh = 25 elemen
- Langkah 7: Sisa populasi tebasan separuh = 13 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 13**
Bebek-bebek di barisan bernomor dada: `[11, 92, 38, 47, 14, 73]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [73, 92, 11, 14, 38, 47]
B. [92, 14, 73, 11, 38, 47]
C. [11, 92, 14, 73, 38, 47]
D. [11, 92, 14, 47, 38, 73]
E. [11, 14, 38, 47, 92, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([11, 14, 38, 47, 92, 73])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[11, 92, 38, 47, 14, 73]`
- Putaran 1: Cari anak terpecebol di area sisa [11, 92, 38, 47, 14, 73]. Ditemukan si `11`. Tukar paksa dudukan dengan `11`. Array mutasi -> `[11, 92, 38, 47, 14, 73]`
- Putaran 2: Cari anak terpecebol di area sisa [14, 38, 47, 92, 73]. Ditemukan si `14`. Tukar paksa dudukan dengan `92`. Array mutasi -> `[11, 14, 38, 47, 92, 73]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[11, 14, 38, 47, 92, 73]**. Opsi murni: **E**.
</details>

---
**Soal 14**
Pak Dengklek memiliki daftar absensi **1137 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 13 langkah
D. 10 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1137 elemen
- Langkah 1: Sisa populasi tebasan separuh = 569 elemen
- Langkah 2: Sisa populasi tebasan separuh = 285 elemen
- Langkah 3: Sisa populasi tebasan separuh = 143 elemen
- Langkah 4: Sisa populasi tebasan separuh = 72 elemen
- Langkah 5: Sisa populasi tebasan separuh = 36 elemen
- Langkah 6: Sisa populasi tebasan separuh = 18 elemen
- Langkah 7: Sisa populasi tebasan separuh = 9 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 15**
Diberikan barisan angka: `[77, 11, 82, 72, 91]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [11, 77, 72, 82, 91]
B. [91, 77, 11, 82, 72]
C. [11, 72, 77, 82, 91]
D. [11, 91, 72, 82, 77]
E. [82, 77, 11, 91, 72]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([11, 77, 72, 82, 91])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[77, 11, 82, 72, 91]`
Cek posisi 0&1 (77 > 11) -> Tukar! Array kini: `[11, 77, 82, 72, 91]`
Cek posisi 1&2 (77 < 82) -> Aman dibiarkan. Array kini: `[11, 77, 82, 72, 91]`
Cek posisi 2&3 (82 > 72) -> Tukar! Array kini: `[11, 77, 72, 82, 91]`
Cek posisi 3&4 (82 < 91) -> Aman dibiarkan. Array kini: `[11, 77, 72, 82, 91]`


Terbukti bahwa elemen maha gemuk (`91`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[11, 77, 72, 82, 91]**.
</details>

---
**Soal 16**
Pak Dengklek memiliki daftar absensi **1939 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 14 langkah
C. 10 langkah
D. 12 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1939 elemen
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
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 17**
Diberikan barisan angka: `[90, 78, 16, 88, 72]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [72, 78, 88, 16, 90]
B. [72, 78, 90, 88, 16]
C. [78, 72, 16, 90, 88]
D. [78, 16, 88, 72, 90]
E. [88, 16, 72, 78, 90]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([78, 16, 88, 72, 90])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[90, 78, 16, 88, 72]`
Cek posisi 0&1 (90 > 78) -> Tukar! Array kini: `[78, 90, 16, 88, 72]`
Cek posisi 1&2 (90 > 16) -> Tukar! Array kini: `[78, 16, 90, 88, 72]`
Cek posisi 2&3 (90 > 88) -> Tukar! Array kini: `[78, 16, 88, 90, 72]`
Cek posisi 3&4 (90 > 72) -> Tukar! Array kini: `[78, 16, 88, 72, 90]`


Terbukti bahwa elemen maha gemuk (`90`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[78, 16, 88, 72, 90]**.
</details>

---
**Soal 18**
Pak Dengklek memiliki daftar absensi **1592 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 13 langkah
D. 14 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1592 elemen
- Langkah 1: Sisa populasi tebasan separuh = 796 elemen
- Langkah 2: Sisa populasi tebasan separuh = 398 elemen
- Langkah 3: Sisa populasi tebasan separuh = 199 elemen
- Langkah 4: Sisa populasi tebasan separuh = 100 elemen
- Langkah 5: Sisa populasi tebasan separuh = 50 elemen
- Langkah 6: Sisa populasi tebasan separuh = 25 elemen
- Langkah 7: Sisa populasi tebasan separuh = 13 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 19**
Bebek-bebek di barisan bernomor dada: `[29, 35, 32, 38, 25, 14]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [29, 25, 14, 38, 32, 35]
B. [14, 25, 32, 38, 35, 29]
C. [32, 29, 25, 14, 35, 38]
D. [14, 35, 38, 32, 25, 29]
E. [25, 14, 35, 29, 32, 38]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([14, 25, 32, 38, 35, 29])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[29, 35, 32, 38, 25, 14]`
- Putaran 1: Cari anak terpecebol di area sisa [14, 35, 32, 38, 25, 29]. Ditemukan si `14`. Tukar paksa dudukan dengan `29`. Array mutasi -> `[14, 35, 32, 38, 25, 29]`
- Putaran 2: Cari anak terpecebol di area sisa [25, 32, 38, 35, 29]. Ditemukan si `25`. Tukar paksa dudukan dengan `35`. Array mutasi -> `[14, 25, 32, 38, 35, 29]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[14, 25, 32, 38, 35, 29]**. Opsi murni: **B**.
</details>

---
**Soal 20**
Bebek-bebek di barisan bernomor dada: `[12, 29, 69, 33, 86, 95]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [33, 95, 86, 69, 29, 12]
B. [29, 86, 69, 12, 95, 33]
C. [12, 69, 29, 95, 33, 86]
D. [86, 12, 69, 33, 95, 29]
E. [12, 29, 69, 33, 86, 95]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([12, 29, 69, 33, 86, 95])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[12, 29, 69, 33, 86, 95]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 29, 69, 33, 86, 95]. Ditemukan si `12`. Tukar paksa dudukan dengan `12`. Array mutasi -> `[12, 29, 69, 33, 86, 95]`
- Putaran 2: Cari anak terpecebol di area sisa [29, 69, 33, 86, 95]. Ditemukan si `29`. Tukar paksa dudukan dengan `29`. Array mutasi -> `[12, 29, 69, 33, 86, 95]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 29, 69, 33, 86, 95]**. Opsi murni: **E**.
</details>

---
**Soal 21**
Bebek-bebek di barisan bernomor dada: `[61, 57, 33, 42, 95, 96]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [96, 57, 33, 61, 42, 95]
B. [33, 42, 61, 57, 95, 96]
C. [33, 57, 95, 61, 96, 42]
D. [95, 57, 33, 96, 42, 61]
E. [61, 57, 96, 42, 95, 33]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([33, 42, 61, 57, 95, 96])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[61, 57, 33, 42, 95, 96]`
- Putaran 1: Cari anak terpecebol di area sisa [33, 57, 61, 42, 95, 96]. Ditemukan si `33`. Tukar paksa dudukan dengan `61`. Array mutasi -> `[33, 57, 61, 42, 95, 96]`
- Putaran 2: Cari anak terpecebol di area sisa [42, 61, 57, 95, 96]. Ditemukan si `42`. Tukar paksa dudukan dengan `57`. Array mutasi -> `[33, 42, 61, 57, 95, 96]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[33, 42, 61, 57, 95, 96]**. Opsi murni: **B**.
</details>

---
**Soal 22**
Bebek-bebek di barisan bernomor dada: `[43, 14, 95, 62, 85, 69]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [69, 85, 62, 95, 43, 14]
B. [69, 14, 62, 85, 43, 95]
C. [95, 85, 14, 62, 69, 43]
D. [85, 43, 14, 62, 69, 95]
E. [14, 43, 95, 62, 85, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([14, 43, 95, 62, 85, 69])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[43, 14, 95, 62, 85, 69]`
- Putaran 1: Cari anak terpecebol di area sisa [14, 43, 95, 62, 85, 69]. Ditemukan si `14`. Tukar paksa dudukan dengan `43`. Array mutasi -> `[14, 43, 95, 62, 85, 69]`
- Putaran 2: Cari anak terpecebol di area sisa [43, 95, 62, 85, 69]. Ditemukan si `43`. Tukar paksa dudukan dengan `43`. Array mutasi -> `[14, 43, 95, 62, 85, 69]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[14, 43, 95, 62, 85, 69]**. Opsi murni: **E**.
</details>

---
**Soal 23**
Diberikan barisan angka: `[74, 68, 90, 30, 85]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [68, 90, 30, 85, 74]
B. [74, 85, 68, 90, 30]
C. [68, 90, 85, 30, 74]
D. [74, 68, 30, 85, 90]
E. [68, 74, 30, 85, 90]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([68, 74, 30, 85, 90])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[74, 68, 90, 30, 85]`
Cek posisi 0&1 (74 > 68) -> Tukar! Array kini: `[68, 74, 90, 30, 85]`
Cek posisi 1&2 (74 < 90) -> Aman dibiarkan. Array kini: `[68, 74, 90, 30, 85]`
Cek posisi 2&3 (90 > 30) -> Tukar! Array kini: `[68, 74, 30, 90, 85]`
Cek posisi 3&4 (90 > 85) -> Tukar! Array kini: `[68, 74, 30, 85, 90]`


Terbukti bahwa elemen maha gemuk (`90`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[68, 74, 30, 85, 90]**.
</details>

---
**Soal 24**
Diberikan barisan angka: `[96, 62, 68, 78, 11]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [62, 11, 96, 68, 78]
B. [62, 68, 11, 96, 78]
C. [62, 68, 78, 11, 96]
D. [78, 62, 68, 11, 96]
E. [78, 62, 11, 68, 96]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([62, 68, 78, 11, 96])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[96, 62, 68, 78, 11]`
Cek posisi 0&1 (96 > 62) -> Tukar! Array kini: `[62, 96, 68, 78, 11]`
Cek posisi 1&2 (96 > 68) -> Tukar! Array kini: `[62, 68, 96, 78, 11]`
Cek posisi 2&3 (96 > 78) -> Tukar! Array kini: `[62, 68, 78, 96, 11]`
Cek posisi 3&4 (96 > 11) -> Tukar! Array kini: `[62, 68, 78, 11, 96]`


Terbukti bahwa elemen maha gemuk (`96`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[62, 68, 78, 11, 96]**.
</details>

---
**Soal 25**
Bebek-bebek di barisan bernomor dada: `[54, 80, 46, 58, 71, 73]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [73, 58, 54, 46, 80, 71]
B. [54, 58, 71, 73, 80, 46]
C. [71, 54, 46, 80, 73, 58]
D. [46, 71, 80, 58, 73, 54]
E. [46, 54, 80, 58, 71, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([46, 54, 80, 58, 71, 73])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[54, 80, 46, 58, 71, 73]`
- Putaran 1: Cari anak terpecebol di area sisa [46, 80, 54, 58, 71, 73]. Ditemukan si `46`. Tukar paksa dudukan dengan `54`. Array mutasi -> `[46, 80, 54, 58, 71, 73]`
- Putaran 2: Cari anak terpecebol di area sisa [54, 80, 58, 71, 73]. Ditemukan si `54`. Tukar paksa dudukan dengan `80`. Array mutasi -> `[46, 54, 80, 58, 71, 73]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[46, 54, 80, 58, 71, 73]**. Opsi murni: **E**.
</details>

---
**Soal 26**
Bebek-bebek di barisan bernomor dada: `[31, 36, 24, 88, 58, 23]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [24, 88, 31, 36, 58, 23]
B. [24, 23, 58, 36, 31, 88]
C. [36, 24, 58, 23, 31, 88]
D. [31, 23, 24, 58, 36, 88]
E. [23, 24, 36, 88, 58, 31]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([23, 24, 36, 88, 58, 31])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[31, 36, 24, 88, 58, 23]`
- Putaran 1: Cari anak terpecebol di area sisa [23, 36, 24, 88, 58, 31]. Ditemukan si `23`. Tukar paksa dudukan dengan `31`. Array mutasi -> `[23, 36, 24, 88, 58, 31]`
- Putaran 2: Cari anak terpecebol di area sisa [24, 36, 88, 58, 31]. Ditemukan si `24`. Tukar paksa dudukan dengan `36`. Array mutasi -> `[23, 24, 36, 88, 58, 31]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[23, 24, 36, 88, 58, 31]**. Opsi murni: **E**.
</details>

---
**Soal 27**
Diberikan barisan angka: `[29, 47, 49, 58, 92]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [49, 92, 29, 47, 58]
B. [49, 47, 58, 29, 92]
C. [92, 58, 47, 49, 29]
D. [29, 47, 49, 58, 92]
E. [29, 49, 47, 92, 58]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([29, 47, 49, 58, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[29, 47, 49, 58, 92]`
Cek posisi 0&1 (29 < 47) -> Aman dibiarkan. Array kini: `[29, 47, 49, 58, 92]`
Cek posisi 1&2 (47 < 49) -> Aman dibiarkan. Array kini: `[29, 47, 49, 58, 92]`
Cek posisi 2&3 (49 < 58) -> Aman dibiarkan. Array kini: `[29, 47, 49, 58, 92]`
Cek posisi 3&4 (58 < 92) -> Aman dibiarkan. Array kini: `[29, 47, 49, 58, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[29, 47, 49, 58, 92]**.
</details>

---
**Soal 28**
Diberikan barisan angka: `[46, 56, 10, 81, 60]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [56, 10, 60, 81, 46]
B. [10, 81, 46, 56, 60]
C. [46, 10, 56, 60, 81]
D. [60, 10, 56, 46, 81]
E. [46, 56, 60, 81, 10]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([46, 10, 56, 60, 81])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[46, 56, 10, 81, 60]`
Cek posisi 0&1 (46 < 56) -> Aman dibiarkan. Array kini: `[46, 56, 10, 81, 60]`
Cek posisi 1&2 (56 > 10) -> Tukar! Array kini: `[46, 10, 56, 81, 60]`
Cek posisi 2&3 (56 < 81) -> Aman dibiarkan. Array kini: `[46, 10, 56, 81, 60]`
Cek posisi 3&4 (81 > 60) -> Tukar! Array kini: `[46, 10, 56, 60, 81]`


Terbukti bahwa elemen maha gemuk (`81`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[46, 10, 56, 60, 81]**.
</details>

---
**Soal 29**
Diberikan barisan angka: `[82, 21, 98, 25, 59]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [21, 82, 59, 98, 25]
B. [59, 25, 98, 82, 21]
C. [25, 98, 82, 21, 59]
D. [21, 82, 25, 59, 98]
E. [82, 25, 59, 98, 21]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([21, 82, 25, 59, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[82, 21, 98, 25, 59]`
Cek posisi 0&1 (82 > 21) -> Tukar! Array kini: `[21, 82, 98, 25, 59]`
Cek posisi 1&2 (82 < 98) -> Aman dibiarkan. Array kini: `[21, 82, 98, 25, 59]`
Cek posisi 2&3 (98 > 25) -> Tukar! Array kini: `[21, 82, 25, 98, 59]`
Cek posisi 3&4 (98 > 59) -> Tukar! Array kini: `[21, 82, 25, 59, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[21, 82, 25, 59, 98]**.
</details>

---
**Soal 30**
Bebek-bebek di barisan bernomor dada: `[98, 48, 27, 74, 93, 22]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [27, 48, 22, 74, 98, 93]
B. [22, 74, 93, 48, 27, 98]
C. [22, 27, 48, 74, 93, 98]
D. [48, 74, 22, 98, 27, 93]
E. [98, 48, 93, 74, 22, 27]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([22, 27, 48, 74, 93, 98])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[98, 48, 27, 74, 93, 22]`
- Putaran 1: Cari anak terpecebol di area sisa [22, 48, 27, 74, 93, 98]. Ditemukan si `22`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[22, 48, 27, 74, 93, 98]`
- Putaran 2: Cari anak terpecebol di area sisa [27, 48, 74, 93, 98]. Ditemukan si `27`. Tukar paksa dudukan dengan `48`. Array mutasi -> `[22, 27, 48, 74, 93, 98]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[22, 27, 48, 74, 93, 98]**. Opsi murni: **C**.
</details>

---
**Soal 31**
Pak Dengklek memiliki daftar absensi **607 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 11 langkah
C. 12 langkah
D. 13 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 607 elemen
- Langkah 1: Sisa populasi tebasan separuh = 304 elemen
- Langkah 2: Sisa populasi tebasan separuh = 152 elemen
- Langkah 3: Sisa populasi tebasan separuh = 76 elemen
- Langkah 4: Sisa populasi tebasan separuh = 38 elemen
- Langkah 5: Sisa populasi tebasan separuh = 19 elemen
- Langkah 6: Sisa populasi tebasan separuh = 10 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 32**
Diberikan barisan angka: `[24, 18, 61, 74, 92]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [74, 18, 24, 61, 92]
B. [92, 24, 18, 61, 74]
C. [18, 61, 24, 92, 74]
D. [18, 24, 61, 74, 92]
E. [24, 18, 92, 61, 74]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([18, 24, 61, 74, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[24, 18, 61, 74, 92]`
Cek posisi 0&1 (24 > 18) -> Tukar! Array kini: `[18, 24, 61, 74, 92]`
Cek posisi 1&2 (24 < 61) -> Aman dibiarkan. Array kini: `[18, 24, 61, 74, 92]`
Cek posisi 2&3 (61 < 74) -> Aman dibiarkan. Array kini: `[18, 24, 61, 74, 92]`
Cek posisi 3&4 (74 < 92) -> Aman dibiarkan. Array kini: `[18, 24, 61, 74, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[18, 24, 61, 74, 92]**.
</details>

---
**Soal 33**
Bebek-bebek di barisan bernomor dada: `[75, 73, 80, 30, 48, 97]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [73, 97, 30, 75, 48, 80]
B. [75, 97, 30, 73, 48, 80]
C. [97, 48, 30, 75, 80, 73]
D. [30, 48, 80, 75, 73, 97]
E. [73, 80, 48, 75, 97, 30]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([30, 48, 80, 75, 73, 97])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[75, 73, 80, 30, 48, 97]`
- Putaran 1: Cari anak terpecebol di area sisa [30, 73, 80, 75, 48, 97]. Ditemukan si `30`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[30, 73, 80, 75, 48, 97]`
- Putaran 2: Cari anak terpecebol di area sisa [48, 80, 75, 73, 97]. Ditemukan si `48`. Tukar paksa dudukan dengan `73`. Array mutasi -> `[30, 48, 80, 75, 73, 97]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[30, 48, 80, 75, 73, 97]**. Opsi murni: **D**.
</details>

---
**Soal 34**
Bebek-bebek di barisan bernomor dada: `[97, 24, 33, 14, 58, 13]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [97, 24, 33, 58, 13, 14]
B. [14, 13, 24, 33, 58, 97]
C. [13, 14, 33, 24, 58, 97]
D. [58, 13, 24, 14, 33, 97]
E. [97, 33, 58, 14, 13, 24]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([13, 14, 33, 24, 58, 97])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[97, 24, 33, 14, 58, 13]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 24, 33, 14, 58, 97]. Ditemukan si `13`. Tukar paksa dudukan dengan `97`. Array mutasi -> `[13, 24, 33, 14, 58, 97]`
- Putaran 2: Cari anak terpecebol di area sisa [14, 33, 24, 58, 97]. Ditemukan si `14`. Tukar paksa dudukan dengan `24`. Array mutasi -> `[13, 14, 33, 24, 58, 97]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 14, 33, 24, 58, 97]**. Opsi murni: **C**.
</details>

---
**Soal 35**
Bebek-bebek di barisan bernomor dada: `[70, 16, 51, 52, 61, 28]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [16, 28, 51, 52, 61, 70]
B. [52, 28, 51, 70, 16, 61]
C. [61, 16, 28, 51, 70, 52]
D. [70, 61, 28, 51, 52, 16]
E. [61, 52, 28, 16, 70, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([16, 28, 51, 52, 61, 70])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[70, 16, 51, 52, 61, 28]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 70, 51, 52, 61, 28]. Ditemukan si `16`. Tukar paksa dudukan dengan `70`. Array mutasi -> `[16, 70, 51, 52, 61, 28]`
- Putaran 2: Cari anak terpecebol di area sisa [28, 51, 52, 61, 70]. Ditemukan si `28`. Tukar paksa dudukan dengan `70`. Array mutasi -> `[16, 28, 51, 52, 61, 70]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 28, 51, 52, 61, 70]**. Opsi murni: **A**.
</details>

---
**Soal 36**
Pak Dengklek memiliki daftar absensi **1792 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 10 langkah
C. 14 langkah
D. 12 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1792 elemen
- Langkah 1: Sisa populasi tebasan separuh = 896 elemen
- Langkah 2: Sisa populasi tebasan separuh = 448 elemen
- Langkah 3: Sisa populasi tebasan separuh = 224 elemen
- Langkah 4: Sisa populasi tebasan separuh = 112 elemen
- Langkah 5: Sisa populasi tebasan separuh = 56 elemen
- Langkah 6: Sisa populasi tebasan separuh = 28 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 37**
Pak Dengklek memiliki daftar absensi **866 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 10 langkah
C. 12 langkah
D. 13 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 866 elemen
- Langkah 1: Sisa populasi tebasan separuh = 433 elemen
- Langkah 2: Sisa populasi tebasan separuh = 217 elemen
- Langkah 3: Sisa populasi tebasan separuh = 109 elemen
- Langkah 4: Sisa populasi tebasan separuh = 55 elemen
- Langkah 5: Sisa populasi tebasan separuh = 28 elemen
- Langkah 6: Sisa populasi tebasan separuh = 14 elemen
- Langkah 7: Sisa populasi tebasan separuh = 7 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 38**
Diberikan barisan angka: `[11, 24, 94, 95, 54]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [94, 95, 24, 11, 54]
B. [11, 94, 24, 95, 54]
C. [11, 24, 94, 54, 95]
D. [54, 24, 94, 95, 11]
E. [54, 24, 11, 95, 94]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([11, 24, 94, 54, 95])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[11, 24, 94, 95, 54]`
Cek posisi 0&1 (11 < 24) -> Aman dibiarkan. Array kini: `[11, 24, 94, 95, 54]`
Cek posisi 1&2 (24 < 94) -> Aman dibiarkan. Array kini: `[11, 24, 94, 95, 54]`
Cek posisi 2&3 (94 < 95) -> Aman dibiarkan. Array kini: `[11, 24, 94, 95, 54]`
Cek posisi 3&4 (95 > 54) -> Tukar! Array kini: `[11, 24, 94, 54, 95]`


Terbukti bahwa elemen maha gemuk (`95`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[11, 24, 94, 54, 95]**.
</details>

---
**Soal 39**
Pak Dengklek memiliki daftar absensi **765 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 13 langkah
C. 12 langkah
D. 10 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 765 elemen
- Langkah 1: Sisa populasi tebasan separuh = 383 elemen
- Langkah 2: Sisa populasi tebasan separuh = 192 elemen
- Langkah 3: Sisa populasi tebasan separuh = 96 elemen
- Langkah 4: Sisa populasi tebasan separuh = 48 elemen
- Langkah 5: Sisa populasi tebasan separuh = 24 elemen
- Langkah 6: Sisa populasi tebasan separuh = 12 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 40**
Pak Dengklek memiliki daftar absensi **1221 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 13 langkah
C. 14 langkah
D. 12 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1221 elemen
- Langkah 1: Sisa populasi tebasan separuh = 611 elemen
- Langkah 2: Sisa populasi tebasan separuh = 306 elemen
- Langkah 3: Sisa populasi tebasan separuh = 153 elemen
- Langkah 4: Sisa populasi tebasan separuh = 77 elemen
- Langkah 5: Sisa populasi tebasan separuh = 39 elemen
- Langkah 6: Sisa populasi tebasan separuh = 20 elemen
- Langkah 7: Sisa populasi tebasan separuh = 10 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 41**
Pak Dengklek memiliki daftar absensi **1707 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 11 langkah
C. 10 langkah
D. 12 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1707 elemen
- Langkah 1: Sisa populasi tebasan separuh = 854 elemen
- Langkah 2: Sisa populasi tebasan separuh = 427 elemen
- Langkah 3: Sisa populasi tebasan separuh = 214 elemen
- Langkah 4: Sisa populasi tebasan separuh = 107 elemen
- Langkah 5: Sisa populasi tebasan separuh = 54 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 42**
Pak Dengklek memiliki daftar absensi **1616 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 11 langkah
D. 13 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1616 elemen
- Langkah 1: Sisa populasi tebasan separuh = 808 elemen
- Langkah 2: Sisa populasi tebasan separuh = 404 elemen
- Langkah 3: Sisa populasi tebasan separuh = 202 elemen
- Langkah 4: Sisa populasi tebasan separuh = 101 elemen
- Langkah 5: Sisa populasi tebasan separuh = 51 elemen
- Langkah 6: Sisa populasi tebasan separuh = 26 elemen
- Langkah 7: Sisa populasi tebasan separuh = 13 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 43**
Pak Dengklek memiliki daftar absensi **963 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 9 langkah
C. 13 langkah
D. 10 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 963 elemen
- Langkah 1: Sisa populasi tebasan separuh = 482 elemen
- Langkah 2: Sisa populasi tebasan separuh = 241 elemen
- Langkah 3: Sisa populasi tebasan separuh = 121 elemen
- Langkah 4: Sisa populasi tebasan separuh = 61 elemen
- Langkah 5: Sisa populasi tebasan separuh = 31 elemen
- Langkah 6: Sisa populasi tebasan separuh = 16 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 44**
Diberikan barisan angka: `[88, 50, 80, 18, 78]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [78, 50, 18, 80, 88]
B. [50, 80, 18, 78, 88]
C. [80, 18, 78, 88, 50]
D. [18, 78, 50, 88, 80]
E. [50, 80, 88, 18, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([50, 80, 18, 78, 88])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[88, 50, 80, 18, 78]`
Cek posisi 0&1 (88 > 50) -> Tukar! Array kini: `[50, 88, 80, 18, 78]`
Cek posisi 1&2 (88 > 80) -> Tukar! Array kini: `[50, 80, 88, 18, 78]`
Cek posisi 2&3 (88 > 18) -> Tukar! Array kini: `[50, 80, 18, 88, 78]`
Cek posisi 3&4 (88 > 78) -> Tukar! Array kini: `[50, 80, 18, 78, 88]`


Terbukti bahwa elemen maha gemuk (`88`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[50, 80, 18, 78, 88]**.
</details>

---
**Soal 45**
Bebek-bebek di barisan bernomor dada: `[87, 21, 11, 78, 63, 32]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [21, 11, 78, 32, 63, 87]
B. [63, 21, 11, 32, 78, 87]
C. [11, 21, 87, 78, 63, 32]
D. [63, 78, 87, 21, 11, 32]
E. [78, 87, 32, 11, 63, 21]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([11, 21, 87, 78, 63, 32])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[87, 21, 11, 78, 63, 32]`
- Putaran 1: Cari anak terpecebol di area sisa [11, 21, 87, 78, 63, 32]. Ditemukan si `11`. Tukar paksa dudukan dengan `87`. Array mutasi -> `[11, 21, 87, 78, 63, 32]`
- Putaran 2: Cari anak terpecebol di area sisa [21, 87, 78, 63, 32]. Ditemukan si `21`. Tukar paksa dudukan dengan `21`. Array mutasi -> `[11, 21, 87, 78, 63, 32]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[11, 21, 87, 78, 63, 32]**. Opsi murni: **C**.
</details>

---
**Soal 46**
Diberikan barisan angka: `[47, 18, 58, 94, 26]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [58, 47, 26, 18, 94]
B. [18, 47, 58, 26, 94]
C. [26, 47, 94, 58, 18]
D. [47, 26, 58, 94, 18]
E. [26, 94, 18, 58, 47]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([18, 47, 58, 26, 94])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[47, 18, 58, 94, 26]`
Cek posisi 0&1 (47 > 18) -> Tukar! Array kini: `[18, 47, 58, 94, 26]`
Cek posisi 1&2 (47 < 58) -> Aman dibiarkan. Array kini: `[18, 47, 58, 94, 26]`
Cek posisi 2&3 (58 < 94) -> Aman dibiarkan. Array kini: `[18, 47, 58, 94, 26]`
Cek posisi 3&4 (94 > 26) -> Tukar! Array kini: `[18, 47, 58, 26, 94]`


Terbukti bahwa elemen maha gemuk (`94`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[18, 47, 58, 26, 94]**.
</details>

---
**Soal 47**
Pak Dengklek memiliki daftar absensi **668 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 13 langkah
C. 9 langkah
D. 12 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 668 elemen
- Langkah 1: Sisa populasi tebasan separuh = 334 elemen
- Langkah 2: Sisa populasi tebasan separuh = 167 elemen
- Langkah 3: Sisa populasi tebasan separuh = 84 elemen
- Langkah 4: Sisa populasi tebasan separuh = 42 elemen
- Langkah 5: Sisa populasi tebasan separuh = 21 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 48**
Pak Dengklek memiliki daftar absensi **1533 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 10 langkah
D. 14 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1533 elemen
- Langkah 1: Sisa populasi tebasan separuh = 767 elemen
- Langkah 2: Sisa populasi tebasan separuh = 384 elemen
- Langkah 3: Sisa populasi tebasan separuh = 192 elemen
- Langkah 4: Sisa populasi tebasan separuh = 96 elemen
- Langkah 5: Sisa populasi tebasan separuh = 48 elemen
- Langkah 6: Sisa populasi tebasan separuh = 24 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 49**
Bebek-bebek di barisan bernomor dada: `[94, 46, 22, 86, 96, 84]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [46, 22, 86, 96, 94, 84]
B. [94, 84, 96, 22, 46, 86]
C. [22, 46, 94, 86, 96, 84]
D. [96, 22, 86, 84, 94, 46]
E. [96, 94, 22, 46, 84, 86]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([22, 46, 94, 86, 96, 84])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[94, 46, 22, 86, 96, 84]`
- Putaran 1: Cari anak terpecebol di area sisa [22, 46, 94, 86, 96, 84]. Ditemukan si `22`. Tukar paksa dudukan dengan `94`. Array mutasi -> `[22, 46, 94, 86, 96, 84]`
- Putaran 2: Cari anak terpecebol di area sisa [46, 94, 86, 96, 84]. Ditemukan si `46`. Tukar paksa dudukan dengan `46`. Array mutasi -> `[22, 46, 94, 86, 96, 84]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[22, 46, 94, 86, 96, 84]**. Opsi murni: **C**.
</details>

---
**Soal 50**
Pak Dengklek memiliki daftar absensi **1633 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 11 langkah
D. 13 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1633 elemen
- Langkah 1: Sisa populasi tebasan separuh = 817 elemen
- Langkah 2: Sisa populasi tebasan separuh = 409 elemen
- Langkah 3: Sisa populasi tebasan separuh = 205 elemen
- Langkah 4: Sisa populasi tebasan separuh = 103 elemen
- Langkah 5: Sisa populasi tebasan separuh = 52 elemen
- Langkah 6: Sisa populasi tebasan separuh = 26 elemen
- Langkah 7: Sisa populasi tebasan separuh = 13 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
