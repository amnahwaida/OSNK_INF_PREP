# Latian Soal: Simulasi & Brute Force (Part 1 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 1**
Sebuah robot bola diletakkan di lantai 100. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 50 detik
B. 52 detik
C. 54 detik
D. 51 detik
E. 53 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (51 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 100 (Garis Start)
- Detik 1: Genap, turun 7 -> 100 - 7 = 93
- Detik 2: Ganjil, naik 3 -> 93 + 3 = 96
- Detik 3: Genap, turun 7 -> 96 - 7 = 89
- Detik 4: Ganjil, naik 3 -> 89 + 3 = 92
- Detik 5: Genap, turun 7 -> 92 - 7 = 85
- Detik 6: Ganjil, naik 3 -> 85 + 3 = 88
- Detik 7: Genap, turun 7 -> 88 - 7 = 81
- Detik 8: Ganjil, naik 3 -> 81 + 3 = 84
- Detik 9: Genap, turun 7 -> 84 - 7 = 77
- Detik 10: Ganjil, naik 3 -> 77 + 3 = 80
- Detik 11: Genap, turun 7 -> 80 - 7 = 73
- Detik 12: Ganjil, naik 3 -> 73 + 3 = 76
- Detik 13: Genap, turun 7 -> 76 - 7 = 69
- Detik 14: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 15: Genap, turun 7 -> 72 - 7 = 65
- Detik 16: Ganjil, naik 3 -> 65 + 3 = 68
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 51: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 2**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBSSSTUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 4 unit langkah
C. 5 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`S`): Koordinat kini `(0, -1)`
- Instruksi 4 (`S`): Koordinat kini `(0, -2)`
- Instruksi 5 (`S`): Koordinat kini `(0, -3)`
- Instruksi 6 (`T`): Koordinat kini `(1, -3)`
- Instruksi 7 (`U`): Koordinat kini `(1, -2)`
- Instruksi 8 (`S`): Koordinat kini `(1, -3)`

Posisi akhir robot adalah di titik `(1, -3)`.
Jarak Manhattan = Murni $|1| + |-3|$ = 1 + 3 = **4 unit**.
Opsi valid: **B**.</details>

