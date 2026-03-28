# 09. Kombinatorika - Latihan Soal Bagian 6
## Topik: Prinsip Sarang Merpati (Pigeonhole Principle)

[< Bagian 5](./09-kombinatorika-soal-part-5.md) | [< Kembali ke Indeks](../09-kombinatorika.md)

---

### Soal #251: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 13 kaos kaki hitam, 13 putih, dan 14 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 15
B. 40
C. 28
D. 4
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**D. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #252: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 12 kelereng Putih, dan 12 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA MERAH. Berapa kelereng minimal yang harus diambil?

A. 39
B. 37
C. 5
D. 29
E. 28


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Merah sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**D. 29**

**Pembahasan:** Sialnya keambil sisa 27 kelereng bukan Merah sampai habis + 2 kelereng Merah = 29 kelereng.</details>

### Soal #253: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 5 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 17
B. 53
C. 60
D. 49
E. 37


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**D. 49**

**Pembahasan:** Terburuk = 12 bulan $\times$ 4 orang = 48. Orang ke-49 PASTI akan bikin 1 bulan ada 5 yang ultah.</details>

### Soal #254: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 9 kelereng Hitam, 14 kelereng Putih, dan 13 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA MERAH. Berapa kelereng minimal yang harus diambil?

A. 34
B. 25
C. 5
D. 24
E. 36


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Merah sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 25**

**Pembahasan:** Sialnya keambil sisa 23 kelereng bukan Merah sampai habis + 2 kelereng Merah = 25 kelereng.</details>

### Soal #255: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 11 kelereng Hitam, 15 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 5
B. 23
C. 37
D. 35
E. 24


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 24**

**Pembahasan:** Sialnya keambil sisa 22 kelereng bukan Putih sampai habis + 2 kelereng Putih = 24 kelereng.</details>

### Soal #256: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 9 kelereng Putih, dan 10 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 32
B. 20
C. 5
D. 34
E. 21


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 21**

**Pembahasan:** Sialnya keambil sisa 19 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 21 kelereng.</details>

### Soal #257: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 8 kelereng Hitam, 14 kelereng Putih, dan 9 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA MERAH. Berapa kelereng minimal yang harus diambil?

A. 23
B. 24
C. 31
D. 5
E. 29


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Merah sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 24**

**Pembahasan:** Sialnya keambil sisa 22 kelereng bukan Merah sampai habis + 2 kelereng Merah = 24 kelereng.</details>

### Soal #258: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 5 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 17
B. 60
C. 37
D. 51
E. 49


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**E. 49**

**Pembahasan:** Terburuk = 12 bulan $\times$ 4 orang = 48. Orang ke-49 PASTI akan bikin 1 bulan ada 5 yang ultah.</details>

### Soal #259: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 5 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 49
B. 37
C. 17
D. 60
E. 51


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**A. 49**

**Pembahasan:** Terburuk = 12 bulan $\times$ 4 orang = 48. Orang ke-49 PASTI akan bikin 1 bulan ada 5 yang ultah.</details>

### Soal #260: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 9 kaos kaki hitam, 13 putih, dan 15 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 4
B. 37
C. 16
D. 24
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**A. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #261: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 9 kaos kaki hitam, 11 putih, dan 11 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 22
B. 31
C. 4
D. 12
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**C. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #262: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 8 kelereng Hitam, 10 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 20
B. 27
C. 5
D. 29
E. 21


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 21**

**Pembahasan:** Sialnya keambil sisa 19 kelereng bukan Putih sampai habis + 2 kelereng Putih = 21 kelereng.</details>

### Soal #263: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 48
B. 16
C. 25
D. 37
E. 38


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**D. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #264: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 15 kaos kaki hitam, 12 putih, dan 8 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 29
B. 3
C. 16
D. 4
E. 35


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**D. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #265: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 9 kelereng Hitam, 15 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 28
B. 33
C. 35
D. 27
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**A. 28**

**Pembahasan:** Sialnya keambil sisa 26 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 28 kelereng.</details>

### Soal #266: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 10 kelereng Hitam, 14 kelereng Putih, dan 13 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 25
B. 5
C. 37
D. 35
E. 24


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**A. 25**

**Pembahasan:** Sialnya keambil sisa 23 kelereng bukan Putih sampai habis + 2 kelereng Putih = 25 kelereng.</details>

### Soal #267: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 10 kelereng Hitam, 13 kelereng Putih, dan 14 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 35
B. 29
C. 37
D. 28
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 29**

**Pembahasan:** Sialnya keambil sisa 27 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 29 kelereng.</details>

### Soal #268: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 3 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 36
B. 13
C. 15
D. 25
E. 29


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**D. 25**

