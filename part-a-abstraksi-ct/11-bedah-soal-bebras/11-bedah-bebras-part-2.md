# 11. Bedah Soal Bebras CAPSTONE - Latihan Soal Bagian 2
## Topik Utama: Wujud Asli KOMBINATORIKA (Translasi & Pola Kembar)

> **Misi Anda**: Jangan buang waktu menggambar manual layaknya anak SD. Gunakan ilmu rahasia Teori Himpunan, Graf, atau Kombinatorika untuk MEMBEDAH wujud asli manipulasi skenario soal-soal ini!

[< Bagian 1](./11-bedah-bebras-part-1.md) | [Bagian 3 >](./11-bedah-bebras-part-3.md)

---

### Soal #21: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 7 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 5 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 42
B. 5040
C. 210
D. 21
E. 2520


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 42**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 7. Kalau seluruhnya berbeda, susunannya adalah $7!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 5 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{7!}{5!}$ = **42 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #22: Kasus Aplikasi Kombinatorika Visual
**Antrian Bebek Rewel Tertinggi**
Sebanyak 15 ekor bebek Pak Dengklek sedang berebut masuk berteduh ke dalam 7 kandang kecil karena hujan lebat. Pak Dengklek yakin walau mereka berdesakan suka-suka mereka secara random di dalam gelap...

Pasti minimal HUKUM ALAM akan **memaksa jaminan 100% AMAN** ada minimal SETIDAKNYA SATU KANDANG yang diduduki bebek sebanyak... ekor?

A. 4
B. 3
C. 1
D. 2
E. 8


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Pigeonhole Principle (PHP) Lanjut**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 3**

**Pembahasan Algoritma (Diagnonis: Sarang Merpati / Pigeonhole Principle)**

1. Samaran Soal: Menyebar objek (bebek) bebas merdeka ke dalam laci (kandang).
2. Membedah Rumus Skenario Apes (PHP): Jika ada $N$ barang dimasukkan acak ke $M$ laci.
   Semua laci diisi secara SANGAT ADIL dan MERATA sejauh yang mereka mampu (Ini adalah kelakuan ter-apes kalau kita mau pancing laci penuh).
3. $N = 15$ bebek, $M = 7$ kandang.
4. Bagi Rata (Worst Case): $15 \div 7 = 2$ ekor sisa 1 ekor di luar kedinginan.
5. Ternyata kalau semua dibagi adil 2-2 di setiap kandang, masih nyisa 1 ekor di luar kandang. Si 1 ekor sialan ini masuk ke kandang manapun pasti akan menyebabkan kandang tersebut meledak jumlah populasinya meroket menjadi $2 + 1 = 3$!
6. Kesimpulan: **Akan ada MINIMAL 3 ekor bebek berdempetan mendominasi satu kandang sial terpadat itu**.

</details>

### Soal #23: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 6 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 3 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 125
B. 120
C. 360
D. 60
E. 720


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 120**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 6. Kalau seluruhnya berbeda, susunannya adalah $6!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 3 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{6!}{3!}$ = **120 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #24: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 4 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 4 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 256
B. 16
C. 1
D. 24
E. 255


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 256**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 4 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 4 pilihan konstan.
6. Formulasi: $Pilihan = 4 \times 4 \times ... \text{(sebanyak 4 kali)}$.
7. Jawabannya bentuk Eksponen: $4^{4}$ = **256 model cetakan robot**.

</details>

### Soal #25: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 5 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 6 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 7774
B. 7776
C. 30
D. 6
E. 720


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 7776**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 5 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 6 pilihan konstan.
6. Formulasi: $Pilihan = 6 \times 6 \times ... \text{(sebanyak 5 kali)}$.
7. Jawabannya bentuk Eksponen: $6^{5}$ = **7776 model cetakan robot**.

</details>

### Soal #26: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 7 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 5 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 42
B. 210
C. 21
D. 5040
E. 2520


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 42**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 7. Kalau seluruhnya berbeda, susunannya adalah $7!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 5 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{7!}{5!}$ = **42 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #27: Kasus Aplikasi Kombinatorika Visual
**Antrian Bebek Rewel Tertinggi**
Sebanyak 15 ekor bebek Pak Dengklek sedang berebut masuk berteduh ke dalam 7 kandang kecil karena hujan lebat. Pak Dengklek yakin walau mereka berdesakan suka-suka mereka secara random di dalam gelap...

