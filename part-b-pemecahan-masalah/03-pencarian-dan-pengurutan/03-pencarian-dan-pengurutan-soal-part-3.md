# Latian Soal: Pencarian & Pengurutan (Part 3 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 101**
Bebek-bebek di barisan bernomor dada: `[94, 32, 59, 83, 97, 76]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [94, 59, 76, 32, 97, 83]
B. [32, 59, 94, 83, 97, 76]
C. [59, 83, 32, 97, 76, 94]
D. [76, 32, 94, 97, 83, 59]
E. [32, 59, 83, 76, 97, 94]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([32, 59, 94, 83, 97, 76])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[94, 32, 59, 83, 97, 76]`
- Putaran 1: Cari anak terpecebol di area sisa [32, 94, 59, 83, 97, 76]. Ditemukan si `32`. Tukar paksa dudukan dengan `94`. Array mutasi -> `[32, 94, 59, 83, 97, 76]`
- Putaran 2: Cari anak terpecebol di area sisa [59, 94, 83, 97, 76]. Ditemukan si `59`. Tukar paksa dudukan dengan `94`. Array mutasi -> `[32, 59, 94, 83, 97, 76]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[32, 59, 94, 83, 97, 76]**. Opsi murni: **B**.
</details>

---
**Soal 102**
Pak Dengklek memiliki daftar absensi **1723 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1723 elemen
- Langkah 1: Sisa populasi tebasan separuh = 862 elemen
- Langkah 2: Sisa populasi tebasan separuh = 431 elemen
- Langkah 3: Sisa populasi tebasan separuh = 216 elemen
- Langkah 4: Sisa populasi tebasan separuh = 108 elemen
- Langkah 5: Sisa populasi tebasan separuh = 54 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 103**
Pak Dengklek memiliki daftar absensi **1904 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1904 elemen
- Langkah 1: Sisa populasi tebasan separuh = 952 elemen
- Langkah 2: Sisa populasi tebasan separuh = 476 elemen
- Langkah 3: Sisa populasi tebasan separuh = 238 elemen
- Langkah 4: Sisa populasi tebasan separuh = 119 elemen
- Langkah 5: Sisa populasi tebasan separuh = 60 elemen
- Langkah 6: Sisa populasi tebasan separuh = 30 elemen
- Langkah 7: Sisa populasi tebasan separuh = 15 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 104**
Bebek-bebek di barisan bernomor dada: `[77, 88, 29, 40, 63, 80]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [63, 77, 88, 80, 40, 29]
B. [29, 77, 63, 88, 80, 40]
C. [29, 40, 77, 88, 63, 80]
D. [88, 40, 80, 63, 77, 29]
E. [88, 63, 80, 40, 29, 77]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([29, 40, 77, 88, 63, 80])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[77, 88, 29, 40, 63, 80]`
- Putaran 1: Cari anak terpecebol di area sisa [29, 88, 77, 40, 63, 80]. Ditemukan si `29`. Tukar paksa dudukan dengan `77`. Array mutasi -> `[29, 88, 77, 40, 63, 80]`
- Putaran 2: Cari anak terpecebol di area sisa [40, 77, 88, 63, 80]. Ditemukan si `40`. Tukar paksa dudukan dengan `88`. Array mutasi -> `[29, 40, 77, 88, 63, 80]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[29, 40, 77, 88, 63, 80]**. Opsi murni: **C**.
</details>

---
**Soal 105**
Diberikan barisan angka: `[35, 89, 69, 71, 45]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [71, 89, 45, 69, 35]
B. [35, 69, 71, 45, 89]
C. [69, 45, 35, 71, 89]
D. [69, 89, 35, 71, 45]
E. [35, 71, 69, 45, 89]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([35, 69, 71, 45, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[35, 89, 69, 71, 45]`
Cek posisi 0&1 (35 < 89) -> Aman dibiarkan. Array kini: `[35, 89, 69, 71, 45]`
Cek posisi 1&2 (89 > 69) -> Tukar! Array kini: `[35, 69, 89, 71, 45]`
Cek posisi 2&3 (89 > 71) -> Tukar! Array kini: `[35, 69, 71, 89, 45]`
Cek posisi 3&4 (89 > 45) -> Tukar! Array kini: `[35, 69, 71, 45, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[35, 69, 71, 45, 89]**.
</details>

---
**Soal 106**
Bebek-bebek di barisan bernomor dada: `[27, 39, 60, 88, 51, 33]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [39, 33, 88, 60, 51, 27]
B. [60, 33, 51, 39, 88, 27]
C. [27, 33, 60, 88, 51, 39]
D. [60, 88, 33, 27, 51, 39]
E. [51, 60, 39, 33, 27, 88]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([27, 33, 60, 88, 51, 39])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[27, 39, 60, 88, 51, 33]`
- Putaran 1: Cari anak terpecebol di area sisa [27, 39, 60, 88, 51, 33]. Ditemukan si `27`. Tukar paksa dudukan dengan `27`. Array mutasi -> `[27, 39, 60, 88, 51, 33]`
- Putaran 2: Cari anak terpecebol di area sisa [33, 60, 88, 51, 39]. Ditemukan si `33`. Tukar paksa dudukan dengan `39`. Array mutasi -> `[27, 33, 60, 88, 51, 39]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[27, 33, 60, 88, 51, 39]**. Opsi murni: **C**.
</details>

