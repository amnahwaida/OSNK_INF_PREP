# Latian Soal: Pencarian & Pengurutan (Part 6 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 251**
Bebek-bebek di barisan bernomor dada: `[44, 46, 57, 52, 42, 72]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [42, 44, 57, 52, 46, 72]
B. [46, 44, 72, 57, 52, 42]
C. [72, 52, 46, 57, 44, 42]
D. [52, 44, 57, 72, 42, 46]
E. [44, 72, 57, 42, 46, 52]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([42, 44, 57, 52, 46, 72])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[44, 46, 57, 52, 42, 72]`
- Putaran 1: Cari anak terpecebol di area sisa [42, 46, 57, 52, 44, 72]. Ditemukan si `42`. Tukar paksa dudukan dengan `44`. Array mutasi -> `[42, 46, 57, 52, 44, 72]`
- Putaran 2: Cari anak terpecebol di area sisa [44, 57, 52, 46, 72]. Ditemukan si `44`. Tukar paksa dudukan dengan `46`. Array mutasi -> `[42, 44, 57, 52, 46, 72]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[42, 44, 57, 52, 46, 72]**. Opsi murni: **A**.
</details>

---
**Soal 252**
Bebek-bebek di barisan bernomor dada: `[47, 26, 21, 62, 91, 58]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [26, 47, 21, 62, 91, 58]
B. [21, 26, 62, 58, 91, 47]
C. [58, 21, 62, 26, 47, 91]
D. [21, 26, 47, 91, 62, 58]
E. [21, 26, 47, 62, 91, 58]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([21, 26, 47, 62, 91, 58])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[47, 26, 21, 62, 91, 58]`
- Putaran 1: Cari anak terpecebol di area sisa [21, 26, 47, 62, 91, 58]. Ditemukan si `21`. Tukar paksa dudukan dengan `47`. Array mutasi -> `[21, 26, 47, 62, 91, 58]`
- Putaran 2: Cari anak terpecebol di area sisa [26, 47, 62, 91, 58]. Ditemukan si `26`. Tukar paksa dudukan dengan `26`. Array mutasi -> `[21, 26, 47, 62, 91, 58]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[21, 26, 47, 62, 91, 58]**. Opsi murni: **E**.
</details>

---
**Soal 253**
Bebek-bebek di barisan bernomor dada: `[64, 22, 96, 38, 97, 74]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [97, 38, 74, 22, 64, 96]
B. [38, 97, 22, 74, 64, 96]
C. [96, 64, 38, 74, 97, 22]
D. [22, 38, 96, 64, 97, 74]
E. [74, 97, 96, 64, 22, 38]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([22, 38, 96, 64, 97, 74])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[64, 22, 96, 38, 97, 74]`
- Putaran 1: Cari anak terpecebol di area sisa [22, 64, 96, 38, 97, 74]. Ditemukan si `22`. Tukar paksa dudukan dengan `64`. Array mutasi -> `[22, 64, 96, 38, 97, 74]`
- Putaran 2: Cari anak terpecebol di area sisa [38, 96, 64, 97, 74]. Ditemukan si `38`. Tukar paksa dudukan dengan `64`. Array mutasi -> `[22, 38, 96, 64, 97, 74]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[22, 38, 96, 64, 97, 74]**. Opsi murni: **D**.
</details>

---
**Soal 254**
Bebek-bebek di barisan bernomor dada: `[92, 10, 50, 27, 66, 80]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [10, 27, 50, 92, 66, 80]
B. [50, 92, 80, 66, 27, 10]
C. [80, 50, 10, 92, 27, 66]
D. [27, 92, 66, 50, 80, 10]
E. [92, 80, 27, 50, 10, 66]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([10, 27, 50, 92, 66, 80])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[92, 10, 50, 27, 66, 80]`
- Putaran 1: Cari anak terpecebol di area sisa [10, 92, 50, 27, 66, 80]. Ditemukan si `10`. Tukar paksa dudukan dengan `92`. Array mutasi -> `[10, 92, 50, 27, 66, 80]`
- Putaran 2: Cari anak terpecebol di area sisa [27, 50, 92, 66, 80]. Ditemukan si `27`. Tukar paksa dudukan dengan `92`. Array mutasi -> `[10, 27, 50, 92, 66, 80]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[10, 27, 50, 92, 66, 80]**. Opsi murni: **A**.
</details>

---
**Soal 255**
Pak Dengklek memiliki daftar absensi **1675 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 13 langkah
C. 11 langkah
D. 12 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1675 elemen
- Langkah 1: Sisa populasi tebasan separuh = 838 elemen
- Langkah 2: Sisa populasi tebasan separuh = 419 elemen
- Langkah 3: Sisa populasi tebasan separuh = 210 elemen
- Langkah 4: Sisa populasi tebasan separuh = 105 elemen
- Langkah 5: Sisa populasi tebasan separuh = 53 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 256**
Pak Dengklek memiliki daftar absensi **559 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 12 langkah
C. 10 langkah
D. 9 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 559 elemen
- Langkah 1: Sisa populasi tebasan separuh = 280 elemen
- Langkah 2: Sisa populasi tebasan separuh = 140 elemen
- Langkah 3: Sisa populasi tebasan separuh = 70 elemen
- Langkah 4: Sisa populasi tebasan separuh = 35 elemen
- Langkah 5: Sisa populasi tebasan separuh = 18 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **C**.</details>