Pasti minimal HUKUM ALAM akan **memaksa jaminan 100% AMAN** ada minimal SETIDAKNYA SATU KANDANG yang diduduki bebek sebanyak... ekor?

A. 2
B. 4
C. 8
D. 3
E. 1


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Pigeonhole Principle (PHP) Lanjut**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. 3**

**Pembahasan Algoritma (Diagnonis: Sarang Merpati / Pigeonhole Principle)**

1. Samaran Soal: Menyebar objek (bebek) bebas merdeka ke dalam laci (kandang).
2. Membedah Rumus Skenario Apes (PHP): Jika ada $N$ barang dimasukkan acak ke $M$ laci.
   Semua laci diisi secara SANGAT ADIL dan MERATA sejauh yang mereka mampu (Ini adalah kelakuan ter-apes kalau kita mau pancing laci penuh).
3. $N = 15$ bebek, $M = 7$ kandang.
4. Bagi Rata (Worst Case): $15 \div 7 = 2$ ekor sisa 1 ekor di luar kedinginan.
5. Ternyata kalau semua dibagi adil 2-2 di setiap kandang, masih nyisa 1 ekor di luar kandang. Si 1 ekor sialan ini masuk ke kandang manapun pasti akan menyebabkan kandang tersebut meledak jumlah populasinya meroket menjadi $2 + 1 = 3$!
6. Kesimpulan: **Akan ada MINIMAL 3 ekor bebek berdempetan mendominasi satu kandang sial terpadat itu**.

</details>

### Soal #28: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 7 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 4 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 209
B. 840
C. 210
D. 5040
E. 105


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 210**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 7. Kalau seluruhnya berbeda, susunannya adalah $7!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 4 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{7!}{4!}$ = **210 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #29: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 5 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 6 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 7774
B. 6
C. 30
D. 720
E. 7776


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 7776**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 5 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 6 pilihan konstan.
6. Formulasi: $Pilihan = 6 \times 6 \times ... \text{(sebanyak 5 kali)}$.
7. Jawabannya bentuk Eksponen: $6^{5}$ = **7776 model cetakan robot**.

</details>

### Soal #30: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 3 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 6 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 120
B. 18
C. 20
D. 720
E. 216


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 216**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 3 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 6 pilihan konstan.
6. Formulasi: $Pilihan = 6 \times 6 \times ... \text{(sebanyak 3 kali)}$.
7. Jawabannya bentuk Eksponen: $6^{3}$ = **216 model cetakan robot**.

</details>

### Soal #31: Kasus Aplikasi Kombinatorika Visual
**Antrian Bebek Rewel Tertinggi**
Sebanyak 13 ekor bebek Pak Dengklek sedang berebut masuk berteduh ke dalam 6 kandang kecil karena hujan lebat. Pak Dengklek yakin walau mereka berdesakan suka-suka mereka secara random di dalam gelap...

Pasti minimal HUKUM ALAM akan **memaksa jaminan 100% AMAN** ada minimal SETIDAKNYA SATU KANDANG yang diduduki bebek sebanyak... ekor?

A. 7
B. 4
C. 3
D. 1
E. 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Pigeonhole Principle (PHP) Lanjut**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 3**

**Pembahasan Algoritma (Diagnonis: Sarang Merpati / Pigeonhole Principle)**

1. Samaran Soal: Menyebar objek (bebek) bebas merdeka ke dalam laci (kandang).
2. Membedah Rumus Skenario Apes (PHP): Jika ada $N$ barang dimasukkan acak ke $M$ laci.
   Semua laci diisi secara SANGAT ADIL dan MERATA sejauh yang mereka mampu (Ini adalah kelakuan ter-apes kalau kita mau pancing laci penuh).
3. $N = 13$ bebek, $M = 6$ kandang.
4. Bagi Rata (Worst Case): $13 \div 6 = 2$ ekor sisa 1 ekor di luar kedinginan.
5. Ternyata kalau semua dibagi adil 2-2 di setiap kandang, masih nyisa 1 ekor di luar kandang. Si 1 ekor sialan ini masuk ke kandang manapun pasti akan menyebabkan kandang tersebut meledak jumlah populasinya meroket menjadi $2 + 1 = 3$!
6. Kesimpulan: **Akan ada MINIMAL 3 ekor bebek berdempetan mendominasi satu kandang sial terpadat itu**.