---
**Soal 107**
Bebek-bebek di barisan bernomor dada: `[15, 55, 73, 44, 43, 92]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [55, 43, 92, 15, 44, 73]
B. [15, 43, 73, 44, 55, 92]
C. [43, 55, 44, 92, 15, 73]
D. [73, 92, 55, 43, 44, 15]
E. [15, 44, 43, 55, 73, 92]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([15, 43, 73, 44, 55, 92])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[15, 55, 73, 44, 43, 92]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 55, 73, 44, 43, 92]. Ditemukan si `15`. Tukar paksa dudukan dengan `15`. Array mutasi -> `[15, 55, 73, 44, 43, 92]`
- Putaran 2: Cari anak terpecebol di area sisa [43, 73, 44, 55, 92]. Ditemukan si `43`. Tukar paksa dudukan dengan `55`. Array mutasi -> `[15, 43, 73, 44, 55, 92]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 43, 73, 44, 55, 92]**. Opsi murni: **B**.
</details>

---
**Soal 108**
Bebek-bebek di barisan bernomor dada: `[28, 70, 86, 61, 98, 37]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [28, 37, 86, 61, 98, 70]
B. [28, 98, 70, 61, 86, 37]
C. [86, 28, 98, 37, 70, 61]
D. [28, 86, 98, 37, 70, 61]
E. [86, 98, 70, 37, 28, 61]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([28, 37, 86, 61, 98, 70])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[28, 70, 86, 61, 98, 37]`
- Putaran 1: Cari anak terpecebol di area sisa [28, 70, 86, 61, 98, 37]. Ditemukan si `28`. Tukar paksa dudukan dengan `28`. Array mutasi -> `[28, 70, 86, 61, 98, 37]`
- Putaran 2: Cari anak terpecebol di area sisa [37, 86, 61, 98, 70]. Ditemukan si `37`. Tukar paksa dudukan dengan `70`. Array mutasi -> `[28, 37, 86, 61, 98, 70]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[28, 37, 86, 61, 98, 70]**. Opsi murni: **A**.
</details>

---
**Soal 109**
Diberikan barisan angka: `[18, 12, 37, 58, 38]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [12, 18, 37, 38, 58]
B. [37, 12, 58, 38, 18]
C. [18, 12, 37, 38, 58]
D. [58, 38, 18, 12, 37]
E. [58, 18, 37, 12, 38]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([12, 18, 37, 38, 58])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[18, 12, 37, 58, 38]`
Cek posisi 0&1 (18 > 12) -> Tukar! Array kini: `[12, 18, 37, 58, 38]`
Cek posisi 1&2 (18 < 37) -> Aman dibiarkan. Array kini: `[12, 18, 37, 58, 38]`
Cek posisi 2&3 (37 < 58) -> Aman dibiarkan. Array kini: `[12, 18, 37, 58, 38]`
Cek posisi 3&4 (58 > 38) -> Tukar! Array kini: `[12, 18, 37, 38, 58]`


Terbukti bahwa elemen maha gemuk (`58`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[12, 18, 37, 38, 58]**.
</details>

---
**Soal 110**
Pak Dengklek memiliki daftar absensi **1768 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 13 langkah
C. 10 langkah
D. 14 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1768 elemen
- Langkah 1: Sisa populasi tebasan separuh = 884 elemen
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
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 111**
Diberikan barisan angka: `[83, 84, 73, 63, 22]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [84, 73, 22, 63, 83]
B. [83, 84, 63, 22, 73]
C. [73, 22, 83, 63, 84]
D. [83, 73, 63, 22, 84]
E. [84, 63, 83, 22, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([83, 73, 63, 22, 84])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[83, 84, 73, 63, 22]`
Cek posisi 0&1 (83 < 84) -> Aman dibiarkan. Array kini: `[83, 84, 73, 63, 22]`
Cek posisi 1&2 (84 > 73) -> Tukar! Array kini: `[83, 73, 84, 63, 22]`
Cek posisi 2&3 (84 > 63) -> Tukar! Array kini: `[83, 73, 63, 84, 22]`
Cek posisi 3&4 (84 > 22) -> Tukar! Array kini: `[83, 73, 63, 22, 84]`


Terbukti bahwa elemen maha gemuk (`84`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[83, 73, 63, 22, 84]**.
</details>

---
**Soal 112**
Bebek-bebek di barisan bernomor dada: `[28, 94, 77, 61, 13, 48]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [28, 94, 13, 61, 48, 77]
B. [94, 77, 28, 61, 13, 48]
C. [28, 61, 13, 48, 94, 77]
D. [94, 13, 77, 61, 28, 48]
E. [13, 28, 77, 61, 94, 48]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([13, 28, 77, 61, 94, 48])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[28, 94, 77, 61, 13, 48]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 94, 77, 61, 28, 48]. Ditemukan si `13`. Tukar paksa dudukan dengan `28`. Array mutasi -> `[13, 94, 77, 61, 28, 48]`
- Putaran 2: Cari anak terpecebol di area sisa [28, 77, 61, 94, 48]. Ditemukan si `28`. Tukar paksa dudukan dengan `94`. Array mutasi -> `[13, 28, 77, 61, 94, 48]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 28, 77, 61, 94, 48]**. Opsi murni: **E**.
</details>

---
**Soal 113**
Pak Dengklek memiliki daftar absensi **1447 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 10 langkah
C. 11 langkah
D. 14 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1447 elemen
- Langkah 1: Sisa populasi tebasan separuh = 724 elemen
- Langkah 2: Sisa populasi tebasan separuh = 362 elemen
- Langkah 3: Sisa populasi tebasan separuh = 181 elemen
- Langkah 4: Sisa populasi tebasan separuh = 91 elemen
- Langkah 5: Sisa populasi tebasan separuh = 46 elemen
- Langkah 6: Sisa populasi tebasan separuh = 23 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 114**
Pak Dengklek memiliki daftar absensi **682 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 9 langkah
D. 11 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 682 elemen
- Langkah 1: Sisa populasi tebasan separuh = 341 elemen
- Langkah 2: Sisa populasi tebasan separuh = 171 elemen
- Langkah 3: Sisa populasi tebasan separuh = 86 elemen
- Langkah 4: Sisa populasi tebasan separuh = 43 elemen
- Langkah 5: Sisa populasi tebasan separuh = 22 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 115**
Diberikan barisan angka: `[37, 78, 39, 50, 90]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [37, 39, 50, 78, 90]
B. [78, 50, 90, 37, 39]
C. [90, 50, 37, 78, 39]
D. [50, 39, 37, 78, 90]
E. [50, 39, 78, 37, 90]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([37, 39, 50, 78, 90])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[37, 78, 39, 50, 90]`
Cek posisi 0&1 (37 < 78) -> Aman dibiarkan. Array kini: `[37, 78, 39, 50, 90]`
Cek posisi 1&2 (78 > 39) -> Tukar! Array kini: `[37, 39, 78, 50, 90]`
Cek posisi 2&3 (78 > 50) -> Tukar! Array kini: `[37, 39, 50, 78, 90]`
Cek posisi 3&4 (78 < 90) -> Aman dibiarkan. Array kini: `[37, 39, 50, 78, 90]`


Terbukti bahwa elemen maha gemuk (`90`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[37, 39, 50, 78, 90]**.
</details>

---
**Soal 116**
Bebek-bebek di barisan bernomor dada: `[87, 32, 41, 90, 17, 72]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [90, 72, 41, 32, 87, 17]
B. [17, 32, 41, 90, 87, 72]
C. [32, 41, 87, 72, 17, 90]
D. [32, 87, 90, 41, 17, 72]
E. [90, 17, 41, 87, 72, 32]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([17, 32, 41, 90, 87, 72])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[87, 32, 41, 90, 17, 72]`
- Putaran 1: Cari anak terpecebol di area sisa [17, 32, 41, 90, 87, 72]. Ditemukan si `17`. Tukar paksa dudukan dengan `87`. Array mutasi -> `[17, 32, 41, 90, 87, 72]`
- Putaran 2: Cari anak terpecebol di area sisa [32, 41, 90, 87, 72]. Ditemukan si `32`. Tukar paksa dudukan dengan `32`. Array mutasi -> `[17, 32, 41, 90, 87, 72]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[17, 32, 41, 90, 87, 72]**. Opsi murni: **B**.
</details>

