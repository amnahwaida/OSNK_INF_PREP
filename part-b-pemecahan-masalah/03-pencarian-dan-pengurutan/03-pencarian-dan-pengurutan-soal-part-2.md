🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Pencarian & Pengurutan (Part 2 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Pencarian & Pengurutan**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin / Table Tracing" DP/Sorting di balik tirai tersembunyi.

---

**Soal 51**
Bebek-bebek di barisan bernomor dada: `[74, 68, 28, 65, 54, 81]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [54, 81, 68, 65, 28, 74]
B. [28, 54, 74, 65, 68, 81]
C. [68, 74, 65, 54, 28, 81]
D. [68, 28, 81, 65, 74, 54]
E. [54, 74, 65, 81, 68, 28]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([28, 54, 74, 65, 68, 81])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[74, 68, 28, 65, 54, 81]`
- Putaran 1: Cari anak terpecebol di area sisa [28, 68, 74, 65, 54, 81]. Ditemukan si `28`. Tukar paksa dudukan dengan `74`. Array mutasi -> `[28, 68, 74, 65, 54, 81]`
- Putaran 2: Cari anak terpecebol di area sisa [54, 74, 65, 68, 81]. Ditemukan si `54`. Tukar paksa dudukan dengan `68`. Array mutasi -> `[28, 54, 74, 65, 68, 81]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[28, 54, 74, 65, 68, 81]**. Opsi murni: **B**.
</details>

---
**Soal 52**
Bebek-bebek di barisan bernomor dada: `[92, 76, 35, 36, 91, 87]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [35, 36, 92, 76, 91, 87]
B. [76, 92, 35, 91, 36, 87]
C. [35, 76, 92, 87, 91, 36]
D. [35, 36, 91, 92, 87, 76]
E. [36, 76, 91, 92, 35, 87]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([35, 36, 92, 76, 91, 87])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[92, 76, 35, 36, 91, 87]`
- Putaran 1: Cari anak terpecebol di area sisa [35, 76, 92, 36, 91, 87]. Ditemukan si `35`. Tukar paksa dudukan dengan `92`. Array mutasi -> `[35, 76, 92, 36, 91, 87]`
- Putaran 2: Cari anak terpecebol di area sisa [36, 92, 76, 91, 87]. Ditemukan si `36`. Tukar paksa dudukan dengan `76`. Array mutasi -> `[35, 36, 92, 76, 91, 87]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[35, 36, 92, 76, 91, 87]**. Opsi murni: **A**.
</details>

---
**Soal 53**
Pak Dengklek memiliki daftar absensi **1823 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 10 langkah
D. 11 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1823 elemen
- Langkah 1: Sisa populasi tebasan separuh = 912 elemen
- Langkah 2: Sisa populasi tebasan separuh = 456 elemen
- Langkah 3: Sisa populasi tebasan separuh = 228 elemen
- Langkah 4: Sisa populasi tebasan separuh = 114 elemen
- Langkah 5: Sisa populasi tebasan separuh = 57 elemen
- Langkah 6: Sisa populasi tebasan separuh = 29 elemen
- Langkah 7: Sisa populasi tebasan separuh = 15 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 54**
Diberikan barisan angka: `[51, 15, 74, 33, 24]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [24, 74, 33, 51, 15]
B. [33, 15, 51, 24, 74]
C. [15, 51, 33, 24, 74]
D. [74, 24, 15, 33, 51]
E. [74, 33, 15, 24, 51]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([15, 51, 33, 24, 74])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[51, 15, 74, 33, 24]`
Cek posisi 0&1 (51 > 15) -> Tukar! Array kini: `[15, 51, 74, 33, 24]`
Cek posisi 1&2 (51 < 74) -> Aman dibiarkan. Array kini: `[15, 51, 74, 33, 24]`
Cek posisi 2&3 (74 > 33) -> Tukar! Array kini: `[15, 51, 33, 74, 24]`
Cek posisi 3&4 (74 > 24) -> Tukar! Array kini: `[15, 51, 33, 24, 74]`


Terbukti bahwa elemen maha gemuk (`74`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[15, 51, 33, 24, 74]**.
</details>

---
**Soal 55**
Bebek-bebek di barisan bernomor dada: `[57, 47, 95, 65, 92, 25]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [25, 47, 95, 65, 92, 57]
B. [25, 57, 47, 92, 65, 95]
C. [92, 95, 47, 57, 65, 25]
D. [65, 92, 25, 95, 57, 47]
E. [95, 57, 47, 92, 65, 25]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([25, 47, 95, 65, 92, 57])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[57, 47, 95, 65, 92, 25]`
- Putaran 1: Cari anak terpecebol di area sisa [25, 47, 95, 65, 92, 57]. Ditemukan si `25`. Tukar paksa dudukan dengan `57`. Array mutasi -> `[25, 47, 95, 65, 92, 57]`
- Putaran 2: Cari anak terpecebol di area sisa [47, 95, 65, 92, 57]. Ditemukan si `47`. Tukar paksa dudukan dengan `47`. Array mutasi -> `[25, 47, 95, 65, 92, 57]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[25, 47, 95, 65, 92, 57]**. Opsi murni: **A**.
</details>

---
**Soal 56**
Bebek-bebek di barisan bernomor dada: `[13, 26, 84, 70, 50, 75]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [75, 26, 70, 84, 50, 13]
B. [13, 70, 75, 26, 84, 50]
C. [84, 50, 70, 13, 26, 75]
D. [70, 50, 84, 75, 13, 26]
E. [13, 26, 84, 70, 50, 75]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([13, 26, 84, 70, 50, 75])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[13, 26, 84, 70, 50, 75]`
- Putaran 1: Cari anak terpecebol di area sisa [13, 26, 84, 70, 50, 75]. Ditemukan si `13`. Tukar paksa dudukan dengan `13`. Array mutasi -> `[13, 26, 84, 70, 50, 75]`
- Putaran 2: Cari anak terpecebol di area sisa [26, 84, 70, 50, 75]. Ditemukan si `26`. Tukar paksa dudukan dengan `26`. Array mutasi -> `[13, 26, 84, 70, 50, 75]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[13, 26, 84, 70, 50, 75]**. Opsi murni: **E**.
</details>

---
**Soal 57**
Pak Dengklek memiliki daftar absensi **1670 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1670 elemen
- Langkah 1: Sisa populasi tebasan separuh = 835 elemen
- Langkah 2: Sisa populasi tebasan separuh = 418 elemen
- Langkah 3: Sisa populasi tebasan separuh = 209 elemen
- Langkah 4: Sisa populasi tebasan separuh = 105 elemen
- Langkah 5: Sisa populasi tebasan separuh = 53 elemen
- Langkah 6: Sisa populasi tebasan separuh = 27 elemen
- Langkah 7: Sisa populasi tebasan separuh = 14 elemen
- Langkah 8: Sisa populasi tebasan separuh = 7 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 58**
Bebek-bebek di barisan bernomor dada: `[56, 69, 17, 35, 28, 29]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [17, 28, 56, 35, 69, 29]
B. [56, 28, 35, 17, 69, 29]
C. [56, 29, 35, 69, 28, 17]
D. [17, 35, 29, 56, 69, 28]
E. [28, 29, 69, 56, 17, 35]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: A ([17, 28, 56, 35, 69, 29])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[56, 69, 17, 35, 28, 29]`
- Putaran 1: Cari anak terpecebol di area sisa [17, 69, 56, 35, 28, 29]. Ditemukan si `17`. Tukar paksa dudukan dengan `56`. Array mutasi -> `[17, 69, 56, 35, 28, 29]`
- Putaran 2: Cari anak terpecebol di area sisa [28, 56, 35, 69, 29]. Ditemukan si `28`. Tukar paksa dudukan dengan `69`. Array mutasi -> `[17, 28, 56, 35, 69, 29]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[17, 28, 56, 35, 69, 29]**. Opsi murni: **A**.
</details>

---
**Soal 59**
Bebek-bebek di barisan bernomor dada: `[53, 85, 26, 65, 38, 40]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [38, 26, 65, 85, 40, 53]
B. [26, 40, 65, 53, 38, 85]
C. [38, 53, 26, 85, 65, 40]
D. [26, 38, 53, 65, 85, 40]
E. [85, 38, 65, 26, 40, 53]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([26, 38, 53, 65, 85, 40])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[53, 85, 26, 65, 38, 40]`
- Putaran 1: Cari anak terpecebol di area sisa [26, 85, 53, 65, 38, 40]. Ditemukan si `26`. Tukar paksa dudukan dengan `53`. Array mutasi -> `[26, 85, 53, 65, 38, 40]`
- Putaran 2: Cari anak terpecebol di area sisa [38, 53, 65, 85, 40]. Ditemukan si `38`. Tukar paksa dudukan dengan `85`. Array mutasi -> `[26, 38, 53, 65, 85, 40]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[26, 38, 53, 65, 85, 40]**. Opsi murni: **D**.
</details>

---
**Soal 60**
Bebek-bebek di barisan bernomor dada: `[67, 98, 93, 54, 27, 72]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [27, 72, 93, 67, 54, 98]
B. [98, 27, 54, 67, 93, 72]
C. [27, 54, 93, 98, 67, 72]
D. [72, 27, 93, 67, 98, 54]
E. [98, 67, 54, 27, 93, 72]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([27, 54, 93, 98, 67, 72])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[67, 98, 93, 54, 27, 72]`
- Putaran 1: Cari anak terpecebol di area sisa [27, 98, 93, 54, 67, 72]. Ditemukan si `27`. Tukar paksa dudukan dengan `67`. Array mutasi -> `[27, 98, 93, 54, 67, 72]`
- Putaran 2: Cari anak terpecebol di area sisa [54, 93, 98, 67, 72]. Ditemukan si `54`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[27, 54, 93, 98, 67, 72]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[27, 54, 93, 98, 67, 72]**. Opsi murni: **C**.
</details>

---
**Soal 61**
Bebek-bebek di barisan bernomor dada: `[66, 45, 22, 78, 25, 12]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [12, 45, 25, 22, 66, 78]
B. [66, 12, 45, 22, 25, 78]
C. [78, 66, 12, 25, 45, 22]
D. [12, 22, 45, 78, 25, 66]
E. [45, 78, 25, 66, 22, 12]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([12, 22, 45, 78, 25, 66])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[66, 45, 22, 78, 25, 12]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 45, 22, 78, 25, 66]. Ditemukan si `12`. Tukar paksa dudukan dengan `66`. Array mutasi -> `[12, 45, 22, 78, 25, 66]`
- Putaran 2: Cari anak terpecebol di area sisa [22, 45, 78, 25, 66]. Ditemukan si `22`. Tukar paksa dudukan dengan `45`. Array mutasi -> `[12, 22, 45, 78, 25, 66]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 22, 45, 78, 25, 66]**. Opsi murni: **D**.
</details>

---
**Soal 62**
Diberikan barisan angka: `[69, 47, 93, 21, 73]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [69, 47, 21, 73, 93]
B. [47, 69, 21, 73, 93]
C. [47, 69, 73, 93, 21]
D. [93, 73, 69, 21, 47]
E. [21, 47, 69, 93, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([47, 69, 21, 73, 93])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[69, 47, 93, 21, 73]`
Cek posisi 0&1 (69 > 47) -> Tukar! Array kini: `[47, 69, 93, 21, 73]`
Cek posisi 1&2 (69 < 93) -> Aman dibiarkan. Array kini: `[47, 69, 93, 21, 73]`
Cek posisi 2&3 (93 > 21) -> Tukar! Array kini: `[47, 69, 21, 93, 73]`
Cek posisi 3&4 (93 > 73) -> Tukar! Array kini: `[47, 69, 21, 73, 93]`


Terbukti bahwa elemen maha gemuk (`93`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[47, 69, 21, 73, 93]**.
</details>

---
**Soal 63**
Diberikan barisan angka: `[88, 36, 41, 42, 83]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [41, 83, 88, 36, 42]
B. [88, 36, 83, 41, 42]
C. [36, 41, 42, 83, 88]
D. [41, 42, 36, 83, 88]
E. [88, 42, 36, 83, 41]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([36, 41, 42, 83, 88])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[88, 36, 41, 42, 83]`
Cek posisi 0&1 (88 > 36) -> Tukar! Array kini: `[36, 88, 41, 42, 83]`
Cek posisi 1&2 (88 > 41) -> Tukar! Array kini: `[36, 41, 88, 42, 83]`
Cek posisi 2&3 (88 > 42) -> Tukar! Array kini: `[36, 41, 42, 88, 83]`
Cek posisi 3&4 (88 > 83) -> Tukar! Array kini: `[36, 41, 42, 83, 88]`


Terbukti bahwa elemen maha gemuk (`88`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[36, 41, 42, 83, 88]**.
</details>

---
**Soal 64**
Diberikan barisan angka: `[91, 62, 94, 43, 25]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [25, 62, 91, 94, 43]
B. [25, 62, 43, 91, 94]
C. [43, 91, 25, 62, 94]
D. [94, 43, 62, 91, 25]
E. [62, 91, 43, 25, 94]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([62, 91, 43, 25, 94])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[91, 62, 94, 43, 25]`
Cek posisi 0&1 (91 > 62) -> Tukar! Array kini: `[62, 91, 94, 43, 25]`
Cek posisi 1&2 (91 < 94) -> Aman dibiarkan. Array kini: `[62, 91, 94, 43, 25]`
Cek posisi 2&3 (94 > 43) -> Tukar! Array kini: `[62, 91, 43, 94, 25]`
Cek posisi 3&4 (94 > 25) -> Tukar! Array kini: `[62, 91, 43, 25, 94]`


Terbukti bahwa elemen maha gemuk (`94`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[62, 91, 43, 25, 94]**.
</details>

---
**Soal 65**
Bebek-bebek di barisan bernomor dada: `[67, 44, 80, 18, 50, 70]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [80, 44, 67, 18, 70, 50]
B. [80, 18, 50, 67, 44, 70]
C. [18, 70, 67, 80, 44, 50]
D. [50, 80, 18, 67, 44, 70]
E. [18, 44, 80, 67, 50, 70]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([18, 44, 80, 67, 50, 70])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[67, 44, 80, 18, 50, 70]`
- Putaran 1: Cari anak terpecebol di area sisa [18, 44, 80, 67, 50, 70]. Ditemukan si `18`. Tukar paksa dudukan dengan `67`. Array mutasi -> `[18, 44, 80, 67, 50, 70]`
- Putaran 2: Cari anak terpecebol di area sisa [44, 80, 67, 50, 70]. Ditemukan si `44`. Tukar paksa dudukan dengan `44`. Array mutasi -> `[18, 44, 80, 67, 50, 70]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[18, 44, 80, 67, 50, 70]**. Opsi murni: **E**.
</details>

---
**Soal 66**
Pak Dengklek memiliki daftar absensi **1662 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 11 langkah
D. 13 langkah
E. 14 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1662 elemen
- Langkah 1: Sisa populasi tebasan separuh = 831 elemen
- Langkah 2: Sisa populasi tebasan separuh = 416 elemen
- Langkah 3: Sisa populasi tebasan separuh = 208 elemen
- Langkah 4: Sisa populasi tebasan separuh = 104 elemen
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
**Soal 67**
Pak Dengklek memiliki daftar absensi **1342 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 11 langkah
C. 13 langkah
D. 10 langkah
E. 12 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1342 elemen
- Langkah 1: Sisa populasi tebasan separuh = 671 elemen
- Langkah 2: Sisa populasi tebasan separuh = 336 elemen
- Langkah 3: Sisa populasi tebasan separuh = 168 elemen
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
**Soal 68**
Pak Dengklek memiliki daftar absensi **1391 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1391 elemen
- Langkah 1: Sisa populasi tebasan separuh = 696 elemen
- Langkah 2: Sisa populasi tebasan separuh = 348 elemen
- Langkah 3: Sisa populasi tebasan separuh = 174 elemen
- Langkah 4: Sisa populasi tebasan separuh = 87 elemen
- Langkah 5: Sisa populasi tebasan separuh = 44 elemen
- Langkah 6: Sisa populasi tebasan separuh = 22 elemen
- Langkah 7: Sisa populasi tebasan separuh = 11 elemen
- Langkah 8: Sisa populasi tebasan separuh = 6 elemen
- Langkah 9: Sisa populasi tebasan separuh = 3 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 69**
Bebek-bebek di barisan bernomor dada: `[21, 12, 91, 84, 49, 69]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [12, 91, 69, 21, 49, 84]
B. [49, 12, 91, 84, 21, 69]
C. [12, 21, 91, 84, 49, 69]
D. [49, 91, 12, 84, 21, 69]
E. [12, 84, 91, 49, 21, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([12, 21, 91, 84, 49, 69])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[21, 12, 91, 84, 49, 69]`
- Putaran 1: Cari anak terpecebol di area sisa [12, 21, 91, 84, 49, 69]. Ditemukan si `12`. Tukar paksa dudukan dengan `21`. Array mutasi -> `[12, 21, 91, 84, 49, 69]`
- Putaran 2: Cari anak terpecebol di area sisa [21, 91, 84, 49, 69]. Ditemukan si `21`. Tukar paksa dudukan dengan `21`. Array mutasi -> `[12, 21, 91, 84, 49, 69]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[12, 21, 91, 84, 49, 69]**. Opsi murni: **C**.
</details>

---
**Soal 70**
Pak Dengklek memiliki daftar absensi **929 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 11 langkah
B. 13 langkah
C. 12 langkah
D. 9 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 929 elemen
- Langkah 1: Sisa populasi tebasan separuh = 465 elemen
- Langkah 2: Sisa populasi tebasan separuh = 233 elemen
- Langkah 3: Sisa populasi tebasan separuh = 117 elemen
- Langkah 4: Sisa populasi tebasan separuh = 59 elemen
- Langkah 5: Sisa populasi tebasan separuh = 30 elemen
- Langkah 6: Sisa populasi tebasan separuh = 15 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 71**
Pak Dengklek memiliki daftar absensi **1101 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1101 elemen
- Langkah 1: Sisa populasi tebasan separuh = 551 elemen
- Langkah 2: Sisa populasi tebasan separuh = 276 elemen
- Langkah 3: Sisa populasi tebasan separuh = 138 elemen
- Langkah 4: Sisa populasi tebasan separuh = 69 elemen
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
**Soal 72**
Pak Dengklek memiliki daftar absensi **1410 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 12 langkah
C. 13 langkah
D. 11 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: D (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1410 elemen
- Langkah 1: Sisa populasi tebasan separuh = 705 elemen
- Langkah 2: Sisa populasi tebasan separuh = 353 elemen
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
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 73**
Diberikan barisan angka: `[84, 75, 43, 22, 58]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [22, 75, 58, 84, 43]
B. [84, 43, 22, 75, 58]
C. [75, 43, 22, 58, 84]
D. [43, 75, 22, 58, 84]
E. [22, 84, 58, 43, 75]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([75, 43, 22, 58, 84])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[84, 75, 43, 22, 58]`
Cek posisi 0&1 (84 > 75) -> Tukar! Array kini: `[75, 84, 43, 22, 58]`
Cek posisi 1&2 (84 > 43) -> Tukar! Array kini: `[75, 43, 84, 22, 58]`
Cek posisi 2&3 (84 > 22) -> Tukar! Array kini: `[75, 43, 22, 84, 58]`
Cek posisi 3&4 (84 > 58) -> Tukar! Array kini: `[75, 43, 22, 58, 84]`


Terbukti bahwa elemen maha gemuk (`84`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[75, 43, 22, 58, 84]**.
</details>

---
**Soal 74**
Pak Dengklek memiliki daftar absensi **1332 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 11 langkah
C. 12 langkah
D. 14 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: B (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1332 elemen
- Langkah 1: Sisa populasi tebasan separuh = 666 elemen
- Langkah 2: Sisa populasi tebasan separuh = 333 elemen
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
**Soal 75**
Diberikan barisan angka: `[79, 91, 38, 85, 46]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [79, 38, 46, 85, 91]
B. [46, 91, 79, 38, 85]
C. [91, 79, 85, 46, 38]
D. [46, 79, 38, 91, 85]
E. [79, 38, 85, 46, 91]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: E ([79, 38, 85, 46, 91])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[79, 91, 38, 85, 46]`
Cek posisi 0&1 (79 < 91) -> Aman dibiarkan. Array kini: `[79, 91, 38, 85, 46]`
Cek posisi 1&2 (91 > 38) -> Tukar! Array kini: `[79, 38, 91, 85, 46]`
Cek posisi 2&3 (91 > 85) -> Tukar! Array kini: `[79, 38, 85, 91, 46]`
Cek posisi 3&4 (91 > 46) -> Tukar! Array kini: `[79, 38, 85, 46, 91]`


Terbukti bahwa elemen maha gemuk (`91`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[79, 38, 85, 46, 91]**.
</details>

---
**Soal 76**
Pak Dengklek memiliki daftar absensi **857 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 11 langkah
D. 9 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 857 elemen
- Langkah 1: Sisa populasi tebasan separuh = 429 elemen
- Langkah 2: Sisa populasi tebasan separuh = 215 elemen
- Langkah 3: Sisa populasi tebasan separuh = 108 elemen
- Langkah 4: Sisa populasi tebasan separuh = 54 elemen
- Langkah 5: Sisa populasi tebasan separuh = 27 elemen
- Langkah 6: Sisa populasi tebasan separuh = 14 elemen
- Langkah 7: Sisa populasi tebasan separuh = 7 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 77**
Bebek-bebek di barisan bernomor dada: `[78, 76, 57, 96, 63, 46]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [96, 63, 46, 78, 76, 57]
B. [76, 46, 78, 57, 63, 96]
C. [46, 57, 96, 78, 76, 63]
D. [46, 57, 76, 96, 63, 78]
E. [96, 46, 76, 57, 63, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([46, 57, 76, 96, 63, 78])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[78, 76, 57, 96, 63, 46]`
- Putaran 1: Cari anak terpecebol di area sisa [46, 76, 57, 96, 63, 78]. Ditemukan si `46`. Tukar paksa dudukan dengan `78`. Array mutasi -> `[46, 76, 57, 96, 63, 78]`
- Putaran 2: Cari anak terpecebol di area sisa [57, 76, 96, 63, 78]. Ditemukan si `57`. Tukar paksa dudukan dengan `76`. Array mutasi -> `[46, 57, 76, 96, 63, 78]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[46, 57, 76, 96, 63, 78]**. Opsi murni: **D**.
</details>

---
**Soal 78**
Pak Dengklek memiliki daftar absensi **953 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 9 langkah
B. 12 langkah
C. 11 langkah
D. 13 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 953 elemen
- Langkah 1: Sisa populasi tebasan separuh = 477 elemen
- Langkah 2: Sisa populasi tebasan separuh = 239 elemen
- Langkah 3: Sisa populasi tebasan separuh = 120 elemen
- Langkah 4: Sisa populasi tebasan separuh = 60 elemen
- Langkah 5: Sisa populasi tebasan separuh = 30 elemen
- Langkah 6: Sisa populasi tebasan separuh = 15 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 79**
Pak Dengklek memiliki daftar absensi **937 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 10 langkah
B. 12 langkah
C. 11 langkah
D. 13 langkah
E. 9 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: A (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 937 elemen
- Langkah 1: Sisa populasi tebasan separuh = 469 elemen
- Langkah 2: Sisa populasi tebasan separuh = 235 elemen
- Langkah 3: Sisa populasi tebasan separuh = 118 elemen
- Langkah 4: Sisa populasi tebasan separuh = 59 elemen
- Langkah 5: Sisa populasi tebasan separuh = 30 elemen
- Langkah 6: Sisa populasi tebasan separuh = 15 elemen
- Langkah 7: Sisa populasi tebasan separuh = 8 elemen
- Langkah 8: Sisa populasi tebasan separuh = 4 elemen
- Langkah 9: Sisa populasi tebasan separuh = 2 elemen
- Langkah 10: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **10 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **A**.</details>

---
**Soal 80**
Diberikan barisan angka: `[44, 59, 67, 76, 95]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [44, 59, 67, 76, 95]
B. [76, 44, 95, 59, 67]
C. [76, 67, 95, 44, 59]
D. [67, 95, 76, 44, 59]
E. [67, 59, 44, 76, 95]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: A ([44, 59, 67, 76, 95])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[44, 59, 67, 76, 95]`
Cek posisi 0&1 (44 < 59) -> Aman dibiarkan. Array kini: `[44, 59, 67, 76, 95]`
Cek posisi 1&2 (59 < 67) -> Aman dibiarkan. Array kini: `[44, 59, 67, 76, 95]`
Cek posisi 2&3 (67 < 76) -> Aman dibiarkan. Array kini: `[44, 59, 67, 76, 95]`
Cek posisi 3&4 (76 < 95) -> Aman dibiarkan. Array kini: `[44, 59, 67, 76, 95]`


Terbukti bahwa elemen maha gemuk (`95`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[44, 59, 67, 76, 95]**.
</details>

---
**Soal 81**
Diberikan barisan angka: `[53, 72, 80, 63, 84]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [63, 72, 84, 80, 53]
B. [80, 63, 72, 84, 53]
C. [63, 80, 72, 53, 84]
D. [53, 72, 63, 80, 84]
E. [63, 80, 53, 72, 84]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([53, 72, 63, 80, 84])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[53, 72, 80, 63, 84]`
Cek posisi 0&1 (53 < 72) -> Aman dibiarkan. Array kini: `[53, 72, 80, 63, 84]`
Cek posisi 1&2 (72 < 80) -> Aman dibiarkan. Array kini: `[53, 72, 80, 63, 84]`
Cek posisi 2&3 (80 > 63) -> Tukar! Array kini: `[53, 72, 63, 80, 84]`
Cek posisi 3&4 (80 < 84) -> Aman dibiarkan. Array kini: `[53, 72, 63, 80, 84]`


Terbukti bahwa elemen maha gemuk (`84`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[53, 72, 63, 80, 84]**.
</details>

---
**Soal 82**
Bebek-bebek di barisan bernomor dada: `[32, 95, 97, 63, 28, 82]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [82, 28, 63, 32, 95, 97]
B. [28, 32, 97, 63, 95, 82]
C. [32, 95, 97, 63, 28, 82]
D. [95, 32, 28, 82, 97, 63]
E. [82, 97, 95, 32, 63, 28]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([28, 32, 97, 63, 95, 82])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[32, 95, 97, 63, 28, 82]`
- Putaran 1: Cari anak terpecebol di area sisa [28, 95, 97, 63, 32, 82]. Ditemukan si `28`. Tukar paksa dudukan dengan `32`. Array mutasi -> `[28, 95, 97, 63, 32, 82]`
- Putaran 2: Cari anak terpecebol di area sisa [32, 97, 63, 95, 82]. Ditemukan si `32`. Tukar paksa dudukan dengan `95`. Array mutasi -> `[28, 32, 97, 63, 95, 82]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[28, 32, 97, 63, 95, 82]**. Opsi murni: **B**.
</details>

---
**Soal 83**
Bebek-bebek di barisan bernomor dada: `[54, 14, 90, 66, 85, 25]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [85, 14, 90, 25, 54, 66]
B. [14, 25, 90, 66, 85, 54]
C. [85, 66, 90, 25, 14, 54]
D. [85, 90, 25, 14, 54, 66]
E. [66, 14, 25, 90, 54, 85]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: B ([14, 25, 90, 66, 85, 54])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[54, 14, 90, 66, 85, 25]`
- Putaran 1: Cari anak terpecebol di area sisa [14, 54, 90, 66, 85, 25]. Ditemukan si `14`. Tukar paksa dudukan dengan `54`. Array mutasi -> `[14, 54, 90, 66, 85, 25]`
- Putaran 2: Cari anak terpecebol di area sisa [25, 90, 66, 85, 54]. Ditemukan si `25`. Tukar paksa dudukan dengan `54`. Array mutasi -> `[14, 25, 90, 66, 85, 54]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[14, 25, 90, 66, 85, 54]**. Opsi murni: **B**.
</details>

---
**Soal 84**
Pak Dengklek memiliki daftar absensi **1883 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1883 elemen
- Langkah 1: Sisa populasi tebasan separuh = 942 elemen
- Langkah 2: Sisa populasi tebasan separuh = 471 elemen
- Langkah 3: Sisa populasi tebasan separuh = 236 elemen
- Langkah 4: Sisa populasi tebasan separuh = 118 elemen
- Langkah 5: Sisa populasi tebasan separuh = 59 elemen
- Langkah 6: Sisa populasi tebasan separuh = 30 elemen
- Langkah 7: Sisa populasi tebasan separuh = 15 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **D**.</details>

---
**Soal 85**
Diberikan barisan angka: `[84, 75, 76, 82, 69]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [69, 75, 84, 82, 76]
B. [69, 84, 75, 76, 82]
C. [75, 76, 82, 69, 84]
D. [84, 76, 75, 69, 82]
E. [76, 69, 82, 84, 75]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([75, 76, 82, 69, 84])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[84, 75, 76, 82, 69]`
Cek posisi 0&1 (84 > 75) -> Tukar! Array kini: `[75, 84, 76, 82, 69]`
Cek posisi 1&2 (84 > 76) -> Tukar! Array kini: `[75, 76, 84, 82, 69]`
Cek posisi 2&3 (84 > 82) -> Tukar! Array kini: `[75, 76, 82, 84, 69]`
Cek posisi 3&4 (84 > 69) -> Tukar! Array kini: `[75, 76, 82, 69, 84]`


Terbukti bahwa elemen maha gemuk (`84`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[75, 76, 82, 69, 84]**.
</details>

---
**Soal 86**
Bebek-bebek di barisan bernomor dada: `[98, 53, 74, 46, 69, 33]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [74, 53, 69, 98, 46, 33]
B. [98, 69, 53, 74, 33, 46]
C. [53, 69, 33, 46, 98, 74]
D. [33, 46, 74, 53, 69, 98]
E. [98, 46, 53, 74, 33, 69]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: D ([33, 46, 74, 53, 69, 98])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[98, 53, 74, 46, 69, 33]`
- Putaran 1: Cari anak terpecebol di area sisa [33, 53, 74, 46, 69, 98]. Ditemukan si `33`. Tukar paksa dudukan dengan `98`. Array mutasi -> `[33, 53, 74, 46, 69, 98]`
- Putaran 2: Cari anak terpecebol di area sisa [46, 74, 53, 69, 98]. Ditemukan si `46`. Tukar paksa dudukan dengan `53`. Array mutasi -> `[33, 46, 74, 53, 69, 98]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[33, 46, 74, 53, 69, 98]**. Opsi murni: **D**.
</details>

---
**Soal 87**
Pak Dengklek memiliki daftar absensi **1620 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 14 langkah
C. 11 langkah
D. 10 langkah
E. 13 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: C (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1620 elemen
- Langkah 1: Sisa populasi tebasan separuh = 810 elemen
- Langkah 2: Sisa populasi tebasan separuh = 405 elemen
- Langkah 3: Sisa populasi tebasan separuh = 203 elemen
- Langkah 4: Sisa populasi tebasan separuh = 102 elemen
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
**Soal 88**
Diberikan barisan angka: `[63, 40, 97, 90, 24]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [90, 97, 40, 63, 24]
B. [40, 63, 24, 97, 90]
C. [63, 90, 97, 24, 40]
D. [40, 63, 90, 24, 97]
E. [90, 97, 24, 40, 63]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([40, 63, 90, 24, 97])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[63, 40, 97, 90, 24]`
Cek posisi 0&1 (63 > 40) -> Tukar! Array kini: `[40, 63, 97, 90, 24]`
Cek posisi 1&2 (63 < 97) -> Aman dibiarkan. Array kini: `[40, 63, 97, 90, 24]`
Cek posisi 2&3 (97 > 90) -> Tukar! Array kini: `[40, 63, 90, 97, 24]`
Cek posisi 3&4 (97 > 24) -> Tukar! Array kini: `[40, 63, 90, 24, 97]`


Terbukti bahwa elemen maha gemuk (`97`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[40, 63, 90, 24, 97]**.
</details>

---
**Soal 89**
Pak Dengklek memiliki daftar absensi **1817 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 14 langkah
B. 12 langkah
C. 10 langkah
D. 13 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1817 elemen
- Langkah 1: Sisa populasi tebasan separuh = 909 elemen
- Langkah 2: Sisa populasi tebasan separuh = 455 elemen
- Langkah 3: Sisa populasi tebasan separuh = 228 elemen
- Langkah 4: Sisa populasi tebasan separuh = 114 elemen
- Langkah 5: Sisa populasi tebasan separuh = 57 elemen
- Langkah 6: Sisa populasi tebasan separuh = 29 elemen
- Langkah 7: Sisa populasi tebasan separuh = 15 elemen
- Langkah 8: Sisa populasi tebasan separuh = 8 elemen
- Langkah 9: Sisa populasi tebasan separuh = 4 elemen
- Langkah 10: Sisa populasi tebasan separuh = 2 elemen
- Langkah 11: Sisa populasi tebasan separuh = 1 elemen

Dalam maksimal **11 langkah** penebasan, area kandidat menyusut menjadi $\le 1$ elemen (entah ketemu tepat atau divonis tidak ada). 
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 90**
Diberikan barisan angka: `[49, 73, 21, 33, 28]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [21, 33, 28, 49, 73]
B. [49, 73, 33, 21, 28]
C. [33, 49, 28, 21, 73]
D. [49, 21, 33, 28, 73]
E. [33, 21, 49, 28, 73]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([49, 21, 33, 28, 73])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[49, 73, 21, 33, 28]`
Cek posisi 0&1 (49 < 73) -> Aman dibiarkan. Array kini: `[49, 73, 21, 33, 28]`
Cek posisi 1&2 (73 > 21) -> Tukar! Array kini: `[49, 21, 73, 33, 28]`
Cek posisi 2&3 (73 > 33) -> Tukar! Array kini: `[49, 21, 33, 73, 28]`
Cek posisi 3&4 (73 > 28) -> Tukar! Array kini: `[49, 21, 33, 28, 73]`


Terbukti bahwa elemen maha gemuk (`73`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[49, 21, 33, 28, 73]**.
</details>

---
**Soal 91**
Bebek-bebek di barisan bernomor dada: `[64, 86, 56, 45, 36, 53]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [64, 86, 45, 36, 56, 53]
B. [53, 45, 56, 36, 86, 64]
C. [36, 45, 56, 86, 64, 53]
D. [36, 45, 56, 53, 64, 86]
E. [64, 53, 45, 56, 86, 36]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: C ([36, 45, 56, 86, 64, 53])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[64, 86, 56, 45, 36, 53]`
- Putaran 1: Cari anak terpecebol di area sisa [36, 86, 56, 45, 64, 53]. Ditemukan si `36`. Tukar paksa dudukan dengan `64`. Array mutasi -> `[36, 86, 56, 45, 64, 53]`
- Putaran 2: Cari anak terpecebol di area sisa [45, 56, 86, 64, 53]. Ditemukan si `45`. Tukar paksa dudukan dengan `86`. Array mutasi -> `[36, 45, 56, 86, 64, 53]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[36, 45, 56, 86, 64, 53]**. Opsi murni: **C**.
</details>

---
**Soal 92**
Pak Dengklek memiliki daftar absensi **993 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 13 langkah
B. 12 langkah
C. 11 langkah
D. 9 langkah
E. 10 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (10 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 993 elemen
- Langkah 1: Sisa populasi tebasan separuh = 497 elemen
- Langkah 2: Sisa populasi tebasan separuh = 249 elemen
- Langkah 3: Sisa populasi tebasan separuh = 125 elemen
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
**Soal 93**
Pak Dengklek memiliki daftar absensi **1944 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
Ia menggunakan metode **Binary Search (Pencarian Lipat Dua)** untuk mencari nama "Kwang Soo". 

Berapa maksimal pertanyaan/langkah pengecekan (pembelahan sisa daftar) paling sial / Kasus Terburuk (Worst-case) yang harus dilalui Pak Dengklek sebelum menyerah atau menemukan nama tersebut?

A. 12 langkah
B. 10 langkah
C. 13 langkah
D. 14 langkah
E. 11 langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Diagnosis O(log N)</b></summary>

**Jawaban: E (11 langkah)**

**Pembahasan (Mengiris Ruang Pencarian):**
Metode Binary Search adalah sihir dengan time complexity $O(\log_2 N)$. Ia selalu menebas ruang pencarian tepat di tengah.
Simulasi ukuran sisa daftar yang dipertahankan:
- Langkah 0: Mula-mula 1944 elemen
- Langkah 1: Sisa populasi tebasan separuh = 972 elemen
- Langkah 2: Sisa populasi tebasan separuh = 486 elemen
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
Oleh karena itu opsi valid mutlak adalah **E**.</details>

---
**Soal 94**
Diberikan barisan angka: `[78, 97, 42, 55, 17]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [55, 78, 17, 97, 42]
B. [55, 42, 97, 78, 17]
C. [97, 78, 17, 42, 55]
D. [78, 42, 55, 17, 97]
E. [55, 42, 97, 17, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([78, 42, 55, 17, 97])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[78, 97, 42, 55, 17]`
Cek posisi 0&1 (78 < 97) -> Aman dibiarkan. Array kini: `[78, 97, 42, 55, 17]`
Cek posisi 1&2 (97 > 42) -> Tukar! Array kini: `[78, 42, 97, 55, 17]`
Cek posisi 2&3 (97 > 55) -> Tukar! Array kini: `[78, 42, 55, 97, 17]`
Cek posisi 3&4 (97 > 17) -> Tukar! Array kini: `[78, 42, 55, 17, 97]`


Terbukti bahwa elemen maha gemuk (`97`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[78, 42, 55, 17, 97]**.
</details>

---
**Soal 95**
Pak Dengklek memiliki daftar absensi **1555 siswa** yang namanya sudah diurutkan sesuai abjad A-Z. 
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
- Langkah 0: Mula-mula 1555 elemen
- Langkah 1: Sisa populasi tebasan separuh = 778 elemen
- Langkah 2: Sisa populasi tebasan separuh = 389 elemen
- Langkah 3: Sisa populasi tebasan separuh = 195 elemen
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
**Soal 96**
Bebek-bebek di barisan bernomor dada: `[68, 48, 52, 69, 21, 84]` akan dioperasi penyetaraan sosial.
Pak RT tiba dan memerintahkan baris-berbaris diurutkan mutlak menggunakan sistem **Selection Sort Asli (Cari Si Paling Miskin Dulu)** secara Mendaki (Ascending).

Susunan anatomi array yang terbentuk tepat setelah **Putaran Utama Ke-2** diselesaikan adalah?

A. [48, 69, 52, 21, 68, 84]
B. [69, 52, 21, 84, 48, 68]
C. [84, 52, 69, 68, 48, 21]
D. [69, 52, 48, 68, 21, 84]
E. [21, 48, 52, 69, 68, 84]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Pemilihan Elite</b></summary>

**Jawaban: E ([21, 48, 52, 69, 68, 84])**

**Pembahasan (Simulasi Cengkeraman Pak RT dari Kiri):**
Falsafah Selection Sort adalah mengunci stabilitas dari SAYAP KIRI. Jika setelah 2 Putaran utama kelar, artinya 100% dua anak bernomor dada paling kecil sebangsa raya harus sudah anteng abadi duduk di 2 kursi deret Kiri terbuntut batas.

Mari Tracing di Kertas:
Array Start: `[68, 48, 52, 69, 21, 84]`
- Putaran 1: Cari anak terpecebol di area sisa [21, 48, 52, 69, 68, 84]. Ditemukan si `21`. Tukar paksa dudukan dengan `68`. Array mutasi -> `[21, 48, 52, 69, 68, 84]`
- Putaran 2: Cari anak terpecebol di area sisa [48, 52, 69, 68, 84]. Ditemukan si `48`. Tukar paksa dudukan dengan `48`. Array mutasi -> `[21, 48, 52, 69, 68, 84]`


Terbukti, sayap kiri sudah kokoh merangkap kasta dua elemen cebol. Susunan jepretan final untuk putaran keduannya pas adalah **[21, 48, 52, 69, 68, 84]**. Opsi murni: **E**.
</details>

---
**Soal 97**
Diberikan barisan angka: `[41, 78, 28, 71, 91]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [28, 78, 91, 71, 41]
B. [41, 28, 71, 78, 91]
C. [78, 28, 91, 71, 41]
D. [91, 41, 71, 28, 78]
E. [71, 28, 91, 41, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([41, 28, 71, 78, 91])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[41, 78, 28, 71, 91]`
Cek posisi 0&1 (41 < 78) -> Aman dibiarkan. Array kini: `[41, 78, 28, 71, 91]`
Cek posisi 1&2 (78 > 28) -> Tukar! Array kini: `[41, 28, 78, 71, 91]`
Cek posisi 2&3 (78 > 71) -> Tukar! Array kini: `[41, 28, 71, 78, 91]`
Cek posisi 3&4 (78 < 91) -> Aman dibiarkan. Array kini: `[41, 28, 71, 78, 91]`


Terbukti bahwa elemen maha gemuk (`91`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[41, 28, 71, 78, 91]**.
</details>

---
**Soal 98**
Diberikan barisan angka: `[52, 62, 19, 78, 82]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [52, 78, 82, 19, 62]
B. [52, 19, 82, 62, 78]
C. [52, 19, 62, 78, 82]
D. [52, 62, 78, 19, 82]
E. [82, 62, 19, 52, 78]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: C ([52, 19, 62, 78, 82])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[52, 62, 19, 78, 82]`
Cek posisi 0&1 (52 < 62) -> Aman dibiarkan. Array kini: `[52, 62, 19, 78, 82]`
Cek posisi 1&2 (62 > 19) -> Tukar! Array kini: `[52, 19, 62, 78, 82]`
Cek posisi 2&3 (62 < 78) -> Aman dibiarkan. Array kini: `[52, 19, 62, 78, 82]`
Cek posisi 3&4 (78 < 82) -> Aman dibiarkan. Array kini: `[52, 19, 62, 78, 82]`


Terbukti bahwa elemen maha gemuk (`82`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[52, 19, 62, 78, 82]**.
</details>

---
**Soal 99**
Diberikan barisan angka: `[19, 74, 62, 66, 13]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [19, 13, 66, 62, 74]
B. [19, 62, 66, 13, 74]
C. [62, 74, 66, 13, 19]
D. [19, 62, 13, 66, 74]
E. [62, 74, 19, 66, 13]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: B ([19, 62, 66, 13, 74])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[19, 74, 62, 66, 13]`
Cek posisi 0&1 (19 < 74) -> Aman dibiarkan. Array kini: `[19, 74, 62, 66, 13]`
Cek posisi 1&2 (74 > 62) -> Tukar! Array kini: `[19, 62, 74, 66, 13]`
Cek posisi 2&3 (74 > 66) -> Tukar! Array kini: `[19, 62, 66, 74, 13]`
Cek posisi 3&4 (74 > 13) -> Tukar! Array kini: `[19, 62, 66, 13, 74]`


Terbukti bahwa elemen maha gemuk (`74`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[19, 62, 66, 13, 74]**.
</details>

---
**Soal 100**
Diberikan barisan angka: `[98, 25, 11, 27, 10]`.
Guru BP berteriak menyuruh barisan ini diurutkan dari KECIL ke BESAR menggunakan algoritma **Bubble Sort Asli (Gelembung Naik)**.

Bagaimanakah konfigurasi urutan barisan ini TEPAT SETELAH PUTARAN UTAMA PERTAMA (Iterasi Garis Terluar / *Outer Pass 1*) diselesaikan secara paripurna?

A. [98, 11, 27, 25, 10]
B. [11, 10, 27, 98, 25]
C. [27, 10, 98, 25, 11]
D. [25, 11, 27, 10, 98]
E. [25, 11, 27, 98, 10]

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Gelembung</b></summary>

**Jawaban: D ([25, 11, 27, 10, 98])**

**Pembahasan (Simulasi Hukum Pukul Geser Kanan):**
Sifat murni Bubble Sort Pass Pertama adalah menggelembungkan satu elemen TERBESAR agar tergusur sampai pojok kanan mentok.
Membedah langkah *Tracing* Pak Guru BP:
Array awal: `[98, 25, 11, 27, 10]`
Cek posisi 0&1 (98 > 25) -> Tukar! Array kini: `[25, 98, 11, 27, 10]`
Cek posisi 1&2 (98 > 11) -> Tukar! Array kini: `[25, 11, 98, 27, 10]`
Cek posisi 2&3 (98 > 27) -> Tukar! Array kini: `[25, 11, 27, 98, 10]`
Cek posisi 3&4 (98 > 10) -> Tukar! Array kini: `[25, 11, 27, 10, 98]`


Terbukti bahwa elemen maha gemuk (`98`) akhirnya sudah bersandar kaku di ujung paling kanan arena. 
Sehingga bentuk final di ujung Putaran-1 adalah tepat **[25, 11, 27, 10, 98]**.
</details>

---
