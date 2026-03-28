🔙 **Kembali ke Materi:** [Materi 11 Bedah Soal Bebras](../11-bedah-soal-bebras.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 11. Bedah Soal Bebras CAPSTONE - Latihan Soal Bagian 1
## Topik Utama: Wujud Asli Teori GRAF (Jaringan & Labirin)

> **Misi Anda**: Jangan buang waktu menggambar manual layaknya anak SD. Gunakan ilmu rahasia Teori Himpunan, Graf, atau Kombinatorika untuk MEMBEDAH wujud asli manipulasi skenario soal-soal ini!

[< Kembali ke Indeks](../11-bedah-soal-bebras.md) | [Bagian 2 >](./11-bedah-bebras-part-2.md)

---

### Soal #1: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 6 desa yang saling terhubung oleh 6 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 10 kali?

A. 20
B. 6
C. 11
D. 9
E. 10


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 10**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 6 desa.
4. Sisi: 6 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 10 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **10 unit waktu**.

</details>

### Soal #2: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 5 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 5 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 4
B. 5
C. 10
D. 6
E. 3


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 4**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 5 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 5 gugusan daratan, dibutuhkan minimal $5 - 1 =$ **4** buah jembatan darurat utama.

</details>

### Soal #3: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 7 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 8 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Mungkin dari segala sisi
B. Hanya jika mulai dari pulau buntu
C. Tidak Pasti
D. Tidak Mungkin
E. 1 Peluang


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 8 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #4: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 3 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 3 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 1
B. 3
C. 2
D. 6
E. 4


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 2**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 3 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 3 gugusan daratan, dibutuhkan minimal $3 - 1 =$ **2** buah jembatan darurat utama.

</details>

### Soal #5: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 7 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 6 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Mungkin dari segala sisi
B. Tidak Pasti
C. Hanya jika mulai dari pulau buntu
D. Tidak Mungkin
E. 1 Peluang


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 6 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #6: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 8 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 8 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. 1 Peluang
B. Tidak Pasti
C. Hanya jika mulai dari pulau buntu
D. Mungkin dari segala sisi
E. Tidak Mungkin


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 8 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #7: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 7 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 8 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Tidak Pasti
B. Hanya jika mulai dari pulau buntu
C. Mungkin dari segala sisi
D. 1 Peluang
E. Tidak Mungkin


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 8 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #8: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 11 desa yang saling terhubung oleh 20 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 6 kali?

A. 12
B. 11
C. 5
D. 6
E. 7


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. 6**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 11 desa.
4. Sisi: 20 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 6 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **6 unit waktu**.

</details>

### Soal #9: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 9 desa yang saling terhubung oleh 9 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 7 kali?

A. 14
B. 6
C. 7
D. 9
E. 8


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 7**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 9 desa.
4. Sisi: 9 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 7 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **7 unit waktu**.

</details>

### Soal #10: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 3 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 3 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 3
B. 6
C. 1
D. 4
E. 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 2**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 3 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 3 gugusan daratan, dibutuhkan minimal $3 - 1 =$ **2** buah jembatan darurat utama.

</details>

### Soal #11: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 4 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 4 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 8
B. 4
C. 3
D. 2
E. 5


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 3**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 4 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 4 gugusan daratan, dibutuhkan minimal $4 - 1 =$ **3** buah jembatan darurat utama.

</details>

### Soal #12: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 4 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 4 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 3
B. 5
C. 8
D. 4
E. 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 3**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 4 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 4 gugusan daratan, dibutuhkan minimal $4 - 1 =$ **3** buah jembatan darurat utama.

</details>

### Soal #13: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 9 desa yang saling terhubung oleh 11 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 9 kali?

A. 18
B. 8
C. 10
D. 14
E. 9


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 9**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 9 desa.
4. Sisi: 11 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 9 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **9 unit waktu**.

</details>

### Soal #14: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 11 desa yang saling terhubung oleh 15 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 7 kali?

A. 8
B. 6
C. 7
D. 11
E. 14


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 7**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 11 desa.
4. Sisi: 15 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 7 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **7 unit waktu**.

</details>

### Soal #15: Kasus Aplikasi Visual Graf
**Bencana Badai Ribut**
Provinsi X tadinya sepenuhnya terhubung (satu daratan). Namun setelah badai dahsyat semalam, banyak jembatan putus sehingga provinsi tersebut terpecah menjadi 4 gugusan daratan (pulau besar) yang terisolir satu sama lain. Gubernur meminta tim SAR sesegera mungkin membangun kembali jembatan darurat agar SEMUA penduduk di 4 gugusan tersebut saling terhubung kembali minimal oleh satu rute tunggal.

Berapakah MINIMAL jembatan darurat yang harus dibangun gubernur?

A. 2
B. 3
C. 5
D. 8
E. 4


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Minimum Spanning Tree (Spanning Forest)**. Untuk menyambungkan C buah komponen graf yang terpisah menjadi 1 graf penuh, butuh (C-1) edge.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 3**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Spanning Tree)**