---
**Soal 257**
Bebek-bebek di barisan bernomor dada: `[16, 33, 51, 52, 57, 61]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [33, 51, 16, 57, 52, 61]
B. [33, 52, 61, 57, 16, 51]
C. [61, 16, 51, 33, 57, 52]
D. [16, 33, 51, 52, 57, 61]
E. [52, 61, 33, 51, 57, 16]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([16, 33, 51, 52, 57, 61])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[16, 33, 51, 52, 57, 61]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 33, 51, 52, 57, 61]. Ditemukan si `16`. Tukar paksa dudukan dengan `16`. Array mutasi -> `[16, 33, 51, 52, 57, 61]`
- Putaran 2: Cari anak terpecebol di area sisa [33, 51, 52, 57, 61]. Ditemukan si `33`. Tukar paksa dudukan dengan `33`. Array mutasi -> `[16, 33, 51, 52, 57, 61]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 33, 51, 52, 57, 61]**. Opsi murni: **D**.
</details>

---
**Soal 258**
Diberikan barisan angka: `[21, 78, 14, 27, 82]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [78, 21, 27, 82, 14]
B. [78, 82, 21, 27, 14]
C. [21, 14, 27, 78, 82]
D. [82, 78, 27, 21, 14]
E. [78, 14, 82, 21, 27]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([21, 14, 27, 78, 82])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[21, 78, 14, 27, 82]`
Cek posisi 0&1 (21 < 78) -> Aman dibiarkan. Array kini: `[21, 78, 14, 27, 82]`
Cek posisi 1&2 (78 > 14) -> Tukar! Array kini: `[21, 14, 78, 27, 82]`
Cek posisi 2&3 (78 > 27) -> Tukar! Array kini: `[21, 14, 27, 78, 82]`
Cek posisi 3&4 (78 < 82) -> Aman dibiarkan. Array kini: `[21, 14, 27, 78, 82]`