---
**Soal 117**
Diberikan barisan angka: `[66, 41, 35, 27, 58]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [27, 58, 66, 41, 35]
B. [35, 41, 58, 66, 27]
C. [41, 35, 27, 58, 66]
D. [58, 41, 35, 27, 66]
E. [35, 66, 58, 27, 41]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([41, 35, 27, 58, 66])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[66, 41, 35, 27, 58]`
Cek posisi 0&1 (66 > 41) -> Tukar! Array kini: `[41, 66, 35, 27, 58]`
Cek posisi 1&2 (66 > 35) -> Tukar! Array kini: `[41, 35, 66, 27, 58]`
Cek posisi 2&3 (66 > 27) -> Tukar! Array kini: `[41, 35, 27, 66, 58]`
Cek posisi 3&4 (66 > 58) -> Tukar! Array kini: `[41, 35, 27, 58, 66]`


Terbukti bahwa elemen maha gemuk (`66`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[41, 35, 27, 58, 66]**.
</details>

---
**Soal 118**
Pak Dengklek memiliki daftar absensi **1414 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1414 elemen
- Langkah 1: Sisa populasi tebasan separuh = 707 elemen
- Langkah 2: Sisa populasi tebasan separuh = 354 elemen
- Langkah 3: Sisa populasi tebasan separuh = 177 elemen
- Langkah 4: Sisa populasi tebasan separuh = 89 elemen
- Langkah 5: Sisa populasi tebasan separuh = 45 elemen
- Langkah 6: Sisa populasi tebasan separuh = 23 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 119**
Pak Dengklek memiliki daftar absensi **1077 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 14 langkah
D. 13 langkah
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
**Soal 120**
Pak Dengklek memiliki daftar absensi **1229 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 14 langkah
C. 12 langkah
D. 13 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1229 elemen
- Langkah 1: Sisa populasi tebasan separuh = 615 elemen
- Langkah 2: Sisa populasi tebasan separuh = 308 elemen
- Langkah 3: Sisa populasi tebasan separuh = 154 elemen
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
**Soal 121**
Pak Dengklek memiliki daftar absensi **1133 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 12 langkah
C. 14 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1133 elemen
- Langkah 1: Sisa populasi tebasan separuh = 567 elemen
- Langkah 2: Sisa populasi tebasan separuh = 284 elemen
- Langkah 3: Sisa populasi tebasan separuh = 142 elemen
- Langkah 4: Sisa populasi tebasan separuh = 71 elemen
- Langkah 5: Sisa populasi tebasan separuh = 36 elemen
- Langkah 6: Sisa populasi tebasan separuh = 18 elemen
- Langkah 7: Sisa populasi tebasan separuh = 9 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 122**
Pak Dengklek memiliki daftar absensi **1215 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 10 langkah
C. 14 langkah
D. 12 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1215 elemen
- Langkah 1: Sisa populasi tebasan separuh = 608 elemen
- Langkah 2: Sisa populasi tebasan separuh = 304 elemen
- Langkah 3: Sisa populasi tebasan separuh = 152 elemen
- Langkah 4: Sisa populasi tebasan separuh = 76 elemen
- Langkah 5: Sisa populasi tebasan separuh = 38 elemen
- Langkah 6: Sisa populasi tebasan separuh = 19 elemen
- Langkah 7: Sisa populasi tebasan separuh = 10 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 123**
Bebek-bebek di barisan bernomor dada: `[85, 96, 30, 69, 32, 20]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [20, 30, 96, 69, 32, 85]
B. [85, 20, 69, 30, 96, 32]
C. [96, 69, 20, 85, 30, 32]
D. [96, 85, 30, 20, 32, 69]
E. [32, 69, 30, 85, 20, 96]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([20, 30, 96, 69, 32, 85])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[85, 96, 30, 69, 32, 20]`
- Putaran 1: Cari anak terpecebol di area sisa [20, 96, 30, 69, 32, 85]. Ditemukan si `20`. Tukar paksa dudukan dengan `85`. Array mutasi -> `[20, 96, 30, 69, 32, 85]`
- Putaran 2: Cari anak terpecebol di area sisa [30, 96, 69, 32, 85]. Ditemukan si `30`. Tukar paksa dudukan dengan `96`. Array mutasi -> `[20, 30, 96, 69, 32, 85]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[20, 30, 96, 69, 32, 85]**. Opsi murni: **A**.
</details>

---
**Soal 124**
Bebek-bebek di barisan bernomor dada: `[91, 27, 73, 66, 13, 54]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [66, 13, 73, 27, 91, 54]
B. [91, 27, 66, 13, 54, 73]
C. [13, 27, 73, 66, 91, 54]
D. [91, 73, 13, 27, 54, 66]
E. [73, 66, 54, 27, 13, 91]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([13, 27, 73, 66, 91, 54])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[91, 27, 73, 66, 13, 54]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 27, 73, 66, 91, 54]. Ditemukan si `13`. Tukar paksa dudukan dengan `91`. Array mutasi -> `[13, 27, 73, 66, 91, 54]`
- Putaran 2: Cari anak terpecebol di area sisa [27, 73, 66, 91, 54]. Ditemukan si `27`. Tukar paksa dudukan dengan `27`. Array mutasi -> `[13, 27, 73, 66, 91, 54]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 27, 73, 66, 91, 54]**. Opsi murni: **C**.
</details>

---
**Soal 125**
Bebek-bebek di barisan bernomor dada: `[26, 39, 67, 54, 91, 41]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [91, 41, 39, 26, 67, 54]
B. [67, 54, 91, 41, 26, 39]
C. [39, 26, 41, 67, 91, 54]
D. [26, 39, 67, 54, 91, 41]
E. [54, 91, 67, 26, 41, 39]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([26, 39, 67, 54, 91, 41])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[26, 39, 67, 54, 91, 41]`
- Putaran 1: Cari anak terpecebol di area sisa [26, 39, 67, 54, 91, 41]. Ditemukan si `26`. Tukar paksa dudukan dengan `26`. Array mutasi -> `[26, 39, 67, 54, 91, 41]`
- Putaran 2: Cari anak terpecebol di area sisa [39, 67, 54, 91, 41]. Ditemukan si `39`. Tukar paksa dudukan dengan `39`. Array mutasi -> `[26, 39, 67, 54, 91, 41]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[26, 39, 67, 54, 91, 41]**. Opsi murni: **D**.
</details>