**Pembahasan:** Terburuk = 12 bulan $\times$ 2 orang = 24. Orang ke-25 PASTI akan bikin 1 bulan ada 3 yang ultah.</details>

### Soal #269: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 5 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 49
B. 17
C. 50
D. 37
E. 60


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**A. 49**

**Pembahasan:** Terburuk = 12 bulan $\times$ 4 orang = 48. Orang ke-49 PASTI akan bikin 1 bulan ada 5 yang ultah.</details>

### Soal #270: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 25
B. 16
C. 48
D. 38
E. 37


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**E. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #271: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 10 kelereng Putih, dan 10 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 22
B. 5
C. 21
D. 35
E. 33


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**A. 22**

**Pembahasan:** Sialnya keambil sisa 20 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 22 kelereng.</details>

### Soal #272: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 11 kaos kaki hitam, 13 putih, dan 13 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 4
B. 37
C. 26
D. 14
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**A. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #273: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 13 kelereng Hitam, 11 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 35
B. 26
C. 5
D. 33
E. 25


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 26**

**Pembahasan:** Sialnya keambil sisa 24 kelereng bukan Putih sampai habis + 2 kelereng Putih = 26 kelereng.</details>

### Soal #274: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 41
B. 48
C. 37
D. 25
E. 16


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**C. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #275: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 5 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 17
B. 37
C. 53
D. 49
E. 60


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**D. 49**

**Pembahasan:** Terburuk = 12 bulan $\times$ 4 orang = 48. Orang ke-49 PASTI akan bikin 1 bulan ada 5 yang ultah.</details>

### Soal #276: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 11 kelereng Hitam, 11 kelereng Putih, dan 10 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 30
B. 5
C. 32
D. 22
E. 23


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 23**

**Pembahasan:** Sialnya keambil sisa 21 kelereng bukan Putih sampai habis + 2 kelereng Putih = 23 kelereng.</details>

### Soal #277: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 10 kelereng Hitam, 9 kelereng Putih, dan 8 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 27
B. 5
C. 25
D. 19
E. 20


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 20**

**Pembahasan:** Sialnya keambil sisa 18 kelereng bukan Putih sampai habis + 2 kelereng Putih = 20 kelereng.</details>

### Soal #278: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 25
B. 38
C. 16
D. 48
E. 37


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**E. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #279: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 8 kelereng Hitam, 13 kelereng Putih, dan 13 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 34
B. 5
C. 27
D. 32
E. 28


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 28**

**Pembahasan:** Sialnya keambil sisa 26 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 28 kelereng.</details>

### Soal #280: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 13 kelereng Hitam, 13 kelereng Putih, dan 14 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 28
B. 29
C. 40
D. 38
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 29**

**Pembahasan:** Sialnya keambil sisa 27 kelereng bukan Putih sampai habis + 2 kelereng Putih = 29 kelereng.</details>

### Soal #281: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 37
B. 48
C. 25
D. 41
E. 16


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**A. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #282: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 11 kelereng Putih, dan 8 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 5
B. 34
C. 21
D. 32
E. 20


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**C. 21**

**Pembahasan:** Sialnya keambil sisa 19 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 21 kelereng.</details>

### Soal #283: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 11 kelereng Hitam, 15 kelereng Putih, dan 13 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 39
B. 37
C. 26
D. 25
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**C. 26**

**Pembahasan:** Sialnya keambil sisa 24 kelereng bukan Putih sampai habis + 2 kelereng Putih = 26 kelereng.</details>

### Soal #284: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 12 kaos kaki hitam, 12 putih, dan 11 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 26
B. 13
C. 3
D. 4
E. 35


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**D. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #285: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 3 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 25
B. 15
C. 27
D. 36
E. 13


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**A. 25**

**Pembahasan:** Terburuk = 12 bulan $\times$ 2 orang = 24. Orang ke-25 PASTI akan bikin 1 bulan ada 3 yang ultah.</details>

### Soal #286: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 9 kelereng Putih, dan 9 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 31
B. 5
C. 25
D. 26
E. 33


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**D. 26**

**Pembahasan:** Sialnya keambil sisa 24 kelereng bukan Putih sampai habis + 2 kelereng Putih = 26 kelereng.</details>

### Soal #287: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 8 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 34
B. 32
C. 21
D. 20
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**C. 21**

**Pembahasan:** Sialnya keambil sisa 19 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 21 kelereng.</details>

### Soal #288: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 4 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 16
B. 40
C. 37
D. 48
E. 25


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**C. 37**

**Pembahasan:** Terburuk = 12 bulan $\times$ 3 orang = 36. Orang ke-37 PASTI akan bikin 1 bulan ada 4 yang ultah.</details>

### Soal #289: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 11 kelereng Hitam, 8 kelereng Putih, dan 8 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 27
B. 25
C. 17
D. 18
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**D. 18**