Terbukti bahwa elemen maha gemuk (`82`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[21, 14, 27, 78, 82]**.
</details>

---
**Soal 259**
Pak Dengklek memiliki daftar absensi **1690 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1690 elemen
- Langkah 1: Sisa populasi tebasan separuh = 845 elemen
- Langkah 2: Sisa populasi tebasan separuh = 423 elemen
- Langkah 3: Sisa populasi tebasan separuh = 212 elemen
- Langkah 4: Sisa populasi tebasan separuh = 106 elemen
- Langkah 5: Sisa populasi tebasan separuh = 53 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 260**
Diberikan barisan angka: `[55, 90, 98, 64, 73]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [98, 90, 55, 73, 64]
B. [55, 64, 73, 98, 90]
C. [98, 64, 55, 73, 90]
D. [55, 90, 64, 73, 98]
E. [73, 64, 55, 98, 90]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([55, 90, 64, 73, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[55, 90, 98, 64, 73]`
Cek posisi 0&1 (55 < 90) -> Aman dibiarkan. Array kini: `[55, 90, 98, 64, 73]`
Cek posisi 1&2 (90 < 98) -> Aman dibiarkan. Array kini: `[55, 90, 98, 64, 73]`
Cek posisi 2&3 (98 > 64) -> Tukar! Array kini: `[55, 90, 64, 98, 73]`
Cek posisi 3&4 (98 > 73) -> Tukar! Array kini: `[55, 90, 64, 73, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[55, 90, 64, 73, 98]**.
</details>

---
**Soal 261**
Diberikan barisan angka: `[68, 26, 15, 92, 69]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [26, 69, 15, 92, 68]
B. [26, 15, 68, 69, 92]
C. [26, 68, 92, 15, 69]
D. [15, 69, 68, 92, 26]
E. [15, 26, 68, 69, 92]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([26, 15, 68, 69, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[68, 26, 15, 92, 69]`
Cek posisi 0&1 (68 > 26) -> Tukar! Array kini: `[26, 68, 15, 92, 69]`
Cek posisi 1&2 (68 > 15) -> Tukar! Array kini: `[26, 15, 68, 92, 69]`
Cek posisi 2&3 (68 < 92) -> Aman dibiarkan. Array kini: `[26, 15, 68, 92, 69]`
Cek posisi 3&4 (92 > 69) -> Tukar! Array kini: `[26, 15, 68, 69, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[26, 15, 68, 69, 92]**.
</details>

---
**Soal 262**
Bebek-bebek di barisan bernomor dada: `[11, 45, 85, 23, 81, 51]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [23, 51, 45, 85, 81, 11]
B. [81, 45, 23, 51, 11, 85]
C. [81, 85, 11, 45, 51, 23]
D. [45, 81, 11, 51, 23, 85]
E. [11, 23, 85, 45, 81, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([11, 23, 85, 45, 81, 51])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[11, 45, 85, 23, 81, 51]`
- Putaran 1: Cari anak terpecebol di area sisa [11, 45, 85, 23, 81, 51]. Ditemukan si `11`. Tukar paksa dudukan dengan `11`. Array mutasi -> `[11, 45, 85, 23, 81, 51]`
- Putaran 2: Cari anak terpecebol di area sisa [23, 85, 45, 81, 51]. Ditemukan si `23`. Tukar paksa dudukan dengan `45`. Array mutasi -> `[11, 23, 85, 45, 81, 51]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[11, 23, 85, 45, 81, 51]**. Opsi murni: **E**.
</details>

---
**Soal 263**
Pak Dengklek memiliki daftar absensi **1116 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 10 langkah
C. 12 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1116 elemen
- Langkah 1: Sisa populasi tebasan separuh = 558 elemen
- Langkah 2: Sisa populasi tebasan separuh = 279 elemen
- Langkah 3: Sisa populasi tebasan separuh = 140 elemen
- Langkah 4: Sisa populasi tebasan separuh = 70 elemen
- Langkah 5: Sisa populasi tebasan separuh = 35 elemen
- Langkah 6: Sisa populasi tebasan separuh = 18 elemen
- Langkah 7: Sisa populasi tebasan separuh = 9 elemen
- Langkah 8: Sisa populasi tebasan separuh = 5 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 264**
Pak Dengklek memiliki daftar absensi **1151 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 14 langkah
C. 11 langkah
D. 10 langkah
E. 12 langkah

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
**Soal 265**
Diberikan barisan angka: `[28, 14, 50, 34, 18]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [34, 50, 18, 14, 28]
B. [50, 14, 34, 28, 18]
C. [50, 34, 14, 18, 28]
D. [14, 28, 34, 18, 50]
E. [28, 18, 50, 34, 14]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([14, 28, 34, 18, 50])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[28, 14, 50, 34, 18]`
Cek posisi 0&1 (28 > 14) -> Tukar! Array kini: `[14, 28, 50, 34, 18]`
Cek posisi 1&2 (28 < 50) -> Aman dibiarkan. Array kini: `[14, 28, 50, 34, 18]`
Cek posisi 2&3 (50 > 34) -> Tukar! Array kini: `[14, 28, 34, 50, 18]`
Cek posisi 3&4 (50 > 18) -> Tukar! Array kini: `[14, 28, 34, 18, 50]`


Terbukti bahwa elemen maha gemuk (`50`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[14, 28, 34, 18, 50]**.
</details>

---
**Soal 266**
Pak Dengklek memiliki daftar absensi **614 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 13 langkah
C. 12 langkah
D. 11 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 614 elemen
- Langkah 1: Sisa populasi tebasan separuh = 307 elemen
- Langkah 2: Sisa populasi tebasan separuh = 154 elemen
- Langkah 3: Sisa populasi tebasan separuh = 77 elemen
- Langkah 4: Sisa populasi tebasan separuh = 39 elemen
- Langkah 5: Sisa populasi tebasan separuh = 20 elemen
- Langkah 6: Sisa populasi tebasan separuh = 10 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 267**
Bebek-bebek di barisan bernomor dada: `[35, 36, 54, 58, 12, 13]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [54, 12, 13, 58, 35, 36]
B. [12, 13, 54, 58, 35, 36]
C. [54, 36, 35, 13, 58, 12]
D. [12, 58, 36, 54, 35, 13]
E. [36, 35, 13, 58, 54, 12]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([12, 13, 54, 58, 35, 36])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[35, 36, 54, 58, 12, 13]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 36, 54, 58, 35, 13]. Ditemukan si `12`. Tukar paksa dudukan dengan `35`. Array mutasi -> `[12, 36, 54, 58, 35, 13]`
- Putaran 2: Cari anak terpecebol di area sisa [13, 54, 58, 35, 36]. Ditemukan si `13`. Tukar paksa dudukan dengan `36`. Array mutasi -> `[12, 13, 54, 58, 35, 36]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 13, 54, 58, 35, 36]**. Opsi murni: **B**.
</details>

---
**Soal 268**
Bebek-bebek di barisan bernomor dada: `[72, 40, 78, 34, 92, 93]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [93, 92, 40, 34, 72, 78]
B. [92, 78, 34, 72, 93, 40]
C. [34, 40, 78, 72, 92, 93]
D. [92, 78, 72, 93, 40, 34]
E. [72, 40, 78, 93, 92, 34]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([34, 40, 78, 72, 92, 93])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[72, 40, 78, 34, 92, 93]`
- Putaran 1: Cari anak terpecebol di area sisa [34, 40, 78, 72, 92, 93]. Ditemukan si `34`. Tukar paksa dudukan dengan `72`. Array mutasi -> `[34, 40, 78, 72, 92, 93]`
- Putaran 2: Cari anak terpecebol di area sisa [40, 78, 72, 92, 93]. Ditemukan si `40`. Tukar paksa dudukan dengan `40`. Array mutasi -> `[34, 40, 78, 72, 92, 93]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[34, 40, 78, 72, 92, 93]**. Opsi murni: **C**.
</details>

---
**Soal 269**
Pak Dengklek memiliki daftar absensi **573 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 10 langkah
C. 12 langkah
D. 9 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 573 elemen
- Langkah 1: Sisa populasi tebasan separuh = 287 elemen
- Langkah 2: Sisa populasi tebasan separuh = 144 elemen
- Langkah 3: Sisa populasi tebasan separuh = 72 elemen
- Langkah 4: Sisa populasi tebasan separuh = 36 elemen
- Langkah 5: Sisa populasi tebasan separuh = 18 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 270**
Diberikan barisan angka: `[28, 22, 54, 89, 32]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [54, 28, 22, 89, 32]
B. [22, 32, 28, 54, 89]
C. [54, 32, 89, 22, 28]
D. [22, 28, 54, 32, 89]
E. [32, 54, 28, 89, 22]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([22, 28, 54, 32, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[28, 22, 54, 89, 32]`
Cek posisi 0&1 (28 > 22) -> Tukar! Array kini: `[22, 28, 54, 89, 32]`
Cek posisi 1&2 (28 < 54) -> Aman dibiarkan. Array kini: `[22, 28, 54, 89, 32]`
Cek posisi 2&3 (54 < 89) -> Aman dibiarkan. Array kini: `[22, 28, 54, 89, 32]`
Cek posisi 3&4 (89 > 32) -> Tukar! Array kini: `[22, 28, 54, 32, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[22, 28, 54, 32, 89]**.
</details>

---
**Soal 271**
Pak Dengklek memiliki daftar absensi **574 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 11 langkah
C. 9 langkah
D. 12 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 574 elemen
- Langkah 1: Sisa populasi tebasan separuh = 287 elemen
- Langkah 2: Sisa populasi tebasan separuh = 144 elemen
- Langkah 3: Sisa populasi tebasan separuh = 72 elemen
- Langkah 4: Sisa populasi tebasan separuh = 36 elemen
- Langkah 5: Sisa populasi tebasan separuh = 18 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 272**
Bebek-bebek di barisan bernomor dada: `[14, 61, 62, 70, 23, 66]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [61, 14, 62, 23, 66, 70]
B. [14, 66, 61, 62, 70, 23]
C. [14, 66, 61, 70, 62, 23]
D. [14, 23, 62, 70, 61, 66]
E. [14, 61, 66, 23, 62, 70]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([14, 23, 62, 70, 61, 66])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[14, 61, 62, 70, 23, 66]`
- Putaran 1: Cari anak terpecebol di area sisa [14, 61, 62, 70, 23, 66]. Ditemukan si `14`. Tukar paksa dudukan dengan `14`. Array mutasi -> `[14, 61, 62, 70, 23, 66]`
- Putaran 2: Cari anak terpecebol di area sisa [23, 62, 70, 61, 66]. Ditemukan si `23`. Tukar paksa dudukan dengan `61`. Array mutasi -> `[14, 23, 62, 70, 61, 66]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[14, 23, 62, 70, 61, 66]**. Opsi murni: **D**.
</details>

---
**Soal 273**
Bebek-bebek di barisan bernomor dada: `[56, 80, 87, 34, 36, 22]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [22, 80, 56, 34, 87, 36]
B. [22, 34, 87, 80, 36, 56]
C. [87, 22, 80, 36, 56, 34]
D. [56, 87, 36, 34, 22, 80]
E. [36, 87, 34, 80, 56, 22]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([22, 34, 87, 80, 36, 56])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[56, 80, 87, 34, 36, 22]`
- Putaran 1: Cari anak terpecebol di area sisa [22, 80, 87, 34, 36, 56]. Ditemukan si `22`. Tukar paksa dudukan dengan `56`. Array mutasi -> `[22, 80, 87, 34, 36, 56]`
- Putaran 2: Cari anak terpecebol di area sisa [34, 87, 80, 36, 56]. Ditemukan si `34`. Tukar paksa dudukan dengan `80`. Array mutasi -> `[22, 34, 87, 80, 36, 56]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[22, 34, 87, 80, 36, 56]**. Opsi murni: **B**.
</details>

---
**Soal 274**
Bebek-bebek di barisan bernomor dada: `[81, 76, 60, 40, 12, 59]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [81, 40, 76, 59, 60, 12]
B. [12, 40, 60, 76, 81, 59]
C. [12, 59, 76, 40, 81, 60]
D. [76, 60, 81, 12, 40, 59]
E. [81, 76, 60, 59, 40, 12]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([12, 40, 60, 76, 81, 59])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[81, 76, 60, 40, 12, 59]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 76, 60, 40, 81, 59]. Ditemukan si `12`. Tukar paksa dudukan dengan `81`. Array mutasi -> `[12, 76, 60, 40, 81, 59]`
- Putaran 2: Cari anak terpecebol di area sisa [40, 60, 76, 81, 59]. Ditemukan si `40`. Tukar paksa dudukan dengan `76`. Array mutasi -> `[12, 40, 60, 76, 81, 59]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 40, 60, 76, 81, 59]**. Opsi murni: **B**.
</details>

---
**Soal 275**
Pak Dengklek memiliki daftar absensi **1615 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 13 langkah
C. 12 langkah
D. 11 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1615 elemen
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
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 276**
Pak Dengklek memiliki daftar absensi **1707 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 277**
Pak Dengklek memiliki daftar absensi **549 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 13 langkah
D. 9 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 549 elemen
- Langkah 1: Sisa populasi tebasan separuh = 275 elemen
- Langkah 2: Sisa populasi tebasan separuh = 138 elemen
- Langkah 3: Sisa populasi tebasan separuh = 69 elemen
- Langkah 4: Sisa populasi tebasan separuh = 35 elemen
- Langkah 5: Sisa populasi tebasan separuh = 18 elemen
- Langkah 6: Sisa populasi tebasan separuh = 9 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 278**
Diberikan barisan angka: `[47, 16, 36, 38, 77]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [16, 36, 38, 47, 77]
B. [47, 16, 36, 77, 38]
C. [38, 36, 16, 47, 77]
D. [38, 77, 36, 47, 16]
E. [16, 38, 36, 77, 47]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([16, 36, 38, 47, 77])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[47, 16, 36, 38, 77]`
Cek posisi 0&1 (47 > 16) -> Tukar! Array kini: `[16, 47, 36, 38, 77]`
Cek posisi 1&2 (47 > 36) -> Tukar! Array kini: `[16, 36, 47, 38, 77]`
Cek posisi 2&3 (47 > 38) -> Tukar! Array kini: `[16, 36, 38, 47, 77]`
Cek posisi 3&4 (47 < 77) -> Aman dibiarkan. Array kini: `[16, 36, 38, 47, 77]`


Terbukti bahwa elemen maha gemuk (`77`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[16, 36, 38, 47, 77]**.
</details>

---
**Soal 279**
Diberikan barisan angka: `[56, 61, 88, 19, 73]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [56, 19, 73, 61, 88]
B. [61, 19, 88, 56, 73]
C. [56, 61, 19, 88, 73]
D. [56, 61, 19, 73, 88]
E. [88, 56, 19, 73, 61]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([56, 61, 19, 73, 88])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[56, 61, 88, 19, 73]`
Cek posisi 0&1 (56 < 61) -> Aman dibiarkan. Array kini: `[56, 61, 88, 19, 73]`
Cek posisi 1&2 (61 < 88) -> Aman dibiarkan. Array kini: `[56, 61, 88, 19, 73]`
Cek posisi 2&3 (88 > 19) -> Tukar! Array kini: `[56, 61, 19, 88, 73]`
Cek posisi 3&4 (88 > 73) -> Tukar! Array kini: `[56, 61, 19, 73, 88]`


Terbukti bahwa elemen maha gemuk (`88`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[56, 61, 19, 73, 88]**.
</details>

---
**Soal 280**
Pak Dengklek memiliki daftar absensi **1437 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1437 elemen
- Langkah 1: Sisa populasi tebasan separuh = 719 elemen
- Langkah 2: Sisa populasi tebasan separuh = 360 elemen
- Langkah 3: Sisa populasi tebasan separuh = 180 elemen
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
**Soal 281**
Bebek-bebek di barisan bernomor dada: `[25, 38, 46, 67, 13, 69]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [46, 13, 25, 67, 38, 69]
B. [13, 25, 46, 67, 38, 69]
C. [25, 46, 13, 38, 69, 67]
D. [69, 38, 13, 46, 67, 25]
E. [69, 67, 38, 25, 46, 13]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([13, 25, 46, 67, 38, 69])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[25, 38, 46, 67, 13, 69]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 38, 46, 67, 25, 69]. Ditemukan si `13`. Tukar paksa dudukan dengan `25`. Array mutasi -> `[13, 38, 46, 67, 25, 69]`
- Putaran 2: Cari anak terpecebol di area sisa [25, 46, 67, 38, 69]. Ditemukan si `25`. Tukar paksa dudukan dengan `38`. Array mutasi -> `[13, 25, 46, 67, 38, 69]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 25, 46, 67, 38, 69]**. Opsi murni: **B**.
</details>

---
**Soal 282**
Pak Dengklek memiliki daftar absensi **1928 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1928 elemen
- Langkah 1: Sisa populasi tebasan separuh = 964 elemen
- Langkah 2: Sisa populasi tebasan separuh = 482 elemen
- Langkah 3: Sisa populasi tebasan separuh = 241 elemen
- Langkah 4: Sisa populasi tebasan separuh = 121 elemen
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
**Soal 283**
Bebek-bebek di barisan bernomor dada: `[16, 83, 91, 84, 21, 32]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [21, 84, 83, 91, 16, 32]
B. [84, 83, 21, 91, 16, 32]
C. [16, 21, 91, 84, 83, 32]
D. [21, 32, 16, 84, 83, 91]
E. [21, 84, 16, 91, 32, 83]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([16, 21, 91, 84, 83, 32])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[16, 83, 91, 84, 21, 32]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 83, 91, 84, 21, 32]. Ditemukan si `16`. Tukar paksa dudukan dengan `16`. Array mutasi -> `[16, 83, 91, 84, 21, 32]`
- Putaran 2: Cari anak terpecebol di area sisa [21, 91, 84, 83, 32]. Ditemukan si `21`. Tukar paksa dudukan dengan `83`. Array mutasi -> `[16, 21, 91, 84, 83, 32]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 21, 91, 84, 83, 32]**. Opsi murni: **C**.
</details>

---
**Soal 284**
Bebek-bebek di barisan bernomor dada: `[21, 98, 80, 69, 61, 92]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [69, 21, 98, 92, 61, 80]
B. [21, 61, 80, 69, 98, 92]
C. [61, 69, 92, 80, 98, 21]
D. [69, 21, 61, 98, 80, 92]
E. [80, 92, 61, 69, 21, 98]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([21, 61, 80, 69, 98, 92])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[21, 98, 80, 69, 61, 92]`
- Putaran 1: Cari anak terpecebol di area sisa [21, 98, 80, 69, 61, 92]. Ditemukan si `21`. Tukar paksa dudukan dengan `21`. Array mutasi -> `[21, 98, 80, 69, 61, 92]`
- Putaran 2: Cari anak terpecebol di area sisa [61, 80, 69, 98, 92]. Ditemukan si `61`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[21, 61, 80, 69, 98, 92]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[21, 61, 80, 69, 98, 92]**. Opsi murni: **B**.
</details>

---
**Soal 285**
Bebek-bebek di barisan bernomor dada: `[89, 91, 68, 21, 62, 57]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [62, 68, 91, 57, 21, 89]
B. [21, 57, 68, 89, 62, 91]
C. [89, 21, 57, 62, 68, 91]
D. [57, 21, 91, 62, 68, 89]
E. [91, 62, 57, 21, 68, 89]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([21, 57, 68, 89, 62, 91])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[89, 91, 68, 21, 62, 57]`
- Putaran 1: Cari anak terpecebol di area sisa [21, 91, 68, 89, 62, 57]. Ditemukan si `21`. Tukar paksa dudukan dengan `89`. Array mutasi -> `[21, 91, 68, 89, 62, 57]`
- Putaran 2: Cari anak terpecebol di area sisa [57, 68, 89, 62, 91]. Ditemukan si `57`. Tukar paksa dudukan dengan `91`. Array mutasi -> `[21, 57, 68, 89, 62, 91]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[21, 57, 68, 89, 62, 91]**. Opsi murni: **B**.
</details>

