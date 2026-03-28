# 11. Bedah Soal Bebras CAPSTONE - Latihan Soal Bagian 3
## Topik Utama: Wujud Asli HIMPUNAN & BOOLEAN (Diagram & Logika Ganda)

> **Misi Anda**: Jangan buang waktu menggambar manual layaknya anak SD. Gunakan ilmu rahasia Teori Himpunan, Graf, atau Kombinatorika untuk MEMBEDAH wujud asli manipulasi skenario soal-soal ini!

[< Bagian 2](./11-bedah-bebras-part-2.md) | [Bagian 4 >](./11-bedah-bebras-part-4.md)

---

### Soal #41: Kasus Aplikasi Himpunan & Boolean Visual
**Klasifikasi Bentuk Kelereng Bebras**
Keluarga Bebras sedang meneliti 68 bongkah batu koleksi di sungai. Mesin pemindai mereka mengeluarkan lampu indikator mendeteksi bahwa 35 batu ternyata memiliki kilau mineral Emas (E). Di satu sisi, pemindai menyala hijau 1 kali ke 40 batu yang mengandung kadar Besi (B) asli. Namun, si bungsu tidak sengaja merusak perhitungan karena mencelupkan 5 batu (kembar E dan B) ke dalam cat minyak yang menutupi kilaunya.

Berapa batu polos di sungai yang sifatnya benar-benar cuma batu gunung tanpa emas maupun besi sama sekali berdasarkan laporan alat tes tersebut?

A. -2
B. 75
C. 63
D. 3
E. -7


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Diagram Venn Inklusi-Eksklusi / Selisih Luar Lingkaran**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. -2**

**Pembahasan Algoritma (Diagnonis: Teori Himpunan / Diagram Venn)**

1. Pemula akan menggambar batu satu-satu.
2. Para Juara memandangnya sebagai Diagram Venn 2 Lingkaran Biasa!
   - Semesta ($S$) = 68 batu
   - Suka/Kena Emas ($A$) = 35 batu
   - Suka/Kena Besi ($B$) = 40 batu
   - Kena irisan Keduanya ($A \cap B$) = 5 batu yang kerendam cat.
3. Pertanyaan aslinya adalah pencarian **Wilayah Komplemen Gabungan (Pinggiran Rumput Luar) / $(A \cup B)^c$**.
4. Hitung Gabungan Utuh Batu Berharga: $A + B - Irisan = 35 + 40 - 5 = 70$ batu gabungan.
5. Yang Buntung Tanpa Unsur (Polos Luaran): $Semesta - Gabungan = 68 - 70 =$ **-2 batu murni**.

</details>

### Soal #42: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 26 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 4 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Bulu Lebat` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Bulu Lebat)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 18
B. 104
C. 30
D. 26
E. 22


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 22**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (26)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 4$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $26 - 4 =$ **22 kandidat berdarah suci**.

</details>

### Soal #43: Kasus Aplikasi Himpunan & Boolean Visual
**Klasifikasi Bentuk Kelereng Bebras**
Keluarga Bebras sedang meneliti 76 bongkah batu koleksi di sungai. Mesin pemindai mereka mengeluarkan lampu indikator mendeteksi bahwa 30 batu ternyata memiliki kilau mineral Emas (E). Di satu sisi, pemindai menyala hijau 1 kali ke 39 batu yang mengandung kadar Besi (B) asli. Namun, si bungsu tidak sengaja merusak perhitungan karena mencelupkan 5 batu (kembar E dan B) ke dalam cat minyak yang menutupi kilaunya.

Berapa batu polos di sungai yang sifatnya benar-benar cuma batu gunung tanpa emas maupun besi sama sekali berdasarkan laporan alat tes tersebut?

A. 7
B. 12
C. 69
D. 17
E. 71


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Diagram Venn Inklusi-Eksklusi / Selisih Luar Lingkaran**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 12**

**Pembahasan Algoritma (Diagnonis: Teori Himpunan / Diagram Venn)**

1. Pemula akan menggambar batu satu-satu.
2. Para Juara memandangnya sebagai Diagram Venn 2 Lingkaran Biasa!
   - Semesta ($S$) = 76 batu
   - Suka/Kena Emas ($A$) = 30 batu
   - Suka/Kena Besi ($B$) = 39 batu
   - Kena irisan Keduanya ($A \cap B$) = 5 batu yang kerendam cat.