---
**Soal 3**
Sebuah robot bola diletakkan di lantai 104. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 26 detik
B. 28 detik
C. 30 detik
D. 27 detik
E. 29 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (27 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 104 (Garis Start)
- Detik 1: Genap, turun 11 -> 104 - 11 = 93
- Detik 2: Ganjil, naik 3 -> 93 + 3 = 96
- Detik 3: Genap, turun 11 -> 96 - 11 = 85
- Detik 4: Ganjil, naik 3 -> 85 + 3 = 88
- Detik 5: Genap, turun 11 -> 88 - 11 = 77
- Detik 6: Ganjil, naik 3 -> 77 + 3 = 80
- Detik 7: Genap, turun 11 -> 80 - 11 = 69
- Detik 8: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 9: Genap, turun 11 -> 72 - 11 = 61
- Detik 10: Ganjil, naik 3 -> 61 + 3 = 64
- Detik 11: Genap, turun 11 -> 64 - 11 = 53
- Detik 12: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 13: Genap, turun 11 -> 56 - 11 = 45
- Detik 14: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 15: Genap, turun 11 -> 48 - 11 = 37
- Detik 16: Ganjil, naik 3 -> 37 + 3 = 40
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 27: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 4**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[2, 5, 23, 12, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 48."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 1 pasang
C. 3 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 2 + Sapi 5 = 7 (❌ Gagal)
- Sapi 2 + Sapi 23 = 25 (❌ Gagal)
- Sapi 2 + Sapi 12 = 14 (❌ Gagal)
- Sapi 2 + Sapi 6 = 8 (❌ Gagal)
- Sapi 5 + Sapi 23 = 28 (❌ Gagal)
- Sapi 5 + Sapi 12 = 17 (❌ Gagal)
- Sapi 5 + Sapi 6 = 11 (❌ Gagal)
- Sapi 23 + Sapi 12 = 35 (❌ Gagal)
- Sapi 23 + Sapi 6 = 29 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)

Total pasangan yang bernilai 48 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 5**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 6, 18, 14, 7]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

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
- Sapi 19 + Sapi 6 = 25 (❌ Gagal)
- Sapi 19 + Sapi 18 = 37 (❌ Gagal)
- Sapi 19 + Sapi 14 = 33 (❌ Gagal)
- Sapi 19 + Sapi 7 = 26 (❌ Gagal)
- Sapi 6 + Sapi 18 = 24 (❌ Gagal)
- Sapi 6 + Sapi 14 = 20 (❌ Gagal)
- Sapi 6 + Sapi 7 = 13 (❌ Gagal)
- Sapi 18 + Sapi 14 = 32 (❌ Gagal)
- Sapi 18 + Sapi 7 = 25 (❌ Gagal)
- Sapi 14 + Sapi 7 = 21 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 6**
Sebuah robot bola diletakkan di lantai 103. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 21 detik
B. 22 detik
C. 20 detik
D. 19 detik
E. 23 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (20 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 103 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 103 + 1 = 104
- Detik 2: Genap, turun 13 -> 104 - 13 = 91
- Detik 3: Ganjil, naik 1 -> 91 + 1 = 92
- Detik 4: Genap, turun 13 -> 92 - 13 = 79
- Detik 5: Ganjil, naik 1 -> 79 + 1 = 80
- Detik 6: Genap, turun 13 -> 80 - 13 = 67
- Detik 7: Ganjil, naik 1 -> 67 + 1 = 68
- Detik 8: Genap, turun 13 -> 68 - 13 = 55
- Detik 9: Ganjil, naik 1 -> 55 + 1 = 56
- Detik 10: Genap, turun 13 -> 56 - 13 = 43
- Detik 11: Ganjil, naik 1 -> 43 + 1 = 44
- Detik 12: Genap, turun 13 -> 44 - 13 = 31
- Detik 13: Ganjil, naik 1 -> 31 + 1 = 32
- Detik 14: Genap, turun 13 -> 32 - 13 = 19
- Detik 15: Ganjil, naik 1 -> 19 + 1 = 20
- Detik 16: Genap, turun 13 -> 20 - 13 = 7
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 20: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 7**
Sebuah robot bola diletakkan di lantai 126. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 62 detik
B. 61 detik
C. 64 detik
D. 63 detik
E. 60 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (61 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 126 (Garis Start)
- Detik 1: Genap, turun 7 -> 126 - 7 = 119
- Detik 2: Ganjil, naik 3 -> 119 + 3 = 122
- Detik 3: Genap, turun 7 -> 122 - 7 = 115
- Detik 4: Ganjil, naik 3 -> 115 + 3 = 118
- Detik 5: Genap, turun 7 -> 118 - 7 = 111
- Detik 6: Ganjil, naik 3 -> 111 + 3 = 114
- Detik 7: Genap, turun 7 -> 114 - 7 = 107
- Detik 8: Ganjil, naik 3 -> 107 + 3 = 110
- Detik 9: Genap, turun 7 -> 110 - 7 = 103
- Detik 10: Ganjil, naik 3 -> 103 + 3 = 106
- Detik 11: Genap, turun 7 -> 106 - 7 = 99
- Detik 12: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 13: Genap, turun 7 -> 102 - 7 = 95
- Detik 14: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 15: Genap, turun 7 -> 98 - 7 = 91
- Detik 16: Ganjil, naik 3 -> 91 + 3 = 94
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 61: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 8**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 12, 23, 21, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 46."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 2 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 12 = 18 (❌ Gagal)
- Sapi 6 + Sapi 23 = 29 (❌ Gagal)
- Sapi 6 + Sapi 21 = 27 (❌ Gagal)
- Sapi 6 + Sapi 5 = 11 (❌ Gagal)
- Sapi 12 + Sapi 23 = 35 (❌ Gagal)
- Sapi 12 + Sapi 21 = 33 (❌ Gagal)
- Sapi 12 + Sapi 5 = 17 (❌ Gagal)
- Sapi 23 + Sapi 21 = 44 (❌ Gagal)
- Sapi 23 + Sapi 5 = 28 (❌ Gagal)
- Sapi 21 + Sapi 5 = 26 (❌ Gagal)

Total pasangan yang bernilai 46 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 9**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `USTUBTTBUSBSB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 0 unit langkah
C. -1 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`S`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(0, 1)`
- Instruksi 6 (`T`): Koordinat kini `(1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(2, 1)`
- Instruksi 8 (`B`): Koordinat kini `(1, 1)`
- Instruksi 9 (`U`): Koordinat kini `(1, 2)`
- Instruksi 10 (`S`): Koordinat kini `(1, 1)`
- Instruksi 11 (`B`): Koordinat kini `(0, 1)`
- Instruksi 12 (`S`): Koordinat kini `(0, 0)`
- Instruksi 13 (`B`): Koordinat kini `(-1, 0)`

Posisi akhir robot adalah di titik `(-1, 0)`.
Jarak Manhattan = Murni $|-1| + |0|$ = 1 + 0 = **1 unit**.
Opsi valid: **A**.</details>

---
**Soal 10**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TTUBBTUSSST`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 3 unit langkah
C. 2 unit langkah
D. 1 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(2, 0)`
- Instruksi 3 (`U`): Koordinat kini `(2, 1)`
- Instruksi 4 (`B`): Koordinat kini `(1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(0, 1)`
- Instruksi 6 (`T`): Koordinat kini `(1, 1)`
- Instruksi 7 (`U`): Koordinat kini `(1, 2)`
- Instruksi 8 (`S`): Koordinat kini `(1, 1)`
- Instruksi 9 (`S`): Koordinat kini `(1, 0)`
- Instruksi 10 (`S`): Koordinat kini `(1, -1)`
- Instruksi 11 (`T`): Koordinat kini `(2, -1)`

Posisi akhir robot adalah di titik `(2, -1)`.
Jarak Manhattan = Murni $|2| + |-1|$ = 2 + 1 = **3 unit**.
Opsi valid: **B**.</details>

---
**Soal 11**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSSTSTBSBTUB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 2 unit langkah
C. 5 unit langkah
D. 3 unit langkah
E. 6 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`S`): Koordinat kini `(1, -2)`
- Instruksi 4 (`T`): Koordinat kini `(2, -2)`
- Instruksi 5 (`S`): Koordinat kini `(2, -3)`
- Instruksi 6 (`T`): Koordinat kini `(3, -3)`
- Instruksi 7 (`B`): Koordinat kini `(2, -3)`
- Instruksi 8 (`S`): Koordinat kini `(2, -4)`
- Instruksi 9 (`B`): Koordinat kini `(1, -4)`
- Instruksi 10 (`T`): Koordinat kini `(2, -4)`
- Instruksi 11 (`U`): Koordinat kini `(2, -3)`
- Instruksi 12 (`B`): Koordinat kini `(1, -3)`

Posisi akhir robot adalah di titik `(1, -3)`.
Jarak Manhattan = Murni $|1| + |-3|$ = 1 + 3 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 12**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSSBUTTU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 5 unit langkah
C. 4 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(0, 1)`
- Instruksi 8 (`T`): Koordinat kini `(1, 1)`
- Instruksi 9 (`U`): Koordinat kini `(1, 2)`

Posisi akhir robot adalah di titik `(1, 2)`.
Jarak Manhattan = Murni $|1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 13**
Sebuah robot bola diletakkan di lantai 114. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 26 detik
B. 27 detik
C. 29 detik
D. 30 detik
E. 28 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (27 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 114 (Garis Start)
- Detik 1: Genap, turun 13 -> 114 - 13 = 101
- Detik 2: Ganjil, naik 5 -> 101 + 5 = 106
- Detik 3: Genap, turun 13 -> 106 - 13 = 93
- Detik 4: Ganjil, naik 5 -> 93 + 5 = 98
- Detik 5: Genap, turun 13 -> 98 - 13 = 85
- Detik 6: Ganjil, naik 5 -> 85 + 5 = 90
- Detik 7: Genap, turun 13 -> 90 - 13 = 77
- Detik 8: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 9: Genap, turun 13 -> 82 - 13 = 69
- Detik 10: Ganjil, naik 5 -> 69 + 5 = 74
- Detik 11: Genap, turun 13 -> 74 - 13 = 61
- Detik 12: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 13: Genap, turun 13 -> 66 - 13 = 53
- Detik 14: Ganjil, naik 5 -> 53 + 5 = 58
- Detik 15: Genap, turun 13 -> 58 - 13 = 45
- Detik 16: Ganjil, naik 5 -> 45 + 5 = 50
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 27: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 14**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSBBSBBBUTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 4 unit langkah
C. 2 unit langkah
D. 5 unit langkah
E. 6 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`B`): Koordinat kini `(-3, 0)`
- Instruksi 8 (`B`): Koordinat kini `(-4, 0)`
- Instruksi 9 (`B`): Koordinat kini `(-5, 0)`
- Instruksi 10 (`U`): Koordinat kini `(-5, 1)`
- Instruksi 11 (`T`): Koordinat kini `(-4, 1)`
- Instruksi 12 (`S`): Koordinat kini `(-4, 0)`

Posisi akhir robot adalah di titik `(-4, 0)`.
Jarak Manhattan = Murni $|-4| + |0|$ = 4 + 0 = **4 unit**.
Opsi valid: **B**.</details>

---
**Soal 15**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 24, 14, 5, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 38."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 3 pasang
C. 2 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 23 + Sapi 24 = 47 (❌ Gagal)
- Sapi 23 + Sapi 14 = 37 (❌ Gagal)
- Sapi 23 + Sapi 5 = 28 (❌ Gagal)
- Sapi 23 + Sapi 19 = 42 (❌ Gagal)
- Sapi 24 + Sapi 14 = 38 (✅ COCOK)
- Sapi 24 + Sapi 5 = 29 (❌ Gagal)
- Sapi 24 + Sapi 19 = 43 (❌ Gagal)
- Sapi 14 + Sapi 5 = 19 (❌ Gagal)
- Sapi 14 + Sapi 19 = 33 (❌ Gagal)
- Sapi 5 + Sapi 19 = 24 (❌ Gagal)

Total pasangan yang bernilai 38 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 16**
Sebuah robot bola diletakkan di lantai 94. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 47 detik
B. 48 detik
C. 45 detik
D. 46 detik
E. 44 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (45 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 94 (Garis Start)
- Detik 1: Genap, turun 9 -> 94 - 9 = 85
- Detik 2: Ganjil, naik 5 -> 85 + 5 = 90
- Detik 3: Genap, turun 9 -> 90 - 9 = 81
- Detik 4: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 5: Genap, turun 9 -> 86 - 9 = 77
- Detik 6: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 7: Genap, turun 9 -> 82 - 9 = 73
- Detik 8: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 9: Genap, turun 9 -> 78 - 9 = 69
- Detik 10: Ganjil, naik 5 -> 69 + 5 = 74
- Detik 11: Genap, turun 9 -> 74 - 9 = 65
- Detik 12: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 13: Genap, turun 9 -> 70 - 9 = 61
- Detik 14: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 15: Genap, turun 9 -> 66 - 9 = 57
- Detik 16: Ganjil, naik 5 -> 57 + 5 = 62
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 45: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 17**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 5, 7, 21, 11]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 49."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 2 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 5 = 15 (❌ Gagal)
- Sapi 10 + Sapi 7 = 17 (❌ Gagal)
- Sapi 10 + Sapi 21 = 31 (❌ Gagal)
- Sapi 10 + Sapi 11 = 21 (❌ Gagal)
- Sapi 5 + Sapi 7 = 12 (❌ Gagal)
- Sapi 5 + Sapi 21 = 26 (❌ Gagal)
- Sapi 5 + Sapi 11 = 16 (❌ Gagal)
- Sapi 7 + Sapi 21 = 28 (❌ Gagal)
- Sapi 7 + Sapi 11 = 18 (❌ Gagal)
- Sapi 21 + Sapi 11 = 32 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 18**
Sebuah robot bola diletakkan di lantai 52. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 17 detik
B. 18 detik
C. 20 detik
D. 19 detik
E. 16 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (17 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 52 (Garis Start)
- Detik 1: Genap, turun 11 -> 52 - 11 = 41
- Detik 2: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 3: Genap, turun 11 -> 46 - 11 = 35
- Detik 4: Ganjil, naik 5 -> 35 + 5 = 40
- Detik 5: Genap, turun 11 -> 40 - 11 = 29
- Detik 6: Ganjil, naik 5 -> 29 + 5 = 34
- Detik 7: Genap, turun 11 -> 34 - 11 = 23
- Detik 8: Ganjil, naik 5 -> 23 + 5 = 28
- Detik 9: Genap, turun 11 -> 28 - 11 = 17
- Detik 10: Ganjil, naik 5 -> 17 + 5 = 22
- Detik 11: Genap, turun 11 -> 22 - 11 = 11
- Detik 12: Ganjil, naik 5 -> 11 + 5 = 16
- Detik 13: Genap, turun 11 -> 16 - 11 = 5
- Detik 14: Ganjil, naik 5 -> 5 + 5 = 10
- Detik 15: Genap, turun 11 -> 10 - 11 = -1
- Detik 16: Ganjil, naik 5 -> -1 + 5 = 4
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 17: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 19**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUTUBUUBUTTUST`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 10 unit langkah
B. 8 unit langkah
C. 6 unit langkah
D. 7 unit langkah
E. 9 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (8 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(2, 1)`
- Instruksi 4 (`U`): Koordinat kini `(2, 2)`
- Instruksi 5 (`B`): Koordinat kini `(1, 2)`
- Instruksi 6 (`U`): Koordinat kini `(1, 3)`
- Instruksi 7 (`U`): Koordinat kini `(1, 4)`
- Instruksi 8 (`B`): Koordinat kini `(0, 4)`
- Instruksi 9 (`U`): Koordinat kini `(0, 5)`
- Instruksi 10 (`T`): Koordinat kini `(1, 5)`
- Instruksi 11 (`T`): Koordinat kini `(2, 5)`
- Instruksi 12 (`U`): Koordinat kini `(2, 6)`
- Instruksi 13 (`S`): Koordinat kini `(2, 5)`
- Instruksi 14 (`T`): Koordinat kini `(3, 5)`

Posisi akhir robot adalah di titik `(3, 5)`.
Jarak Manhattan = Murni $|3| + |5|$ = 3 + 5 = **8 unit**.
Opsi valid: **B**.</details>

---
**Soal 20**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 8, 21, 16, 7]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 4 pasang
C. 1 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 23 + Sapi 8 = 31 (❌ Gagal)
- Sapi 23 + Sapi 21 = 44 (❌ Gagal)
- Sapi 23 + Sapi 16 = 39 (❌ Gagal)
- Sapi 23 + Sapi 7 = 30 (❌ Gagal)
- Sapi 8 + Sapi 21 = 29 (❌ Gagal)
- Sapi 8 + Sapi 16 = 24 (❌ Gagal)
- Sapi 8 + Sapi 7 = 15 (❌ Gagal)
- Sapi 21 + Sapi 16 = 37 (❌ Gagal)
- Sapi 21 + Sapi 7 = 28 (❌ Gagal)
- Sapi 16 + Sapi 7 = 23 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 21**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 14, 10, 21, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 40."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 4 pasang
C. 3 pasang
D. 2 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 14 = 20 (❌ Gagal)
- Sapi 6 + Sapi 10 = 16 (❌ Gagal)
- Sapi 6 + Sapi 21 = 27 (❌ Gagal)
- Sapi 6 + Sapi 4 = 10 (❌ Gagal)
- Sapi 14 + Sapi 10 = 24 (❌ Gagal)
- Sapi 14 + Sapi 21 = 35 (❌ Gagal)
- Sapi 14 + Sapi 4 = 18 (❌ Gagal)
- Sapi 10 + Sapi 21 = 31 (❌ Gagal)
- Sapi 10 + Sapi 4 = 14 (❌ Gagal)
- Sapi 21 + Sapi 4 = 25 (❌ Gagal)

Total pasangan yang bernilai 40 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 22**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSSBUTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. -2 unit langkah
C. 2 unit langkah
D. -1 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (0 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(0, 1)`
- Instruksi 8 (`S`): Koordinat kini `(0, 0)`

Posisi akhir robot adalah di titik `(0, 0)`.
Jarak Manhattan = Murni $|0| + |0|$ = 0 + 0 = **0 unit**.
Opsi valid: **A**.</details>

---
**Soal 23**
Sebuah robot bola diletakkan di lantai 113. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 29 detik
B. 31 detik
C. 33 detik
D. 32 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (30 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 113 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 113 + 3 = 116
- Detik 2: Genap, turun 11 -> 116 - 11 = 105
- Detik 3: Ganjil, naik 3 -> 105 + 3 = 108
- Detik 4: Genap, turun 11 -> 108 - 11 = 97
- Detik 5: Ganjil, naik 3 -> 97 + 3 = 100
- Detik 6: Genap, turun 11 -> 100 - 11 = 89
- Detik 7: Ganjil, naik 3 -> 89 + 3 = 92
- Detik 8: Genap, turun 11 -> 92 - 11 = 81
- Detik 9: Ganjil, naik 3 -> 81 + 3 = 84
- Detik 10: Genap, turun 11 -> 84 - 11 = 73
- Detik 11: Ganjil, naik 3 -> 73 + 3 = 76
- Detik 12: Genap, turun 11 -> 76 - 11 = 65
- Detik 13: Ganjil, naik 3 -> 65 + 3 = 68
- Detik 14: Genap, turun 11 -> 68 - 11 = 57
- Detik 15: Ganjil, naik 3 -> 57 + 3 = 60
- Detik 16: Genap, turun 11 -> 60 - 11 = 49
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 30: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 24**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[9, 6, 20, 3, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 38."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 4 pasang
C. 1 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 9 + Sapi 6 = 15 (❌ Gagal)
- Sapi 9 + Sapi 20 = 29 (❌ Gagal)
- Sapi 9 + Sapi 3 = 12 (❌ Gagal)
- Sapi 9 + Sapi 19 = 28 (❌ Gagal)
- Sapi 6 + Sapi 20 = 26 (❌ Gagal)
- Sapi 6 + Sapi 3 = 9 (❌ Gagal)
- Sapi 6 + Sapi 19 = 25 (❌ Gagal)
- Sapi 20 + Sapi 3 = 23 (❌ Gagal)
- Sapi 20 + Sapi 19 = 39 (❌ Gagal)
- Sapi 3 + Sapi 19 = 22 (❌ Gagal)

Total pasangan yang bernilai 38 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 25**
Sebuah robot bola diletakkan di lantai 69. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
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
- Detik 0: Posisi = 69 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 2: Genap, turun 9 -> 70 - 9 = 61
- Detik 3: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 4: Genap, turun 9 -> 62 - 9 = 53
- Detik 5: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 6: Genap, turun 9 -> 54 - 9 = 45
- Detik 7: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 8: Genap, turun 9 -> 46 - 9 = 37
- Detik 9: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 10: Genap, turun 9 -> 38 - 9 = 29
- Detik 11: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 12: Genap, turun 9 -> 30 - 9 = 21
- Detik 13: Ganjil, naik 1 -> 21 + 1 = 22
- Detik 14: Genap, turun 9 -> 22 - 9 = 13
- Detik 15: Ganjil, naik 1 -> 13 + 1 = 14
- Detik 16: Genap, turun 9 -> 14 - 9 = 5
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 18: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 26**
Sebuah robot bola diletakkan di lantai 116. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 26 detik
C. 30 detik
D. 29 detik
E. 27 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (27 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 116 (Garis Start)
- Detik 1: Genap, turun 13 -> 116 - 13 = 103
- Detik 2: Ganjil, naik 5 -> 103 + 5 = 108
- Detik 3: Genap, turun 13 -> 108 - 13 = 95
- Detik 4: Ganjil, naik 5 -> 95 + 5 = 100
- Detik 5: Genap, turun 13 -> 100 - 13 = 87
- Detik 6: Ganjil, naik 5 -> 87 + 5 = 92
- Detik 7: Genap, turun 13 -> 92 - 13 = 79
- Detik 8: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 9: Genap, turun 13 -> 84 - 13 = 71
- Detik 10: Ganjil, naik 5 -> 71 + 5 = 76
- Detik 11: Genap, turun 13 -> 76 - 13 = 63
- Detik 12: Ganjil, naik 5 -> 63 + 5 = 68
- Detik 13: Genap, turun 13 -> 68 - 13 = 55
- Detik 14: Ganjil, naik 5 -> 55 + 5 = 60
- Detik 15: Genap, turun 13 -> 60 - 13 = 47
- Detik 16: Ganjil, naik 5 -> 47 + 5 = 52
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 27: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 27**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 8, 5, 4, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 1 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 8 = 14 (❌ Gagal)
- Sapi 6 + Sapi 5 = 11 (❌ Gagal)
- Sapi 6 + Sapi 4 = 10 (❌ Gagal)
- Sapi 6 + Sapi 17 = 23 (❌ Gagal)
- Sapi 8 + Sapi 5 = 13 (❌ Gagal)
- Sapi 8 + Sapi 4 = 12 (❌ Gagal)
- Sapi 8 + Sapi 17 = 25 (❌ Gagal)
- Sapi 5 + Sapi 4 = 9 (❌ Gagal)
- Sapi 5 + Sapi 17 = 22 (❌ Gagal)
- Sapi 4 + Sapi 17 = 21 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 28**
Sebuah robot bola diletakkan di lantai 55. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 20 detik
B. 19 detik
C. 22 detik
D. 23 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (20 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 55 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 2: Genap, turun 9 -> 58 - 9 = 49
- Detik 3: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 4: Genap, turun 9 -> 52 - 9 = 43
- Detik 5: Ganjil, naik 3 -> 43 + 3 = 46
- Detik 6: Genap, turun 9 -> 46 - 9 = 37
- Detik 7: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 8: Genap, turun 9 -> 40 - 9 = 31
- Detik 9: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 10: Genap, turun 9 -> 34 - 9 = 25
- Detik 11: Ganjil, naik 3 -> 25 + 3 = 28
- Detik 12: Genap, turun 9 -> 28 - 9 = 19
- Detik 13: Ganjil, naik 3 -> 19 + 3 = 22
- Detik 14: Genap, turun 9 -> 22 - 9 = 13
- Detik 15: Ganjil, naik 3 -> 13 + 3 = 16
- Detik 16: Genap, turun 9 -> 16 - 9 = 7
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 20: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 29**
Sebuah robot bola diletakkan di lantai 93. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 27 detik
B. 26 detik
C. 25 detik
D. 23 detik
E. 24 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (24 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 93 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 93 + 1 = 94
- Detik 2: Genap, turun 9 -> 94 - 9 = 85
- Detik 3: Ganjil, naik 1 -> 85 + 1 = 86
- Detik 4: Genap, turun 9 -> 86 - 9 = 77
- Detik 5: Ganjil, naik 1 -> 77 + 1 = 78
- Detik 6: Genap, turun 9 -> 78 - 9 = 69
- Detik 7: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 8: Genap, turun 9 -> 70 - 9 = 61
- Detik 9: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 10: Genap, turun 9 -> 62 - 9 = 53
- Detik 11: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 12: Genap, turun 9 -> 54 - 9 = 45
- Detik 13: Ganjil, naik 1 -> 45 + 1 = 46
- Detik 14: Genap, turun 9 -> 46 - 9 = 37
- Detik 15: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 16: Genap, turun 9 -> 38 - 9 = 29
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 24: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 30**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SUBUUUUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 2 unit langkah
C. 4 unit langkah
D. 6 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 0)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`U`): Koordinat kini `(-1, 3)`
- Instruksi 7 (`U`): Koordinat kini `(-1, 4)`
- Instruksi 8 (`S`): Koordinat kini `(-1, 3)`

Posisi akhir robot adalah di titik `(-1, 3)`.
Jarak Manhattan = Murni $|-1| + |3|$ = 1 + 3 = **4 unit**.
Opsi valid: **C**.</details>

---
**Soal 31**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 7, 15, 23, 12]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 2 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 7 = 17 (❌ Gagal)
- Sapi 10 + Sapi 15 = 25 (❌ Gagal)
- Sapi 10 + Sapi 23 = 33 (❌ Gagal)
- Sapi 10 + Sapi 12 = 22 (❌ Gagal)
- Sapi 7 + Sapi 15 = 22 (❌ Gagal)
- Sapi 7 + Sapi 23 = 30 (❌ Gagal)
- Sapi 7 + Sapi 12 = 19 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 15 + Sapi 12 = 27 (❌ Gagal)
- Sapi 23 + Sapi 12 = 35 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 32**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 15, 19, 11, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 48."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 0 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 15 = 39 (❌ Gagal)
- Sapi 24 + Sapi 19 = 43 (❌ Gagal)
- Sapi 24 + Sapi 11 = 35 (❌ Gagal)
- Sapi 24 + Sapi 2 = 26 (❌ Gagal)
- Sapi 15 + Sapi 19 = 34 (❌ Gagal)
- Sapi 15 + Sapi 11 = 26 (❌ Gagal)
- Sapi 15 + Sapi 2 = 17 (❌ Gagal)
- Sapi 19 + Sapi 11 = 30 (❌ Gagal)
- Sapi 19 + Sapi 2 = 21 (❌ Gagal)
- Sapi 11 + Sapi 2 = 13 (❌ Gagal)

Total pasangan yang bernilai 48 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 33**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUBTTUUTTBUTBBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 4 unit langkah
C. 3 unit langkah
D. 5 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(0, 1)`
- Instruksi 4 (`T`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`U`): Koordinat kini `(2, 2)`
- Instruksi 7 (`U`): Koordinat kini `(2, 3)`
- Instruksi 8 (`T`): Koordinat kini `(3, 3)`
- Instruksi 9 (`T`): Koordinat kini `(4, 3)`
- Instruksi 10 (`B`): Koordinat kini `(3, 3)`
- Instruksi 11 (`U`): Koordinat kini `(3, 4)`
- Instruksi 12 (`T`): Koordinat kini `(4, 4)`
- Instruksi 13 (`B`): Koordinat kini `(3, 4)`
- Instruksi 14 (`B`): Koordinat kini `(2, 4)`
- Instruksi 15 (`S`): Koordinat kini `(2, 3)`

Posisi akhir robot adalah di titik `(2, 3)`.
Jarak Manhattan = Murni $|2| + |3|$ = 2 + 3 = **5 unit**.
Opsi valid: **D**.</details>

---
**Soal 34**
Sebuah robot bola diletakkan di lantai 82. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 16 detik
B. 17 detik
C. 20 detik
D. 19 detik
E. 18 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (17 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 82 (Garis Start)
- Detik 1: Genap, turun 13 -> 82 - 13 = 69
- Detik 2: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 3: Genap, turun 13 -> 72 - 13 = 59
- Detik 4: Ganjil, naik 3 -> 59 + 3 = 62
- Detik 5: Genap, turun 13 -> 62 - 13 = 49
- Detik 6: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 7: Genap, turun 13 -> 52 - 13 = 39
- Detik 8: Ganjil, naik 3 -> 39 + 3 = 42
- Detik 9: Genap, turun 13 -> 42 - 13 = 29
- Detik 10: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 11: Genap, turun 13 -> 32 - 13 = 19
- Detik 12: Ganjil, naik 3 -> 19 + 3 = 22
- Detik 13: Genap, turun 13 -> 22 - 13 = 9
- Detik 14: Ganjil, naik 3 -> 9 + 3 = 12
- Detik 15: Genap, turun 13 -> 12 - 13 = -1
- Detik 16: Ganjil, naik 3 -> -1 + 3 = 2
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 17: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 35**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 15, 12, 9, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 0 pasang
D. 4 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 15 = 18 (❌ Gagal)
- Sapi 3 + Sapi 12 = 15 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 6 = 9 (❌ Gagal)
- Sapi 15 + Sapi 12 = 27 (❌ Gagal)
- Sapi 15 + Sapi 9 = 24 (❌ Gagal)
- Sapi 15 + Sapi 6 = 21 (❌ Gagal)
- Sapi 12 + Sapi 9 = 21 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 9 + Sapi 6 = 15 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 36**
Sebuah robot bola diletakkan di lantai 121. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 32 detik
B. 34 detik
C. 33 detik
D. 31 detik
E. 35 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (32 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 121 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 121 + 3 = 124
- Detik 2: Genap, turun 11 -> 124 - 11 = 113
- Detik 3: Ganjil, naik 3 -> 113 + 3 = 116
- Detik 4: Genap, turun 11 -> 116 - 11 = 105
- Detik 5: Ganjil, naik 3 -> 105 + 3 = 108
- Detik 6: Genap, turun 11 -> 108 - 11 = 97
- Detik 7: Ganjil, naik 3 -> 97 + 3 = 100
- Detik 8: Genap, turun 11 -> 100 - 11 = 89
- Detik 9: Ganjil, naik 3 -> 89 + 3 = 92
- Detik 10: Genap, turun 11 -> 92 - 11 = 81
- Detik 11: Ganjil, naik 3 -> 81 + 3 = 84
- Detik 12: Genap, turun 11 -> 84 - 11 = 73
- Detik 13: Ganjil, naik 3 -> 73 + 3 = 76
- Detik 14: Genap, turun 11 -> 76 - 11 = 65
- Detik 15: Ganjil, naik 3 -> 65 + 3 = 68
- Detik 16: Genap, turun 11 -> 68 - 11 = 57
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 32: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 37**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBSTUSSTSSSSB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 7 unit langkah
B. 8 unit langkah
C. 9 unit langkah
D. 6 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (7 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`S`): Koordinat kini `(0, -1)`
- Instruksi 4 (`T`): Koordinat kini `(1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(1, -2)`
- Instruksi 8 (`T`): Koordinat kini `(2, -2)`
- Instruksi 9 (`S`): Koordinat kini `(2, -3)`
- Instruksi 10 (`S`): Koordinat kini `(2, -4)`
- Instruksi 11 (`S`): Koordinat kini `(2, -5)`
- Instruksi 12 (`S`): Koordinat kini `(2, -6)`
- Instruksi 13 (`B`): Koordinat kini `(1, -6)`

Posisi akhir robot adalah di titik `(1, -6)`.
Jarak Manhattan = Murni $|1| + |-6|$ = 1 + 6 = **7 unit**.
Opsi valid: **A**.</details>

---
**Soal 38**
Sebuah robot bola diletakkan di lantai 109. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 40 detik
B. 42 detik
C. 39 detik
D. 43 detik
E. 41 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (40 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 109 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 109 + 3 = 112
- Detik 2: Genap, turun 9 -> 112 - 9 = 103
- Detik 3: Ganjil, naik 3 -> 103 + 3 = 106
- Detik 4: Genap, turun 9 -> 106 - 9 = 97
- Detik 5: Ganjil, naik 3 -> 97 + 3 = 100
- Detik 6: Genap, turun 9 -> 100 - 9 = 91
- Detik 7: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 8: Genap, turun 9 -> 94 - 9 = 85
- Detik 9: Ganjil, naik 3 -> 85 + 3 = 88
- Detik 10: Genap, turun 9 -> 88 - 9 = 79
- Detik 11: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 12: Genap, turun 9 -> 82 - 9 = 73
- Detik 13: Ganjil, naik 3 -> 73 + 3 = 76
- Detik 14: Genap, turun 9 -> 76 - 9 = 67
- Detik 15: Ganjil, naik 3 -> 67 + 3 = 70
- Detik 16: Genap, turun 9 -> 70 - 9 = 61
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 40: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 39**
Sebuah robot bola diletakkan di lantai 52. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 15 detik
B. 12 detik
C. 13 detik
D. 14 detik
E. 16 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (13 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 52 (Garis Start)
- Detik 1: Genap, turun 9 -> 52 - 9 = 43
- Detik 2: Ganjil, naik 1 -> 43 + 1 = 44
- Detik 3: Genap, turun 9 -> 44 - 9 = 35
- Detik 4: Ganjil, naik 1 -> 35 + 1 = 36
- Detik 5: Genap, turun 9 -> 36 - 9 = 27
- Detik 6: Ganjil, naik 1 -> 27 + 1 = 28
- Detik 7: Genap, turun 9 -> 28 - 9 = 19
- Detik 8: Ganjil, naik 1 -> 19 + 1 = 20
- Detik 9: Genap, turun 9 -> 20 - 9 = 11
- Detik 10: Ganjil, naik 1 -> 11 + 1 = 12
- Detik 11: Genap, turun 9 -> 12 - 9 = 3
- Detik 12: Ganjil, naik 1 -> 3 + 1 = 4
- Detik 13: Genap, turun 9 -> 4 - 9 = -5
Simulasi berakhir pada detik ke-13. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 40**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SUUBUSTTSSUSBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. 4 unit langkah
C. 3 unit langkah
D. 1 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 0)`
- Instruksi 3 (`U`): Koordinat kini `(0, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(0, 1)`
- Instruksi 8 (`T`): Koordinat kini `(1, 1)`
- Instruksi 9 (`S`): Koordinat kini `(1, 0)`
- Instruksi 10 (`S`): Koordinat kini `(1, -1)`
- Instruksi 11 (`U`): Koordinat kini `(1, 0)`
- Instruksi 12 (`S`): Koordinat kini `(1, -1)`
- Instruksi 13 (`B`): Koordinat kini `(0, -1)`
- Instruksi 14 (`B`): Koordinat kini `(-1, -1)`

Posisi akhir robot adalah di titik `(-1, -1)`.
Jarak Manhattan = Murni $|-1| + |-1|$ = 1 + 1 = **2 unit**.
Opsi valid: **E**.</details>

---
**Soal 41**
Sebuah robot bola diletakkan di lantai 71. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 17 detik
B. 20 detik
C. 19 detik
D. 18 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (18 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 71 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 2: Genap, turun 11 -> 74 - 11 = 63
- Detik 3: Ganjil, naik 3 -> 63 + 3 = 66
- Detik 4: Genap, turun 11 -> 66 - 11 = 55
- Detik 5: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 6: Genap, turun 11 -> 58 - 11 = 47
- Detik 7: Ganjil, naik 3 -> 47 + 3 = 50
- Detik 8: Genap, turun 11 -> 50 - 11 = 39
- Detik 9: Ganjil, naik 3 -> 39 + 3 = 42
- Detik 10: Genap, turun 11 -> 42 - 11 = 31
- Detik 11: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 12: Genap, turun 11 -> 34 - 11 = 23
- Detik 13: Ganjil, naik 3 -> 23 + 3 = 26
- Detik 14: Genap, turun 11 -> 26 - 11 = 15
- Detik 15: Ganjil, naik 3 -> 15 + 3 = 18
- Detik 16: Genap, turun 11 -> 18 - 11 = 7
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 18: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 42**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBBTSSTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 0 unit langkah
C. 3 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 4 (`T`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`T`): Koordinat kini `(0, -1)`
- Instruksi 8 (`T`): Koordinat kini `(1, -1)`

Posisi akhir robot adalah di titik `(1, -1)`.
Jarak Manhattan = Murni $|1| + |-1|$ = 1 + 1 = **2 unit**.
Opsi valid: **D**.</details>

---
**Soal 43**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[20, 13, 4, 12, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 34."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 0 pasang
C. 3 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 20 + Sapi 13 = 33 (❌ Gagal)
- Sapi 20 + Sapi 4 = 24 (❌ Gagal)
- Sapi 20 + Sapi 12 = 32 (❌ Gagal)
- Sapi 20 + Sapi 5 = 25 (❌ Gagal)
- Sapi 13 + Sapi 4 = 17 (❌ Gagal)
- Sapi 13 + Sapi 12 = 25 (❌ Gagal)
- Sapi 13 + Sapi 5 = 18 (❌ Gagal)
- Sapi 4 + Sapi 12 = 16 (❌ Gagal)
- Sapi 4 + Sapi 5 = 9 (❌ Gagal)
- Sapi 12 + Sapi 5 = 17 (❌ Gagal)

Total pasangan yang bernilai 34 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 44**
Sebuah robot bola diletakkan di lantai 58. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 21 detik
B. 24 detik
C. 20 detik
D. 23 detik
E. 22 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (21 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 58 (Garis Start)
- Detik 1: Genap, turun 9 -> 58 - 9 = 49
- Detik 2: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 3: Genap, turun 9 -> 52 - 9 = 43
- Detik 4: Ganjil, naik 3 -> 43 + 3 = 46
- Detik 5: Genap, turun 9 -> 46 - 9 = 37
- Detik 6: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 7: Genap, turun 9 -> 40 - 9 = 31
- Detik 8: Ganjil, naik 3 -> 31 + 3 = 34
- Detik 9: Genap, turun 9 -> 34 - 9 = 25
- Detik 10: Ganjil, naik 3 -> 25 + 3 = 28
- Detik 11: Genap, turun 9 -> 28 - 9 = 19
- Detik 12: Ganjil, naik 3 -> 19 + 3 = 22
- Detik 13: Genap, turun 9 -> 22 - 9 = 13
- Detik 14: Ganjil, naik 3 -> 13 + 3 = 16
- Detik 15: Genap, turun 9 -> 16 - 9 = 7
- Detik 16: Ganjil, naik 3 -> 7 + 3 = 10
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 21: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 45**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 17, 18, 10, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 31."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 4 pasang
C. 1 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 17 = 41 (❌ Gagal)
- Sapi 24 + Sapi 18 = 42 (❌ Gagal)
- Sapi 24 + Sapi 10 = 34 (❌ Gagal)
- Sapi 24 + Sapi 19 = 43 (❌ Gagal)
- Sapi 17 + Sapi 18 = 35 (❌ Gagal)
- Sapi 17 + Sapi 10 = 27 (❌ Gagal)
- Sapi 17 + Sapi 19 = 36 (❌ Gagal)
- Sapi 18 + Sapi 10 = 28 (❌ Gagal)
- Sapi 18 + Sapi 19 = 37 (❌ Gagal)
- Sapi 10 + Sapi 19 = 29 (❌ Gagal)

Total pasangan yang bernilai 31 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 46**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[5, 14, 6, 20, 3]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 46."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 0 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 5 + Sapi 14 = 19 (❌ Gagal)
- Sapi 5 + Sapi 6 = 11 (❌ Gagal)
- Sapi 5 + Sapi 20 = 25 (❌ Gagal)
- Sapi 5 + Sapi 3 = 8 (❌ Gagal)
- Sapi 14 + Sapi 6 = 20 (❌ Gagal)
- Sapi 14 + Sapi 20 = 34 (❌ Gagal)
- Sapi 14 + Sapi 3 = 17 (❌ Gagal)
- Sapi 6 + Sapi 20 = 26 (❌ Gagal)
- Sapi 6 + Sapi 3 = 9 (❌ Gagal)
- Sapi 20 + Sapi 3 = 23 (❌ Gagal)

Total pasangan yang bernilai 46 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 47**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[2, 16, 10, 14, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 2 pasang
D. 0 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 2 + Sapi 16 = 18 (❌ Gagal)
- Sapi 2 + Sapi 10 = 12 (❌ Gagal)
- Sapi 2 + Sapi 14 = 16 (❌ Gagal)
- Sapi 2 + Sapi 15 = 17 (❌ Gagal)
- Sapi 16 + Sapi 10 = 26 (❌ Gagal)
- Sapi 16 + Sapi 14 = 30 (❌ Gagal)
- Sapi 16 + Sapi 15 = 31 (❌ Gagal)
- Sapi 10 + Sapi 14 = 24 (❌ Gagal)
- Sapi 10 + Sapi 15 = 25 (❌ Gagal)
- Sapi 14 + Sapi 15 = 29 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 48**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBTUTBUBUBSSU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 3 unit langkah
C. 5 unit langkah
D. 4 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`B`): Koordinat kini `(1, 1)`
- Instruksi 7 (`U`): Koordinat kini `(1, 2)`
- Instruksi 8 (`B`): Koordinat kini `(0, 2)`
- Instruksi 9 (`U`): Koordinat kini `(0, 3)`
- Instruksi 10 (`B`): Koordinat kini `(-1, 3)`
- Instruksi 11 (`S`): Koordinat kini `(-1, 2)`
- Instruksi 12 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 13 (`U`): Koordinat kini `(-1, 2)`

Posisi akhir robot adalah di titik `(-1, 2)`.
Jarak Manhattan = Murni $|-1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **B**.</details>

---
**Soal 49**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 2, 10, 12, 20]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 40."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 2 pasang
C. 0 pasang
D. 4 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 2 = 26 (❌ Gagal)
- Sapi 24 + Sapi 10 = 34 (❌ Gagal)
- Sapi 24 + Sapi 12 = 36 (❌ Gagal)
- Sapi 24 + Sapi 20 = 44 (❌ Gagal)
- Sapi 2 + Sapi 10 = 12 (❌ Gagal)
- Sapi 2 + Sapi 12 = 14 (❌ Gagal)
- Sapi 2 + Sapi 20 = 22 (❌ Gagal)
- Sapi 10 + Sapi 12 = 22 (❌ Gagal)
- Sapi 10 + Sapi 20 = 30 (❌ Gagal)
- Sapi 12 + Sapi 20 = 32 (❌ Gagal)

Total pasangan yang bernilai 40 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 50**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 12, 9, 3, 23]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 49."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 0 pasang
C. 2 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 12 = 36 (❌ Gagal)
- Sapi 24 + Sapi 9 = 33 (❌ Gagal)
- Sapi 24 + Sapi 3 = 27 (❌ Gagal)
- Sapi 24 + Sapi 23 = 47 (❌ Gagal)
- Sapi 12 + Sapi 9 = 21 (❌ Gagal)
- Sapi 12 + Sapi 3 = 15 (❌ Gagal)
- Sapi 12 + Sapi 23 = 35 (❌ Gagal)
- Sapi 9 + Sapi 3 = 12 (❌ Gagal)
- Sapi 9 + Sapi 23 = 32 (❌ Gagal)
- Sapi 3 + Sapi 23 = 26 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