</details>

### Soal #32: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 3 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 5 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 120
B. 60
C. 125
D. 15
E. 10


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 125**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 3 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 5 pilihan konstan.
6. Formulasi: $Pilihan = 5 \times 5 \times ... \text{(sebanyak 3 kali)}$.
7. Jawabannya bentuk Eksponen: $5^{3}$ = **125 model cetakan robot**.

</details>

### Soal #33: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 7 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 5 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 5040
B. 2520
C. 21
D. 42
E. 210


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. 42**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 7. Kalau seluruhnya berbeda, susunannya adalah $7!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 5 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{7!}{5!}$ = **42 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #34: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 4 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 4 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 256
B. 16
C. 1
D. 24
E. 261


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 256**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 4 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 4 pilihan konstan.
6. Formulasi: $Pilihan = 4 \times 4 \times ... \text{(sebanyak 4 kali)}$.
7. Jawabannya bentuk Eksponen: $4^{4}$ = **256 model cetakan robot**.

</details>

### Soal #35: Kasus Aplikasi Kombinatorika Visual
**Antrian Bebek Rewel Tertinggi**
Sebanyak 11 ekor bebek Pak Dengklek sedang berebut masuk berteduh ke dalam 5 kandang kecil karena hujan lebat. Pak Dengklek yakin walau mereka berdesakan suka-suka mereka secara random di dalam gelap...

Pasti minimal HUKUM ALAM akan **memaksa jaminan 100% AMAN** ada minimal SETIDAKNYA SATU KANDANG yang diduduki bebek sebanyak... ekor?

A. 2
B. 1
C. 4
D. 6
E. 3


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Pigeonhole Principle (PHP) Lanjut**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 3**

**Pembahasan Algoritma (Diagnonis: Sarang Merpati / Pigeonhole Principle)**

1. Samaran Soal: Menyebar objek (bebek) bebas merdeka ke dalam laci (kandang).
2. Membedah Rumus Skenario Apes (PHP): Jika ada $N$ barang dimasukkan acak ke $M$ laci.
   Semua laci diisi secara SANGAT ADIL dan MERATA sejauh yang mereka mampu (Ini adalah kelakuan ter-apes kalau kita mau pancing laci penuh).
3. $N = 11$ bebek, $M = 5$ kandang.
4. Bagi Rata (Worst Case): $11 \div 5 = 2$ ekor sisa 1 ekor di luar kedinginan.
5. Ternyata kalau semua dibagi adil 2-2 di setiap kandang, masih nyisa 1 ekor di luar kandang. Si 1 ekor sialan ini masuk ke kandang manapun pasti akan menyebabkan kandang tersebut meledak jumlah populasinya meroket menjadi $2 + 1 = 3$!
6. Kesimpulan: **Akan ada MINIMAL 3 ekor bebek berdempetan mendominasi satu kandang sial terpadat itu**.

</details>

### Soal #36: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 6 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 3 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 720
B. 125
C. 120
D. 360
E. 60


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 120**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 6. Kalau seluruhnya berbeda, susunannya adalah $6!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 3 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{6!}{3!}$ = **120 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #37: Kasus Aplikasi Kombinatorika Visual
**Antrian Bebek Rewel Tertinggi**
Sebanyak 13 ekor bebek Pak Dengklek sedang berebut masuk berteduh ke dalam 6 kandang kecil karena hujan lebat. Pak Dengklek yakin walau mereka berdesakan suka-suka mereka secara random di dalam gelap...

Pasti minimal HUKUM ALAM akan **memaksa jaminan 100% AMAN** ada minimal SETIDAKNYA SATU KANDANG yang diduduki bebek sebanyak... ekor?

A. 3
B. 4
C. 1
D. 7
E. 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Pigeonhole Principle (PHP) Lanjut**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 3**

**Pembahasan Algoritma (Diagnonis: Sarang Merpati / Pigeonhole Principle)**

1. Samaran Soal: Menyebar objek (bebek) bebas merdeka ke dalam laci (kandang).
2. Membedah Rumus Skenario Apes (PHP): Jika ada $N$ barang dimasukkan acak ke $M$ laci.
   Semua laci diisi secara SANGAT ADIL dan MERATA sejauh yang mereka mampu (Ini adalah kelakuan ter-apes kalau kita mau pancing laci penuh).
