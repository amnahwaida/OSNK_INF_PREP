# 09. Kombinatorika - Latihan Soal Bagian 5
## Topik: Kombinasi Multigrup & Bersyarat

[< Bagian 4](./09-kombinatorika-soal-part-4.md) | [Bagian 6 >](./09-kombinatorika-soal-part-6.md)

---

### Soal #201: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 6 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 3003
B. 1260
C. 99
D. 630
E. 720


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 1260**

**Pembahasan:** C(9,3) $\times$ C(6,2) = 1260 cara.</details>

### Soal #202: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 28
B. 1
C. 56
D. 210
E. 45


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**A. 28**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 8 stok. C(8, 6) = 28 cara.</details>

### Soal #203: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 5 siswa laki-laki dan 8 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 280
B. 564
C. 66
D. 1716
E. 560


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**E. 560**

**Pembahasan:** C(5,3) $\times$ C(8,3) = 560 cara.</details>

### Soal #204: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 7 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 112
B. 252
C. 8
D. 56
E. 120


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 56**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 5 sisa dari 8 stok. C(8, 5) = 56 cara.</details>

### Soal #205: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 14 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 924
B. 925
C. 495
D. 1848
E. 3003


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**A. 924**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 12 stok. C(12, 6) = 924 cara.</details>

### Soal #206: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 7 bola merah dan 7 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 80
B. 147
C. 1225
D. 364
E. 70


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**E. 70**

**Pembahasan:** C(7,3) + C(7,3) = 70 cara.</details>

### Soal #207: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 15 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 1287
B. 1716
C. 3432
D. 5005
E. 6435


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**B. 1716**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 13 stok. C(13, 6) = 1716 cara.</details>

### Soal #208: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 10 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 3780
B. 4320
C. 2160
D. 156
E. 11628


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 4320**

**Pembahasan:** C(9,2) $\times$ C(10,3) = 4320 cara.</details>

### Soal #209: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 14 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 3003
B. 1848
C. 923
D. 495
E. 924


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**E. 924**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 12 stok. C(12, 6) = 924 cara.</details>

### Soal #210: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 6 bola merah dan 6 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 90
B. 50
C. 400
D. 40
E. 220


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**D. 40**

**Pembahasan:** C(6,3) + C(6,3) = 40 cara.</details>

### Soal #211: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 7 buah dari pilihan total 13 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 210
B. 420
C. 120
D. 715
E. 1716


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**A. 210**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 4 sisa dari 10 stok. C(10, 4) = 210 cara.</details>

### Soal #212: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 15 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 1287
B. 5005
C. 6435
D. 1716
E. 3432


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 1716**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 13 stok. C(13, 6) = 1716 cara.</details>

### Soal #213: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 6 bola merah dan 7 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 286
B. 126
C. 55
D. 700
E. 65


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**C. 55**

**Pembahasan:** C(6,3) + C(7,3) = 55 cara.</details>

### Soal #214: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 12 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 214
B. 924
C. 420
D. 210
E. 495


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 210**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 4 sisa dari 10 stok. C(10, 4) = 210 cara.</details>

### Soal #215: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 5 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 365
B. 360
C. 1001
D. 46
E. 180


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 360**

**Pembahasan:** C(9,2) $\times$ C(5,2) = 360 cara.</details>

### Soal #216: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 7 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 8008
B. 2942
C. 119
D. 2940
E. 1470


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**D. 2940**

**Pembahasan:** C(9,3) $\times$ C(7,3) = 2940 cara.</details>

### Soal #217: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 7 siswa laki-laki dan 8 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 1176
B. 77
C. 3003
D. 588
E. 980


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**A. 1176**

**Pembahasan:** C(7,2) $\times$ C(8,3) = 1176 cara.</details>

### Soal #218: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 12 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 45
B. 420
C. 495
D. 210
E. 924


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 210**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 6 sisa dari 10 stok. C(10, 6) = 210 cara.</details>

### Soal #219: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 4 bola merah dan 7 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 165
B. 140
C. 39
D. 49
E. 84


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**C. 39**

**Pembahasan:** C(4,3) + C(7,3) = 39 cara.</details>

### Soal #220: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 5 siswa laki-laki dan 7 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 792
B. 350
C. 45
D. 210
E. 175


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 350**