---
**Soal 126**
Diberikan barisan angka: `[71, 25, 10, 15, 56]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [10, 15, 25, 71, 56]
B. [71, 10, 15, 25, 56]
C. [10, 25, 71, 56, 15]
D. [25, 10, 15, 56, 71]
E. [10, 25, 56, 15, 71]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([25, 10, 15, 56, 71])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[71, 25, 10, 15, 56]`
Cek posisi 0&1 (71 > 25) -> Tukar! Array kini: `[25, 71, 10, 15, 56]`
Cek posisi 1&2 (71 > 10) -> Tukar! Array kini: `[25, 10, 71, 15, 56]`
Cek posisi 2&3 (71 > 15) -> Tukar! Array kini: `[25, 10, 15, 71, 56]`
Cek posisi 3&4 (71 > 56) -> Tukar! Array kini: `[25, 10, 15, 56, 71]`


Terbukti bahwa elemen maha gemuk (`71`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[25, 10, 15, 56, 71]**.
</details>

---
**Soal 127**
Bebek-bebek di barisan bernomor dada: `[75, 29, 50, 98, 77, 66]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [29, 50, 75, 98, 77, 66]
B. [50, 77, 29, 66, 98, 75]
C. [98, 77, 29, 66, 75, 50]
D. [75, 98, 77, 29, 66, 50]
E. [50, 98, 66, 29, 77, 75]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([29, 50, 75, 98, 77, 66])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[75, 29, 50, 98, 77, 66]`
- Putaran 1: Cari anak terpecebol di area sisa [29, 75, 50, 98, 77, 66]. Ditemukan si `29`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[29, 75, 50, 98, 77, 66]`
- Putaran 2: Cari anak terpecebol di area sisa [50, 75, 98, 77, 66]. Ditemukan si `50`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[29, 50, 75, 98, 77, 66]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[29, 50, 75, 98, 77, 66]**. Opsi murni: **A**.
</details>

---
**Soal 128**
Bebek-bebek di barisan bernomor dada: `[30, 58, 53, 54, 80, 50]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [53, 58, 50, 80, 30, 54]
B. [30, 50, 53, 54, 80, 58]
C. [58, 54, 30, 80, 50, 53]
D. [53, 58, 54, 30, 80, 50]
E. [58, 53, 54, 50, 80, 30]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([30, 50, 53, 54, 80, 58])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[30, 58, 53, 54, 80, 50]`
- Putaran 1: Cari anak terpecebol di area sisa [30, 58, 53, 54, 80, 50]. Ditemukan si `30`. Tukar paksa dudukan dengan `30`. Array mutasi -> `[30, 58, 53, 54, 80, 50]`
- Putaran 2: Cari anak terpecebol di area sisa [50, 53, 54, 80, 58]. Ditemukan si `50`. Tukar paksa dudukan dengan `58`. Array mutasi -> `[30, 50, 53, 54, 80, 58]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[30, 50, 53, 54, 80, 58]**. Opsi murni: **B**.
</details>

---
**Soal 129**
Pak Dengklek memiliki daftar absensi **674 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 9 langkah
D. 11 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 674 elemen
- Langkah 1: Sisa populasi tebasan separuh = 337 elemen
- Langkah 2: Sisa populasi tebasan separuh = 169 elemen
- Langkah 3: Sisa populasi tebasan separuh = 85 elemen
- Langkah 4: Sisa populasi tebasan separuh = 43 elemen
- Langkah 5: Sisa populasi tebasan separuh = 22 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 130**
Bebek-bebek di barisan bernomor dada: `[98, 93, 10, 32, 61, 63]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [32, 61, 63, 10, 93, 98]
B. [93, 98, 32, 63, 10, 61]
C. [61, 98, 63, 10, 32, 93]
D. [93, 63, 32, 98, 10, 61]
E. [10, 32, 98, 93, 61, 63]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([10, 32, 98, 93, 61, 63])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[98, 93, 10, 32, 61, 63]`
- Putaran 1: Cari anak terpecebol di area sisa [10, 93, 98, 32, 61, 63]. Ditemukan si `10`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[10, 93, 98, 32, 61, 63]`
- Putaran 2: Cari anak terpecebol di area sisa [32, 98, 93, 61, 63]. Ditemukan si `32`. Tukar paksa dudukan dengan `93`. Array mutasi -> `[10, 32, 98, 93, 61, 63]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[10, 32, 98, 93, 61, 63]**. Opsi murni: **E**.
</details>

---
**Soal 131**
Pak Dengklek memiliki daftar absensi **971 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 13 langkah
C. 10 langkah
D. 11 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 971 elemen
- Langkah 1: Sisa populasi tebasan separuh = 486 elemen
- Langkah 2: Sisa populasi tebasan separuh = 243 elemen
- Langkah 3: Sisa populasi tebasan separuh = 122 elemen
- Langkah 4: Sisa populasi tebasan separuh = 61 elemen
- Langkah 5: Sisa populasi tebasan separuh = 31 elemen
- Langkah 6: Sisa populasi tebasan separuh = 16 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 132**
Bebek-bebek di barisan bernomor dada: `[32, 18, 70, 85, 16, 37]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [16, 18, 70, 85, 32, 37]
B. [85, 18, 37, 16, 70, 32]
C. [32, 16, 37, 70, 18, 85]
D. [16, 85, 32, 37, 70, 18]
E. [85, 32, 70, 37, 16, 18]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([16, 18, 70, 85, 32, 37])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[32, 18, 70, 85, 16, 37]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 18, 70, 85, 32, 37]. Ditemukan si `16`. Tukar paksa dudukan dengan `32`. Array mutasi -> `[16, 18, 70, 85, 32, 37]`
- Putaran 2: Cari anak terpecebol di area sisa [18, 70, 85, 32, 37]. Ditemukan si `18`. Tukar paksa dudukan dengan `18`. Array mutasi -> `[16, 18, 70, 85, 32, 37]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 18, 70, 85, 32, 37]**. Opsi murni: **A**.
</details>