3. Pertanyaan aslinya adalah pencarian **Wilayah Komplemen Gabungan (Pinggiran Rumput Luar) / $(A \cup B)^c$**.
4. Hitung Gabungan Utuh Batu Berharga: $A + B - Irisan = 30 + 39 - 5 = 64$ batu gabungan.
5. Yang Buntung Tanpa Unsur (Polos Luaran): $Semesta - Gabungan = 76 - 64 =$ **12 batu murni**.

</details>

### Soal #44: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Robot X Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Robot X malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.
B. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan
C. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
D. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.
E. Bawa Otorisasi ATAU Cepat saja.


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #45: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 33 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 10 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Taring Tajam` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Taring Tajam)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 13
B. 43
C. 33
D. 330
E. 23


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 23**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (33)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 10$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $33 - 10 =$ **23 kandidat berdarah suci**.

</details>

### Soal #46: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 26 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 4 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Mata Hijau` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Mata Hijau)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 22
B. 26
C. 30
D. 18
E. 104


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 22**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (26)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 4$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $26 - 4 =$ **22 kandidat berdarah suci**.

</details>

### Soal #47: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Robot X Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Robot X malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. Bawa Otorisasi ATAU Cepat saja.
B. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
C. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.
D. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.
E. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #48: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Sistem Omega Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Sistem Omega malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.
B. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
C. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.
D. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan
E. Bawa Otorisasi ATAU Cepat saja.


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #49: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 21 alien mini yang memiliki DNA `Kumis Panjang`. Tapi usut punya usut, ada mutan ganda, yakni 5 alien dari rombongan `Kumis Panjang` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Mata Hijau` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Kumis Panjang` saja (Benci banget sama tipe Mata Hijau)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 21
B. 16
C. 105
D. 26
E. 11


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 16**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (21)$ Alien bertipe Kumis Panjang.
   - Angka irisan persilangan $(A \cap B) = 5$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $21 - 5 =$ **16 kandidat berdarah suci**.

</details>

### Soal #50: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 24 alien mini yang memiliki DNA `Kumis Panjang`. Tapi usut punya usut, ada mutan ganda, yakni 9 alien dari rombongan `Kumis Panjang` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Bulu Lebat` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Kumis Panjang` saja (Benci banget sama tipe Bulu Lebat)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 15
B. 216
C. 6
D. 24
E. 33


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 15**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (24)$ Alien bertipe Kumis Panjang.
   - Angka irisan persilangan $(A \cap B) = 9$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $24 - 9 =$ **15 kandidat berdarah suci**.

</details>

### Soal #51: Kasus Aplikasi Himpunan & Boolean Visual
**Klasifikasi Bentuk Kelereng Bebras**
Keluarga Bebras sedang meneliti 72 bongkah batu koleksi di sungai. Mesin pemindai mereka mengeluarkan lampu indikator mendeteksi bahwa 40 batu ternyata memiliki kilau mineral Emas (E). Di satu sisi, pemindai menyala hijau 1 kali ke 39 batu yang mengandung kadar Besi (B) asli. Namun, si bungsu tidak sengaja merusak perhitungan karena mencelupkan 11 batu (kembar E dan B) ke dalam cat minyak yang menutupi kilaunya.

Berapa batu polos di sungai yang sifatnya benar-benar cuma batu gunung tanpa emas maupun besi sama sekali berdasarkan laporan alat tes tersebut?

A. 79
B. 15
C. 61
D. 4
E. -7


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Diagram Venn Inklusi-Eksklusi / Selisih Luar Lingkaran**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. 4**

**Pembahasan Algoritma (Diagnonis: Teori Himpunan / Diagram Venn)**

1. Pemula akan menggambar batu satu-satu.
2. Para Juara memandangnya sebagai Diagram Venn 2 Lingkaran Biasa!
   - Semesta ($S$) = 72 batu
   - Suka/Kena Emas ($A$) = 40 batu
   - Suka/Kena Besi ($B$) = 39 batu
   - Kena irisan Keduanya ($A \cap B$) = 11 batu yang kerendam cat.
3. Pertanyaan aslinya adalah pencarian **Wilayah Komplemen Gabungan (Pinggiran Rumput Luar) / $(A \cup B)^c$**.
4. Hitung Gabungan Utuh Batu Berharga: $A + B - Irisan = 40 + 39 - 11 = 68$ batu gabungan.
5. Yang Buntung Tanpa Unsur (Polos Luaran): $Semesta - Gabungan = 72 - 68 =$ **4 batu murni**.

</details>

