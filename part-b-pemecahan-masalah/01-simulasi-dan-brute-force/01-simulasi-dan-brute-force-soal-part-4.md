# Latian Soal: Simulasi & Brute Force (Part 4 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 151**
Sebuah robot bola diletakkan di lantai 93. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 22 detik
B. 23 detik
C. 19 detik
D. 20 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (20 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 93 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 93 + 3 = 96
- Detik 2: Genap, turun 13 -> 96 - 13 = 83
- Detik 3: Ganjil, naik 3 -> 83 + 3 = 86
- Detik 4: Genap, turun 13 -> 86 - 13 = 73
- Detik 5: Ganjil, naik 3 -> 73 + 3 = 76
- Detik 6: Genap, turun 13 -> 76 - 13 = 63
- Detik 7: Ganjil, naik 3 -> 63 + 3 = 66
- Detik 8: Genap, turun 13 -> 66 - 13 = 53
- Detik 9: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 10: Genap, turun 13 -> 56 - 13 = 43
- Detik 11: Ganjil, naik 3 -> 43 + 3 = 46
- Detik 12: Genap, turun 13 -> 46 - 13 = 33
- Detik 13: Ganjil, naik 3 -> 33 + 3 = 36
- Detik 14: Genap, turun 13 -> 36 - 13 = 23
- Detik 15: Ganjil, naik 3 -> 23 + 3 = 26
- Detik 16: Genap, turun 13 -> 26 - 13 = 13
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 20: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 152**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 12, 2, 18, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 25."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 3 pasang
D. 1 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 12 = 34 (❌ Gagal)
- Sapi 22 + Sapi 2 = 24 (❌ Gagal)
- Sapi 22 + Sapi 18 = 40 (❌ Gagal)
- Sapi 22 + Sapi 19 = 41 (❌ Gagal)
- Sapi 12 + Sapi 2 = 14 (❌ Gagal)
- Sapi 12 + Sapi 18 = 30 (❌ Gagal)
- Sapi 12 + Sapi 19 = 31 (❌ Gagal)
- Sapi 2 + Sapi 18 = 20 (❌ Gagal)
- Sapi 2 + Sapi 19 = 21 (❌ Gagal)
- Sapi 18 + Sapi 19 = 37 (❌ Gagal)

Total pasangan yang bernilai 25 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 153**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BBSBBUSUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 3 unit langkah
C. 4 unit langkah
D. 7 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 3 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`B`): Koordinat kini `(-3, -1)`
- Instruksi 5 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 6 (`U`): Koordinat kini `(-4, 0)`
- Instruksi 7 (`S`): Koordinat kini `(-4, -1)`
- Instruksi 8 (`U`): Koordinat kini `(-4, 0)`
- Instruksi 9 (`S`): Koordinat kini `(-4, -1)`

Posisi akhir robot adalah di titik `(-4, -1)`.
Jarak Manhattan = Murni $|-4| + |-1|$ = 4 + 1 = **5 unit**.
Opsi valid: **E**.</details>

---
**Soal 154**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSBSTUSBUTTBBU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 3 unit langkah
C. 4 unit langkah
D. 2 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`T`): Koordinat kini `(0, 0)`
- Instruksi 7 (`U`): Koordinat kini `(0, 1)`
- Instruksi 8 (`S`): Koordinat kini `(0, 0)`
- Instruksi 9 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 10 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 11 (`T`): Koordinat kini `(0, 1)`
- Instruksi 12 (`T`): Koordinat kini `(1, 1)`
- Instruksi 13 (`B`): Koordinat kini `(0, 1)`
- Instruksi 14 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 15 (`U`): Koordinat kini `(-1, 2)`

Posisi akhir robot adalah di titik `(-1, 2)`.
Jarak Manhattan = Murni $|-1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **B**.</details>