1. Dalam bahasa sehari-hari: Menyambung pulau terpisah.
2. Dalama bahasa Komputer/Graf: Menyambung 4 *Connected Components* (Komponen Terhubung) menjadi sebuah Graf Gabungan berstatus *Fully Connected*.
3. Aturan dasar penyambungan minimal: Sama seperti membangun fondasi pohon (Tree). Jika ada $N$ titik terpisah yang harus disambung tanpa pemborosan (tanpa sirkuit tertutup / siklus), maka dibutuhkan $(N - 1)$ garis penghubung.
4. Maka dari 4 gugusan daratan, dibutuhkan minimal $4 - 1 =$ **3** buah jembatan darurat utama.

</details>

### Soal #16: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 9 desa yang saling terhubung oleh 18 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 5 kali?

A. 5
B. 9
C. 4
D. 10
E. 6


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 5**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 9 desa.
4. Sisi: 18 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 5 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **5 unit waktu**.

</details>

### Soal #17: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 6 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 4 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Hanya jika mulai dari pulau buntu
B. Tidak Mungkin
C. Mungkin dari segala sisi
D. 1 Peluang
E. Tidak Pasti


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 4 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #18: Kasus Aplikasi Visual Graf
**Bebas Labirin Bersarang**
Pak Dengklek membuat labirin rumit berbentuk peta kota tua. Terdapat 12 desa yang saling terhubung oleh 14 jalan tembus (bisa dilewati 2 arah). Dari Pintu Masuk (Desa A), setiap melewati 1 jalan dihitung sebagai 1 unit waktu. Bebek Pak Dengklek mengendus jejak tercepat dan langsung lari dari Desa A ke Desa Z. Berapa WAKTU MINIMAL bagi si bebek sampai tujuan, jika panjang jalur rahasia terpendeknya memiliki loncatan 6 kali?

A. 6
B. 5
C. 7
D. 12
E. 8


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Graf tak Berarah (Shortest Path / BFS)**. Ini adalah abstraksi dari lintasan terpendek Graf.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 6**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Lintasan Terpendek)**

1. Secara kasat mata, ini adalah gambar Labirin.
2. Di balik layar, ini adalah operasi algoritma BFS (Breadth-First Search) pada teori Graf!
3. Simpul: 12 desa.
4. Sisi: 14 jalan raya dua arah.
5. Pertanyaan aslinya adalah pencarian **Jarak Terpendek** (Shortest Path) dari Node A ke Node Z.
6. Berdasarkan informasi lintasan, rute paling ideal memerlukan 6 buah lompatan garis antar Node. Karena 1 jalan = 1 unit waktu, jawabannya adalah **6 unit waktu**.

</details>

### Soal #19: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 9 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 6 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Tidak Pasti
B. Hanya jika mulai dari pulau buntu
C. 1 Peluang
D. Mungkin dari segala sisi
E. Tidak Mungkin


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 6 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

### Soal #20: Kasus Aplikasi Visual Graf
**Keliling Pulau Pak Dengklek**
Di gugusan kepulauan Bebekia, ada 11 pulau yang dihubungkan oleh jembatan kayu. Pak Dengklek ingin melakukan inspeksi tahunan. Ia memberi sayembara: "Siapa yang bisa berjalan melewati SELURUH jembatan yang ada MASING-MASING TEPAT SATU KALI tanpa berenang, akan diberi hadiah hadiah." Kamu melihat peta kepulauan tersebut dan menghitung ternyata ada 4 buah pulau yang memiliki jumlah jembatan ganjil.

Berapa peluang ada orang yang bisa memenangkan sayembara tersebut?

A. Tidak Mungkin
B. Tidak Pasti
C. Hanya jika mulai dari pulau buntu
D. 1 Peluang
E. Mungkin dari segala sisi


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Euler Path di Teori Graf**. Syarat bisa melewati semua sisi persis sekali adalah jumlah *node derajat ganjil* maksimal 2.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. Tidak Mungkin**

**Pembahasan Algoritma (Diagnonis: Teori GRAF - Jejak Euler)**

1. Pemula akan mencoba menggambar garis secara trial-and-error di atas kertas sampai waktunya habis.
2. Pakar OSN-K langsung mendiagnosis bahwa ini murni soal **Euler Path**.
3. Syarat absolut sebuah graf memiliki Jejak Euler (bisa digambar 1 tarikan tanpa putus & tanpa double sisi) adalah: Total Node yang berderajat Ganjil **harus persis 0 atau maksimal MAHAL 2 buah**.
4. Di peta yang diberikan soal, ada 4 buah pulau bercabang ganjil.
5. Kesimpulan: **Sangat mustahil / Tidak Mungkin** memenangkan sayembara karena melanggar hukum Euler.

</details>

---
[< Kembali ke Indeks](../11-bedah-soal-bebras.md) | [Bagian 2 >](./11-bedah-bebras-part-2.md)
