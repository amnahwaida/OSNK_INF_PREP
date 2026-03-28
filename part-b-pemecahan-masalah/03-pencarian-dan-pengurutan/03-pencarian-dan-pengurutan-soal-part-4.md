🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Pencarian & Pengurutan (Part 4 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 151**
Pak Dengklek memiliki daftar absensi **1565 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 14 langkah
C. 12 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1565 elemen
- Langkah 1: Sisa populasi tebasan separuh = 783 elemen
- Langkah 2: Sisa populasi tebasan separuh = 392 elemen
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
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 152**
Pak Dengklek memiliki daftar absensi **1006 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 13 langkah
D. 9 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1006 elemen
- Langkah 1: Sisa populasi tebasan separuh = 503 elemen
- Langkah 2: Sisa populasi tebasan separuh = 252 elemen
- Langkah 3: Sisa populasi tebasan separuh = 126 elemen
- Langkah 4: Sisa populasi tebasan separuh = 63 elemen
- Langkah 5: Sisa populasi tebasan separuh = 32 elemen
- Langkah 6: Sisa populasi tebasan separuh = 16 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 153**
Diberikan barisan angka: `[12, 34, 98, 72, 75]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [12, 72, 98, 34, 75]
B. [34, 12, 72, 75, 98]
C. [12, 34, 72, 75, 98]
D. [72, 98, 75, 12, 34]
E. [75, 72, 98, 34, 12]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([12, 34, 72, 75, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[12, 34, 98, 72, 75]`
Cek posisi 0&1 (12 < 34) -> Aman dibiarkan. Array kini: `[12, 34, 98, 72, 75]`
Cek posisi 1&2 (34 < 98) -> Aman dibiarkan. Array kini: `[12, 34, 98, 72, 75]`
Cek posisi 2&3 (98 > 72) -> Tukar! Array kini: `[12, 34, 72, 98, 75]`
Cek posisi 3&4 (98 > 75) -> Tukar! Array kini: `[12, 34, 72, 75, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[12, 34, 72, 75, 98]**.
</details>

---
**Soal 154**
Pak Dengklek memiliki daftar absensi **1461 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 10 langkah
C. 13 langkah
D. 11 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1461 elemen
- Langkah 1: Sisa populasi tebasan separuh = 731 elemen
- Langkah 2: Sisa populasi tebasan separuh = 366 elemen
- Langkah 3: Sisa populasi tebasan separuh = 183 elemen
- Langkah 4: Sisa populasi tebasan separuh = 92 elemen
- Langkah 5: Sisa populasi tebasan separuh = 46 elemen
- Langkah 6: Sisa populasi tebasan separuh = 23 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 155**
Bebek-bebek di barisan bernomor dada: `[58, 96, 32, 42, 52, 93]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [96, 58, 52, 42, 32, 93]
B. [32, 58, 96, 93, 52, 42]
C. [32, 42, 58, 96, 52, 93]
D. [58, 96, 32, 52, 93, 42]
E. [96, 52, 42, 32, 58, 93]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([32, 42, 58, 96, 52, 93])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[58, 96, 32, 42, 52, 93]`
- Putaran 1: Cari anak terpecebol di area sisa [32, 96, 58, 42, 52, 93]. Ditemukan si `32`. Tukar paksa dudukan dengan `58`. Array mutasi -> `[32, 96, 58, 42, 52, 93]`
- Putaran 2: Cari anak terpecebol di area sisa [42, 58, 96, 52, 93]. Ditemukan si `42`. Tukar paksa dudukan dengan `96`. Array mutasi -> `[32, 42, 58, 96, 52, 93]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[32, 42, 58, 96, 52, 93]**. Opsi murni: **C**.
</details>

---
**Soal 156**
Diberikan barisan angka: `[72, 10, 92, 15, 37]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [10, 15, 72, 92, 37]
B. [10, 72, 92, 15, 37]
C. [10, 92, 15, 37, 72]
D. [10, 72, 15, 37, 92]
E. [72, 15, 92, 10, 37]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([10, 72, 15, 37, 92])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[72, 10, 92, 15, 37]`
Cek posisi 0&1 (72 > 10) -> Tukar! Array kini: `[10, 72, 92, 15, 37]`
Cek posisi 1&2 (72 < 92) -> Aman dibiarkan. Array kini: `[10, 72, 92, 15, 37]`
Cek posisi 2&3 (92 > 15) -> Tukar! Array kini: `[10, 72, 15, 92, 37]`
Cek posisi 3&4 (92 > 37) -> Tukar! Array kini: `[10, 72, 15, 37, 92]`


Terbukti bahwa elemen maha gemuk (`92`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[10, 72, 15, 37, 92]**.
</details>

---
**Soal 157**
Bebek-bebek di barisan bernomor dada: `[47, 52, 63, 25, 65, 20]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [47, 20, 52, 65, 63, 25]
B. [47, 52, 20, 65, 25, 63]
C. [47, 63, 25, 52, 65, 20]
D. [20, 63, 52, 65, 47, 25]
E. [20, 25, 63, 52, 65, 47]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([20, 25, 63, 52, 65, 47])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[47, 52, 63, 25, 65, 20]`
- Putaran 1: Cari anak terpecebol di area sisa [20, 52, 63, 25, 65, 47]. Ditemukan si `20`. Tukar paksa dudukan dengan `47`. Array mutasi -> `[20, 52, 63, 25, 65, 47]`
- Putaran 2: Cari anak terpecebol di area sisa [25, 63, 52, 65, 47]. Ditemukan si `25`. Tukar paksa dudukan dengan `52`. Array mutasi -> `[20, 25, 63, 52, 65, 47]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[20, 25, 63, 52, 65, 47]**. Opsi murni: **E**.
</details>

---
**Soal 158**
Bebek-bebek di barisan bernomor dada: `[21, 38, 15, 91, 47, 19]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [38, 15, 19, 91, 21, 47]
B. [21, 19, 15, 38, 47, 91]
C. [38, 15, 19, 47, 91, 21]
D. [38, 47, 19, 15, 91, 21]
E. [15, 19, 21, 91, 47, 38]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([15, 19, 21, 91, 47, 38])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[21, 38, 15, 91, 47, 19]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 38, 21, 91, 47, 19]. Ditemukan si `15`. Tukar paksa dudukan dengan `21`. Array mutasi -> `[15, 38, 21, 91, 47, 19]`
- Putaran 2: Cari anak terpecebol di area sisa [19, 21, 91, 47, 38]. Ditemukan si `19`. Tukar paksa dudukan dengan `38`. Array mutasi -> `[15, 19, 21, 91, 47, 38]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 19, 21, 91, 47, 38]**. Opsi murni: **E**.
</details>

---
**Soal 159**
Diberikan barisan angka: `[55, 89, 36, 69, 67]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [36, 55, 89, 69, 67]
B. [36, 89, 69, 55, 67]
C. [55, 36, 69, 67, 89]
D. [67, 55, 69, 36, 89]
E. [55, 89, 69, 36, 67]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([55, 36, 69, 67, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[55, 89, 36, 69, 67]`
Cek posisi 0&1 (55 < 89) -> Aman dibiarkan. Array kini: `[55, 89, 36, 69, 67]`
Cek posisi 1&2 (89 > 36) -> Tukar! Array kini: `[55, 36, 89, 69, 67]`
Cek posisi 2&3 (89 > 69) -> Tukar! Array kini: `[55, 36, 69, 89, 67]`
Cek posisi 3&4 (89 > 67) -> Tukar! Array kini: `[55, 36, 69, 67, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[55, 36, 69, 67, 89]**.
</details>

---
**Soal 160**
Pak Dengklek memiliki daftar absensi **1505 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 10 langkah
C. 12 langkah
D. 11 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1505 elemen
- Langkah 1: Sisa populasi tebasan separuh = 753 elemen
- Langkah 2: Sisa populasi tebasan separuh = 377 elemen
- Langkah 3: Sisa populasi tebasan separuh = 189 elemen
- Langkah 4: Sisa populasi tebasan separuh = 95 elemen
- Langkah 5: Sisa populasi tebasan separuh = 48 elemen
- Langkah 6: Sisa populasi tebasan separuh = 24 elemen
- Langkah 7: Sisa populasi tebasan separuh = 12 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 161**
Bebek-bebek di barisan bernomor dada: `[63, 61, 95, 73, 16, 67]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [73, 61, 67, 95, 16, 63]
B. [95, 61, 16, 67, 63, 73]
C. [73, 16, 67, 61, 63, 95]
D. [61, 63, 16, 73, 95, 67]
E. [16, 61, 95, 73, 63, 67]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([16, 61, 95, 73, 63, 67])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[63, 61, 95, 73, 16, 67]`
- Putaran 1: Cari anak terpecebol di area sisa [16, 61, 95, 73, 63, 67]. Ditemukan si `16`. Tukar paksa dudukan dengan `63`. Array mutasi -> `[16, 61, 95, 73, 63, 67]`
- Putaran 2: Cari anak terpecebol di area sisa [61, 95, 73, 63, 67]. Ditemukan si `61`. Tukar paksa dudukan dengan `61`. Array mutasi -> `[16, 61, 95, 73, 63, 67]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[16, 61, 95, 73, 63, 67]**. Opsi murni: **E**.
</details>

---
**Soal 162**
Diberikan barisan angka: `[55, 16, 20, 82, 23]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [16, 20, 55, 23, 82]
B. [23, 16, 20, 82, 55]
C. [82, 55, 20, 23, 16]
D. [16, 20, 82, 55, 23]
E. [16, 55, 23, 82, 20]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([16, 20, 55, 23, 82])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[55, 16, 20, 82, 23]`
Cek posisi 0&1 (55 > 16) -> Tukar! Array kini: `[16, 55, 20, 82, 23]`
Cek posisi 1&2 (55 > 20) -> Tukar! Array kini: `[16, 20, 55, 82, 23]`
Cek posisi 2&3 (55 < 82) -> Aman dibiarkan. Array kini: `[16, 20, 55, 82, 23]`
Cek posisi 3&4 (82 > 23) -> Tukar! Array kini: `[16, 20, 55, 23, 82]`


Terbukti bahwa elemen maha gemuk (`82`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[16, 20, 55, 23, 82]**.
</details>

---
**Soal 163**
Pak Dengklek memiliki daftar absensi **1284 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 14 langkah
C. 10 langkah
D. 12 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1284 elemen
- Langkah 1: Sisa populasi tebasan separuh = 642 elemen
- Langkah 2: Sisa populasi tebasan separuh = 321 elemen
- Langkah 3: Sisa populasi tebasan separuh = 161 elemen
- Langkah 4: Sisa populasi tebasan separuh = 81 elemen
- Langkah 5: Sisa populasi tebasan separuh = 41 elemen
- Langkah 6: Sisa populasi tebasan separuh = 21 elemen
- Langkah 7: Sisa populasi tebasan separuh = 11 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 164**
Pak Dengklek memiliki daftar absensi **823 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 823 elemen
- Langkah 1: Sisa populasi tebasan separuh = 412 elemen
- Langkah 2: Sisa populasi tebasan separuh = 206 elemen
- Langkah 3: Sisa populasi tebasan separuh = 103 elemen
- Langkah 4: Sisa populasi tebasan separuh = 52 elemen
- Langkah 5: Sisa populasi tebasan separuh = 26 elemen
- Langkah 6: Sisa populasi tebasan separuh = 13 elemen
- Langkah 7: Sisa populasi tebasan separuh = 7 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 165**
Pak Dengklek memiliki daftar absensi **651 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 11 langkah
D. 13 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 651 elemen
- Langkah 1: Sisa populasi tebasan separuh = 326 elemen
- Langkah 2: Sisa populasi tebasan separuh = 163 elemen
- Langkah 3: Sisa populasi tebasan separuh = 82 elemen
- Langkah 4: Sisa populasi tebasan separuh = 41 elemen
- Langkah 5: Sisa populasi tebasan separuh = 21 elemen
- Langkah 6: Sisa populasi tebasan separuh = 11 elemen
- Langkah 7: Sisa populasi tebasan separuh = 6 elemen
- Langkah 8: Sisa populasi tebasan separuh = 3 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 166**
Pak Dengklek memiliki daftar absensi **1191 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 11 langkah
C. 14 langkah
D. 13 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1191 elemen
- Langkah 1: Sisa populasi tebasan separuh = 596 elemen
- Langkah 2: Sisa populasi tebasan separuh = 298 elemen
- Langkah 3: Sisa populasi tebasan separuh = 149 elemen
- Langkah 4: Sisa populasi tebasan separuh = 75 elemen
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
**Soal 167**
Bebek-bebek di barisan bernomor dada: `[72, 35, 14, 39, 64, 22]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [14, 22, 72, 39, 64, 35]
B. [35, 72, 39, 64, 22, 14]
C. [35, 72, 64, 14, 22, 39]
D. [64, 35, 14, 72, 22, 39]
E. [35, 14, 72, 39, 64, 22]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([14, 22, 72, 39, 64, 35])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[72, 35, 14, 39, 64, 22]`
- Putaran 1: Cari anak terpecebol di area sisa [14, 35, 72, 39, 64, 22]. Ditemukan si `14`. Tukar paksa dudukan dengan `72`. Array mutasi -> `[14, 35, 72, 39, 64, 22]`
- Putaran 2: Cari anak terpecebol di area sisa [22, 72, 39, 64, 35]. Ditemukan si `22`. Tukar paksa dudukan dengan `35`. Array mutasi -> `[14, 22, 72, 39, 64, 35]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[14, 22, 72, 39, 64, 35]**. Opsi murni: **A**.
</details>

---
**Soal 168**
Diberikan barisan angka: `[75, 45, 89, 19, 58]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [19, 75, 58, 45, 89]
B. [45, 19, 89, 58, 75]
C. [89, 58, 75, 45, 19]
D. [89, 45, 58, 75, 19]
E. [45, 75, 19, 58, 89]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([45, 75, 19, 58, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[75, 45, 89, 19, 58]`
Cek posisi 0&1 (75 > 45) -> Tukar! Array kini: `[45, 75, 89, 19, 58]`
Cek posisi 1&2 (75 < 89) -> Aman dibiarkan. Array kini: `[45, 75, 89, 19, 58]`
Cek posisi 2&3 (89 > 19) -> Tukar! Array kini: `[45, 75, 19, 89, 58]`
Cek posisi 3&4 (89 > 58) -> Tukar! Array kini: `[45, 75, 19, 58, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[45, 75, 19, 58, 89]**.
</details>

---
**Soal 169**
Pak Dengklek memiliki daftar absensi **1647 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 10 langkah
C. 12 langkah
D. 13 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1647 elemen
- Langkah 1: Sisa populasi tebasan separuh = 824 elemen
- Langkah 2: Sisa populasi tebasan separuh = 412 elemen
- Langkah 3: Sisa populasi tebasan separuh = 206 elemen
- Langkah 4: Sisa populasi tebasan separuh = 103 elemen
- Langkah 5: Sisa populasi tebasan separuh = 52 elemen
- Langkah 6: Sisa populasi tebasan separuh = 26 elemen
- Langkah 7: Sisa populasi tebasan separuh = 13 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 170**
Bebek-bebek di barisan bernomor dada: `[20, 85, 60, 91, 63, 78]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [85, 91, 20, 60, 63, 78]
B. [85, 20, 63, 60, 78, 91]
C. [20, 60, 85, 91, 63, 78]
D. [85, 78, 60, 20, 63, 91]
E. [78, 60, 85, 20, 63, 91]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([20, 60, 85, 91, 63, 78])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[20, 85, 60, 91, 63, 78]`
- Putaran 1: Cari anak terpecebol di area sisa [20, 85, 60, 91, 63, 78]. Ditemukan si `20`. Tukar paksa dudukan dengan `20`. Array mutasi -> `[20, 85, 60, 91, 63, 78]`
- Putaran 2: Cari anak terpecebol di area sisa [60, 85, 91, 63, 78]. Ditemukan si `60`. Tukar paksa dudukan dengan `85`. Array mutasi -> `[20, 60, 85, 91, 63, 78]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[20, 60, 85, 91, 63, 78]**. Opsi murni: **C**.
</details>

---
**Soal 171**
Diberikan barisan angka: `[68, 40, 60, 96, 62]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [60, 68, 40, 96, 62]
B. [96, 60, 40, 62, 68]
C. [68, 60, 62, 40, 96]
D. [40, 60, 68, 62, 96]
E. [40, 62, 68, 60, 96]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([40, 60, 68, 62, 96])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[68, 40, 60, 96, 62]`
Cek posisi 0&1 (68 > 40) -> Tukar! Array kini: `[40, 68, 60, 96, 62]`
Cek posisi 1&2 (68 > 60) -> Tukar! Array kini: `[40, 60, 68, 96, 62]`
Cek posisi 2&3 (68 < 96) -> Aman dibiarkan. Array kini: `[40, 60, 68, 96, 62]`
Cek posisi 3&4 (96 > 62) -> Tukar! Array kini: `[40, 60, 68, 62, 96]`


Terbukti bahwa elemen maha gemuk (`96`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[40, 60, 68, 62, 96]**.
</details>

---
**Soal 172**
Diberikan barisan angka: `[84, 32, 40, 60, 35]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [40, 35, 32, 84, 60]
B. [84, 32, 60, 40, 35]
C. [32, 40, 84, 35, 60]
D. [32, 40, 60, 35, 84]
E. [32, 60, 84, 40, 35]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([32, 40, 60, 35, 84])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[84, 32, 40, 60, 35]`
Cek posisi 0&1 (84 > 32) -> Tukar! Array kini: `[32, 84, 40, 60, 35]`
Cek posisi 1&2 (84 > 40) -> Tukar! Array kini: `[32, 40, 84, 60, 35]`
Cek posisi 2&3 (84 > 60) -> Tukar! Array kini: `[32, 40, 60, 84, 35]`
Cek posisi 3&4 (84 > 35) -> Tukar! Array kini: `[32, 40, 60, 35, 84]`


Terbukti bahwa elemen maha gemuk (`84`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[32, 40, 60, 35, 84]**.
</details>

---
**Soal 173**
Pak Dengklek memiliki daftar absensi **970 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 12 langkah
C. 10 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 970 elemen
- Langkah 1: Sisa populasi tebasan separuh = 485 elemen
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
**Soal 174**
Diberikan barisan angka: `[13, 51, 46, 24, 18]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [51, 13, 24, 18, 46]
B. [24, 13, 51, 18, 46]
C. [13, 46, 24, 18, 51]
D. [46, 51, 24, 13, 18]
E. [18, 13, 46, 24, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([13, 46, 24, 18, 51])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[13, 51, 46, 24, 18]`
Cek posisi 0&1 (13 < 51) -> Aman dibiarkan. Array kini: `[13, 51, 46, 24, 18]`
Cek posisi 1&2 (51 > 46) -> Tukar! Array kini: `[13, 46, 51, 24, 18]`
Cek posisi 2&3 (51 > 24) -> Tukar! Array kini: `[13, 46, 24, 51, 18]`
Cek posisi 3&4 (51 > 18) -> Tukar! Array kini: `[13, 46, 24, 18, 51]`


Terbukti bahwa elemen maha gemuk (`51`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[13, 46, 24, 18, 51]**.
</details>

---
**Soal 175**
Pak Dengklek memiliki daftar absensi **1590 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 14 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1590 elemen
- Langkah 1: Sisa populasi tebasan separuh = 795 elemen
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
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 176**
Bebek-bebek di barisan bernomor dada: `[75, 25, 32, 20, 29, 58]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [32, 29, 58, 20, 75, 25]
B. [29, 58, 75, 25, 20, 32]
C. [29, 25, 20, 58, 75, 32]
D. [20, 25, 32, 75, 29, 58]
E. [29, 75, 58, 20, 32, 25]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([20, 25, 32, 75, 29, 58])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[75, 25, 32, 20, 29, 58]`
- Putaran 1: Cari anak terpecebol di area sisa [20, 25, 32, 75, 29, 58]. Ditemukan si `20`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[20, 25, 32, 75, 29, 58]`
- Putaran 2: Cari anak terpecebol di area sisa [25, 32, 75, 29, 58]. Ditemukan si `25`. Tukar paksa dudukan dengan `25`. Array mutasi -> `[20, 25, 32, 75, 29, 58]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[20, 25, 32, 75, 29, 58]**. Opsi murni: **D**.
</details>

---
**Soal 177**
Diberikan barisan angka: `[50, 68, 89, 93, 61]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [50, 68, 89, 61, 93]
B. [68, 93, 61, 89, 50]
C. [68, 61, 89, 93, 50]
D. [61, 68, 93, 89, 50]
E. [93, 61, 50, 68, 89]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([50, 68, 89, 61, 93])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[50, 68, 89, 93, 61]`
Cek posisi 0&1 (50 < 68) -> Aman dibiarkan. Array kini: `[50, 68, 89, 93, 61]`
Cek posisi 1&2 (68 < 89) -> Aman dibiarkan. Array kini: `[50, 68, 89, 93, 61]`
Cek posisi 2&3 (89 < 93) -> Aman dibiarkan. Array kini: `[50, 68, 89, 93, 61]`
Cek posisi 3&4 (93 > 61) -> Tukar! Array kini: `[50, 68, 89, 61, 93]`


Terbukti bahwa elemen maha gemuk (`93`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[50, 68, 89, 61, 93]**.
</details>

---
**Soal 178**
Diberikan barisan angka: `[51, 16, 47, 97, 40]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [47, 51, 40, 97, 16]
B. [16, 47, 51, 40, 97]
C. [51, 16, 97, 47, 40]
D. [51, 16, 40, 47, 97]
E. [16, 97, 47, 40, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([16, 47, 51, 40, 97])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[51, 16, 47, 97, 40]`
Cek posisi 0&1 (51 > 16) -> Tukar! Array kini: `[16, 51, 47, 97, 40]`
Cek posisi 1&2 (51 > 47) -> Tukar! Array kini: `[16, 47, 51, 97, 40]`
Cek posisi 2&3 (51 < 97) -> Aman dibiarkan. Array kini: `[16, 47, 51, 97, 40]`
Cek posisi 3&4 (97 > 40) -> Tukar! Array kini: `[16, 47, 51, 40, 97]`


Terbukti bahwa elemen maha gemuk (`97`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[16, 47, 51, 40, 97]**.
</details>

---
**Soal 179**
Diberikan barisan angka: `[79, 20, 44, 51, 14]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [79, 51, 20, 44, 14]
B. [51, 44, 14, 79, 20]
C. [20, 44, 51, 14, 79]
D. [79, 51, 14, 20, 44]
E. [51, 79, 20, 44, 14]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([20, 44, 51, 14, 79])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[79, 20, 44, 51, 14]`
Cek posisi 0&1 (79 > 20) -> Tukar! Array kini: `[20, 79, 44, 51, 14]`
Cek posisi 1&2 (79 > 44) -> Tukar! Array kini: `[20, 44, 79, 51, 14]`
Cek posisi 2&3 (79 > 51) -> Tukar! Array kini: `[20, 44, 51, 79, 14]`
Cek posisi 3&4 (79 > 14) -> Tukar! Array kini: `[20, 44, 51, 14, 79]`


Terbukti bahwa elemen maha gemuk (`79`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[20, 44, 51, 14, 79]**.
</details>

---
**Soal 180**
Diberikan barisan angka: `[87, 17, 31, 45, 44]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [87, 17, 45, 31, 44]
B. [17, 87, 45, 31, 44]
C. [45, 17, 31, 87, 44]
D. [17, 31, 45, 44, 87]
E. [45, 17, 87, 31, 44]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([17, 31, 45, 44, 87])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[87, 17, 31, 45, 44]`
Cek posisi 0&1 (87 > 17) -> Tukar! Array kini: `[17, 87, 31, 45, 44]`
Cek posisi 1&2 (87 > 31) -> Tukar! Array kini: `[17, 31, 87, 45, 44]`
Cek posisi 2&3 (87 > 45) -> Tukar! Array kini: `[17, 31, 45, 87, 44]`
Cek posisi 3&4 (87 > 44) -> Tukar! Array kini: `[17, 31, 45, 44, 87]`


Terbukti bahwa elemen maha gemuk (`87`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[17, 31, 45, 44, 87]**.
</details>

---
**Soal 181**
Bebek-bebek di barisan bernomor dada: `[64, 73, 66, 12, 97, 56]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [66, 56, 64, 73, 97, 12]
B. [73, 64, 56, 97, 66, 12]
C. [12, 56, 66, 64, 97, 73]
D. [97, 64, 73, 12, 56, 66]
E. [64, 56, 12, 73, 97, 66]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([12, 56, 66, 64, 97, 73])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[64, 73, 66, 12, 97, 56]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 73, 66, 64, 97, 56]. Ditemukan si `12`. Tukar paksa dudukan dengan `64`. Array mutasi -> `[12, 73, 66, 64, 97, 56]`
- Putaran 2: Cari anak terpecebol di area sisa [56, 66, 64, 97, 73]. Ditemukan si `56`. Tukar paksa dudukan dengan `73`. Array mutasi -> `[12, 56, 66, 64, 97, 73]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 56, 66, 64, 97, 73]**. Opsi murni: **C**.
</details>

---
**Soal 182**
Pak Dengklek memiliki daftar absensi **1084 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 13 langkah
C. 14 langkah
D. 10 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1084 elemen
- Langkah 1: Sisa populasi tebasan separuh = 542 elemen
- Langkah 2: Sisa populasi tebasan separuh = 271 elemen
- Langkah 3: Sisa populasi tebasan separuh = 136 elemen
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
**Soal 183**
Diberikan barisan angka: `[47, 98, 35, 25, 10]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [47, 35, 10, 98, 25]
B. [25, 10, 98, 35, 47]
C. [35, 98, 25, 47, 10]
D. [47, 35, 25, 10, 98]
E. [98, 35, 10, 47, 25]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([47, 35, 25, 10, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[47, 98, 35, 25, 10]`
Cek posisi 0&1 (47 < 98) -> Aman dibiarkan. Array kini: `[47, 98, 35, 25, 10]`
Cek posisi 1&2 (98 > 35) -> Tukar! Array kini: `[47, 35, 98, 25, 10]`
Cek posisi 2&3 (98 > 25) -> Tukar! Array kini: `[47, 35, 25, 98, 10]`
Cek posisi 3&4 (98 > 10) -> Tukar! Array kini: `[47, 35, 25, 10, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[47, 35, 25, 10, 98]**.
</details>

---
**Soal 184**
Diberikan barisan angka: `[25, 53, 24, 60, 98]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [60, 24, 98, 25, 53]
B. [24, 53, 98, 25, 60]
C. [25, 53, 60, 24, 98]
D. [60, 25, 24, 53, 98]
E. [25, 24, 53, 60, 98]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([25, 24, 53, 60, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[25, 53, 24, 60, 98]`
Cek posisi 0&1 (25 < 53) -> Aman dibiarkan. Array kini: `[25, 53, 24, 60, 98]`
Cek posisi 1&2 (53 > 24) -> Tukar! Array kini: `[25, 24, 53, 60, 98]`
Cek posisi 2&3 (53 < 60) -> Aman dibiarkan. Array kini: `[25, 24, 53, 60, 98]`
Cek posisi 3&4 (60 < 98) -> Aman dibiarkan. Array kini: `[25, 24, 53, 60, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[25, 24, 53, 60, 98]**.
</details>

---
**Soal 185**
Bebek-bebek di barisan bernomor dada: `[56, 49, 87, 54, 34, 38]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [34, 87, 49, 56, 38, 54]
B. [49, 54, 87, 56, 34, 38]
C. [54, 56, 49, 87, 38, 34]
D. [87, 54, 34, 49, 38, 56]
E. [34, 38, 87, 54, 56, 49]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([34, 38, 87, 54, 56, 49])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[56, 49, 87, 54, 34, 38]`
- Putaran 1: Cari anak terpecebol di area sisa [34, 49, 87, 54, 56, 38]. Ditemukan si `34`. Tukar paksa dudukan dengan `56`. Array mutasi -> `[34, 49, 87, 54, 56, 38]`
- Putaran 2: Cari anak terpecebol di area sisa [38, 87, 54, 56, 49]. Ditemukan si `38`. Tukar paksa dudukan dengan `49`. Array mutasi -> `[34, 38, 87, 54, 56, 49]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[34, 38, 87, 54, 56, 49]**. Opsi murni: **E**.
</details>

---
**Soal 186**
Diberikan barisan angka: `[18, 35, 69, 77, 66]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [18, 69, 66, 77, 35]
B. [18, 35, 69, 66, 77]
C. [77, 35, 66, 18, 69]
D. [69, 77, 35, 18, 66]
E. [69, 18, 77, 66, 35]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([18, 35, 69, 66, 77])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[18, 35, 69, 77, 66]`
Cek posisi 0&1 (18 < 35) -> Aman dibiarkan. Array kini: `[18, 35, 69, 77, 66]`
Cek posisi 1&2 (35 < 69) -> Aman dibiarkan. Array kini: `[18, 35, 69, 77, 66]`
Cek posisi 2&3 (69 < 77) -> Aman dibiarkan. Array kini: `[18, 35, 69, 77, 66]`
Cek posisi 3&4 (77 > 66) -> Tukar! Array kini: `[18, 35, 69, 66, 77]`


Terbukti bahwa elemen maha gemuk (`77`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[18, 35, 69, 66, 77]**.
</details>

---
**Soal 187**
Pak Dengklek memiliki daftar absensi **1945 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 14 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1945 elemen
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
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 188**
Bebek-bebek di barisan bernomor dada: `[88, 75, 77, 34, 35, 58]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [88, 34, 58, 35, 77, 75]
B. [34, 77, 75, 58, 35, 88]
C. [77, 58, 35, 88, 75, 34]
D. [34, 35, 77, 88, 75, 58]
E. [58, 34, 75, 35, 88, 77]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([34, 35, 77, 88, 75, 58])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[88, 75, 77, 34, 35, 58]`
- Putaran 1: Cari anak terpecebol di area sisa [34, 75, 77, 88, 35, 58]. Ditemukan si `34`. Tukar paksa dudukan dengan `88`. Array mutasi -> `[34, 75, 77, 88, 35, 58]`
- Putaran 2: Cari anak terpecebol di area sisa [35, 77, 88, 75, 58]. Ditemukan si `35`. Tukar paksa dudukan dengan `75`. Array mutasi -> `[34, 35, 77, 88, 75, 58]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[34, 35, 77, 88, 75, 58]**. Opsi murni: **D**.
</details>

---
**Soal 189**
Diberikan barisan angka: `[83, 75, 21, 89, 32]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [89, 21, 75, 83, 32]
B. [83, 89, 21, 32, 75]
C. [75, 21, 83, 32, 89]
D. [21, 89, 83, 75, 32]
E. [83, 89, 75, 21, 32]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([75, 21, 83, 32, 89])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[83, 75, 21, 89, 32]`
Cek posisi 0&1 (83 > 75) -> Tukar! Array kini: `[75, 83, 21, 89, 32]`
Cek posisi 1&2 (83 > 21) -> Tukar! Array kini: `[75, 21, 83, 89, 32]`
Cek posisi 2&3 (83 < 89) -> Aman dibiarkan. Array kini: `[75, 21, 83, 89, 32]`
Cek posisi 3&4 (89 > 32) -> Tukar! Array kini: `[75, 21, 83, 32, 89]`


Terbukti bahwa elemen maha gemuk (`89`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[75, 21, 83, 32, 89]**.
</details>

---
**Soal 190**
Diberikan barisan angka: `[31, 48, 80, 16, 63]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [31, 48, 16, 63, 80]
B. [80, 31, 16, 48, 63]
C. [63, 16, 31, 48, 80]
D. [80, 48, 31, 63, 16]
E. [16, 80, 31, 63, 48]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([31, 48, 16, 63, 80])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[31, 48, 80, 16, 63]`
Cek posisi 0&1 (31 < 48) -> Aman dibiarkan. Array kini: `[31, 48, 80, 16, 63]`
Cek posisi 1&2 (48 < 80) -> Aman dibiarkan. Array kini: `[31, 48, 80, 16, 63]`
Cek posisi 2&3 (80 > 16) -> Tukar! Array kini: `[31, 48, 16, 80, 63]`
Cek posisi 3&4 (80 > 63) -> Tukar! Array kini: `[31, 48, 16, 63, 80]`


Terbukti bahwa elemen maha gemuk (`80`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[31, 48, 16, 63, 80]**.
</details>

---
**Soal 191**
Pak Dengklek memiliki daftar absensi **1909 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 13 langkah
D. 14 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1909 elemen
- Langkah 1: Sisa populasi tebasan separuh = 955 elemen
- Langkah 2: Sisa populasi tebasan separuh = 478 elemen
- Langkah 3: Sisa populasi tebasan separuh = 239 elemen
- Langkah 4: Sisa populasi tebasan separuh = 120 elemen
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
**Soal 192**
Pak Dengklek memiliki daftar absensi **1640 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 11 langkah
D. 14 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1640 elemen
- Langkah 1: Sisa populasi tebasan separuh = 820 elemen
- Langkah 2: Sisa populasi tebasan separuh = 410 elemen
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
**Soal 193**
Diberikan barisan angka: `[38, 62, 67, 59, 35]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [67, 38, 59, 35, 62]
B. [38, 62, 67, 35, 59]
C. [38, 62, 59, 35, 67]
D. [38, 62, 59, 67, 35]
E. [62, 35, 59, 67, 38]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([38, 62, 59, 35, 67])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[38, 62, 67, 59, 35]`
Cek posisi 0&1 (38 < 62) -> Aman dibiarkan. Array kini: `[38, 62, 67, 59, 35]`
Cek posisi 1&2 (62 < 67) -> Aman dibiarkan. Array kini: `[38, 62, 67, 59, 35]`
Cek posisi 2&3 (67 > 59) -> Tukar! Array kini: `[38, 62, 59, 67, 35]`
Cek posisi 3&4 (67 > 35) -> Tukar! Array kini: `[38, 62, 59, 35, 67]`


Terbukti bahwa elemen maha gemuk (`67`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[38, 62, 59, 35, 67]**.
</details>

---
**Soal 194**
Pak Dengklek memiliki daftar absensi **1686 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 10 langkah
C. 13 langkah
D. 14 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1686 elemen
- Langkah 1: Sisa populasi tebasan separuh = 843 elemen
- Langkah 2: Sisa populasi tebasan separuh = 422 elemen
- Langkah 3: Sisa populasi tebasan separuh = 211 elemen
- Langkah 4: Sisa populasi tebasan separuh = 106 elemen
- Langkah 5: Sisa populasi tebasan separuh = 53 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 195**
Bebek-bebek di barisan bernomor dada: `[15, 52, 54, 45, 94, 41]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [45, 54, 15, 41, 52, 94]
B. [94, 54, 41, 45, 15, 52]
C. [15, 41, 94, 52, 45, 54]
D. [15, 41, 54, 45, 94, 52]
E. [15, 45, 94, 52, 41, 54]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([15, 41, 54, 45, 94, 52])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[15, 52, 54, 45, 94, 41]`
- Putaran 1: Cari anak terpecebol di area sisa [15, 52, 54, 45, 94, 41]. Ditemukan si `15`. Tukar paksa dudukan dengan `15`. Array mutasi -> `[15, 52, 54, 45, 94, 41]`
- Putaran 2: Cari anak terpecebol di area sisa [41, 54, 45, 94, 52]. Ditemukan si `41`. Tukar paksa dudukan dengan `52`. Array mutasi -> `[15, 41, 54, 45, 94, 52]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[15, 41, 54, 45, 94, 52]**. Opsi murni: **D**.
</details>

---
**Soal 196**
Pak Dengklek memiliki daftar absensi **1612 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1612 elemen
- Langkah 1: Sisa populasi tebasan separuh = 806 elemen
- Langkah 2: Sisa populasi tebasan separuh = 403 elemen
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
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 197**
Pak Dengklek memiliki daftar absensi **1229 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 14 langkah
C. 10 langkah
D. 11 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

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
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 198**
Pak Dengklek memiliki daftar absensi **1336 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1336 elemen
- Langkah 1: Sisa populasi tebasan separuh = 668 elemen
- Langkah 2: Sisa populasi tebasan separuh = 334 elemen
- Langkah 3: Sisa populasi tebasan separuh = 167 elemen
- Langkah 4: Sisa populasi tebasan separuh = 84 elemen
- Langkah 5: Sisa populasi tebasan separuh = 42 elemen
- Langkah 6: Sisa populasi tebasan separuh = 21 elemen
- Langkah 7: Sisa populasi tebasan separuh = 11 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **B**.</details>

---
**Soal 199**
Bebek-bebek di barisan bernomor dada: `[74, 82, 75, 72, 66, 23]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [82, 66, 75, 74, 23, 72]
B. [72, 23, 75, 74, 66, 82]
C. [72, 75, 23, 66, 82, 74]
D. [66, 74, 75, 72, 23, 82]
E. [23, 66, 75, 72, 82, 74]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([23, 66, 75, 72, 82, 74])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[74, 82, 75, 72, 66, 23]`
- Putaran 1: Cari anak terpecebol di area sisa [23, 82, 75, 72, 66, 74]. Ditemukan si `23`. Tukar paksa dudukan dengan `74`. Array mutasi -> `[23, 82, 75, 72, 66, 74]`
- Putaran 2: Cari anak terpecebol di area sisa [66, 75, 72, 82, 74]. Ditemukan si `66`. Tukar paksa dudukan dengan `82`. Array mutasi -> `[23, 66, 75, 72, 82, 74]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[23, 66, 75, 72, 82, 74]**. Opsi murni: **E**.
</details>

---
**Soal 200**
Bebek-bebek di barisan bernomor dada: `[63, 13, 94, 65, 17, 70]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [94, 70, 65, 63, 13, 17]
B. [13, 17, 94, 65, 63, 70]
C. [70, 13, 63, 94, 65, 17]
D. [17, 70, 13, 63, 65, 94]
E. [94, 63, 70, 13, 65, 17]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([13, 17, 94, 65, 63, 70])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[63, 13, 94, 65, 17, 70]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 63, 94, 65, 17, 70]. Ditemukan si `13`. Tukar paksa dudukan dengan `63`. Array mutasi -> `[13, 63, 94, 65, 17, 70]`
- Putaran 2: Cari anak terpecebol di area sisa [17, 94, 65, 63, 70]. Ditemukan si `17`. Tukar paksa dudukan dengan `63`. Array mutasi -> `[13, 17, 94, 65, 63, 70]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 17, 94, 65, 63, 70]**. Opsi murni: **B**.
</details>

---