### Soal #52: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Robot X Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Robot X malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.
B. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan
C. Bawa Otorisasi ATAU Cepat saja.
D. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
E. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #53: Kasus Aplikasi Himpunan & Boolean Visual
**Klasifikasi Bentuk Kelereng Bebras**
Keluarga Bebras sedang meneliti 66 bongkah batu koleksi di sungai. Mesin pemindai mereka mengeluarkan lampu indikator mendeteksi bahwa 36 batu ternyata memiliki kilau mineral Emas (E). Di satu sisi, pemindai menyala hijau 1 kali ke 28 batu yang mengandung kadar Besi (B) asli. Namun, si bungsu tidak sengaja merusak perhitungan karena mencelupkan 15 batu (kembar E dan B) ke dalam cat minyak yang menutupi kilaunya.

Berapa batu polos di sungai yang sifatnya benar-benar cuma batu gunung tanpa emas maupun besi sama sekali berdasarkan laporan alat tes tersebut?

A. 2
B. 17
C. 32
D. 64
E. 51


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Diagram Venn Inklusi-Eksklusi / Selisih Luar Lingkaran**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 17**

**Pembahasan Algoritma (Diagnonis: Teori Himpunan / Diagram Venn)**

1. Pemula akan menggambar batu satu-satu.
2. Para Juara memandangnya sebagai Diagram Venn 2 Lingkaran Biasa!
   - Semesta ($S$) = 66 batu
   - Suka/Kena Emas ($A$) = 36 batu
   - Suka/Kena Besi ($B$) = 28 batu
   - Kena irisan Keduanya ($A \cap B$) = 15 batu yang kerendam cat.
3. Pertanyaan aslinya adalah pencarian **Wilayah Komplemen Gabungan (Pinggiran Rumput Luar) / $(A \cup B)^c$**.
4. Hitung Gabungan Utuh Batu Berharga: $A + B - Irisan = 36 + 28 - 15 = 49$ batu gabungan.
5. Yang Buntung Tanpa Unsur (Polos Luaran): $Semesta - Gabungan = 66 - 49 =$ **17 batu murni**.

</details>

### Soal #54: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Drone Z Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Drone Z malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan
B. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.
C. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.
D. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
E. Bawa Otorisasi ATAU Cepat saja.


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #55: Kasus Aplikasi Himpunan & Boolean Visual
**Klasifikasi Bentuk Kelereng Bebras**
Keluarga Bebras sedang meneliti 55 bongkah batu koleksi di sungai. Mesin pemindai mereka mengeluarkan lampu indikator mendeteksi bahwa 32 batu ternyata memiliki kilau mineral Emas (E). Di satu sisi, pemindai menyala hijau 1 kali ke 39 batu yang mengandung kadar Besi (B) asli. Namun, si bungsu tidak sengaja merusak perhitungan karena mencelupkan 11 batu (kembar E dan B) ke dalam cat minyak yang menutupi kilaunya.

Berapa batu polos di sungai yang sifatnya benar-benar cuma batu gunung tanpa emas maupun besi sama sekali berdasarkan laporan alat tes tersebut?

A. 6
B. -16
C. 71
D. -5
E. 44


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Diagram Venn Inklusi-Eksklusi / Selisih Luar Lingkaran**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. -5**

**Pembahasan Algoritma (Diagnonis: Teori Himpunan / Diagram Venn)**

1. Pemula akan menggambar batu satu-satu.
2. Para Juara memandangnya sebagai Diagram Venn 2 Lingkaran Biasa!
   - Semesta ($S$) = 55 batu
   - Suka/Kena Emas ($A$) = 32 batu
   - Suka/Kena Besi ($B$) = 39 batu
   - Kena irisan Keduanya ($A \cap B$) = 11 batu yang kerendam cat.
3. Pertanyaan aslinya adalah pencarian **Wilayah Komplemen Gabungan (Pinggiran Rumput Luar) / $(A \cup B)^c$**.
4. Hitung Gabungan Utuh Batu Berharga: $A + B - Irisan = 32 + 39 - 11 = 60$ batu gabungan.
5. Yang Buntung Tanpa Unsur (Polos Luaran): $Semesta - Gabungan = 55 - 60 =$ **-5 batu murni**.

</details>

### Soal #56: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 20 alien mini yang memiliki DNA `Kumis Panjang`. Tapi usut punya usut, ada mutan ganda, yakni 4 alien dari rombongan `Kumis Panjang` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Mata Hijau` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Kumis Panjang` saja (Benci banget sama tipe Mata Hijau)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 12
B. 16
C. 24
D. 20
E. 80


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 16**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (20)$ Alien bertipe Kumis Panjang.
   - Angka irisan persilangan $(A \cap B) = 4$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $20 - 4 =$ **16 kandidat berdarah suci**.

</details>