---
**Soal 286**
Diberikan barisan angka: `[59, 17, 86, 26, 70]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [26, 59, 86, 70, 17]
B. [17, 59, 26, 70, 86]
C. [26, 86, 70, 17, 59]
D. [17, 70, 86, 59, 26]
E. [59, 86, 17, 26, 70]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([17, 59, 26, 70, 86])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[59, 17, 86, 26, 70]`
Cek posisi 0&1 (59 > 17) -> Tukar! Array kini: `[17, 59, 86, 26, 70]`
Cek posisi 1&2 (59 < 86) -> Aman dibiarkan. Array kini: `[17, 59, 86, 26, 70]`
Cek posisi 2&3 (86 > 26) -> Tukar! Array kini: `[17, 59, 26, 86, 70]`
Cek posisi 3&4 (86 > 70) -> Tukar! Array kini: `[17, 59, 26, 70, 86]`


Terbukti bahwa elemen maha gemuk (`86`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[17, 59, 26, 70, 86]**.
</details>

---
**Soal 287**
Diberikan barisan angka: `[22, 89, 14, 70, 78]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [78, 22, 89, 14, 70]
B. [78, 22, 14, 89, 70]
C. [70, 14, 78, 22, 89]
D. [22, 14, 70, 78, 89]
E. [78, 70, 89, 22, 14]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([22, 14, 70, 78, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[22, 89, 14, 70, 78]`
Cek posisi 0&1 (22 < 89) -> Aman dibiarkan. Array kini: `[22, 89, 14, 70, 78]`
Cek posisi 1&2 (89 > 14) -> Tukar! Array kini: `[22, 14, 89, 70, 78]`
Cek posisi 2&3 (89 > 70) -> Tukar! Array kini: `[22, 14, 70, 89, 78]`
Cek posisi 3&4 (89 > 78) -> Tukar! Array kini: `[22, 14, 70, 78, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[22, 14, 70, 78, 89]**.
</details>

---
**Soal 288**
Bebek-bebek di barisan bernomor dada: `[69, 74, 48, 37, 10, 31]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [10, 48, 37, 31, 69, 74]
B. [10, 31, 48, 37, 69, 74]
C. [10, 74, 37, 69, 31, 48]
D. [69, 74, 10, 37, 48, 31]
E. [48, 37, 10, 31, 74, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([10, 31, 48, 37, 69, 74])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[69, 74, 48, 37, 10, 31]`
- Putaran 1: Cari anak terpecebol di area sisa [10, 74, 48, 37, 69, 31]. Ditemukan si `10`. Tukar paksa dudukan dengan `69`. Array mutasi -> `[10, 74, 48, 37, 69, 31]`
- Putaran 2: Cari anak terpecebol di area sisa [31, 48, 37, 69, 74]. Ditemukan si `31`. Tukar paksa dudukan dengan `74`. Array mutasi -> `[10, 31, 48, 37, 69, 74]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[10, 31, 48, 37, 69, 74]**. Opsi murni: **B**.
</details>

---
**Soal 289**
Bebek-bebek di barisan bernomor dada: `[55, 80, 38, 25, 34, 63]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [38, 25, 55, 80, 63, 34]
B. [25, 34, 38, 55, 80, 63]
C. [63, 38, 55, 80, 34, 25]
D. [34, 55, 25, 38, 63, 80]
E. [63, 80, 55, 25, 38, 34]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([25, 34, 38, 55, 80, 63])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[55, 80, 38, 25, 34, 63]`
- Putaran 1: Cari anak terpecebol di area sisa [25, 80, 38, 55, 34, 63]. Ditemukan si `25`. Tukar paksa dudukan dengan `55`. Array mutasi -> `[25, 80, 38, 55, 34, 63]`
- Putaran 2: Cari anak terpecebol di area sisa [34, 38, 55, 80, 63]. Ditemukan si `34`. Tukar paksa dudukan dengan `80`. Array mutasi -> `[25, 34, 38, 55, 80, 63]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[25, 34, 38, 55, 80, 63]**. Opsi murni: **B**.
</details>

---
**Soal 290**
Pak Dengklek memiliki daftar absensi **809 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 9 langkah
C. 11 langkah
D. 13 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 809 elemen
- Langkah 1: Sisa populasi tebasan separuh = 405 elemen
- Langkah 2: Sisa populasi tebasan separuh = 203 elemen
- Langkah 3: Sisa populasi tebasan separuh = 102 elemen
- Langkah 4: Sisa populasi tebasan separuh = 51 elemen
- Langkah 5: Sisa populasi tebasan separuh = 26 elemen
- Langkah 6: Sisa populasi tebasan separuh = 13 elemen
- Langkah 7: Sisa populasi tebasan separuh = 7 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 291**
Bebek-bebek di barisan bernomor dada: `[13, 18, 89, 57, 34, 49]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [34, 18, 49, 13, 89, 57]
B. [18, 89, 57, 34, 13, 49]
C. [13, 18, 89, 57, 34, 49]
D. [18, 34, 57, 49, 89, 13]
E. [34, 13, 89, 57, 49, 18]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([13, 18, 89, 57, 34, 49])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[13, 18, 89, 57, 34, 49]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 18, 89, 57, 34, 49]. Ditemukan si `13`. Tukar paksa dudukan dengan `13`. Array mutasi -> `[13, 18, 89, 57, 34, 49]`
- Putaran 2: Cari anak terpecebol di area sisa [18, 89, 57, 34, 49]. Ditemukan si `18`. Tukar paksa dudukan dengan `18`. Array mutasi -> `[13, 18, 89, 57, 34, 49]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 18, 89, 57, 34, 49]**. Opsi murni: **C**.
</details>

---
**Soal 292**
Diberikan barisan angka: `[25, 91, 74, 69, 11]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [11, 25, 91, 74, 69]
B. [25, 74, 69, 11, 91]
C. [91, 69, 11, 74, 25]
D. [74, 25, 69, 91, 11]
E. [69, 11, 74, 25, 91]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([25, 74, 69, 11, 91])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[25, 91, 74, 69, 11]`
Cek posisi 0&1 (25 < 91) -> Aman dibiarkan. Array kini: `[25, 91, 74, 69, 11]`
Cek posisi 1&2 (91 > 74) -> Tukar! Array kini: `[25, 74, 91, 69, 11]`
Cek posisi 2&3 (91 > 69) -> Tukar! Array kini: `[25, 74, 69, 91, 11]`
Cek posisi 3&4 (91 > 11) -> Tukar! Array kini: `[25, 74, 69, 11, 91]`


Terbukti bahwa elemen maha gemuk (`91`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[25, 74, 69, 11, 91]**.
</details>

---
**Soal 293**
Diberikan barisan angka: `[69, 12, 30, 48, 93]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [30, 48, 69, 12, 93]
B. [48, 69, 93, 12, 30]
C. [69, 12, 48, 30, 93]
D. [48, 12, 93, 30, 69]
E. [12, 30, 48, 69, 93]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([12, 30, 48, 69, 93])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[69, 12, 30, 48, 93]`
Cek posisi 0&1 (69 > 12) -> Tukar! Array kini: `[12, 69, 30, 48, 93]`
Cek posisi 1&2 (69 > 30) -> Tukar! Array kini: `[12, 30, 69, 48, 93]`
Cek posisi 2&3 (69 > 48) -> Tukar! Array kini: `[12, 30, 48, 69, 93]`
Cek posisi 3&4 (69 < 93) -> Aman dibiarkan. Array kini: `[12, 30, 48, 69, 93]`


Terbukti bahwa elemen maha gemuk (`93`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[12, 30, 48, 69, 93]**.
</details>

---
**Soal 294**
Pak Dengklek memiliki daftar absensi **505 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 8 langkah
C. 12 langkah
D. 9 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (9 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 505 elemen
- Langkah 1: Sisa populasi tebasan separuh = 253 elemen
- Langkah 2: Sisa populasi tebasan separuh = 127 elemen
- Langkah 3: Sisa populasi tebasan separuh = 64 elemen
- Langkah 4: Sisa populasi tebasan separuh = 32 elemen
- Langkah 5: Sisa populasi tebasan separuh = 16 elemen
- Langkah 6: Sisa populasi tebasan separuh = 8 elemen
- Langkah 7: Sisa populasi tebasan separuh = 4 elemen
- Langkah 8: Sisa populasi tebasan separuh = 2 elemen
- Langkah 9: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **9 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 295**
Bebek-bebek di barisan bernomor dada: `[81, 93, 26, 92, 34, 79]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [93, 81, 92, 34, 26, 79]
B. [93, 34, 79, 26, 92, 81]
C. [34, 92, 26, 79, 81, 93]
D. [26, 34, 81, 92, 93, 79]
E. [81, 26, 93, 34, 92, 79]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([26, 34, 81, 92, 93, 79])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[81, 93, 26, 92, 34, 79]`
- Putaran 1: Cari anak terpecebol di area sisa [26, 93, 81, 92, 34, 79]. Ditemukan si `26`. Tukar paksa dudukan dengan `81`. Array mutasi -> `[26, 93, 81, 92, 34, 79]`
- Putaran 2: Cari anak terpecebol di area sisa [34, 81, 92, 93, 79]. Ditemukan si `34`. Tukar paksa dudukan dengan `93`. Array mutasi -> `[26, 34, 81, 92, 93, 79]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[26, 34, 81, 92, 93, 79]**. Opsi murni: **D**.
</details>

---
**Soal 296**
Diberikan barisan angka: `[16, 88, 95, 73, 23]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [16, 88, 73, 23, 95]
B. [95, 88, 16, 23, 73]
C. [73, 95, 88, 23, 16]
D. [88, 23, 16, 95, 73]
E. [23, 73, 95, 88, 16]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([16, 88, 73, 23, 95])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[16, 88, 95, 73, 23]`
Cek posisi 0&1 (16 < 88) -> Aman dibiarkan. Array kini: `[16, 88, 95, 73, 23]`
Cek posisi 1&2 (88 < 95) -> Aman dibiarkan. Array kini: `[16, 88, 95, 73, 23]`
Cek posisi 2&3 (95 > 73) -> Tukar! Array kini: `[16, 88, 73, 95, 23]`
Cek posisi 3&4 (95 > 23) -> Tukar! Array kini: `[16, 88, 73, 23, 95]`


Terbukti bahwa elemen maha gemuk (`95`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[16, 88, 73, 23, 95]**.
</details>

---
**Soal 297**
Diberikan barisan angka: `[51, 68, 65, 31, 78]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [78, 51, 31, 68, 65]
B. [51, 78, 31, 65, 68]
C. [51, 65, 31, 68, 78]
D. [65, 31, 78, 51, 68]
E. [51, 31, 68, 65, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([51, 65, 31, 68, 78])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[51, 68, 65, 31, 78]`
Cek posisi 0&1 (51 < 68) -> Aman dibiarkan. Array kini: `[51, 68, 65, 31, 78]`
Cek posisi 1&2 (68 > 65) -> Tukar! Array kini: `[51, 65, 68, 31, 78]`
Cek posisi 2&3 (68 > 31) -> Tukar! Array kini: `[51, 65, 31, 68, 78]`
Cek posisi 3&4 (68 < 78) -> Aman dibiarkan. Array kini: `[51, 65, 31, 68, 78]`


Terbukti bahwa elemen maha gemuk (`78`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[51, 65, 31, 68, 78]**.
</details>

---
**Soal 298**
Bebek-bebek di barisan bernomor dada: `[52, 55, 51, 41, 82, 36]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [36, 41, 55, 51, 82, 52]
B. [55, 51, 36, 41, 52, 82]
C. [41, 82, 51, 36, 52, 55]
D. [52, 82, 55, 36, 41, 51]
E. [36, 41, 51, 55, 82, 52]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([36, 41, 51, 55, 82, 52])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[52, 55, 51, 41, 82, 36]`
- Putaran 1: Cari anak terpecebol di area sisa [36, 55, 51, 41, 82, 52]. Ditemukan si `36`. Tukar paksa dudukan dengan `52`. Array mutasi -> `[36, 55, 51, 41, 82, 52]`
- Putaran 2: Cari anak terpecebol di area sisa [41, 51, 55, 82, 52]. Ditemukan si `41`. Tukar paksa dudukan dengan `55`. Array mutasi -> `[36, 41, 51, 55, 82, 52]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[36, 41, 51, 55, 82, 52]**. Opsi murni: **E**.
</details>

---
**Soal 299**
Pak Dengklek memiliki daftar absensi **629 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 10 langkah
C. 12 langkah
D. 13 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 629 elemen
- Langkah 1: Sisa populasi tebasan separuh = 315 elemen
- Langkah 2: Sisa populasi tebasan separuh = 158 elemen
- Langkah 3: Sisa populasi tebasan separuh = 79 elemen
- Langkah 4: Sisa populasi tebasan separuh = 40 elemen
- Langkah 5: Sisa populasi tebasan separuh = 20 elemen
- Langkah 6: Sisa populasi tebasan separuh = 10 elemen
- Langkah 7: Sisa populasi tebasan separuh = 5 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 300**
Bebek-bebek di barisan bernomor dada: `[28, 75, 74, 21, 15, 38]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [15, 21, 74, 75, 28, 38]
B. [28, 74, 38, 21, 75, 15]
C. [21, 15, 28, 38, 75, 74]
D. [74, 28, 21, 38, 75, 15]
E. [74, 75, 38, 28, 15, 21]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([15, 21, 74, 75, 28, 38])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[28, 75, 74, 21, 15, 38]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 75, 74, 21, 28, 38]. Ditemukan si `15`. Tukar paksa dudukan dengan `28`. Array mutasi -> `[15, 75, 74, 21, 28, 38]`
- Putaran 2: Cari anak terpecebol di area sisa [21, 74, 75, 28, 38]. Ditemukan si `21`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[15, 21, 74, 75, 28, 38]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 21, 74, 75, 28, 38]**. Opsi murni: **A**.
</details>

---