**Pembahasan:** C(5,2) $\times$ C(7,3) = 350 cara.</details>

### Soal #221: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 11 soal yang ada. NAMUN, soal nomor 1 sampai 2 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 84
B. 126
C. 462
D. 252
E. 330


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**B. 126**

**Pembahasan:** Karena 2 soal wajib, kita tinggal milih 4 sisa dari 9 stok. C(9, 4) = 126 cara.</details>

### Soal #222: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 6 bola merah dan 7 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 55
B. 65
C. 126
D. 700
E. 286


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**A. 55**

**Pembahasan:** C(6,3) + C(7,3) = 55 cara.</details>

### Soal #223: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 7 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 70
B. 1
C. 120
D. 35
E. 210


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 35**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 4 sisa dari 7 stok. C(7, 4) = 35 cara.</details>

### Soal #224: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 7 bola merah dan 5 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 55
B. 45
C. 220
D. 350
E. 70


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**B. 45**

**Pembahasan:** C(7,3) + C(5,3) = 45 cara.</details>

### Soal #225: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 4 bola merah dan 4 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 56
B. 18
C. 24
D. 16
E. 8


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**E. 8**

**Pembahasan:** C(4,3) + C(4,3) = 8 cara.</details>

### Soal #226: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 5 siswa laki-laki dan 8 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 140
B. 38
C. 280
D. 1287
E. 560


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**C. 280**

**Pembahasan:** C(5,3) $\times$ C(8,2) = 280 cara.</details>

### Soal #227: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 10 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 10084
B. 10080
C. 5040
D. 27132
E. 204


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 10080**

**Pembahasan:** C(9,3) $\times$ C(10,3) = 10080 cara.</details>

### Soal #228: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 8 siswa laki-laki dan 7 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 77
B. 3003
C. 980
D. 588
E. 1176


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**E. 1176**

**Pembahasan:** C(8,3) $\times$ C(7,2) = 1176 cara.</details>

### Soal #229: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 14 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 924
B. 2002
C. 462
D. 3003
E. 165


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**C. 462**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 5 sisa dari 11 stok. C(11, 5) = 462 cara.</details>

### Soal #230: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 6 bola merah dan 5 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 60
B. 165
C. 200
D. 30
E. 40


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**D. 30**

**Pembahasan:** C(6,3) + C(5,3) = 30 cara.</details>

### Soal #231: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 12 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 87
B. 220
C. 84
D. 168
E. 924


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**C. 84**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 3 sisa dari 9 stok. C(9, 3) = 84 cara.</details>

### Soal #232: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 6 siswa laki-laki dan 5 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 152
B. 150
C. 75
D. 25
E. 330


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 150**

**Pembahasan:** C(6,2) $\times$ C(5,2) = 150 cara.</details>

### Soal #233: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 45
B. 42
C. 21
D. 0
E. 252


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**C. 21**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 5 sisa dari 7 stok. C(7, 5) = 21 cara.</details>

### Soal #234: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 6 siswa laki-laki dan 8 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 48
B. 280
C. 560
D. 2002
E. 840


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**C. 560**

**Pembahasan:** C(6,3) $\times$ C(8,2) = 560 cara.</details>

### Soal #235: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 5 bola merah dan 4 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 84
B. 24
C. 40
D. 30
E. 14


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**E. 14**

**Pembahasan:** C(5,3) + C(4,3) = 14 cara.</details>

### Soal #236: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 70
B. 35
C. 120
D. 7
E. 210


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**B. 35**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 3 sisa dari 7 stok. C(7, 3) = 35 cara.</details>

### Soal #237: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 5 siswa laki-laki dan 6 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 462
B. 30
C. 200
D. 150
E. 100


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**C. 200**

**Pembahasan:** C(5,2) $\times$ C(6,3) = 200 cara.</details>

### Soal #238: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 8 buah dari pilihan total 10 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 0
B. 42
C. 45
D. 21
E. 252


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**D. 21**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 5 sisa dari 7 stok. C(7, 5) = 21 cara.</details>

### Soal #239: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 5 bola merah dan 6 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 40
B. 200
C. 165
D. 30
E. 75


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**D. 30**

**Pembahasan:** C(5,3) + C(6,3) = 30 cara.</details>

### Soal #240: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 5 siswa laki-laki dan 8 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 140
B. 281
C. 280
D. 38
E. 715


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**C. 280**