---
**Soal 155**
Sebuah robot bola diletakkan di lantai 87. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 47 detik
B. 45 detik
C. 44 detik
D. 46 detik
E. 43 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (44 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 87 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 87 + 5 = 92
- Detik 2: Genap, turun 9 -> 92 - 9 = 83
- Detik 3: Ganjil, naik 5 -> 83 + 5 = 88
- Detik 4: Genap, turun 9 -> 88 - 9 = 79
- Detik 5: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 6: Genap, turun 9 -> 84 - 9 = 75
- Detik 7: Ganjil, naik 5 -> 75 + 5 = 80
- Detik 8: Genap, turun 9 -> 80 - 9 = 71
- Detik 9: Ganjil, naik 5 -> 71 + 5 = 76
- Detik 10: Genap, turun 9 -> 76 - 9 = 67
- Detik 11: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 12: Genap, turun 9 -> 72 - 9 = 63
- Detik 13: Ganjil, naik 5 -> 63 + 5 = 68
- Detik 14: Genap, turun 9 -> 68 - 9 = 59
- Detik 15: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 16: Genap, turun 9 -> 64 - 9 = 55
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 44: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 156**
Sebuah robot bola diletakkan di lantai 115. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 57 detik
B. 61 detik
C. 59 detik
D. 58 detik
E. 60 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (58 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 115 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 115 + 3 = 118
- Detik 2: Genap, turun 7 -> 118 - 7 = 111
- Detik 3: Ganjil, naik 3 -> 111 + 3 = 114
- Detik 4: Genap, turun 7 -> 114 - 7 = 107
- Detik 5: Ganjil, naik 3 -> 107 + 3 = 110
- Detik 6: Genap, turun 7 -> 110 - 7 = 103
- Detik 7: Ganjil, naik 3 -> 103 + 3 = 106
- Detik 8: Genap, turun 7 -> 106 - 7 = 99
- Detik 9: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 10: Genap, turun 7 -> 102 - 7 = 95
- Detik 11: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 12: Genap, turun 7 -> 98 - 7 = 91
- Detik 13: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 14: Genap, turun 7 -> 94 - 7 = 87
- Detik 15: Ganjil, naik 3 -> 87 + 3 = 90
- Detik 16: Genap, turun 7 -> 90 - 7 = 83
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 58: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 157**
Sebuah robot bola diletakkan di lantai 139. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 30 detik
C. 29 detik
D. 27 detik
E. 31 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (28 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 139 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 139 + 3 = 142
- Detik 2: Genap, turun 13 -> 142 - 13 = 129
- Detik 3: Ganjil, naik 3 -> 129 + 3 = 132
- Detik 4: Genap, turun 13 -> 132 - 13 = 119
- Detik 5: Ganjil, naik 3 -> 119 + 3 = 122
- Detik 6: Genap, turun 13 -> 122 - 13 = 109
- Detik 7: Ganjil, naik 3 -> 109 + 3 = 112
- Detik 8: Genap, turun 13 -> 112 - 13 = 99
- Detik 9: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 10: Genap, turun 13 -> 102 - 13 = 89
- Detik 11: Ganjil, naik 3 -> 89 + 3 = 92
- Detik 12: Genap, turun 13 -> 92 - 13 = 79
- Detik 13: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 14: Genap, turun 13 -> 82 - 13 = 69
- Detik 15: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 16: Genap, turun 13 -> 72 - 13 = 59
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 28: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 158**
Sebuah robot bola diletakkan di lantai 143. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 52 detik
B. 50 detik
C. 51 detik
D. 49 detik
E. 53 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (50 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 143 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 143 + 1 = 144
- Detik 2: Genap, turun 7 -> 144 - 7 = 137
- Detik 3: Ganjil, naik 1 -> 137 + 1 = 138
- Detik 4: Genap, turun 7 -> 138 - 7 = 131
- Detik 5: Ganjil, naik 1 -> 131 + 1 = 132
- Detik 6: Genap, turun 7 -> 132 - 7 = 125
- Detik 7: Ganjil, naik 1 -> 125 + 1 = 126
- Detik 8: Genap, turun 7 -> 126 - 7 = 119
- Detik 9: Ganjil, naik 1 -> 119 + 1 = 120
- Detik 10: Genap, turun 7 -> 120 - 7 = 113
- Detik 11: Ganjil, naik 1 -> 113 + 1 = 114
- Detik 12: Genap, turun 7 -> 114 - 7 = 107
- Detik 13: Ganjil, naik 1 -> 107 + 1 = 108
- Detik 14: Genap, turun 7 -> 108 - 7 = 101
- Detik 15: Ganjil, naik 1 -> 101 + 1 = 102
- Detik 16: Genap, turun 7 -> 102 - 7 = 95
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 50: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 159**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[8, 10, 23, 16, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 50."*

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
- Sapi 8 + Sapi 10 = 18 (❌ Gagal)
- Sapi 8 + Sapi 23 = 31 (❌ Gagal)
- Sapi 8 + Sapi 16 = 24 (❌ Gagal)
- Sapi 8 + Sapi 2 = 10 (❌ Gagal)
- Sapi 10 + Sapi 23 = 33 (❌ Gagal)
- Sapi 10 + Sapi 16 = 26 (❌ Gagal)
- Sapi 10 + Sapi 2 = 12 (❌ Gagal)
- Sapi 23 + Sapi 16 = 39 (❌ Gagal)
- Sapi 23 + Sapi 2 = 25 (❌ Gagal)
- Sapi 16 + Sapi 2 = 18 (❌ Gagal)

Total pasangan yang bernilai 50 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 160**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUTSBBUSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 1 unit langkah
C. -1 unit langkah
D. 3 unit langkah
E. 0 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`T`): Koordinat kini `(1, 2)`
- Instruksi 4 (`S`): Koordinat kini `(1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(0, 1)`
- Instruksi 6 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 8 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 9 (`S`): Koordinat kini `(-1, 0)`

Posisi akhir robot adalah di titik `(-1, 0)`.
Jarak Manhattan = Murni $|-1| + |0|$ = 1 + 0 = **1 unit**.
Opsi valid: **B**.</details>

---
**Soal 161**
Sebuah robot bola diletakkan di lantai 80. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 12 detik
B. 16 detik
C. 15 detik
D. 14 detik
E. 13 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (13 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 80 (Garis Start)
- Detik 1: Genap, turun 13 -> 80 - 13 = 67
- Detik 2: Ganjil, naik 1 -> 67 + 1 = 68
- Detik 3: Genap, turun 13 -> 68 - 13 = 55
- Detik 4: Ganjil, naik 1 -> 55 + 1 = 56
- Detik 5: Genap, turun 13 -> 56 - 13 = 43
- Detik 6: Ganjil, naik 1 -> 43 + 1 = 44
- Detik 7: Genap, turun 13 -> 44 - 13 = 31
- Detik 8: Ganjil, naik 1 -> 31 + 1 = 32
- Detik 9: Genap, turun 13 -> 32 - 13 = 19
- Detik 10: Ganjil, naik 1 -> 19 + 1 = 20
- Detik 11: Genap, turun 13 -> 20 - 13 = 7
- Detik 12: Ganjil, naik 1 -> 7 + 1 = 8
- Detik 13: Genap, turun 13 -> 8 - 13 = -5
Simulasi berakhir pada detik ke-13. Jawaban yang tepat adalah opsi **E**.
</details>

---
**Soal 162**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[21, 15, 9, 6, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 31."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 2 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 21 + Sapi 15 = 36 (❌ Gagal)
- Sapi 21 + Sapi 9 = 30 (❌ Gagal)
- Sapi 21 + Sapi 6 = 27 (❌ Gagal)
- Sapi 21 + Sapi 10 = 31 (✅ COCOK)
- Sapi 15 + Sapi 9 = 24 (❌ Gagal)
- Sapi 15 + Sapi 6 = 21 (❌ Gagal)
- Sapi 15 + Sapi 10 = 25 (❌ Gagal)
- Sapi 9 + Sapi 6 = 15 (❌ Gagal)
- Sapi 9 + Sapi 10 = 19 (❌ Gagal)
- Sapi 6 + Sapi 10 = 16 (❌ Gagal)

Total pasangan yang bernilai 31 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 163**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 7, 13, 6, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 2 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 3 + Sapi 6 = 9 (❌ Gagal)
- Sapi 3 + Sapi 15 = 18 (❌ Gagal)
- Sapi 7 + Sapi 13 = 20 (❌ Gagal)
- Sapi 7 + Sapi 6 = 13 (❌ Gagal)
- Sapi 7 + Sapi 15 = 22 (❌ Gagal)
- Sapi 13 + Sapi 6 = 19 (❌ Gagal)
- Sapi 13 + Sapi 15 = 28 (❌ Gagal)
- Sapi 6 + Sapi 15 = 21 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 164**
Sebuah robot bola diletakkan di lantai 136. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 73 detik
B. 72 detik
C. 74 detik
D. 70 detik
E. 71 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (71 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 136 (Garis Start)
- Detik 1: Genap, turun 9 -> 136 - 9 = 127
- Detik 2: Ganjil, naik 5 -> 127 + 5 = 132
- Detik 3: Genap, turun 9 -> 132 - 9 = 123
- Detik 4: Ganjil, naik 5 -> 123 + 5 = 128
- Detik 5: Genap, turun 9 -> 128 - 9 = 119
- Detik 6: Ganjil, naik 5 -> 119 + 5 = 124
- Detik 7: Genap, turun 9 -> 124 - 9 = 115
- Detik 8: Ganjil, naik 5 -> 115 + 5 = 120
- Detik 9: Genap, turun 9 -> 120 - 9 = 111
- Detik 10: Ganjil, naik 5 -> 111 + 5 = 116
- Detik 11: Genap, turun 9 -> 116 - 9 = 107
- Detik 12: Ganjil, naik 5 -> 107 + 5 = 112
- Detik 13: Genap, turun 9 -> 112 - 9 = 103
- Detik 14: Ganjil, naik 5 -> 103 + 5 = 108
- Detik 15: Genap, turun 9 -> 108 - 9 = 99
- Detik 16: Ganjil, naik 5 -> 99 + 5 = 104
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 71: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 165**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 5, 19, 4, 8]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 1 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 5 = 15 (❌ Gagal)
- Sapi 10 + Sapi 19 = 29 (❌ Gagal)
- Sapi 10 + Sapi 4 = 14 (❌ Gagal)
- Sapi 10 + Sapi 8 = 18 (❌ Gagal)
- Sapi 5 + Sapi 19 = 24 (❌ Gagal)
- Sapi 5 + Sapi 4 = 9 (❌ Gagal)
- Sapi 5 + Sapi 8 = 13 (❌ Gagal)
- Sapi 19 + Sapi 4 = 23 (❌ Gagal)
- Sapi 19 + Sapi 8 = 27 (❌ Gagal)
- Sapi 4 + Sapi 8 = 12 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 166**
Sebuah robot bola diletakkan di lantai 97. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 37 detik
B. 33 detik
C. 35 detik
D. 36 detik
E. 34 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (34 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 97 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 97 + 1 = 98
- Detik 2: Genap, turun 7 -> 98 - 7 = 91
- Detik 3: Ganjil, naik 1 -> 91 + 1 = 92
- Detik 4: Genap, turun 7 -> 92 - 7 = 85
- Detik 5: Ganjil, naik 1 -> 85 + 1 = 86
- Detik 6: Genap, turun 7 -> 86 - 7 = 79
- Detik 7: Ganjil, naik 1 -> 79 + 1 = 80
- Detik 8: Genap, turun 7 -> 80 - 7 = 73
- Detik 9: Ganjil, naik 1 -> 73 + 1 = 74
- Detik 10: Genap, turun 7 -> 74 - 7 = 67
- Detik 11: Ganjil, naik 1 -> 67 + 1 = 68
- Detik 12: Genap, turun 7 -> 68 - 7 = 61
- Detik 13: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 14: Genap, turun 7 -> 62 - 7 = 55
- Detik 15: Ganjil, naik 1 -> 55 + 1 = 56
- Detik 16: Genap, turun 7 -> 56 - 7 = 49
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 34: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 167**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `USBSUSTBT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. -1 unit langkah
B. 1 unit langkah
C. 0 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`S`): Koordinat kini `(0, 0)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`T`): Koordinat kini `(0, -1)`
- Instruksi 8 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`T`): Koordinat kini `(0, -1)`

Posisi akhir robot adalah di titik `(0, -1)`.
Jarak Manhattan = Murni $|0| + |-1|$ = 0 + 1 = **1 unit**.
Opsi valid: **B**.</details>

---
**Soal 168**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUTSTBTUTBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 2 unit langkah
C. 3 unit langkah
D. 5 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(2, 1)`
- Instruksi 4 (`S`): Koordinat kini `(2, 0)`
- Instruksi 5 (`T`): Koordinat kini `(3, 0)`
- Instruksi 6 (`B`): Koordinat kini `(2, 0)`
- Instruksi 7 (`T`): Koordinat kini `(3, 0)`
- Instruksi 8 (`U`): Koordinat kini `(3, 1)`
- Instruksi 9 (`T`): Koordinat kini `(4, 1)`
- Instruksi 10 (`B`): Koordinat kini `(3, 1)`
- Instruksi 11 (`B`): Koordinat kini `(2, 1)`

Posisi akhir robot adalah di titik `(2, 1)`.
Jarak Manhattan = Murni $|2| + |1|$ = 2 + 1 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 169**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[14, 21, 12, 9, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 45."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 0 pasang
C. 3 pasang
D. 2 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 14 + Sapi 21 = 35 (❌ Gagal)
- Sapi 14 + Sapi 12 = 26 (❌ Gagal)
- Sapi 14 + Sapi 9 = 23 (❌ Gagal)
- Sapi 14 + Sapi 2 = 16 (❌ Gagal)
- Sapi 21 + Sapi 12 = 33 (❌ Gagal)
- Sapi 21 + Sapi 9 = 30 (❌ Gagal)
- Sapi 21 + Sapi 2 = 23 (❌ Gagal)
- Sapi 12 + Sapi 9 = 21 (❌ Gagal)
- Sapi 12 + Sapi 2 = 14 (❌ Gagal)
- Sapi 9 + Sapi 2 = 11 (❌ Gagal)

Total pasangan yang bernilai 45 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 170**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBTTTSSBBBBBUTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. -1 unit langkah
C. 3 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(0, 1)`
- Instruksi 4 (`T`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`S`): Koordinat kini `(2, 0)`
- Instruksi 7 (`S`): Koordinat kini `(2, -1)`
- Instruksi 8 (`B`): Koordinat kini `(1, -1)`
- Instruksi 9 (`B`): Koordinat kini `(0, -1)`
- Instruksi 10 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 11 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 12 (`B`): Koordinat kini `(-3, -1)`
- Instruksi 13 (`U`): Koordinat kini `(-3, 0)`
- Instruksi 14 (`T`): Koordinat kini `(-2, 0)`
- Instruksi 15 (`T`): Koordinat kini `(-1, 0)`

Posisi akhir robot adalah di titik `(-1, 0)`.
Jarak Manhattan = Murni $|-1| + |0|$ = 1 + 0 = **1 unit**.
Opsi valid: **E**.</details>

---
**Soal 171**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BTTUBUTBTBTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 3 unit langkah
C. 4 unit langkah
D. 6 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(0, 1)`
- Instruksi 6 (`U`): Koordinat kini `(0, 2)`
- Instruksi 7 (`T`): Koordinat kini `(1, 2)`
- Instruksi 8 (`B`): Koordinat kini `(0, 2)`
- Instruksi 9 (`T`): Koordinat kini `(1, 2)`
- Instruksi 10 (`B`): Koordinat kini `(0, 2)`
- Instruksi 11 (`T`): Koordinat kini `(1, 2)`
- Instruksi 12 (`T`): Koordinat kini `(2, 2)`

Posisi akhir robot adalah di titik `(2, 2)`.
Jarak Manhattan = Murni $|2| + |2|$ = 2 + 2 = **4 unit**.
Opsi valid: **C**.</details>

---
**Soal 172**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[13, 19, 16, 22, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 49."*

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
- Sapi 13 + Sapi 19 = 32 (❌ Gagal)
- Sapi 13 + Sapi 16 = 29 (❌ Gagal)
- Sapi 13 + Sapi 22 = 35 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)
- Sapi 19 + Sapi 16 = 35 (❌ Gagal)
- Sapi 19 + Sapi 22 = 41 (❌ Gagal)
- Sapi 19 + Sapi 10 = 29 (❌ Gagal)
- Sapi 16 + Sapi 22 = 38 (❌ Gagal)
- Sapi 16 + Sapi 10 = 26 (❌ Gagal)
- Sapi 22 + Sapi 10 = 32 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 173**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[13, 18, 2, 4, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 28."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 3 pasang
D. 0 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 13 + Sapi 18 = 31 (❌ Gagal)
- Sapi 13 + Sapi 2 = 15 (❌ Gagal)
- Sapi 13 + Sapi 4 = 17 (❌ Gagal)
- Sapi 13 + Sapi 6 = 19 (❌ Gagal)
- Sapi 18 + Sapi 2 = 20 (❌ Gagal)
- Sapi 18 + Sapi 4 = 22 (❌ Gagal)
- Sapi 18 + Sapi 6 = 24 (❌ Gagal)
- Sapi 2 + Sapi 4 = 6 (❌ Gagal)
- Sapi 2 + Sapi 6 = 8 (❌ Gagal)
- Sapi 4 + Sapi 6 = 10 (❌ Gagal)

Total pasangan yang bernilai 28 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 174**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUUSBSBBTSTSBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 5 unit langkah
C. 2 unit langkah
D. 6 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`U`): Koordinat kini `(0, 3)`
- Instruksi 4 (`S`): Koordinat kini `(0, 2)`
- Instruksi 5 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 8 (`B`): Koordinat kini `(-3, 1)`
- Instruksi 9 (`T`): Koordinat kini `(-2, 1)`
- Instruksi 10 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 11 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 12 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 13 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 14 (`B`): Koordinat kini `(-3, -1)`

Posisi akhir robot adalah di titik `(-3, -1)`.
Jarak Manhattan = Murni $|-3| + |-1|$ = 3 + 1 = **4 unit**.
Opsi valid: **E**.</details>

---
**Soal 175**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSTBBTTUUBBBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 2 unit langkah
C. 5 unit langkah
D. 3 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(0, -1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 5 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 6 (`T`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`T`): Koordinat kini `(0, -1)`
- Instruksi 8 (`U`): Koordinat kini `(0, 0)`
- Instruksi 9 (`U`): Koordinat kini `(0, 1)`
- Instruksi 10 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 11 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 12 (`B`): Koordinat kini `(-3, 1)`
- Instruksi 13 (`S`): Koordinat kini `(-3, 0)`

Posisi akhir robot adalah di titik `(-3, 0)`.
Jarak Manhattan = Murni $|-3| + |0|$ = 3 + 0 = **3 unit**.
Opsi valid: **D**.</details>

---
**Soal 176**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 13, 17, 18, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

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
- Sapi 23 + Sapi 13 = 36 (❌ Gagal)
- Sapi 23 + Sapi 17 = 40 (❌ Gagal)
- Sapi 23 + Sapi 18 = 41 (❌ Gagal)
- Sapi 23 + Sapi 2 = 25 (❌ Gagal)
- Sapi 13 + Sapi 17 = 30 (❌ Gagal)
- Sapi 13 + Sapi 18 = 31 (❌ Gagal)
- Sapi 13 + Sapi 2 = 15 (❌ Gagal)
- Sapi 17 + Sapi 18 = 35 (❌ Gagal)
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)
- Sapi 18 + Sapi 2 = 20 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 177**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 9, 21, 2, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 4 pasang
D. 1 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 21 = 24 (❌ Gagal)
- Sapi 3 + Sapi 2 = 5 (❌ Gagal)
- Sapi 3 + Sapi 5 = 8 (❌ Gagal)
- Sapi 9 + Sapi 21 = 30 (❌ Gagal)
- Sapi 9 + Sapi 2 = 11 (❌ Gagal)
- Sapi 9 + Sapi 5 = 14 (❌ Gagal)
- Sapi 21 + Sapi 2 = 23 (❌ Gagal)
- Sapi 21 + Sapi 5 = 26 (❌ Gagal)
- Sapi 2 + Sapi 5 = 7 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 178**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBTSTTSUTTUUUBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 6 unit langkah
C. 4 unit langkah
D. 7 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`T`): Koordinat kini `(1, 0)`
- Instruksi 6 (`T`): Koordinat kini `(2, 0)`
- Instruksi 7 (`S`): Koordinat kini `(2, -1)`
- Instruksi 8 (`U`): Koordinat kini `(2, 0)`
- Instruksi 9 (`T`): Koordinat kini `(3, 0)`
- Instruksi 10 (`T`): Koordinat kini `(4, 0)`
- Instruksi 11 (`U`): Koordinat kini `(4, 1)`
- Instruksi 12 (`U`): Koordinat kini `(4, 2)`
- Instruksi 13 (`U`): Koordinat kini `(4, 3)`
- Instruksi 14 (`B`): Koordinat kini `(3, 3)`
- Instruksi 15 (`S`): Koordinat kini `(3, 2)`

Posisi akhir robot adalah di titik `(3, 2)`.
Jarak Manhattan = Murni $|3| + |2|$ = 3 + 2 = **5 unit**.
Opsi valid: **A**.</details>

---
**Soal 179**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSTSUUBT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. -1 unit langkah
B. 0 unit langkah
C. 1 unit langkah
D. 2 unit langkah
E. -2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (0 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(0, -1)`
- Instruksi 4 (`S`): Koordinat kini `(0, -2)`
- Instruksi 5 (`U`): Koordinat kini `(0, -1)`
- Instruksi 6 (`U`): Koordinat kini `(0, 0)`
- Instruksi 7 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 8 (`T`): Koordinat kini `(0, 0)`

Posisi akhir robot adalah di titik `(0, 0)`.
Jarak Manhattan = Murni $|0| + |0|$ = 0 + 0 = **0 unit**.
Opsi valid: **B**.</details>

---
**Soal 180**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[17, 12, 6, 13, 3]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 48."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 2 pasang
C. 3 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 17 + Sapi 12 = 29 (❌ Gagal)
- Sapi 17 + Sapi 6 = 23 (❌ Gagal)
- Sapi 17 + Sapi 13 = 30 (❌ Gagal)
- Sapi 17 + Sapi 3 = 20 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 12 + Sapi 13 = 25 (❌ Gagal)
- Sapi 12 + Sapi 3 = 15 (❌ Gagal)
- Sapi 6 + Sapi 13 = 19 (❌ Gagal)
- Sapi 6 + Sapi 3 = 9 (❌ Gagal)
- Sapi 13 + Sapi 3 = 16 (❌ Gagal)

Total pasangan yang bernilai 48 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 181**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `USUTTBTSUUUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 2 unit langkah
C. 6 unit langkah
D. 3 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`S`): Koordinat kini `(0, 0)`
- Instruksi 3 (`U`): Koordinat kini `(0, 1)`
- Instruksi 4 (`T`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`B`): Koordinat kini `(1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(2, 1)`
- Instruksi 8 (`S`): Koordinat kini `(2, 0)`
- Instruksi 9 (`U`): Koordinat kini `(2, 1)`
- Instruksi 10 (`U`): Koordinat kini `(2, 2)`
- Instruksi 11 (`U`): Koordinat kini `(2, 3)`
- Instruksi 12 (`S`): Koordinat kini `(2, 2)`

Posisi akhir robot adalah di titik `(2, 2)`.
Jarak Manhattan = Murni $|2| + |2|$ = 2 + 2 = **4 unit**.
Opsi valid: **E**.</details>

---
**Soal 182**
Sebuah robot bola diletakkan di lantai 55. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 16 detik
B. 18 detik
C. 15 detik
D. 19 detik
E. 17 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (16 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 55 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 2: Genap, turun 11 -> 58 - 11 = 47
- Detik 3: Ganjil, naik 3 -> 47 + 3 = 50
- Detik 4: Genap, turun 11 -> 50 - 11 = 39
- Detik 5: Ganjil, naik 3 -> 39 + 3 = 42
- Detik 6: Genap, turun 11 -> 42 - 11 = 31
- Detik 7: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 8: Genap, turun 11 -> 34 - 11 = 23
- Detik 9: Ganjil, naik 3 -> 23 + 3 = 26
- Detik 10: Genap, turun 11 -> 26 - 11 = 15
- Detik 11: Ganjil, naik 3 -> 15 + 3 = 18
- Detik 12: Genap, turun 11 -> 18 - 11 = 7
- Detik 13: Ganjil, naik 3 -> 7 + 3 = 10
- Detik 14: Genap, turun 11 -> 10 - 11 = -1
- Detik 15: Ganjil, naik 3 -> -1 + 3 = 2
- Detik 16: Genap, turun 11 -> 2 - 11 = -9
</details>

---
**Soal 183**
Sebuah robot bola diletakkan di lantai 78. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 18 detik
B. 19 detik
C. 16 detik
D. 17 detik
E. 20 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (17 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 78 (Garis Start)
- Detik 1: Genap, turun 13 -> 78 - 13 = 65
- Detik 2: Ganjil, naik 3 -> 65 + 3 = 68
- Detik 3: Genap, turun 13 -> 68 - 13 = 55
- Detik 4: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 5: Genap, turun 13 -> 58 - 13 = 45
- Detik 6: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 7: Genap, turun 13 -> 48 - 13 = 35
- Detik 8: Ganjil, naik 3 -> 35 + 3 = 38
- Detik 9: Genap, turun 13 -> 38 - 13 = 25
- Detik 10: Ganjil, naik 3 -> 25 + 3 = 28
- Detik 11: Genap, turun 13 -> 28 - 13 = 15
- Detik 12: Ganjil, naik 3 -> 15 + 3 = 18
- Detik 13: Genap, turun 13 -> 18 - 13 = 5
- Detik 14: Ganjil, naik 3 -> 5 + 3 = 8
- Detik 15: Genap, turun 13 -> 8 - 13 = -5
- Detik 16: Ganjil, naik 3 -> -5 + 3 = -2
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 17: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 184**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BBSTUBUUBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 4 unit langkah
C. 8 unit langkah
D. 6 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 3 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`T`): Koordinat kini `(-1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`U`): Koordinat kini `(-2, 1)`
- Instruksi 8 (`U`): Koordinat kini `(-2, 2)`
- Instruksi 9 (`B`): Koordinat kini `(-3, 2)`
- Instruksi 10 (`B`): Koordinat kini `(-4, 2)`

Posisi akhir robot adalah di titik `(-4, 2)`.
Jarak Manhattan = Murni $|-4| + |2|$ = 4 + 2 = **6 unit**.
Opsi valid: **D**.</details>

---
**Soal 185**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 7, 8, 12, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 0 pasang
C. 2 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 7 = 13 (❌ Gagal)
- Sapi 6 + Sapi 8 = 14 (❌ Gagal)
- Sapi 6 + Sapi 12 = 18 (❌ Gagal)
- Sapi 6 + Sapi 10 = 16 (❌ Gagal)
- Sapi 7 + Sapi 8 = 15 (❌ Gagal)
- Sapi 7 + Sapi 12 = 19 (❌ Gagal)
- Sapi 7 + Sapi 10 = 17 (❌ Gagal)
- Sapi 8 + Sapi 12 = 20 (❌ Gagal)
- Sapi 8 + Sapi 10 = 18 (❌ Gagal)
- Sapi 12 + Sapi 10 = 22 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 186**
Sebuah robot bola diletakkan di lantai 54. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 14 detik
B. 12 detik
C. 13 detik
D. 10 detik
E. 11 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (11 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 54 (Garis Start)
- Detik 1: Genap, turun 13 -> 54 - 13 = 41
- Detik 2: Ganjil, naik 3 -> 41 + 3 = 44
- Detik 3: Genap, turun 13 -> 44 - 13 = 31
- Detik 4: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 5: Genap, turun 13 -> 34 - 13 = 21
- Detik 6: Ganjil, naik 3 -> 21 + 3 = 24
- Detik 7: Genap, turun 13 -> 24 - 13 = 11
- Detik 8: Ganjil, naik 3 -> 11 + 3 = 14
- Detik 9: Genap, turun 13 -> 14 - 13 = 1
- Detik 10: Ganjil, naik 3 -> 1 + 3 = 4
- Detik 11: Genap, turun 13 -> 4 - 13 = -9
Simulasi berakhir pada detik ke-11. Jawaban yang tepat adalah opsi **E**.
</details>

---
**Soal 187**
Sebuah robot bola diletakkan di lantai 85. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 24 detik
B. 22 detik
C. 23 detik
D. 25 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (22 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 85 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 85 + 1 = 86
- Detik 2: Genap, turun 9 -> 86 - 9 = 77
- Detik 3: Ganjil, naik 1 -> 77 + 1 = 78
- Detik 4: Genap, turun 9 -> 78 - 9 = 69
- Detik 5: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 6: Genap, turun 9 -> 70 - 9 = 61
- Detik 7: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 8: Genap, turun 9 -> 62 - 9 = 53
- Detik 9: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 10: Genap, turun 9 -> 54 - 9 = 45
- Detik 11: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 12: Genap, turun 9 -> 46 - 9 = 37
- Detik 13: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 14: Genap, turun 9 -> 38 - 9 = 29
- Detik 15: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 16: Genap, turun 9 -> 30 - 9 = 21
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 22: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 188**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSTTUUUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 5 unit langkah
C. 2 unit langkah
D. 6 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(2, -1)`
- Instruksi 4 (`T`): Koordinat kini `(3, -1)`
- Instruksi 5 (`U`): Koordinat kini `(3, 0)`
- Instruksi 6 (`U`): Koordinat kini `(3, 1)`
- Instruksi 7 (`U`): Koordinat kini `(3, 2)`
- Instruksi 8 (`S`): Koordinat kini `(3, 1)`

Posisi akhir robot adalah di titik `(3, 1)`.
Jarak Manhattan = Murni $|3| + |1|$ = 3 + 1 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 189**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `STSUSSBTB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 5 unit langkah
C. 1 unit langkah
D. 2 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`T`): Koordinat kini `(1, -1)`
- Instruksi 3 (`S`): Koordinat kini `(1, -2)`
- Instruksi 4 (`U`): Koordinat kini `(1, -1)`
- Instruksi 5 (`S`): Koordinat kini `(1, -2)`
- Instruksi 6 (`S`): Koordinat kini `(1, -3)`
- Instruksi 7 (`B`): Koordinat kini `(0, -3)`
- Instruksi 8 (`T`): Koordinat kini `(1, -3)`
- Instruksi 9 (`B`): Koordinat kini `(0, -3)`

Posisi akhir robot adalah di titik `(0, -3)`.
Jarak Manhattan = Murni $|0| + |-3|$ = 0 + 3 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 190**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTUUUBSSUUSBBUU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 7 unit langkah
B. 9 unit langkah
C. 8 unit langkah
D. 6 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (7 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`U`): Koordinat kini `(1, 2)`
- Instruksi 4 (`U`): Koordinat kini `(1, 3)`
- Instruksi 5 (`U`): Koordinat kini `(1, 4)`
- Instruksi 6 (`B`): Koordinat kini `(0, 4)`
- Instruksi 7 (`S`): Koordinat kini `(0, 3)`
- Instruksi 8 (`S`): Koordinat kini `(0, 2)`
- Instruksi 9 (`U`): Koordinat kini `(0, 3)`
- Instruksi 10 (`U`): Koordinat kini `(0, 4)`
- Instruksi 11 (`S`): Koordinat kini `(0, 3)`
- Instruksi 12 (`B`): Koordinat kini `(-1, 3)`
- Instruksi 13 (`B`): Koordinat kini `(-2, 3)`
- Instruksi 14 (`U`): Koordinat kini `(-2, 4)`
- Instruksi 15 (`U`): Koordinat kini `(-2, 5)`

Posisi akhir robot adalah di titik `(-2, 5)`.
Jarak Manhattan = Murni $|-2| + |5|$ = 2 + 5 = **7 unit**.
Opsi valid: **A**.</details>

---
**Soal 191**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 11, 10, 16, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 1 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 11 = 33 (❌ Gagal)
- Sapi 22 + Sapi 10 = 32 (❌ Gagal)
- Sapi 22 + Sapi 16 = 38 (❌ Gagal)
- Sapi 22 + Sapi 17 = 39 (❌ Gagal)
- Sapi 11 + Sapi 10 = 21 (❌ Gagal)
- Sapi 11 + Sapi 16 = 27 (❌ Gagal)
- Sapi 11 + Sapi 17 = 28 (❌ Gagal)
- Sapi 10 + Sapi 16 = 26 (❌ Gagal)
- Sapi 10 + Sapi 17 = 27 (❌ Gagal)
- Sapi 16 + Sapi 17 = 33 (❌ Gagal)

Total pasangan yang bernilai 29 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 192**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TTUTSSSBSBUBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 4 unit langkah
C. 3 unit langkah
D. 5 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(2, 0)`
- Instruksi 3 (`U`): Koordinat kini `(2, 1)`
- Instruksi 4 (`T`): Koordinat kini `(3, 1)`
- Instruksi 5 (`S`): Koordinat kini `(3, 0)`
- Instruksi 6 (`S`): Koordinat kini `(3, -1)`
- Instruksi 7 (`S`): Koordinat kini `(3, -2)`
- Instruksi 8 (`B`): Koordinat kini `(2, -2)`
- Instruksi 9 (`S`): Koordinat kini `(2, -3)`
- Instruksi 10 (`B`): Koordinat kini `(1, -3)`
- Instruksi 11 (`U`): Koordinat kini `(1, -2)`
- Instruksi 12 (`B`): Koordinat kini `(0, -2)`
- Instruksi 13 (`B`): Koordinat kini `(-1, -2)`

Posisi akhir robot adalah di titik `(-1, -2)`.
Jarak Manhattan = Murni $|-1| + |-2|$ = 1 + 2 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 193**
Sebuah robot bola diletakkan di lantai 103. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 55 detik
B. 56 detik
C. 57 detik
D. 54 detik
E. 53 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (54 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 103 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 103 + 3 = 106
- Detik 2: Genap, turun 7 -> 106 - 7 = 99
- Detik 3: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 4: Genap, turun 7 -> 102 - 7 = 95
- Detik 5: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 6: Genap, turun 7 -> 98 - 7 = 91
- Detik 7: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 8: Genap, turun 7 -> 94 - 7 = 87
- Detik 9: Ganjil, naik 3 -> 87 + 3 = 90
- Detik 10: Genap, turun 7 -> 90 - 7 = 83
- Detik 11: Ganjil, naik 3 -> 83 + 3 = 86
- Detik 12: Genap, turun 7 -> 86 - 7 = 79
- Detik 13: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 14: Genap, turun 7 -> 82 - 7 = 75
- Detik 15: Ganjil, naik 3 -> 75 + 3 = 78
- Detik 16: Genap, turun 7 -> 78 - 7 = 71
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 54: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 194**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[15, 7, 23, 8, 11]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 4 pasang
D. 1 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 15 + Sapi 7 = 22 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 15 + Sapi 8 = 23 (❌ Gagal)
- Sapi 15 + Sapi 11 = 26 (❌ Gagal)
- Sapi 7 + Sapi 23 = 30 (❌ Gagal)
- Sapi 7 + Sapi 8 = 15 (❌ Gagal)
- Sapi 7 + Sapi 11 = 18 (❌ Gagal)
- Sapi 23 + Sapi 8 = 31 (❌ Gagal)
- Sapi 23 + Sapi 11 = 34 (❌ Gagal)
- Sapi 8 + Sapi 11 = 19 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 195**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `STUBUBSB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 2 unit langkah
C. 0 unit langkah
D. 3 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`T`): Koordinat kini `(1, -1)`
- Instruksi 3 (`U`): Koordinat kini `(1, 0)`
- Instruksi 4 (`B`): Koordinat kini `(0, 0)`
- Instruksi 5 (`U`): Koordinat kini `(0, 1)`
- Instruksi 6 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`S`): Koordinat kini `(-1, 0)`
- Instruksi 8 (`B`): Koordinat kini `(-2, 0)`

Posisi akhir robot adalah di titik `(-2, 0)`.
Jarak Manhattan = Murni $|-2| + |0|$ = 2 + 0 = **2 unit**.
Opsi valid: **B**.</details>

---
**Soal 196**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBBBUTUSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 5 unit langkah
C. 2 unit langkah
D. 3 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-3, 1)`
- Instruksi 5 (`U`): Koordinat kini `(-3, 2)`
- Instruksi 6 (`T`): Koordinat kini `(-2, 2)`
- Instruksi 7 (`U`): Koordinat kini `(-2, 3)`
- Instruksi 8 (`S`): Koordinat kini `(-2, 2)`
- Instruksi 9 (`S`): Koordinat kini `(-2, 1)`

Posisi akhir robot adalah di titik `(-2, 1)`.
Jarak Manhattan = Murni $|-2| + |1|$ = 2 + 1 = **3 unit**.
Opsi valid: **D**.</details>

---
**Soal 197**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[11, 6, 15, 23, 7]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 50."*

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
- Sapi 11 + Sapi 6 = 17 (❌ Gagal)
- Sapi 11 + Sapi 15 = 26 (❌ Gagal)
- Sapi 11 + Sapi 23 = 34 (❌ Gagal)
- Sapi 11 + Sapi 7 = 18 (❌ Gagal)
- Sapi 6 + Sapi 15 = 21 (❌ Gagal)
- Sapi 6 + Sapi 23 = 29 (❌ Gagal)
- Sapi 6 + Sapi 7 = 13 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 15 + Sapi 7 = 22 (❌ Gagal)
- Sapi 23 + Sapi 7 = 30 (❌ Gagal)

Total pasangan yang bernilai 50 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 198**
Sebuah robot bola diletakkan di lantai 86. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 23 detik
B. 26 detik
C. 24 detik
D. 25 detik
E. 22 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (23 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 86 (Garis Start)
- Detik 1: Genap, turun 9 -> 86 - 9 = 77
- Detik 2: Ganjil, naik 1 -> 77 + 1 = 78
- Detik 3: Genap, turun 9 -> 78 - 9 = 69
- Detik 4: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 5: Genap, turun 9 -> 70 - 9 = 61
- Detik 6: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 7: Genap, turun 9 -> 62 - 9 = 53
- Detik 8: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 9: Genap, turun 9 -> 54 - 9 = 45
- Detik 10: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 11: Genap, turun 9 -> 46 - 9 = 37
- Detik 12: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 13: Genap, turun 9 -> 38 - 9 = 29
- Detik 14: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 15: Genap, turun 9 -> 30 - 9 = 21
- Detik 16: Ganjil, naik 1 -> 21 + 1 = 22
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 23: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 199**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[15, 24, 6, 2, 14]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 41."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 1 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 15 + Sapi 24 = 39 (❌ Gagal)
- Sapi 15 + Sapi 6 = 21 (❌ Gagal)
- Sapi 15 + Sapi 2 = 17 (❌ Gagal)
- Sapi 15 + Sapi 14 = 29 (❌ Gagal)
- Sapi 24 + Sapi 6 = 30 (❌ Gagal)
- Sapi 24 + Sapi 2 = 26 (❌ Gagal)
- Sapi 24 + Sapi 14 = 38 (❌ Gagal)
- Sapi 6 + Sapi 2 = 8 (❌ Gagal)
- Sapi 6 + Sapi 14 = 20 (❌ Gagal)
- Sapi 2 + Sapi 14 = 16 (❌ Gagal)

Total pasangan yang bernilai 41 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 200**
Sebuah robot bola diletakkan di lantai 105. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 42 detik
B. 43 detik
C. 41 detik
D. 40 detik
E. 39 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (40 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 105 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 105 + 1 = 106
- Detik 2: Genap, turun 7 -> 106 - 7 = 99
- Detik 3: Ganjil, naik 1 -> 99 + 1 = 100
- Detik 4: Genap, turun 7 -> 100 - 7 = 93
- Detik 5: Ganjil, naik 1 -> 93 + 1 = 94
- Detik 6: Genap, turun 7 -> 94 - 7 = 87
- Detik 7: Ganjil, naik 1 -> 87 + 1 = 88
- Detik 8: Genap, turun 7 -> 88 - 7 = 81
- Detik 9: Ganjil, naik 1 -> 81 + 1 = 82
- Detik 10: Genap, turun 7 -> 82 - 7 = 75
- Detik 11: Ganjil, naik 1 -> 75 + 1 = 76
- Detik 12: Genap, turun 7 -> 76 - 7 = 69
- Detik 13: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 14: Genap, turun 7 -> 70 - 7 = 63
- Detik 15: Ganjil, naik 1 -> 63 + 1 = 64
- Detik 16: Genap, turun 7 -> 64 - 7 = 57
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 40: Menyentuh batas lantai <= -10. Selesai.
</details>

---
