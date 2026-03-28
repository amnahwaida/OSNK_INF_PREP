🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Simulasi & Brute Force (Part 6 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 251**
Sebuah robot bola diletakkan di lantai 145. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 49 detik
B. 50 detik
C. 53 detik
D. 51 detik
E. 52 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (50 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 145 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 145 + 5 = 150
- Detik 2: Genap, turun 11 -> 150 - 11 = 139
- Detik 3: Ganjil, naik 5 -> 139 + 5 = 144
- Detik 4: Genap, turun 11 -> 144 - 11 = 133
- Detik 5: Ganjil, naik 5 -> 133 + 5 = 138
- Detik 6: Genap, turun 11 -> 138 - 11 = 127
- Detik 7: Ganjil, naik 5 -> 127 + 5 = 132
- Detik 8: Genap, turun 11 -> 132 - 11 = 121
- Detik 9: Ganjil, naik 5 -> 121 + 5 = 126
- Detik 10: Genap, turun 11 -> 126 - 11 = 115
- Detik 11: Ganjil, naik 5 -> 115 + 5 = 120
- Detik 12: Genap, turun 11 -> 120 - 11 = 109
- Detik 13: Ganjil, naik 5 -> 109 + 5 = 114
- Detik 14: Genap, turun 11 -> 114 - 11 = 103
- Detik 15: Ganjil, naik 5 -> 103 + 5 = 108
- Detik 16: Genap, turun 11 -> 108 - 11 = 97
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 50: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 252**
Sebuah robot bola diletakkan di lantai 106. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 30 detik
B. 29 detik
C. 26 detik
D. 27 detik
E. 28 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (27 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 106 (Garis Start)
- Detik 1: Genap, turun 11 -> 106 - 11 = 95
- Detik 2: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 3: Genap, turun 11 -> 98 - 11 = 87
- Detik 4: Ganjil, naik 3 -> 87 + 3 = 90
- Detik 5: Genap, turun 11 -> 90 - 11 = 79
- Detik 6: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 7: Genap, turun 11 -> 82 - 11 = 71
- Detik 8: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 9: Genap, turun 11 -> 74 - 11 = 63
- Detik 10: Ganjil, naik 3 -> 63 + 3 = 66
- Detik 11: Genap, turun 11 -> 66 - 11 = 55
- Detik 12: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 13: Genap, turun 11 -> 58 - 11 = 47
- Detik 14: Ganjil, naik 3 -> 47 + 3 = 50
- Detik 15: Genap, turun 11 -> 50 - 11 = 39
- Detik 16: Ganjil, naik 3 -> 39 + 3 = 42
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 27: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 253**
Sebuah robot bola diletakkan di lantai 81. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 21 detik
B. 19 detik
C. 22 detik
D. 23 detik
E. 20 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (20 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 81 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 81 + 3 = 84
- Detik 2: Genap, turun 13 -> 84 - 13 = 71
- Detik 3: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 4: Genap, turun 13 -> 74 - 13 = 61
- Detik 5: Ganjil, naik 3 -> 61 + 3 = 64
- Detik 6: Genap, turun 13 -> 64 - 13 = 51
- Detik 7: Ganjil, naik 3 -> 51 + 3 = 54
- Detik 8: Genap, turun 13 -> 54 - 13 = 41
- Detik 9: Ganjil, naik 3 -> 41 + 3 = 44
- Detik 10: Genap, turun 13 -> 44 - 13 = 31
- Detik 11: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 12: Genap, turun 13 -> 34 - 13 = 21
- Detik 13: Ganjil, naik 3 -> 21 + 3 = 24
- Detik 14: Genap, turun 13 -> 24 - 13 = 11
- Detik 15: Ganjil, naik 3 -> 11 + 3 = 14
- Detik 16: Genap, turun 13 -> 14 - 13 = 1
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 20: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 254**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTBUUUBUBSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 6 unit langkah
C. 5 unit langkah
D. 7 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(0, 1)`
- Instruksi 4 (`U`): Koordinat kini `(0, 2)`
- Instruksi 5 (`U`): Koordinat kini `(0, 3)`
- Instruksi 6 (`U`): Koordinat kini `(0, 4)`
- Instruksi 7 (`B`): Koordinat kini `(-1, 4)`
- Instruksi 8 (`U`): Koordinat kini `(-1, 5)`
- Instruksi 9 (`B`): Koordinat kini `(-2, 5)`
- Instruksi 10 (`S`): Koordinat kini `(-2, 4)`
- Instruksi 11 (`S`): Koordinat kini `(-2, 3)`

Posisi akhir robot adalah di titik `(-2, 3)`.
Jarak Manhattan = Murni $|-2| + |3|$ = 2 + 3 = **5 unit**.
Opsi valid: **C**.</details>

---
**Soal 255**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 23, 18, 17, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 26."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 4 pasang
C. 1 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 23 = 47 (❌ Gagal)
- Sapi 24 + Sapi 18 = 42 (❌ Gagal)
- Sapi 24 + Sapi 17 = 41 (❌ Gagal)
- Sapi 24 + Sapi 2 = 26 (✅ COCOK)
- Sapi 23 + Sapi 18 = 41 (❌ Gagal)
- Sapi 23 + Sapi 17 = 40 (❌ Gagal)
- Sapi 23 + Sapi 2 = 25 (❌ Gagal)
- Sapi 18 + Sapi 17 = 35 (❌ Gagal)
- Sapi 18 + Sapi 2 = 20 (❌ Gagal)
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)

Total pasangan yang bernilai 26 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 256**
Sebuah robot bola diletakkan di lantai 102. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 19 detik
B. 21 detik
C. 20 detik
D. 18 detik
E. 22 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (19 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 102 (Garis Start)
- Detik 1: Genap, turun 13 -> 102 - 13 = 89
- Detik 2: Ganjil, naik 3 -> 89 + 3 = 92
- Detik 3: Genap, turun 13 -> 92 - 13 = 79
- Detik 4: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 5: Genap, turun 13 -> 82 - 13 = 69
- Detik 6: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 7: Genap, turun 13 -> 72 - 13 = 59
- Detik 8: Ganjil, naik 3 -> 59 + 3 = 62
- Detik 9: Genap, turun 13 -> 62 - 13 = 49
- Detik 10: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 11: Genap, turun 13 -> 52 - 13 = 39
- Detik 12: Ganjil, naik 3 -> 39 + 3 = 42
- Detik 13: Genap, turun 13 -> 42 - 13 = 29
- Detik 14: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 15: Genap, turun 13 -> 32 - 13 = 19
- Detik 16: Ganjil, naik 3 -> 19 + 3 = 22
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 19: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 257**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[9, 17, 2, 6, 20]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 42."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 4 pasang
C. 0 pasang
D. 3 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 9 + Sapi 17 = 26 (❌ Gagal)
- Sapi 9 + Sapi 2 = 11 (❌ Gagal)
- Sapi 9 + Sapi 6 = 15 (❌ Gagal)
- Sapi 9 + Sapi 20 = 29 (❌ Gagal)
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)
- Sapi 17 + Sapi 6 = 23 (❌ Gagal)
- Sapi 17 + Sapi 20 = 37 (❌ Gagal)
- Sapi 2 + Sapi 6 = 8 (❌ Gagal)
- Sapi 2 + Sapi 20 = 22 (❌ Gagal)
- Sapi 6 + Sapi 20 = 26 (❌ Gagal)

Total pasangan yang bernilai 42 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 258**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BTBSSBBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 6 unit langkah
C. 5 unit langkah
D. 7 unit langkah
E. 8 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(0, 0)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 5 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 6 (`B`): Koordinat kini `(-2, -2)`
- Instruksi 7 (`B`): Koordinat kini `(-3, -2)`
- Instruksi 8 (`B`): Koordinat kini `(-4, -2)`

Posisi akhir robot adalah di titik `(-4, -2)`.
Jarak Manhattan = Murni $|-4| + |-2|$ = 4 + 2 = **6 unit**.
Opsi valid: **B**.</details>

---
**Soal 259**
Sebuah robot bola diletakkan di lantai 68. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 23 detik
B. 22 detik
C. 24 detik
D. 26 detik
E. 25 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (23 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 68 (Garis Start)
- Detik 1: Genap, turun 9 -> 68 - 9 = 59
- Detik 2: Ganjil, naik 3 -> 59 + 3 = 62
- Detik 3: Genap, turun 9 -> 62 - 9 = 53
- Detik 4: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 5: Genap, turun 9 -> 56 - 9 = 47
- Detik 6: Ganjil, naik 3 -> 47 + 3 = 50
- Detik 7: Genap, turun 9 -> 50 - 9 = 41
- Detik 8: Ganjil, naik 3 -> 41 + 3 = 44
- Detik 9: Genap, turun 9 -> 44 - 9 = 35
- Detik 10: Ganjil, naik 3 -> 35 + 3 = 38
- Detik 11: Genap, turun 9 -> 38 - 9 = 29
- Detik 12: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 13: Genap, turun 9 -> 32 - 9 = 23
- Detik 14: Ganjil, naik 3 -> 23 + 3 = 26
- Detik 15: Genap, turun 9 -> 26 - 9 = 17
- Detik 16: Ganjil, naik 3 -> 17 + 3 = 20
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 23: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 260**
Sebuah robot bola diletakkan di lantai 138. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 29 detik
C. 31 detik
D. 32 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (29 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 138 (Garis Start)
- Detik 1: Genap, turun 13 -> 138 - 13 = 125
- Detik 2: Ganjil, naik 3 -> 125 + 3 = 128
- Detik 3: Genap, turun 13 -> 128 - 13 = 115
- Detik 4: Ganjil, naik 3 -> 115 + 3 = 118
- Detik 5: Genap, turun 13 -> 118 - 13 = 105
- Detik 6: Ganjil, naik 3 -> 105 + 3 = 108
- Detik 7: Genap, turun 13 -> 108 - 13 = 95
- Detik 8: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 9: Genap, turun 13 -> 98 - 13 = 85
- Detik 10: Ganjil, naik 3 -> 85 + 3 = 88
- Detik 11: Genap, turun 13 -> 88 - 13 = 75
- Detik 12: Ganjil, naik 3 -> 75 + 3 = 78
- Detik 13: Genap, turun 13 -> 78 - 13 = 65
- Detik 14: Ganjil, naik 3 -> 65 + 3 = 68
- Detik 15: Genap, turun 13 -> 68 - 13 = 55
- Detik 16: Ganjil, naik 3 -> 55 + 3 = 58
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 29: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 261**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUSUSTUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 1 unit langkah
C. 2 unit langkah
D. 0 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`S`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(1, 0)`
- Instruksi 6 (`T`): Koordinat kini `(2, 0)`
- Instruksi 7 (`U`): Koordinat kini `(2, 1)`
- Instruksi 8 (`S`): Koordinat kini `(2, 0)`

Posisi akhir robot adalah di titik `(2, 0)`.
Jarak Manhattan = Murni $|2| + |0|$ = 2 + 0 = **2 unit**.
Opsi valid: **C**.</details>

---
**Soal 262**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[15, 14, 10, 6, 20]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 3 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 15 + Sapi 14 = 29 (❌ Gagal)
- Sapi 15 + Sapi 10 = 25 (❌ Gagal)
- Sapi 15 + Sapi 6 = 21 (❌ Gagal)
- Sapi 15 + Sapi 20 = 35 (❌ Gagal)
- Sapi 14 + Sapi 10 = 24 (❌ Gagal)
- Sapi 14 + Sapi 6 = 20 (❌ Gagal)
- Sapi 14 + Sapi 20 = 34 (❌ Gagal)
- Sapi 10 + Sapi 6 = 16 (❌ Gagal)
- Sapi 10 + Sapi 20 = 30 (❌ Gagal)
- Sapi 6 + Sapi 20 = 26 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 263**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BUTSTTSUBSU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 3 unit langkah
C. 2 unit langkah
D. 0 unit langkah
E. -1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`T`): Koordinat kini `(1, 0)`
- Instruksi 6 (`T`): Koordinat kini `(2, 0)`
- Instruksi 7 (`S`): Koordinat kini `(2, -1)`
- Instruksi 8 (`U`): Koordinat kini `(2, 0)`
- Instruksi 9 (`B`): Koordinat kini `(1, 0)`
- Instruksi 10 (`S`): Koordinat kini `(1, -1)`
- Instruksi 11 (`U`): Koordinat kini `(1, 0)`

Posisi akhir robot adalah di titik `(1, 0)`.
Jarak Manhattan = Murni $|1| + |0|$ = 1 + 0 = **1 unit**.
Opsi valid: **A**.</details>

---
**Soal 264**
Sebuah robot bola diletakkan di lantai 97. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 27 detik
B. 29 detik
C. 31 detik
D. 28 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (28 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 97 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 2: Genap, turun 13 -> 102 - 13 = 89
- Detik 3: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 4: Genap, turun 13 -> 94 - 13 = 81
- Detik 5: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 6: Genap, turun 13 -> 86 - 13 = 73
- Detik 7: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 8: Genap, turun 13 -> 78 - 13 = 65
- Detik 9: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 10: Genap, turun 13 -> 70 - 13 = 57
- Detik 11: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 12: Genap, turun 13 -> 62 - 13 = 49
- Detik 13: Ganjil, naik 5 -> 49 + 5 = 54
- Detik 14: Genap, turun 13 -> 54 - 13 = 41
- Detik 15: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 16: Genap, turun 13 -> 46 - 13 = 33
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 28: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 265**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[15, 24, 14, 21, 23]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 26."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 2 pasang
C. 4 pasang
D. 1 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 15 + Sapi 24 = 39 (❌ Gagal)
- Sapi 15 + Sapi 14 = 29 (❌ Gagal)
- Sapi 15 + Sapi 21 = 36 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 24 + Sapi 14 = 38 (❌ Gagal)
- Sapi 24 + Sapi 21 = 45 (❌ Gagal)
- Sapi 24 + Sapi 23 = 47 (❌ Gagal)
- Sapi 14 + Sapi 21 = 35 (❌ Gagal)
- Sapi 14 + Sapi 23 = 37 (❌ Gagal)
- Sapi 21 + Sapi 23 = 44 (❌ Gagal)

Total pasangan yang bernilai 26 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 266**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[18, 11, 4, 10, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 43."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 0 pasang
C. 1 pasang
D. 3 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 18 + Sapi 11 = 29 (❌ Gagal)
- Sapi 18 + Sapi 4 = 22 (❌ Gagal)
- Sapi 18 + Sapi 10 = 28 (❌ Gagal)
- Sapi 18 + Sapi 15 = 33 (❌ Gagal)
- Sapi 11 + Sapi 4 = 15 (❌ Gagal)
- Sapi 11 + Sapi 10 = 21 (❌ Gagal)
- Sapi 11 + Sapi 15 = 26 (❌ Gagal)
- Sapi 4 + Sapi 10 = 14 (❌ Gagal)
- Sapi 4 + Sapi 15 = 19 (❌ Gagal)
- Sapi 10 + Sapi 15 = 25 (❌ Gagal)

Total pasangan yang bernilai 43 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 267**
Sebuah robot bola diletakkan di lantai 59. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 15 detik
B. 17 detik
C. 14 detik
D. 16 detik
E. 13 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (14 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 59 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 59 + 3 = 62
- Detik 2: Genap, turun 13 -> 62 - 13 = 49
- Detik 3: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 4: Genap, turun 13 -> 52 - 13 = 39
- Detik 5: Ganjil, naik 3 -> 39 + 3 = 42
- Detik 6: Genap, turun 13 -> 42 - 13 = 29
- Detik 7: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 8: Genap, turun 13 -> 32 - 13 = 19
- Detik 9: Ganjil, naik 3 -> 19 + 3 = 22
- Detik 10: Genap, turun 13 -> 22 - 13 = 9
- Detik 11: Ganjil, naik 3 -> 9 + 3 = 12
- Detik 12: Genap, turun 13 -> 12 - 13 = -1
- Detik 13: Ganjil, naik 3 -> -1 + 3 = 2
- Detik 14: Genap, turun 13 -> 2 - 13 = -11
Simulasi berakhir pada detik ke-14. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 268**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 7, 14, 13, 22]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 3 pasang
C. 4 pasang
D. 1 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 14 = 17 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 3 + Sapi 22 = 25 (❌ Gagal)
- Sapi 7 + Sapi 14 = 21 (❌ Gagal)
- Sapi 7 + Sapi 13 = 20 (❌ Gagal)
- Sapi 7 + Sapi 22 = 29 (❌ Gagal)
- Sapi 14 + Sapi 13 = 27 (❌ Gagal)
- Sapi 14 + Sapi 22 = 36 (❌ Gagal)
- Sapi 13 + Sapi 22 = 35 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 269**
Sebuah robot bola diletakkan di lantai 73. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 29 detik
C. 30 detik
D. 31 detik
E. 27 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (28 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 73 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 73 + 1 = 74
- Detik 2: Genap, turun 7 -> 74 - 7 = 67
- Detik 3: Ganjil, naik 1 -> 67 + 1 = 68
- Detik 4: Genap, turun 7 -> 68 - 7 = 61
- Detik 5: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 6: Genap, turun 7 -> 62 - 7 = 55
- Detik 7: Ganjil, naik 1 -> 55 + 1 = 56
- Detik 8: Genap, turun 7 -> 56 - 7 = 49
- Detik 9: Ganjil, naik 1 -> 49 + 1 = 50
- Detik 10: Genap, turun 7 -> 50 - 7 = 43
- Detik 11: Ganjil, naik 1 -> 43 + 1 = 44
- Detik 12: Genap, turun 7 -> 44 - 7 = 37
- Detik 13: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 14: Genap, turun 7 -> 38 - 7 = 31
- Detik 15: Ganjil, naik 1 -> 31 + 1 = 32
- Detik 16: Genap, turun 7 -> 32 - 7 = 25
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 28: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 270**
Sebuah robot bola diletakkan di lantai 70. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 21 detik
B. 18 detik
C. 22 detik
D. 19 detik
E. 20 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (19 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 70 (Garis Start)
- Detik 1: Genap, turun 9 -> 70 - 9 = 61
- Detik 2: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 3: Genap, turun 9 -> 62 - 9 = 53
- Detik 4: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 5: Genap, turun 9 -> 54 - 9 = 45
- Detik 6: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 7: Genap, turun 9 -> 46 - 9 = 37
- Detik 8: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 9: Genap, turun 9 -> 38 - 9 = 29
- Detik 10: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 11: Genap, turun 9 -> 30 - 9 = 21
- Detik 12: Ganjil, naik 1 -> 21 + 1 = 22
- Detik 13: Genap, turun 9 -> 22 - 9 = 13
- Detik 14: Ganjil, naik 1 -> 13 + 1 = 14
- Detik 15: Genap, turun 9 -> 14 - 9 = 5
- Detik 16: Ganjil, naik 1 -> 5 + 1 = 6
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 19: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 271**
Sebuah robot bola diletakkan di lantai 123. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 34 detik
B. 35 detik
C. 31 detik
D. 33 detik
E. 32 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (32 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 123 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 123 + 5 = 128
- Detik 2: Genap, turun 13 -> 128 - 13 = 115
- Detik 3: Ganjil, naik 5 -> 115 + 5 = 120
- Detik 4: Genap, turun 13 -> 120 - 13 = 107
- Detik 5: Ganjil, naik 5 -> 107 + 5 = 112
- Detik 6: Genap, turun 13 -> 112 - 13 = 99
- Detik 7: Ganjil, naik 5 -> 99 + 5 = 104
- Detik 8: Genap, turun 13 -> 104 - 13 = 91
- Detik 9: Ganjil, naik 5 -> 91 + 5 = 96
- Detik 10: Genap, turun 13 -> 96 - 13 = 83
- Detik 11: Ganjil, naik 5 -> 83 + 5 = 88
- Detik 12: Genap, turun 13 -> 88 - 13 = 75
- Detik 13: Ganjil, naik 5 -> 75 + 5 = 80
- Detik 14: Genap, turun 13 -> 80 - 13 = 67
- Detik 15: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 16: Genap, turun 13 -> 72 - 13 = 59
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 32: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 272**
Sebuah robot bola diletakkan di lantai 65. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 17 detik
B. 19 detik
C. 20 detik
D. 18 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (18 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 65 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 2: Genap, turun 13 -> 70 - 13 = 57
- Detik 3: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 4: Genap, turun 13 -> 62 - 13 = 49
- Detik 5: Ganjil, naik 5 -> 49 + 5 = 54
- Detik 6: Genap, turun 13 -> 54 - 13 = 41
- Detik 7: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 8: Genap, turun 13 -> 46 - 13 = 33
- Detik 9: Ganjil, naik 5 -> 33 + 5 = 38
- Detik 10: Genap, turun 13 -> 38 - 13 = 25
- Detik 11: Ganjil, naik 5 -> 25 + 5 = 30
- Detik 12: Genap, turun 13 -> 30 - 13 = 17
- Detik 13: Ganjil, naik 5 -> 17 + 5 = 22
- Detik 14: Genap, turun 13 -> 22 - 13 = 9
- Detik 15: Ganjil, naik 5 -> 9 + 5 = 14
- Detik 16: Genap, turun 13 -> 14 - 13 = 1
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 18: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 273**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 6, 12, 11, 8]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 3 pasang
D. 0 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 19 + Sapi 6 = 25 (❌ Gagal)
- Sapi 19 + Sapi 12 = 31 (❌ Gagal)
- Sapi 19 + Sapi 11 = 30 (❌ Gagal)
- Sapi 19 + Sapi 8 = 27 (❌ Gagal)
- Sapi 6 + Sapi 12 = 18 (❌ Gagal)
- Sapi 6 + Sapi 11 = 17 (❌ Gagal)
- Sapi 6 + Sapi 8 = 14 (❌ Gagal)
- Sapi 12 + Sapi 11 = 23 (❌ Gagal)
- Sapi 12 + Sapi 8 = 20 (❌ Gagal)
- Sapi 11 + Sapi 8 = 19 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 274**
Sebuah robot bola diletakkan di lantai 143. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 151 detik
B. 148 detik
C. 150 detik
D. 147 detik
E. 149 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (148 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 143 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 143 + 5 = 148
- Detik 2: Genap, turun 7 -> 148 - 7 = 141
- Detik 3: Ganjil, naik 5 -> 141 + 5 = 146
- Detik 4: Genap, turun 7 -> 146 - 7 = 139
- Detik 5: Ganjil, naik 5 -> 139 + 5 = 144
- Detik 6: Genap, turun 7 -> 144 - 7 = 137
- Detik 7: Ganjil, naik 5 -> 137 + 5 = 142
- Detik 8: Genap, turun 7 -> 142 - 7 = 135
- Detik 9: Ganjil, naik 5 -> 135 + 5 = 140
- Detik 10: Genap, turun 7 -> 140 - 7 = 133
- Detik 11: Ganjil, naik 5 -> 133 + 5 = 138
- Detik 12: Genap, turun 7 -> 138 - 7 = 131
- Detik 13: Ganjil, naik 5 -> 131 + 5 = 136
- Detik 14: Genap, turun 7 -> 136 - 7 = 129
- Detik 15: Ganjil, naik 5 -> 129 + 5 = 134
- Detik 16: Genap, turun 7 -> 134 - 7 = 127
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 148: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 275**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TTSBUBUBUUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 1 unit langkah
C. 3 unit langkah
D. 2 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(2, 0)`
- Instruksi 3 (`S`): Koordinat kini `(2, -1)`
- Instruksi 4 (`B`): Koordinat kini `(1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(1, 0)`
- Instruksi 6 (`B`): Koordinat kini `(0, 0)`
- Instruksi 7 (`U`): Koordinat kini `(0, 1)`
- Instruksi 8 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 9 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 10 (`U`): Koordinat kini `(-1, 3)`
- Instruksi 11 (`S`): Koordinat kini `(-1, 2)`

Posisi akhir robot adalah di titik `(-1, 2)`.
Jarak Manhattan = Murni $|-1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 276**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[11, 20, 5, 21, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 0 pasang
D. 1 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 11 + Sapi 20 = 31 (❌ Gagal)
- Sapi 11 + Sapi 5 = 16 (❌ Gagal)
- Sapi 11 + Sapi 21 = 32 (❌ Gagal)
- Sapi 11 + Sapi 10 = 21 (❌ Gagal)
- Sapi 20 + Sapi 5 = 25 (❌ Gagal)
- Sapi 20 + Sapi 21 = 41 (❌ Gagal)
- Sapi 20 + Sapi 10 = 30 (❌ Gagal)
- Sapi 5 + Sapi 21 = 26 (❌ Gagal)
- Sapi 5 + Sapi 10 = 15 (❌ Gagal)
- Sapi 21 + Sapi 10 = 31 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 277**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBBSUBSTSSTBUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. 1 unit langkah
C. 2 unit langkah
D. 4 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 8 (`T`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 10 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 11 (`T`): Koordinat kini `(0, -3)`
- Instruksi 12 (`B`): Koordinat kini `(-1, -3)`
- Instruksi 13 (`U`): Koordinat kini `(-1, -2)`
- Instruksi 14 (`T`): Koordinat kini `(0, -2)`

Posisi akhir robot adalah di titik `(0, -2)`.
Jarak Manhattan = Murni $|0| + |-2|$ = 0 + 2 = **2 unit**.
Opsi valid: **C**.</details>

---
**Soal 278**
Sebuah robot bola diletakkan di lantai 134. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 46 detik
B. 49 detik
C. 47 detik
D. 48 detik
E. 50 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (47 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 134 (Garis Start)
- Detik 1: Genap, turun 11 -> 134 - 11 = 123
- Detik 2: Ganjil, naik 5 -> 123 + 5 = 128
- Detik 3: Genap, turun 11 -> 128 - 11 = 117
- Detik 4: Ganjil, naik 5 -> 117 + 5 = 122
- Detik 5: Genap, turun 11 -> 122 - 11 = 111
- Detik 6: Ganjil, naik 5 -> 111 + 5 = 116
- Detik 7: Genap, turun 11 -> 116 - 11 = 105
- Detik 8: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 9: Genap, turun 11 -> 110 - 11 = 99
- Detik 10: Ganjil, naik 5 -> 99 + 5 = 104
- Detik 11: Genap, turun 11 -> 104 - 11 = 93
- Detik 12: Ganjil, naik 5 -> 93 + 5 = 98
- Detik 13: Genap, turun 11 -> 98 - 11 = 87
- Detik 14: Ganjil, naik 5 -> 87 + 5 = 92
- Detik 15: Genap, turun 11 -> 92 - 11 = 81
- Detik 16: Ganjil, naik 5 -> 81 + 5 = 86
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 47: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 279**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[8, 19, 21, 23, 11]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 38."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 2 pasang
C. 4 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 8 + Sapi 19 = 27 (❌ Gagal)
- Sapi 8 + Sapi 21 = 29 (❌ Gagal)
- Sapi 8 + Sapi 23 = 31 (❌ Gagal)
- Sapi 8 + Sapi 11 = 19 (❌ Gagal)
- Sapi 19 + Sapi 21 = 40 (❌ Gagal)
- Sapi 19 + Sapi 23 = 42 (❌ Gagal)
- Sapi 19 + Sapi 11 = 30 (❌ Gagal)
- Sapi 21 + Sapi 23 = 44 (❌ Gagal)
- Sapi 21 + Sapi 11 = 32 (❌ Gagal)
- Sapi 23 + Sapi 11 = 34 (❌ Gagal)

Total pasangan yang bernilai 38 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 280**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTTUUSBUSBUSSU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 0 unit langkah
C. 1 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(2, 1)`
- Instruksi 4 (`U`): Koordinat kini `(2, 2)`
- Instruksi 5 (`U`): Koordinat kini `(2, 3)`
- Instruksi 6 (`S`): Koordinat kini `(2, 2)`
- Instruksi 7 (`B`): Koordinat kini `(1, 2)`
- Instruksi 8 (`U`): Koordinat kini `(1, 3)`
- Instruksi 9 (`S`): Koordinat kini `(1, 2)`
- Instruksi 10 (`B`): Koordinat kini `(0, 2)`
- Instruksi 11 (`U`): Koordinat kini `(0, 3)`
- Instruksi 12 (`S`): Koordinat kini `(0, 2)`
- Instruksi 13 (`S`): Koordinat kini `(0, 1)`
- Instruksi 14 (`U`): Koordinat kini `(0, 2)`

Posisi akhir robot adalah di titik `(0, 2)`.
Jarak Manhattan = Murni $|0| + |2|$ = 0 + 2 = **2 unit**.
Opsi valid: **E**.</details>

---
**Soal 281**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 18, 3, 24, 11]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 49."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 0 pasang
C. 4 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 18 = 28 (❌ Gagal)
- Sapi 10 + Sapi 3 = 13 (❌ Gagal)
- Sapi 10 + Sapi 24 = 34 (❌ Gagal)
- Sapi 10 + Sapi 11 = 21 (❌ Gagal)
- Sapi 18 + Sapi 3 = 21 (❌ Gagal)
- Sapi 18 + Sapi 24 = 42 (❌ Gagal)
- Sapi 18 + Sapi 11 = 29 (❌ Gagal)
- Sapi 3 + Sapi 24 = 27 (❌ Gagal)
- Sapi 3 + Sapi 11 = 14 (❌ Gagal)
- Sapi 24 + Sapi 11 = 35 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 282**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[4, 15, 2, 10, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 28."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 4 pasang
C. 2 pasang
D. 1 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 4 + Sapi 15 = 19 (❌ Gagal)
- Sapi 4 + Sapi 2 = 6 (❌ Gagal)
- Sapi 4 + Sapi 10 = 14 (❌ Gagal)
- Sapi 4 + Sapi 17 = 21 (❌ Gagal)
- Sapi 15 + Sapi 2 = 17 (❌ Gagal)
- Sapi 15 + Sapi 10 = 25 (❌ Gagal)
- Sapi 15 + Sapi 17 = 32 (❌ Gagal)
- Sapi 2 + Sapi 10 = 12 (❌ Gagal)
- Sapi 2 + Sapi 17 = 19 (❌ Gagal)
- Sapi 10 + Sapi 17 = 27 (❌ Gagal)

Total pasangan yang bernilai 28 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 283**
Sebuah robot bola diletakkan di lantai 149. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 54 detik
B. 53 detik
C. 55 detik
D. 57 detik
E. 56 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (54 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 149 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 149 + 3 = 152
- Detik 2: Genap, turun 9 -> 152 - 9 = 143
- Detik 3: Ganjil, naik 3 -> 143 + 3 = 146
- Detik 4: Genap, turun 9 -> 146 - 9 = 137
- Detik 5: Ganjil, naik 3 -> 137 + 3 = 140
- Detik 6: Genap, turun 9 -> 140 - 9 = 131
- Detik 7: Ganjil, naik 3 -> 131 + 3 = 134
- Detik 8: Genap, turun 9 -> 134 - 9 = 125
- Detik 9: Ganjil, naik 3 -> 125 + 3 = 128
- Detik 10: Genap, turun 9 -> 128 - 9 = 119
- Detik 11: Ganjil, naik 3 -> 119 + 3 = 122
- Detik 12: Genap, turun 9 -> 122 - 9 = 113
- Detik 13: Ganjil, naik 3 -> 113 + 3 = 116
- Detik 14: Genap, turun 9 -> 116 - 9 = 107
- Detik 15: Ganjil, naik 3 -> 107 + 3 = 110
- Detik 16: Genap, turun 9 -> 110 - 9 = 101
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 54: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 284**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBBBSSBT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 3 unit langkah
C. 2 unit langkah
D. 6 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-3, 1)`
- Instruksi 5 (`S`): Koordinat kini `(-3, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-3, -1)`
- Instruksi 7 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 8 (`T`): Koordinat kini `(-3, -1)`

Posisi akhir robot adalah di titik `(-3, -1)`.
Jarak Manhattan = Murni $|-3| + |-1|$ = 3 + 1 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 285**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUBTTSTUTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 5 unit langkah
C. 4 unit langkah
D. 8 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 4 (`T`): Koordinat kini `(0, 2)`
- Instruksi 5 (`T`): Koordinat kini `(1, 2)`
- Instruksi 6 (`S`): Koordinat kini `(1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(2, 1)`
- Instruksi 8 (`U`): Koordinat kini `(2, 2)`
- Instruksi 9 (`T`): Koordinat kini `(3, 2)`
- Instruksi 10 (`T`): Koordinat kini `(4, 2)`

Posisi akhir robot adalah di titik `(4, 2)`.
Jarak Manhattan = Murni $|4| + |2|$ = 4 + 2 = **6 unit**.
Opsi valid: **A**.</details>

---
**Soal 286**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSSTUSSUSUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 1 unit langkah
C. 3 unit langkah
D. 4 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 4 (`T`): Koordinat kini `(0, -2)`
- Instruksi 5 (`U`): Koordinat kini `(0, -1)`
- Instruksi 6 (`S`): Koordinat kini `(0, -2)`
- Instruksi 7 (`S`): Koordinat kini `(0, -3)`
- Instruksi 8 (`U`): Koordinat kini `(0, -2)`
- Instruksi 9 (`S`): Koordinat kini `(0, -3)`
- Instruksi 10 (`U`): Koordinat kini `(0, -2)`
- Instruksi 11 (`S`): Koordinat kini `(0, -3)`

Posisi akhir robot adalah di titik `(0, -3)`.
Jarak Manhattan = Murni $|0| + |-3|$ = 0 + 3 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 287**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BUUBTUSUUTSBBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 2 unit langkah
C. 4 unit langkah
D. 6 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 4 (`B`): Koordinat kini `(-2, 2)`
- Instruksi 5 (`T`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`U`): Koordinat kini `(-1, 3)`
- Instruksi 7 (`S`): Koordinat kini `(-1, 2)`
- Instruksi 8 (`U`): Koordinat kini `(-1, 3)`
- Instruksi 9 (`U`): Koordinat kini `(-1, 4)`
- Instruksi 10 (`T`): Koordinat kini `(0, 4)`
- Instruksi 11 (`S`): Koordinat kini `(0, 3)`
- Instruksi 12 (`B`): Koordinat kini `(-1, 3)`
- Instruksi 13 (`B`): Koordinat kini `(-2, 3)`
- Instruksi 14 (`S`): Koordinat kini `(-2, 2)`

Posisi akhir robot adalah di titik `(-2, 2)`.
Jarak Manhattan = Murni $|-2| + |2|$ = 2 + 2 = **4 unit**.
Opsi valid: **C**.</details>

---
**Soal 288**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[12, 22, 7, 6, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 4 pasang
D. 2 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 12 + Sapi 22 = 34 (❌ Gagal)
- Sapi 12 + Sapi 7 = 19 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 12 + Sapi 10 = 22 (❌ Gagal)
- Sapi 22 + Sapi 7 = 29 (✅ COCOK)
- Sapi 22 + Sapi 6 = 28 (❌ Gagal)
- Sapi 22 + Sapi 10 = 32 (❌ Gagal)
- Sapi 7 + Sapi 6 = 13 (❌ Gagal)
- Sapi 7 + Sapi 10 = 17 (❌ Gagal)
- Sapi 6 + Sapi 10 = 16 (❌ Gagal)

Total pasangan yang bernilai 29 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 289**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 4, 7, 9, 13]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 2 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 4 = 7 (❌ Gagal)
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 4 + Sapi 7 = 11 (❌ Gagal)
- Sapi 4 + Sapi 9 = 13 (❌ Gagal)
- Sapi 4 + Sapi 13 = 17 (❌ Gagal)
- Sapi 7 + Sapi 9 = 16 (❌ Gagal)
- Sapi 7 + Sapi 13 = 20 (❌ Gagal)
- Sapi 9 + Sapi 13 = 22 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 290**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 11, 16, 24, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 45."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 4 pasang
C. 3 pasang
D. 0 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 11 = 14 (❌ Gagal)
- Sapi 3 + Sapi 16 = 19 (❌ Gagal)
- Sapi 3 + Sapi 24 = 27 (❌ Gagal)
- Sapi 3 + Sapi 6 = 9 (❌ Gagal)
- Sapi 11 + Sapi 16 = 27 (❌ Gagal)
- Sapi 11 + Sapi 24 = 35 (❌ Gagal)
- Sapi 11 + Sapi 6 = 17 (❌ Gagal)
- Sapi 16 + Sapi 24 = 40 (❌ Gagal)
- Sapi 16 + Sapi 6 = 22 (❌ Gagal)
- Sapi 24 + Sapi 6 = 30 (❌ Gagal)

Total pasangan yang bernilai 45 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 291**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 7, 20, 22, 9]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 1 pasang
D. 3 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 23 + Sapi 7 = 30 (❌ Gagal)
- Sapi 23 + Sapi 20 = 43 (❌ Gagal)
- Sapi 23 + Sapi 22 = 45 (❌ Gagal)
- Sapi 23 + Sapi 9 = 32 (❌ Gagal)
- Sapi 7 + Sapi 20 = 27 (❌ Gagal)
- Sapi 7 + Sapi 22 = 29 (❌ Gagal)
- Sapi 7 + Sapi 9 = 16 (❌ Gagal)
- Sapi 20 + Sapi 22 = 42 (❌ Gagal)
- Sapi 20 + Sapi 9 = 29 (❌ Gagal)
- Sapi 22 + Sapi 9 = 31 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 292**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 5, 3, 9, 18]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 27."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 0 pasang
C. 3 pasang
D. 2 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 19 + Sapi 5 = 24 (❌ Gagal)
- Sapi 19 + Sapi 3 = 22 (❌ Gagal)
- Sapi 19 + Sapi 9 = 28 (❌ Gagal)
- Sapi 19 + Sapi 18 = 37 (❌ Gagal)
- Sapi 5 + Sapi 3 = 8 (❌ Gagal)
- Sapi 5 + Sapi 9 = 14 (❌ Gagal)
- Sapi 5 + Sapi 18 = 23 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 18 = 21 (❌ Gagal)
- Sapi 9 + Sapi 18 = 27 (✅ COCOK)

Total pasangan yang bernilai 27 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 293**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[8, 3, 7, 14, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 49."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 1 pasang
C. 4 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 8 + Sapi 3 = 11 (❌ Gagal)
- Sapi 8 + Sapi 7 = 15 (❌ Gagal)
- Sapi 8 + Sapi 14 = 22 (❌ Gagal)
- Sapi 8 + Sapi 4 = 12 (❌ Gagal)
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 14 = 17 (❌ Gagal)
- Sapi 3 + Sapi 4 = 7 (❌ Gagal)
- Sapi 7 + Sapi 14 = 21 (❌ Gagal)
- Sapi 7 + Sapi 4 = 11 (❌ Gagal)
- Sapi 14 + Sapi 4 = 18 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 294**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 3, 8, 20, 13]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 1 pasang
C. 4 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 19 + Sapi 3 = 22 (❌ Gagal)
- Sapi 19 + Sapi 8 = 27 (❌ Gagal)
- Sapi 19 + Sapi 20 = 39 (❌ Gagal)
- Sapi 19 + Sapi 13 = 32 (❌ Gagal)
- Sapi 3 + Sapi 8 = 11 (❌ Gagal)
- Sapi 3 + Sapi 20 = 23 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 8 + Sapi 20 = 28 (❌ Gagal)
- Sapi 8 + Sapi 13 = 21 (❌ Gagal)
- Sapi 20 + Sapi 13 = 33 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 295**
Sebuah robot bola diletakkan di lantai 56. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 27 detik
C. 26 detik
D. 25 detik
E. 24 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (25 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 56 (Garis Start)
- Detik 1: Genap, turun 9 -> 56 - 9 = 47
- Detik 2: Ganjil, naik 5 -> 47 + 5 = 52
- Detik 3: Genap, turun 9 -> 52 - 9 = 43
- Detik 4: Ganjil, naik 5 -> 43 + 5 = 48
- Detik 5: Genap, turun 9 -> 48 - 9 = 39
- Detik 6: Ganjil, naik 5 -> 39 + 5 = 44
- Detik 7: Genap, turun 9 -> 44 - 9 = 35
- Detik 8: Ganjil, naik 5 -> 35 + 5 = 40
- Detik 9: Genap, turun 9 -> 40 - 9 = 31
- Detik 10: Ganjil, naik 5 -> 31 + 5 = 36
- Detik 11: Genap, turun 9 -> 36 - 9 = 27
- Detik 12: Ganjil, naik 5 -> 27 + 5 = 32
- Detik 13: Genap, turun 9 -> 32 - 9 = 23
- Detik 14: Ganjil, naik 5 -> 23 + 5 = 28
- Detik 15: Genap, turun 9 -> 28 - 9 = 19
- Detik 16: Ganjil, naik 5 -> 19 + 5 = 24
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 25: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 296**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BBBTSSUUTTSTSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 4 unit langkah
C. 5 unit langkah
D. 6 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 3 (`B`): Koordinat kini `(-3, 0)`
- Instruksi 4 (`T`): Koordinat kini `(-2, 0)`
- Instruksi 5 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 6 (`S`): Koordinat kini `(-2, -2)`
- Instruksi 7 (`U`): Koordinat kini `(-2, -1)`
- Instruksi 8 (`U`): Koordinat kini `(-2, 0)`
- Instruksi 9 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 10 (`T`): Koordinat kini `(0, 0)`
- Instruksi 11 (`S`): Koordinat kini `(0, -1)`
- Instruksi 12 (`T`): Koordinat kini `(1, -1)`
- Instruksi 13 (`S`): Koordinat kini `(1, -2)`
- Instruksi 14 (`S`): Koordinat kini `(1, -3)`

Posisi akhir robot adalah di titik `(1, -3)`.
Jarak Manhattan = Murni $|1| + |-3|$ = 1 + 3 = **4 unit**.
Opsi valid: **B**.</details>

---
**Soal 297**
Sebuah robot bola diletakkan di lantai 57. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 11 detik
B. 13 detik
C. 14 detik
D. 12 detik
E. 15 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (12 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 57 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 57 + 1 = 58
- Detik 2: Genap, turun 13 -> 58 - 13 = 45
- Detik 3: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 4: Genap, turun 13 -> 46 - 13 = 33
- Detik 5: Ganjil, naik 1 -> 33 + 1 = 34
- Detik 6: Genap, turun 13 -> 34 - 13 = 21
- Detik 7: Ganjil, naik 1 -> 21 + 1 = 22
- Detik 8: Genap, turun 13 -> 22 - 13 = 9
- Detik 9: Ganjil, naik 1 -> 9 + 1 = 10
- Detik 10: Genap, turun 13 -> 10 - 13 = -3
- Detik 11: Ganjil, naik 1 -> -3 + 1 = -2
- Detik 12: Genap, turun 13 -> -2 - 13 = -15
Simulasi berakhir pada detik ke-12. Jawaban yang tepat adalah opsi **D**.
</details>

---
**Soal 298**
Sebuah robot bola diletakkan di lantai 138. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 36 detik
B. 35 detik
C. 37 detik
D. 34 detik
E. 38 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (35 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 138 (Garis Start)
- Detik 1: Genap, turun 9 -> 138 - 9 = 129
- Detik 2: Ganjil, naik 1 -> 129 + 1 = 130
- Detik 3: Genap, turun 9 -> 130 - 9 = 121
- Detik 4: Ganjil, naik 1 -> 121 + 1 = 122
- Detik 5: Genap, turun 9 -> 122 - 9 = 113
- Detik 6: Ganjil, naik 1 -> 113 + 1 = 114
- Detik 7: Genap, turun 9 -> 114 - 9 = 105
- Detik 8: Ganjil, naik 1 -> 105 + 1 = 106
- Detik 9: Genap, turun 9 -> 106 - 9 = 97
- Detik 10: Ganjil, naik 1 -> 97 + 1 = 98
- Detik 11: Genap, turun 9 -> 98 - 9 = 89
- Detik 12: Ganjil, naik 1 -> 89 + 1 = 90
- Detik 13: Genap, turun 9 -> 90 - 9 = 81
- Detik 14: Ganjil, naik 1 -> 81 + 1 = 82
- Detik 15: Genap, turun 9 -> 82 - 9 = 73
- Detik 16: Ganjil, naik 1 -> 73 + 1 = 74
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 35: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 299**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 18, 19, 16, 13]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 41."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 4 pasang
C. 1 pasang
D. 0 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 18 = 24 (❌ Gagal)
- Sapi 6 + Sapi 19 = 25 (❌ Gagal)
- Sapi 6 + Sapi 16 = 22 (❌ Gagal)
- Sapi 6 + Sapi 13 = 19 (❌ Gagal)
- Sapi 18 + Sapi 19 = 37 (❌ Gagal)
- Sapi 18 + Sapi 16 = 34 (❌ Gagal)
- Sapi 18 + Sapi 13 = 31 (❌ Gagal)
- Sapi 19 + Sapi 16 = 35 (❌ Gagal)
- Sapi 19 + Sapi 13 = 32 (❌ Gagal)
- Sapi 16 + Sapi 13 = 29 (❌ Gagal)

Total pasangan yang bernilai 41 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 300**
Sebuah robot bola diletakkan di lantai 129. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 27 detik
B. 28 detik
C. 29 detik
D. 25 detik
E. 26 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (26 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 129 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 129 + 1 = 130
- Detik 2: Genap, turun 11 -> 130 - 11 = 119
- Detik 3: Ganjil, naik 1 -> 119 + 1 = 120
- Detik 4: Genap, turun 11 -> 120 - 11 = 109
- Detik 5: Ganjil, naik 1 -> 109 + 1 = 110
- Detik 6: Genap, turun 11 -> 110 - 11 = 99
- Detik 7: Ganjil, naik 1 -> 99 + 1 = 100
- Detik 8: Genap, turun 11 -> 100 - 11 = 89
- Detik 9: Ganjil, naik 1 -> 89 + 1 = 90
- Detik 10: Genap, turun 11 -> 90 - 11 = 79
- Detik 11: Ganjil, naik 1 -> 79 + 1 = 80
- Detik 12: Genap, turun 11 -> 80 - 11 = 69
- Detik 13: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 14: Genap, turun 11 -> 70 - 11 = 59
- Detik 15: Ganjil, naik 1 -> 59 + 1 = 60
- Detik 16: Genap, turun 11 -> 60 - 11 = 49
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 26: Menyentuh batas lantai <= 0. Selesai.
</details>

---