### Soal #57: Kasus Aplikasi Himpunan & Boolean Visual
**Filter Drone Z Bermasalah**
Pusat komando membuat skrip keamanan pintar yang menyaring benda melayang berbahaya. Benda akan ditembak mati jika lolos IF syarat verifikasi sakat:
`NOT (Terdeteksi_Aman OR Bawa_Otorisasi) AND Kecepatan_Tinggi`

Penduduk lokal mengeluh drone biasa malah ikut meledak. Manakah status yang sesungguhnya MURNI SESUAI LOGIKA sehingga Drone Z malang akan dieksekusi tembakan misil itu? (Ubah kalimatnya ke Teori Himpunan).

A. Bawa Otorisasi ATAU Cepat saja.
B. Hanya Aman ATAU Bawa Otorisasi, dan Pelan.
C. TIDAK Aman ATAU Bawa Otorisasi, ATAU Pelan
D. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.
E. TIDAK Aman DAN TIDAK Cepat, TAPI Bawa Otorisasi.


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Hukum De Morgan's Law Himpunan Komplemen**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. TIDAK Aman DAN TIDAK Bawa Otorisasi, TETAPI Cepat.**

**Pembahasan Algoritma (Diagnonis: Operasi Boolean / De Morgan's Law)**

1. Soal ini mengujikan hukum dasar gerbang logika diskrit logika OR dan AND.
2. Pernyataan `NOT (A OR B)` secara matematis (Teori De Morgan's) akan menjungkirbalikkan tanda serunya masuk mendongkrak operan di dalam kurungnya.
   Hukum De Morgan: `NOT (A OR B) === (NOT A) AND (NOT B)`
3. Maka penggalan perintah mesin itu sejatinya mengeksekusi sifat:
   `(!Aman AND !Otorisasi) AND Cepat_Tinggi`
4. Diterjemahkan bebas untuk warga lokal: Drone meledak **HANYA JIKA drone itu TIDAK Aman, DAN drone itu TIDAK bawa Otorisasi, TAPI drone-nya sedang ngebut kencang Kecepatan Tinggi**.
5. Siapapun yang terbang santai pelan tidak akan tertembak.

</details>

### Soal #58: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 29 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 8 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Taring Tajam` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Taring Tajam)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 21
B. 37
C. 232
D. 13
E. 29


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 21**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (29)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 8$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $29 - 8 =$ **21 kandidat berdarah suci**.

</details>

### Soal #59: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 28 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 8 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Mata Hijau` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Mata Hijau)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 224
B. 12
C. 20
D. 28
E. 36


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 20**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (28)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 8$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $28 - 8 =$ **20 kandidat berdarah suci**.

</details>

### Soal #60: Kasus Aplikasi Himpunan & Boolean Visual
**Buku Genetik Bebras**
Ilmuwan Desa mencatat temuan genetik aneh di penangkaran. Dilaporkan ada 27 alien mini yang memiliki DNA `Ekor Runcing`. Tapi usut punya usut, ada mutan ganda, yakni 4 alien dari rombongan `Ekor Runcing` tadi ternyata kedapatan juga membawa susupan DNA tambahan berspesifikasi `Bulu Lebat` di darahnya.

Jika Profesor A murni hanya mencari alien 'darah suci' dengan karakter khusus WAJIB dan MURNI HANYA MENAMPAKKAN wujud karakter `Ekor Runcing` saja (Benci banget sama tipe Bulu Lebat)... Ada berapa kandidat yang pantas diboyong oleh Profesor tersebut?

A. 31
B. 19
C. 23
D. 27
E. 108


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Selisih Himpunan (Himpunan A - B) atau Pinggiran Lingkaran Venn kiri murni.**

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 23**

**Pembahasan Algoritma (Diagnonis: Operasi Selisih Himpunan Semrawut)**

1. Wujud Asli Soal: 
   - Himpunan $A = (27)$ Alien bertipe Ekor Runcing.
   - Angka irisan persilangan $(A \cap B) = 4$ Mutan ganda campuran.
2. Soal ini mengalihkan bahasa awam yang merepotkan menjadi permintaan kalkulasi Himpunan Matematika murni yakni Wilayah "HANYA A" tanpa kecampuran B alias $A - B$.
3. Maka eksekusi cepatnya: Total A Murni minus yang ikut tercampur irisan mutan.
   Hasil = $27 - 4 =$ **23 kandidat berdarah suci**.

</details>

---
[< Bagian 2](./11-bedah-bebras-part-2.md) | [Bagian 4 >](./11-bedah-bebras-part-4.md)