**Pembahasan:** Sialnya keambil sisa 16 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 18 kelereng.</details>

### Soal #290: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 13 kaos kaki hitam, 10 putih, dan 12 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 3
B. 14
C. 35
D. 4
E. 25


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**D. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #291: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 3 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 36
B. 13
C. 25
D. 26
E. 15


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**C. 25**

**Pembahasan:** Terburuk = 12 bulan $\times$ 2 orang = 24. Orang ke-25 PASTI akan bikin 1 bulan ada 3 yang ultah.</details>

### Soal #292: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 3 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 15
B. 25
C. 26
D. 13
E. 36


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**B. 25**

**Pembahasan:** Terburuk = 12 bulan $\times$ 2 orang = 24. Orang ke-25 PASTI akan bikin 1 bulan ada 3 yang ultah.</details>

### Soal #293: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 13 kaos kaki hitam, 9 putih, dan 14 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 15
B. 4
C. 24
D. 36
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**B. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #294: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 15 kelereng Hitam, 12 kelereng Putih, dan 15 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 28
B. 40
C. 42
D. 29
E. 5


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**D. 29**

**Pembahasan:** Sialnya keambil sisa 27 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 29 kelereng.</details>

### Soal #295: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 14 kelereng Hitam, 8 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 5
B. 33
C. 31
D. 20
E. 21


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**E. 21**

**Pembahasan:** Sialnya keambil sisa 19 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 21 kelereng.</details>

### Soal #296: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 15 kaos kaki hitam, 15 putih, dan 15 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 16
B. 4
C. 32
D. 45
E. 3


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**B. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #297: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 12 kelereng Hitam, 10 kelereng Putih, dan 8 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA PUTIH. Berapa kelereng minimal yang harus diambil?

A. 28
B. 22
C. 5
D. 21
E. 30


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Putih sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 22**

**Pembahasan:** Sialnya keambil sisa 20 kelereng bukan Putih sampai habis + 2 kelereng Putih = 22 kelereng.</details>

### Soal #298: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam laci gelap terdapat 9 kaos kaki hitam, 8 putih, dan 10 merah. Berapa jumlah kaos kaki MINIMAL yang harus diambil acak agar DIJAMIN 100% mendapatkan MINTA SEPASANG (2 buah) kaos kaki berwarna APA SAJA ASAL WARNANYA SAMA?

A. 11
B. 19
C. 3
D. 27
E. 4


<details><summary>💡 Hint</summary>Skenario terburuk (apes): Ambil 1 warna beda-beda terus (Dapat 1 hitam, 1 putih, 1 merah). Tarikan ke-4 pasti membuat ada warna yang sepasang!</details>
<details><summary>✅ Jawaban</summary>**E. 4**

**Pembahasan:** 3 warna berbeda + 1 tarikan = 4 kaos kaki (Pigeonhole Principle).</details>

### Soal #299: Pilihan Ganda - Pigeonhole Principle (PHP)
Berapa minimal jumlah orang yang harus ada di sebuah kumpul keluarga, agar DIJAMIN (100% Pasti) minimal ada 3 orang yang merayakan ulang tahun pada bulan yang SAMA?

A. 36
B. 15
C. 30
D. 25
E. 13


<details><summary>💡 Hint</summary>PHP: Semesta laci (sarang) = 12 bulan. Skenario terapes: Setiap bulan diisi (n-1) orang. Baru setelah ke-12 bulan terisi, orang terakhir akan menuhin kotak jadi (n) orang.</details>
<details><summary>✅ Jawaban</summary>**D. 25**

**Pembahasan:** Terburuk = 12 bulan $\times$ 2 orang = 24. Orang ke-25 PASTI akan bikin 1 bulan ada 3 yang ultah.</details>

### Soal #300: Pilihan Ganda - Pigeonhole Principle (PHP)
Di dalam keranjang ajaib terdapat 14 kelereng Hitam, 11 kelereng Putih, dan 11 kelereng Merah. Tanpa melihat, Budi ingin mendapatkan DIJAMIN SEPASANG (2 kelereng) BERWARNA HITAM. Berapa kelereng minimal yang harus diambil?

A. 5
B. 24
C. 34
D. 23
E. 36


<details><summary>💡 Hint</summary>Skenario terapesnya: Warna yang keambil malah warna-warna selain Hitam sampai mereka habis, baru sisa target.</details>
<details><summary>✅ Jawaban</summary>**B. 24**

**Pembahasan:** Sialnya keambil sisa 22 kelereng bukan Hitam sampai habis + 2 kelereng Hitam = 24 kelereng.</details>

---
[< Bagian 5](./09-kombinatorika-soal-part-5.md) | [< Kembali ke Indeks](../09-kombinatorika.md)