3. $N = 13$ bebek, $M = 6$ kandang.
4. Bagi Rata (Worst Case): $13 \div 6 = 2$ ekor sisa 1 ekor di luar kedinginan.
5. Ternyata kalau semua dibagi adil 2-2 di setiap kandang, masih nyisa 1 ekor di luar kandang. Si 1 ekor sialan ini masuk ke kandang manapun pasti akan menyebabkan kandang tersebut meledak jumlah populasinya meroket menjadi $2 + 1 = 3$!
6. Kesimpulan: **Akan ada MINIMAL 3 ekor bebek berdempetan mendominasi satu kandang sial terpadat itu**.

</details>

### Soal #38: Kasus Aplikasi Kombinatorika Visual
**Warna-Warni Robot Perakitan**
Di pabrik mainan *Bebras Robotics*, ada 5 bagian tubuh robot yang harus diwarnai (Kepala, Badan, Tangan dll). Pabrik itu memiliki 6 wadah cat berbeda. Mesin otomatis diprogram agar ia boleh menggunakan cat yang sama untuk bagian tubuh yang berbeda (Misal: Robot full merah muda itu valid).

Berapa banyak koleksi variasi robot lengkap yang bisa diproduksi si mesin otomatis?

A. 6
B. 7778
C. 720
D. 30
E. 7776


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Aturan Perkalian dengan Pengulangan Blok Kosong (*Filling Slots*)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 7776**

**Pembahasan Algoritma (Diagnonis: Kombinatorika Dasar - Filling Slots dgn Pengulangan)**

1. Pemula akan kewalahan menulis satu-satu pola warnanya di kertas buram.
2. Kita panggil Aturan Slot Kosong dari Modul 9.
3. Terdapat 5 buah bagian tubuh (slot pasif perlengkapan) yang harus dialokasikan nilai.
4. Syarat Soal: Warnanya independen dan **Boleh Diulang**. Artinya, wadah cat tidak habis/berkurang kesempatannya setelah dipakai mengecat satu bagian.
5. Kemungkinan pengecatan per bagian = 6 pilihan konstan.
6. Formulasi: $Pilihan = 6 \times 6 \times ... \text{(sebanyak 5 kali)}$.
7. Jawabannya bentuk Eksponen: $6^{5}$ = **7776 model cetakan robot**.

</details>

### Soal #39: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 5 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 2 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 60
B. 59
C. 120
D. 20
E. 30


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 60**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 5. Kalau seluruhnya berbeda, susunannya adalah $5!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 2 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{5!}{2!}$ = **60 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

### Soal #40: Kasus Aplikasi Kombinatorika Visual
**Mesin Penerjemah Alien**
Pak Dengklek diundang alien dan disodorkan 2 tombol ajaib. Alien itu memasukkan benda dengan pola unik: `B-I-N-T-A-N-G`. 
Misalkan kita memiliki sebuah urutan susunan kartu Ajaib dengan total 6 huruf. Berapa banyak susunan output SANDI ACAK yang bisa dihasilkan mesin mesin tersebut jika ada tepat 4 buah karakter yang rupanya sama persis ketika dilihat lewat mesin tersebut?

A. 15
B. 360
C. 30
D. 120
E. 720


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Permutasi Huruf Kembar (Anagram)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 30**

**Pembahasan Algoritma (Diagnonis: Kombinatorika - Susunan Unsur Sama)**

1. Samaran Soal: Membuat Sandi Alien / Menyusun Kartu.
2. Modul 9 (Kombinatorika) mengajarkan ini adalah Permutasi Unsur Kembar.
3. Total huruf di layar sandi: 6. Kalau seluruhnya berbeda, susunannya adalah $6!$.
4. Tapi, mata mesin tidak bisa membedakan adanya 4 buah simbol yang kembar dempet. Karena ada objek yang indistinguishable (tak terbedakan), kita wajib membuang susunan repetitifnya.
5. Tarik faktorial: $\frac{6!}{4!}$ = **30 bentuk sandi berbeda** yang keluar dari mulut mesin.

</details>

---
[< Bagian 1](./11-bedah-bebras-part-1.md) | [Bagian 3 >](./11-bedah-bebras-part-3.md)