---
**Soal 133**
Diberikan barisan angka: `[92, 36, 14, 96, 35]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [92, 35, 96, 36, 14]
B. [35, 96, 92, 14, 36]
C. [96, 35, 92, 14, 36]
D. [36, 14, 92, 35, 96]
E. [96, 35, 14, 36, 92]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([36, 14, 92, 35, 96])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[92, 36, 14, 96, 35]`
Cek posisi 0&1 (92 > 36) -> Tukar! Array kini: `[36, 92, 14, 96, 35]`
Cek posisi 1&2 (92 > 14) -> Tukar! Array kini: `[36, 14, 92, 96, 35]`
Cek posisi 2&3 (92 < 96) -> Aman dibiarkan. Array kini: `[36, 14, 92, 96, 35]`
Cek posisi 3&4 (96 > 35) -> Tukar! Array kini: `[36, 14, 92, 35, 96]`


Terbukti bahwa elemen maha gemuk (`96`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[36, 14, 92, 35, 96]**.
</details>

---
**Soal 134**
Bebek-bebek di barisan bernomor dada: `[69, 50, 97, 46, 61, 85]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [69, 97, 50, 61, 85, 46]
B. [50, 85, 97, 69, 46, 61]
C. [46, 97, 85, 50, 61, 69]
D. [46, 50, 97, 69, 61, 85]
E. [61, 50, 85, 69, 46, 97]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([46, 50, 97, 69, 61, 85])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[69, 50, 97, 46, 61, 85]`
- Putaran 1: Cari anak terpecebol di area sisa [46, 50, 97, 69, 61, 85]. Ditemukan si `46`. Tukar paksa dudukan dengan `69`. Array mutasi -> `[46, 50, 97, 69, 61, 85]`
- Putaran 2: Cari anak terpecebol di area sisa [50, 97, 69, 61, 85]. Ditemukan si `50`. Tukar paksa dudukan dengan `50`. Array mutasi -> `[46, 50, 97, 69, 61, 85]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[46, 50, 97, 69, 61, 85]**. Opsi murni: **D**.
</details>

---
**Soal 135**
Pak Dengklek memiliki daftar absensi **850 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 13 langkah
C. 10 langkah
D. 9 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 850 elemen
- Langkah 1: Sisa populasi tebasan separuh = 425 elemen
- Langkah 2: Sisa populasi tebasan separuh = 213 elemen
- Langkah 3: Sisa populasi tebasan separuh = 107 elemen
- Langkah 4: Sisa populasi tebasan separuh = 54 elemen
- Langkah 5: Sisa populasi tebasan separuh = 27 elemen
- Langkah 6: Sisa populasi tebasan separuh = 14 elemen
- Langkah 7: Sisa populasi tebasan separuh = 7 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 136**
Diberikan barisan angka: `[60, 87, 68, 84, 42]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [60, 87, 68, 84, 42]
B. [68, 84, 87, 42, 60]
C. [60, 68, 84, 42, 87]
D. [87, 84, 60, 42, 68]
E. [68, 87, 42, 60, 84]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([60, 68, 84, 42, 87])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[60, 87, 68, 84, 42]`
Cek posisi 0&1 (60 < 87) -> Aman dibiarkan. Array kini: `[60, 87, 68, 84, 42]`
Cek posisi 1&2 (87 > 68) -> Tukar! Array kini: `[60, 68, 87, 84, 42]`
Cek posisi 2&3 (87 > 84) -> Tukar! Array kini: `[60, 68, 84, 87, 42]`
Cek posisi 3&4 (87 > 42) -> Tukar! Array kini: `[60, 68, 84, 42, 87]`


Terbukti bahwa elemen maha gemuk (`87`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[60, 68, 84, 42, 87]**.
</details>

---
**Soal 137**
Diberikan barisan angka: `[29, 81, 89, 42, 90]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [29, 89, 90, 81, 42]
B. [90, 89, 29, 42, 81]
C. [29, 81, 42, 89, 90]
D. [42, 29, 90, 81, 89]
E. [81, 90, 89, 29, 42]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([29, 81, 42, 89, 90])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[29, 81, 89, 42, 90]`
Cek posisi 0&1 (29 < 81) -> Aman dibiarkan. Array kini: `[29, 81, 89, 42, 90]`
Cek posisi 1&2 (81 < 89) -> Aman dibiarkan. Array kini: `[29, 81, 89, 42, 90]`
Cek posisi 2&3 (89 > 42) -> Tukar! Array kini: `[29, 81, 42, 89, 90]`
Cek posisi 3&4 (89 < 90) -> Aman dibiarkan. Array kini: `[29, 81, 42, 89, 90]`


Terbukti bahwa elemen maha gemuk (`90`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[29, 81, 42, 89, 90]**.
</details>

---
**Soal 138**
Bebek-bebek di barisan bernomor dada: `[49, 42, 35, 28, 85, 81]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [28, 42, 81, 49, 35, 85]
B. [81, 35, 85, 28, 42, 49]
C. [42, 35, 49, 28, 85, 81]
D. [28, 35, 42, 49, 85, 81]
E. [35, 81, 85, 28, 49, 42]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([28, 35, 42, 49, 85, 81])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[49, 42, 35, 28, 85, 81]`
- Putaran 1: Cari anak terpecebol di area sisa [28, 42, 35, 49, 85, 81]. Ditemukan si `28`. Tukar paksa dudukan dengan `49`. Array mutasi -> `[28, 42, 35, 49, 85, 81]`
- Putaran 2: Cari anak terpecebol di area sisa [35, 42, 49, 85, 81]. Ditemukan si `35`. Tukar paksa dudukan dengan `42`. Array mutasi -> `[28, 35, 42, 49, 85, 81]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[28, 35, 42, 49, 85, 81]**. Opsi murni: **D**.
</details>

---
**Soal 139**
Pak Dengklek memiliki daftar absensi **1170 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 13 langkah
C. 11 langkah
D. 10 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1170 elemen
- Langkah 1: Sisa populasi tebasan separuh = 585 elemen
- Langkah 2: Sisa populasi tebasan separuh = 293 elemen
- Langkah 3: Sisa populasi tebasan separuh = 147 elemen
- Langkah 4: Sisa populasi tebasan separuh = 74 elemen
- Langkah 5: Sisa populasi tebasan separuh = 37 elemen
- Langkah 6: Sisa populasi tebasan separuh = 19 elemen
- Langkah 7: Sisa populasi tebasan separuh = 10 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 140**
Diberikan barisan angka: `[11, 76, 12, 19, 80]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [76, 80, 19, 12, 11]
B. [19, 11, 76, 12, 80]
C. [12, 19, 76, 11, 80]
D. [11, 12, 19, 76, 80]
E. [12, 80, 11, 76, 19]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([11, 12, 19, 76, 80])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[11, 76, 12, 19, 80]`
Cek posisi 0&1 (11 < 76) -> Aman dibiarkan. Array kini: `[11, 76, 12, 19, 80]`
Cek posisi 1&2 (76 > 12) -> Tukar! Array kini: `[11, 12, 76, 19, 80]`
Cek posisi 2&3 (76 > 19) -> Tukar! Array kini: `[11, 12, 19, 76, 80]`
Cek posisi 3&4 (76 < 80) -> Aman dibiarkan. Array kini: `[11, 12, 19, 76, 80]`


Terbukti bahwa elemen maha gemuk (`80`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[11, 12, 19, 76, 80]**.
</details>

---
**Soal 141**
Pak Dengklek memiliki daftar absensi **625 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 13 langkah
C. 12 langkah
D. 11 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 625 elemen
- Langkah 1: Sisa populasi tebasan separuh = 313 elemen
- Langkah 2: Sisa populasi tebasan separuh = 157 elemen
- Langkah 3: Sisa populasi tebasan separuh = 79 elemen
- Langkah 4: Sisa populasi tebasan separuh = 40 elemen
- Langkah 5: Sisa populasi tebasan separuh = 20 elemen
- Langkah 6: Sisa populasi tebasan separuh = 10 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 142**
Pak Dengklek memiliki daftar absensi **645 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 13 langkah
D. 10 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 645 elemen
- Langkah 1: Sisa populasi tebasan separuh = 323 elemen
- Langkah 2: Sisa populasi tebasan separuh = 162 elemen
- Langkah 3: Sisa populasi tebasan separuh = 81 elemen
- Langkah 4: Sisa populasi tebasan separuh = 41 elemen
- Langkah 5: Sisa populasi tebasan separuh = 21 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 143**
Diberikan barisan angka: `[20, 41, 76, 67, 80]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [20, 41, 67, 76, 80]
B. [20, 41, 80, 76, 67]
C. [41, 80, 67, 76, 20]
D. [67, 76, 80, 41, 20]
E. [76, 80, 67, 20, 41]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([20, 41, 67, 76, 80])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[20, 41, 76, 67, 80]`
Cek posisi 0&1 (20 < 41) -> Aman dibiarkan. Array kini: `[20, 41, 76, 67, 80]`
Cek posisi 1&2 (41 < 76) -> Aman dibiarkan. Array kini: `[20, 41, 76, 67, 80]`
Cek posisi 2&3 (76 > 67) -> Tukar! Array kini: `[20, 41, 67, 76, 80]`
Cek posisi 3&4 (76 < 80) -> Aman dibiarkan. Array kini: `[20, 41, 67, 76, 80]`


Terbukti bahwa elemen maha gemuk (`80`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[20, 41, 67, 76, 80]**.
</details>

---
**Soal 144**
Pak Dengklek memiliki daftar absensi **1854 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 14 langkah
C. 13 langkah
D. 10 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1854 elemen
- Langkah 1: Sisa populasi tebasan separuh = 927 elemen
- Langkah 2: Sisa populasi tebasan separuh = 464 elemen
- Langkah 3: Sisa populasi tebasan separuh = 232 elemen
- Langkah 4: Sisa populasi tebasan separuh = 116 elemen
- Langkah 5: Sisa populasi tebasan separuh = 58 elemen
- Langkah 6: Sisa populasi tebasan separuh = 29 elemen
- Langkah 7: Sisa populasi tebasan separuh = 15 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 145**
Diberikan barisan angka: `[86, 52, 29, 81, 59]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [86, 29, 81, 52, 59]
B. [81, 59, 29, 86, 52]
C. [52, 59, 29, 81, 86]
D. [59, 29, 86, 52, 81]
E. [52, 29, 81, 59, 86]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([52, 29, 81, 59, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[86, 52, 29, 81, 59]`
Cek posisi 0&1 (86 > 52) -> Tukar! Array kini: `[52, 86, 29, 81, 59]`
Cek posisi 1&2 (86 > 29) -> Tukar! Array kini: `[52, 29, 86, 81, 59]`
Cek posisi 2&3 (86 > 81) -> Tukar! Array kini: `[52, 29, 81, 86, 59]`
Cek posisi 3&4 (86 > 59) -> Tukar! Array kini: `[52, 29, 81, 59, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[52, 29, 81, 59, 86]**.
</details>

---
**Soal 146**
Diberikan barisan angka: `[68, 27, 58, 18, 91]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [27, 91, 18, 68, 58]
B. [91, 58, 68, 18, 27]
C. [91, 58, 27, 18, 68]
D. [58, 91, 18, 68, 27]
E. [27, 58, 18, 68, 91]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([27, 58, 18, 68, 91])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[68, 27, 58, 18, 91]`
Cek posisi 0&1 (68 > 27) -> Tukar! Array kini: `[27, 68, 58, 18, 91]`
Cek posisi 1&2 (68 > 58) -> Tukar! Array kini: `[27, 58, 68, 18, 91]`
Cek posisi 2&3 (68 > 18) -> Tukar! Array kini: `[27, 58, 18, 68, 91]`
Cek posisi 3&4 (68 < 91) -> Aman dibiarkan. Array kini: `[27, 58, 18, 68, 91]`


Terbukti bahwa elemen maha gemuk (`91`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[27, 58, 18, 68, 91]**.
</details>

---
**Soal 147**
Diberikan barisan angka: `[33, 55, 10, 34, 16]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [33, 34, 16, 55, 10]
B. [34, 10, 33, 16, 55]
C. [55, 33, 16, 34, 10]
D. [33, 10, 34, 16, 55]
E. [16, 33, 10, 55, 34]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([33, 10, 34, 16, 55])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[33, 55, 10, 34, 16]`
Cek posisi 0&1 (33 < 55) -> Aman dibiarkan. Array kini: `[33, 55, 10, 34, 16]`
Cek posisi 1&2 (55 > 10) -> Tukar! Array kini: `[33, 10, 55, 34, 16]`
Cek posisi 2&3 (55 > 34) -> Tukar! Array kini: `[33, 10, 34, 55, 16]`
Cek posisi 3&4 (55 > 16) -> Tukar! Array kini: `[33, 10, 34, 16, 55]`


Terbukti bahwa elemen maha gemuk (`55`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[33, 10, 34, 16, 55]**.
</details>

---
**Soal 148**
Diberikan barisan angka: `[89, 72, 59, 81, 71]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [89, 59, 81, 72, 71]
B. [72, 81, 59, 71, 89]
C. [72, 59, 81, 71, 89]
D. [71, 81, 59, 89, 72]
E. [89, 71, 81, 72, 59]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([72, 59, 81, 71, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[89, 72, 59, 81, 71]`
Cek posisi 0&1 (89 > 72) -> Tukar! Array kini: `[72, 89, 59, 81, 71]`
Cek posisi 1&2 (89 > 59) -> Tukar! Array kini: `[72, 59, 89, 81, 71]`
Cek posisi 2&3 (89 > 81) -> Tukar! Array kini: `[72, 59, 81, 89, 71]`
Cek posisi 3&4 (89 > 71) -> Tukar! Array kini: `[72, 59, 81, 71, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[72, 59, 81, 71, 89]**.
</details>

---
**Soal 149**
Bebek-bebek di barisan bernomor dada: `[78, 43, 73, 74, 52, 47]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [74, 52, 78, 43, 73, 47]
B. [43, 47, 73, 74, 52, 78]
C. [47, 78, 43, 74, 52, 73]
D. [52, 74, 43, 47, 73, 78]
E. [47, 52, 43, 78, 74, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([43, 47, 73, 74, 52, 78])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[78, 43, 73, 74, 52, 47]`
- Putaran 1: Cari anak terpecebol di area sisa [43, 78, 73, 74, 52, 47]. Ditemukan si `43`. Tukar paksa dudukan dengan `78`. Array mutasi -> `[43, 78, 73, 74, 52, 47]`
- Putaran 2: Cari anak terpecebol di area sisa [47, 73, 74, 52, 78]. Ditemukan si `47`. Tukar paksa dudukan dengan `78`. Array mutasi -> `[43, 47, 73, 74, 52, 78]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[43, 47, 73, 74, 52, 78]**. Opsi murni: **B**.
</details>

---
**Soal 150**
Diberikan barisan angka: `[43, 97, 24, 39, 48]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [97, 24, 48, 39, 43]
B. [43, 24, 39, 48, 97]
C. [48, 39, 24, 43, 97]
D. [24, 39, 97, 48, 43]
E. [43, 97, 24, 48, 39]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([43, 24, 39, 48, 97])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[43, 97, 24, 39, 48]`
Cek posisi 0&1 (43 < 97) -> Aman dibiarkan. Array kini: `[43, 97, 24, 39, 48]`
Cek posisi 1&2 (97 > 24) -> Tukar! Array kini: `[43, 24, 97, 39, 48]`
Cek posisi 2&3 (97 > 39) -> Tukar! Array kini: `[43, 24, 39, 97, 48]`
Cek posisi 3&4 (97 > 48) -> Tukar! Array kini: `[43, 24, 39, 48, 97]`


Terbukti bahwa elemen maha gemuk (`97`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[43, 24, 39, 48, 97]**.
</details>

---