**Pembahasan:** C(5,2) $\times$ C(8,2) = 280 cara.</details>

### Soal #241: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 8 siswa laki-laki dan 10 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 6720
B. 176
C. 18564
D. 3360
E. 6721


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**A. 6720**

**Pembahasan:** C(8,3) $\times$ C(10,3) = 6720 cara.</details>

### Soal #242: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 8 siswa laki-laki dan 9 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 2352
B. 112
C. 6188
D. 1176
E. 2016


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**A. 2352**

**Pembahasan:** C(8,2) $\times$ C(9,3) = 2352 cara.</details>

### Soal #243: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 6 bola merah dan 5 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 40
B. 200
C. 30
D. 165
E. 60


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**C. 30**

**Pembahasan:** C(6,3) + C(5,3) = 30 cara.</details>

### Soal #244: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 9 siswa laki-laki dan 7 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 2 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 1764
B. 1260
C. 4368
D. 71
E. 630


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**B. 1260**

**Pembahasan:** C(9,2) $\times$ C(7,3) = 1260 cara.</details>

### Soal #245: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam kotak terdapat 4 bola merah dan 7 bola putih. Akan diambil 3 bola SEKALIGUS. Berapa banyak cara pengambilan jika SEMUA yang terambil harus punya WARNA SAMA?

A. 84
B. 140
C. 165
D. 49
E. 39


<details><summary>💡 Hint</summary>Kasusnya bercabang: (3 Merah) ATAU (3 Putih). Ingat kata ATAU? Ya, Aturan Penjumlahan!</details>
<details><summary>✅ Jawaban</summary>**E. 39**

**Pembahasan:** C(4,3) + C(7,3) = 39 cara.</details>

### Soal #246: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 7 siswa laki-laki dan 5 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 2 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 210
B. 45
C. 350
D. 792
E. 175


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**C. 350**

**Pembahasan:** C(7,3) $\times$ C(5,2) = 350 cara.</details>

### Soal #247: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 13 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 286
B. 120
C. 210
D. 240
E. 1716


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**B. 120**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 3 sisa dari 10 stok. C(10, 3) = 120 cara.</details>

### Soal #248: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Di sebuah kelas terdapat 8 siswa laki-laki dan 10 siswa perempuan. Akan dibentuk kelompok diskusi yang MENGHARUSKAN berisi 3 siswa laki-laki DAN 3 siswa perempuan. Berapa banyak cara membentuk kelompok tersebut?

A. 6721
B. 3360
C. 18564
D. 6720
E. 176


<details><summary>💡 Hint</summary>Hitung Kombinasi laki-laki C({n},{k_n}), lalu hitung Kombinasi perempuan C({m},{k_m}). Karena pakai DAN (berturut-turut), hasil keduanya DIPAKAI DI ATURAN PERKALIAN.</details>
<details><summary>✅ Jawaban</summary>**D. 6720**

**Pembahasan:** C(8,3) $\times$ C(10,3) = 6720 cara.</details>

### Soal #249: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 7 buah dari pilihan total 11 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 330
B. 70
C. 8
D. 140
E. 71


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**B. 70**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 4 sisa dari 8 stok. C(8, 4) = 70 cara.</details>

### Soal #250: Pilihan Ganda - Kombinasi Lanjut Bersyarat
Dalam ujian OSN-K Matematika, peserta disuruh mengerjakan soal sebanyak 6 buah dari pilihan total 11 soal yang ada. NAMUN, soal nomor 1 sampai 3 SIFATNYA WAJIB DIKERJAKAN. Berapa banyak pilihan soal yang dapat diambil peserta?

A. 112
B. 165
C. 28
D. 462
E. 56


<details><summary>💡 Hint</summary>Karena {wajib} soal sudah pasti diambil, jatah milih bersisa ({r}-{wajib}) soal saja. Kumpulan soal bebas yang bisa dipilih sisa ({n}-{wajib}).</details>
<details><summary>✅ Jawaban</summary>**E. 56**

**Pembahasan:** Karena 3 soal wajib, kita tinggal milih 3 sisa dari 8 stok. C(8, 3) = 56 cara.</details>

---
[< Bagian 4](./09-kombinatorika-soal-part-4.md) | [Bagian 6 >](./09-kombinatorika-soal-part-6.md)
