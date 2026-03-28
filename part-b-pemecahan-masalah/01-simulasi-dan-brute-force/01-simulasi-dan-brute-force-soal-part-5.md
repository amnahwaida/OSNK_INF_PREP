# Latian Soal: Simulasi & Brute Force (Part 5 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 201**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSTTUTTSTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 7 unit langkah
B. 6 unit langkah
C. 10 unit langkah
D. 8 unit langkah
E. 9 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (8 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`T`): Koordinat kini `(1, -2)`
- Instruksi 4 (`T`): Koordinat kini `(2, -2)`
- Instruksi 5 (`U`): Koordinat kini `(2, -1)`
- Instruksi 6 (`T`): Koordinat kini `(3, -1)`
- Instruksi 7 (`T`): Koordinat kini `(4, -1)`
- Instruksi 8 (`S`): Koordinat kini `(4, -2)`
- Instruksi 9 (`T`): Koordinat kini `(5, -2)`
- Instruksi 10 (`S`): Koordinat kini `(5, -3)`

Posisi akhir robot adalah di titik `(5, -3)`.
Jarak Manhattan = Murni $|5| + |-3|$ = 5 + 3 = **8 unit**.
Opsi valid: **D**.</details>

---
**Soal 202**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSTSSUTTTUSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 8 unit langkah
C. 5 unit langkah
D. 6 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(0, -1)`
- Instruksi 4 (`S`): Koordinat kini `(0, -2)`
- Instruksi 5 (`S`): Koordinat kini `(0, -3)`
- Instruksi 6 (`U`): Koordinat kini `(0, -2)`
- Instruksi 7 (`T`): Koordinat kini `(1, -2)`
- Instruksi 8 (`T`): Koordinat kini `(2, -2)`
- Instruksi 9 (`T`): Koordinat kini `(3, -2)`
- Instruksi 10 (`U`): Koordinat kini `(3, -1)`
- Instruksi 11 (`S`): Koordinat kini `(3, -2)`
- Instruksi 12 (`S`): Koordinat kini `(3, -3)`

Posisi akhir robot adalah di titik `(3, -3)`.
Jarak Manhattan = Murni $|3| + |-3|$ = 3 + 3 = **6 unit**.
Opsi valid: **D**.</details>

---
**Soal 203**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSTBSBUBUBUTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 1 unit langkah
C. 2 unit langkah
D. 0 unit langkah
E. -1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(2, -1)`
- Instruksi 4 (`B`): Koordinat kini `(1, -1)`
- Instruksi 5 (`S`): Koordinat kini `(1, -2)`
- Instruksi 6 (`B`): Koordinat kini `(0, -2)`
- Instruksi 7 (`U`): Koordinat kini `(0, -1)`
- Instruksi 8 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 10 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 11 (`U`): Koordinat kini `(-2, 1)`
- Instruksi 12 (`T`): Koordinat kini `(-1, 1)`
- Instruksi 13 (`S`): Koordinat kini `(-1, 0)`

Posisi akhir robot adalah di titik `(-1, 0)`.
Jarak Manhattan = Murni $|-1| + |0|$ = 1 + 0 = **1 unit**.
Opsi valid: **B**.</details>

---
**Soal 204**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 2, 16, 7, 14]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 2 pasang
C. 3 pasang
D. 0 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 2 = 26 (❌ Gagal)
- Sapi 24 + Sapi 16 = 40 (❌ Gagal)
- Sapi 24 + Sapi 7 = 31 (❌ Gagal)
- Sapi 24 + Sapi 14 = 38 (❌ Gagal)
- Sapi 2 + Sapi 16 = 18 (❌ Gagal)
- Sapi 2 + Sapi 7 = 9 (❌ Gagal)
- Sapi 2 + Sapi 14 = 16 (❌ Gagal)
- Sapi 16 + Sapi 7 = 23 (❌ Gagal)
- Sapi 16 + Sapi 14 = 30 (❌ Gagal)
- Sapi 7 + Sapi 14 = 21 (❌ Gagal)

Total pasangan yang bernilai 29 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 205**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 20, 6, 13, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 2 pasang
C. 1 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 23 + Sapi 20 = 43 (❌ Gagal)
- Sapi 23 + Sapi 6 = 29 (✅ COCOK)
- Sapi 23 + Sapi 13 = 36 (❌ Gagal)
- Sapi 23 + Sapi 10 = 33 (❌ Gagal)
- Sapi 20 + Sapi 6 = 26 (❌ Gagal)
- Sapi 20 + Sapi 13 = 33 (❌ Gagal)
- Sapi 20 + Sapi 10 = 30 (❌ Gagal)
- Sapi 6 + Sapi 13 = 19 (❌ Gagal)
- Sapi 6 + Sapi 10 = 16 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)

Total pasangan yang bernilai 29 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 206**
Sebuah robot bola diletakkan di lantai 76. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 30 detik
C. 29 detik
D. 27 detik
E. 26 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (27 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 76 (Garis Start)
- Detik 1: Genap, turun 11 -> 76 - 11 = 65
- Detik 2: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 3: Genap, turun 11 -> 70 - 11 = 59
- Detik 4: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 5: Genap, turun 11 -> 64 - 11 = 53
- Detik 6: Ganjil, naik 5 -> 53 + 5 = 58
- Detik 7: Genap, turun 11 -> 58 - 11 = 47
- Detik 8: Ganjil, naik 5 -> 47 + 5 = 52
- Detik 9: Genap, turun 11 -> 52 - 11 = 41
- Detik 10: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 11: Genap, turun 11 -> 46 - 11 = 35
- Detik 12: Ganjil, naik 5 -> 35 + 5 = 40
- Detik 13: Genap, turun 11 -> 40 - 11 = 29
- Detik 14: Ganjil, naik 5 -> 29 + 5 = 34
- Detik 15: Genap, turun 11 -> 34 - 11 = 23
- Detik 16: Ganjil, naik 5 -> 23 + 5 = 28
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 27: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 207**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBUSBTTTBTTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 3 unit langkah
C. 5 unit langkah
D. 4 unit langkah
E. 6 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 4 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`T`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(0, 1)`
- Instruksi 8 (`T`): Koordinat kini `(1, 1)`
- Instruksi 9 (`B`): Koordinat kini `(0, 1)`
- Instruksi 10 (`T`): Koordinat kini `(1, 1)`
- Instruksi 11 (`T`): Koordinat kini `(2, 1)`
- Instruksi 12 (`T`): Koordinat kini `(3, 1)`

Posisi akhir robot adalah di titik `(3, 1)`.
Jarak Manhattan = Murni $|3| + |1|$ = 3 + 1 = **4 unit**.
Opsi valid: **D**.</details>

---
**Soal 208**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[7, 3, 2, 9, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 41."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 0 pasang
D. 4 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 7 + Sapi 3 = 10 (❌ Gagal)
- Sapi 7 + Sapi 2 = 9 (❌ Gagal)
- Sapi 7 + Sapi 9 = 16 (❌ Gagal)
- Sapi 7 + Sapi 4 = 11 (❌ Gagal)
- Sapi 3 + Sapi 2 = 5 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 4 = 7 (❌ Gagal)
- Sapi 2 + Sapi 9 = 11 (❌ Gagal)
- Sapi 2 + Sapi 4 = 6 (❌ Gagal)
- Sapi 9 + Sapi 4 = 13 (❌ Gagal)

Total pasangan yang bernilai 41 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 209**
Sebuah robot bola diletakkan di lantai 54. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 16 detik
B. 18 detik
C. 20 detik
D. 19 detik
E. 17 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (17 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 54 (Garis Start)
- Detik 1: Genap, turun 7 -> 54 - 7 = 47
- Detik 2: Ganjil, naik 1 -> 47 + 1 = 48
- Detik 3: Genap, turun 7 -> 48 - 7 = 41
- Detik 4: Ganjil, naik 1 -> 41 + 1 = 42
- Detik 5: Genap, turun 7 -> 42 - 7 = 35
- Detik 6: Ganjil, naik 1 -> 35 + 1 = 36
- Detik 7: Genap, turun 7 -> 36 - 7 = 29
- Detik 8: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 9: Genap, turun 7 -> 30 - 7 = 23
- Detik 10: Ganjil, naik 1 -> 23 + 1 = 24
- Detik 11: Genap, turun 7 -> 24 - 7 = 17
- Detik 12: Ganjil, naik 1 -> 17 + 1 = 18
- Detik 13: Genap, turun 7 -> 18 - 7 = 11
- Detik 14: Ganjil, naik 1 -> 11 + 1 = 12
- Detik 15: Genap, turun 7 -> 12 - 7 = 5
- Detik 16: Ganjil, naik 1 -> 5 + 1 = 6
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 17: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 210**
Sebuah robot bola diletakkan di lantai 149. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 43 detik
B. 41 detik
C. 42 detik
D. 40 detik
E. 39 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (40 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 149 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 149 + 3 = 152
- Detik 2: Genap, turun 11 -> 152 - 11 = 141
- Detik 3: Ganjil, naik 3 -> 141 + 3 = 144
- Detik 4: Genap, turun 11 -> 144 - 11 = 133
- Detik 5: Ganjil, naik 3 -> 133 + 3 = 136
- Detik 6: Genap, turun 11 -> 136 - 11 = 125
- Detik 7: Ganjil, naik 3 -> 125 + 3 = 128
- Detik 8: Genap, turun 11 -> 128 - 11 = 117
- Detik 9: Ganjil, naik 3 -> 117 + 3 = 120
- Detik 10: Genap, turun 11 -> 120 - 11 = 109
- Detik 11: Ganjil, naik 3 -> 109 + 3 = 112
- Detik 12: Genap, turun 11 -> 112 - 11 = 101
- Detik 13: Ganjil, naik 3 -> 101 + 3 = 104
- Detik 14: Genap, turun 11 -> 104 - 11 = 93
- Detik 15: Ganjil, naik 3 -> 93 + 3 = 96
- Detik 16: Genap, turun 11 -> 96 - 11 = 85
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 40: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 211**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 17, 11, 15, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 28."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 0 pasang
D. 4 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 17 = 20 (❌ Gagal)
- Sapi 3 + Sapi 11 = 14 (❌ Gagal)
- Sapi 3 + Sapi 15 = 18 (❌ Gagal)
- Sapi 3 + Sapi 4 = 7 (❌ Gagal)
- Sapi 17 + Sapi 11 = 28 (✅ COCOK)
- Sapi 17 + Sapi 15 = 32 (❌ Gagal)
- Sapi 17 + Sapi 4 = 21 (❌ Gagal)
- Sapi 11 + Sapi 15 = 26 (❌ Gagal)
- Sapi 11 + Sapi 4 = 15 (❌ Gagal)
- Sapi 15 + Sapi 4 = 19 (❌ Gagal)

Total pasangan yang bernilai 28 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 212**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 18, 16, 23, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 4 pasang
C. 2 pasang
D. 1 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 18 = 40 (❌ Gagal)
- Sapi 22 + Sapi 16 = 38 (❌ Gagal)
- Sapi 22 + Sapi 23 = 45 (❌ Gagal)
- Sapi 22 + Sapi 19 = 41 (❌ Gagal)
- Sapi 18 + Sapi 16 = 34 (❌ Gagal)
- Sapi 18 + Sapi 23 = 41 (❌ Gagal)
- Sapi 18 + Sapi 19 = 37 (❌ Gagal)
- Sapi 16 + Sapi 23 = 39 (❌ Gagal)
- Sapi 16 + Sapi 19 = 35 (❌ Gagal)
- Sapi 23 + Sapi 19 = 42 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 213**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BTUTTUTBBBBST`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. -1 unit langkah
B. 2 unit langkah
C. 1 unit langkah
D. 3 unit langkah
E. 0 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(0, 0)`
- Instruksi 3 (`U`): Koordinat kini `(0, 1)`
- Instruksi 4 (`T`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`U`): Koordinat kini `(2, 2)`
- Instruksi 7 (`T`): Koordinat kini `(3, 2)`
- Instruksi 8 (`B`): Koordinat kini `(2, 2)`
- Instruksi 9 (`B`): Koordinat kini `(1, 2)`
- Instruksi 10 (`B`): Koordinat kini `(0, 2)`
- Instruksi 11 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 12 (`S`): Koordinat kini `(-1, 1)`
- Instruksi 13 (`T`): Koordinat kini `(0, 1)`

Posisi akhir robot adalah di titik `(0, 1)`.
Jarak Manhattan = Murni $|0| + |1|$ = 0 + 1 = **1 unit**.
Opsi valid: **C**.</details>

---
**Soal 214**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TTTBUTUUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 8 unit langkah
B. 7 unit langkah
C. 6 unit langkah
D. 9 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (7 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(2, 0)`
- Instruksi 3 (`T`): Koordinat kini `(3, 0)`
- Instruksi 4 (`B`): Koordinat kini `(2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(2, 1)`
- Instruksi 6 (`T`): Koordinat kini `(3, 1)`
- Instruksi 7 (`U`): Koordinat kini `(3, 2)`
- Instruksi 8 (`U`): Koordinat kini `(3, 3)`
- Instruksi 9 (`T`): Koordinat kini `(4, 3)`

Posisi akhir robot adalah di titik `(4, 3)`.
Jarak Manhattan = Murni $|4| + |3|$ = 4 + 3 = **7 unit**.
Opsi valid: **B**.</details>

---
**Soal 215**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUUBUSSBT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 4 unit langkah
C. 5 unit langkah
D. 1 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`U`): Koordinat kini `(0, 3)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 3)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 4)`
- Instruksi 6 (`S`): Koordinat kini `(-1, 3)`
- Instruksi 7 (`S`): Koordinat kini `(-1, 2)`
- Instruksi 8 (`B`): Koordinat kini `(-2, 2)`
- Instruksi 9 (`T`): Koordinat kini `(-1, 2)`

Posisi akhir robot adalah di titik `(-1, 2)`.
Jarak Manhattan = Murni $|-1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 216**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSTUUSUBBBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 4 unit langkah
C. 3 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(2, -1)`
- Instruksi 4 (`U`): Koordinat kini `(2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(2, 1)`
- Instruksi 6 (`S`): Koordinat kini `(2, 0)`
- Instruksi 7 (`U`): Koordinat kini `(2, 1)`
- Instruksi 8 (`B`): Koordinat kini `(1, 1)`
- Instruksi 9 (`B`): Koordinat kini `(0, 1)`
- Instruksi 10 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 11 (`B`): Koordinat kini `(-2, 1)`

Posisi akhir robot adalah di titik `(-2, 1)`.
Jarak Manhattan = Murni $|-2| + |1|$ = 2 + 1 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 217**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[16, 15, 13, 2, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 36."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 4 pasang
C. 2 pasang
D. 3 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 16 + Sapi 15 = 31 (❌ Gagal)
- Sapi 16 + Sapi 13 = 29 (❌ Gagal)
- Sapi 16 + Sapi 2 = 18 (❌ Gagal)
- Sapi 16 + Sapi 5 = 21 (❌ Gagal)
- Sapi 15 + Sapi 13 = 28 (❌ Gagal)
- Sapi 15 + Sapi 2 = 17 (❌ Gagal)
- Sapi 15 + Sapi 5 = 20 (❌ Gagal)
- Sapi 13 + Sapi 2 = 15 (❌ Gagal)
- Sapi 13 + Sapi 5 = 18 (❌ Gagal)
- Sapi 2 + Sapi 5 = 7 (❌ Gagal)

Total pasangan yang bernilai 36 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 218**
Sebuah robot bola diletakkan di lantai 90. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 18 detik
B. 17 detik
C. 15 detik
D. 16 detik
E. 14 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (15 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 90 (Garis Start)
- Detik 1: Genap, turun 13 -> 90 - 13 = 77
- Detik 2: Ganjil, naik 1 -> 77 + 1 = 78
- Detik 3: Genap, turun 13 -> 78 - 13 = 65
- Detik 4: Ganjil, naik 1 -> 65 + 1 = 66
- Detik 5: Genap, turun 13 -> 66 - 13 = 53
- Detik 6: Ganjil, naik 1 -> 53 + 1 = 54
- Detik 7: Genap, turun 13 -> 54 - 13 = 41
- Detik 8: Ganjil, naik 1 -> 41 + 1 = 42
- Detik 9: Genap, turun 13 -> 42 - 13 = 29
- Detik 10: Ganjil, naik 1 -> 29 + 1 = 30
- Detik 11: Genap, turun 13 -> 30 - 13 = 17
- Detik 12: Ganjil, naik 1 -> 17 + 1 = 18
- Detik 13: Genap, turun 13 -> 18 - 13 = 5
- Detik 14: Ganjil, naik 1 -> 5 + 1 = 6
- Detik 15: Genap, turun 13 -> 6 - 13 = -7
Simulasi berakhir pada detik ke-15. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 219**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 9, 17, 20, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 25."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 0 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 9 = 15 (❌ Gagal)
- Sapi 6 + Sapi 17 = 23 (❌ Gagal)
- Sapi 6 + Sapi 20 = 26 (❌ Gagal)
- Sapi 6 + Sapi 2 = 8 (❌ Gagal)
- Sapi 9 + Sapi 17 = 26 (❌ Gagal)
- Sapi 9 + Sapi 20 = 29 (❌ Gagal)
- Sapi 9 + Sapi 2 = 11 (❌ Gagal)
- Sapi 17 + Sapi 20 = 37 (❌ Gagal)
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)
- Sapi 20 + Sapi 2 = 22 (❌ Gagal)

Total pasangan yang bernilai 25 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 220**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 8, 24, 11, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 36."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 4 pasang
C. 0 pasang
D. 2 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 8 = 18 (❌ Gagal)
- Sapi 10 + Sapi 24 = 34 (❌ Gagal)
- Sapi 10 + Sapi 11 = 21 (❌ Gagal)
- Sapi 10 + Sapi 15 = 25 (❌ Gagal)
- Sapi 8 + Sapi 24 = 32 (❌ Gagal)
- Sapi 8 + Sapi 11 = 19 (❌ Gagal)
- Sapi 8 + Sapi 15 = 23 (❌ Gagal)
- Sapi 24 + Sapi 11 = 35 (❌ Gagal)
- Sapi 24 + Sapi 15 = 39 (❌ Gagal)
- Sapi 11 + Sapi 15 = 26 (❌ Gagal)

Total pasangan yang bernilai 36 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 221**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BBSUUTTBSSBSUSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 7 unit langkah
C. 4 unit langkah
D. 5 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 3 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`U`): Koordinat kini `(-2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`T`): Koordinat kini `(-1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(0, 1)`
- Instruksi 8 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 9 (`S`): Koordinat kini `(-1, 0)`
- Instruksi 10 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 11 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 12 (`S`): Koordinat kini `(-2, -2)`
- Instruksi 13 (`U`): Koordinat kini `(-2, -1)`
- Instruksi 14 (`S`): Koordinat kini `(-2, -2)`
- Instruksi 15 (`S`): Koordinat kini `(-2, -3)`

Posisi akhir robot adalah di titik `(-2, -3)`.
Jarak Manhattan = Murni $|-2| + |-3|$ = 2 + 3 = **5 unit**.
Opsi valid: **D**.</details>

---
**Soal 222**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `STSUBBSSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 3 unit langkah
C. 5 unit langkah
D. 4 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`T`): Koordinat kini `(1, -1)`
- Instruksi 3 (`S`): Koordinat kini `(1, -2)`
- Instruksi 4 (`U`): Koordinat kini `(1, -1)`
- Instruksi 5 (`B`): Koordinat kini `(0, -1)`
- Instruksi 6 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 8 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 9 (`S`): Koordinat kini `(-1, -4)`

Posisi akhir robot adalah di titik `(-1, -4)`.
Jarak Manhattan = Murni $|-1| + |-4|$ = 1 + 4 = **5 unit**.
Opsi valid: **C**.</details>

---
**Soal 223**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[18, 12, 6, 7, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

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
- Sapi 18 + Sapi 12 = 30 (❌ Gagal)
- Sapi 18 + Sapi 6 = 24 (❌ Gagal)
- Sapi 18 + Sapi 7 = 25 (❌ Gagal)
- Sapi 18 + Sapi 5 = 23 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 12 + Sapi 7 = 19 (❌ Gagal)
- Sapi 12 + Sapi 5 = 17 (❌ Gagal)
- Sapi 6 + Sapi 7 = 13 (❌ Gagal)
- Sapi 6 + Sapi 5 = 11 (❌ Gagal)
- Sapi 7 + Sapi 5 = 12 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 224**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[15, 11, 4, 21, 3]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 25."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 3 pasang
C. 4 pasang
D. 2 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 15 + Sapi 11 = 26 (❌ Gagal)
- Sapi 15 + Sapi 4 = 19 (❌ Gagal)
- Sapi 15 + Sapi 21 = 36 (❌ Gagal)
- Sapi 15 + Sapi 3 = 18 (❌ Gagal)
- Sapi 11 + Sapi 4 = 15 (❌ Gagal)
- Sapi 11 + Sapi 21 = 32 (❌ Gagal)
- Sapi 11 + Sapi 3 = 14 (❌ Gagal)
- Sapi 4 + Sapi 21 = 25 (✅ COCOK)
- Sapi 4 + Sapi 3 = 7 (❌ Gagal)
- Sapi 21 + Sapi 3 = 24 (❌ Gagal)

Total pasangan yang bernilai 25 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 225**
Sebuah robot bola diletakkan di lantai 107. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 27 detik
C. 31 detik
D. 30 detik
E. 29 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (28 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 107 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 107 + 5 = 112
- Detik 2: Genap, turun 13 -> 112 - 13 = 99
- Detik 3: Ganjil, naik 5 -> 99 + 5 = 104
- Detik 4: Genap, turun 13 -> 104 - 13 = 91
- Detik 5: Ganjil, naik 5 -> 91 + 5 = 96
- Detik 6: Genap, turun 13 -> 96 - 13 = 83
- Detik 7: Ganjil, naik 5 -> 83 + 5 = 88
- Detik 8: Genap, turun 13 -> 88 - 13 = 75
- Detik 9: Ganjil, naik 5 -> 75 + 5 = 80
- Detik 10: Genap, turun 13 -> 80 - 13 = 67
- Detik 11: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 12: Genap, turun 13 -> 72 - 13 = 59
- Detik 13: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 14: Genap, turun 13 -> 64 - 13 = 51
- Detik 15: Ganjil, naik 5 -> 51 + 5 = 56
- Detik 16: Genap, turun 13 -> 56 - 13 = 43
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 28: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 226**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 12, 11, 22, 2]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 43."*

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
- Sapi 3 + Sapi 12 = 15 (❌ Gagal)
- Sapi 3 + Sapi 11 = 14 (❌ Gagal)
- Sapi 3 + Sapi 22 = 25 (❌ Gagal)
- Sapi 3 + Sapi 2 = 5 (❌ Gagal)
- Sapi 12 + Sapi 11 = 23 (❌ Gagal)
- Sapi 12 + Sapi 22 = 34 (❌ Gagal)
- Sapi 12 + Sapi 2 = 14 (❌ Gagal)
- Sapi 11 + Sapi 22 = 33 (❌ Gagal)
- Sapi 11 + Sapi 2 = 13 (❌ Gagal)
- Sapi 22 + Sapi 2 = 24 (❌ Gagal)

Total pasangan yang bernilai 43 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 227**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SBUBUSTB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 1 unit langkah
C. 3 unit langkah
D. 0 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 8 (`B`): Koordinat kini `(-2, 0)`

Posisi akhir robot adalah di titik `(-2, 0)`.
Jarak Manhattan = Murni $|-2| + |0|$ = 2 + 0 = **2 unit**.
Opsi valid: **E**.</details>

---
**Soal 228**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[14, 20, 2, 16, 7]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 4 pasang
C. 0 pasang
D. 3 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 14 + Sapi 20 = 34 (❌ Gagal)
- Sapi 14 + Sapi 2 = 16 (❌ Gagal)
- Sapi 14 + Sapi 16 = 30 (✅ COCOK)
- Sapi 14 + Sapi 7 = 21 (❌ Gagal)
- Sapi 20 + Sapi 2 = 22 (❌ Gagal)
- Sapi 20 + Sapi 16 = 36 (❌ Gagal)
- Sapi 20 + Sapi 7 = 27 (❌ Gagal)
- Sapi 2 + Sapi 16 = 18 (❌ Gagal)
- Sapi 2 + Sapi 7 = 9 (❌ Gagal)
- Sapi 16 + Sapi 7 = 23 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 229**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 13, 6, 7, 16]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 0 pasang
D. 4 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 13 = 35 (❌ Gagal)
- Sapi 22 + Sapi 6 = 28 (❌ Gagal)
- Sapi 22 + Sapi 7 = 29 (❌ Gagal)
- Sapi 22 + Sapi 16 = 38 (❌ Gagal)
- Sapi 13 + Sapi 6 = 19 (❌ Gagal)
- Sapi 13 + Sapi 7 = 20 (❌ Gagal)
- Sapi 13 + Sapi 16 = 29 (❌ Gagal)
- Sapi 6 + Sapi 7 = 13 (❌ Gagal)
- Sapi 6 + Sapi 16 = 22 (❌ Gagal)
- Sapi 7 + Sapi 16 = 23 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 230**
Sebuah robot bola diletakkan di lantai 144. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 29 detik
B. 31 detik
C. 28 detik
D. 30 detik
E. 32 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (29 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 144 (Garis Start)
- Detik 1: Genap, turun 13 -> 144 - 13 = 131
- Detik 2: Ganjil, naik 3 -> 131 + 3 = 134
- Detik 3: Genap, turun 13 -> 134 - 13 = 121
- Detik 4: Ganjil, naik 3 -> 121 + 3 = 124
- Detik 5: Genap, turun 13 -> 124 - 13 = 111
- Detik 6: Ganjil, naik 3 -> 111 + 3 = 114
- Detik 7: Genap, turun 13 -> 114 - 13 = 101
- Detik 8: Ganjil, naik 3 -> 101 + 3 = 104
- Detik 9: Genap, turun 13 -> 104 - 13 = 91
- Detik 10: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 11: Genap, turun 13 -> 94 - 13 = 81
- Detik 12: Ganjil, naik 3 -> 81 + 3 = 84
- Detik 13: Genap, turun 13 -> 84 - 13 = 71
- Detik 14: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 15: Genap, turun 13 -> 74 - 13 = 61
- Detik 16: Ganjil, naik 3 -> 61 + 3 = 64
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 29: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 231**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 16, 19, 10, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 3 pasang
C. 1 pasang
D. 2 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 16 = 40 (❌ Gagal)
- Sapi 24 + Sapi 19 = 43 (❌ Gagal)
- Sapi 24 + Sapi 10 = 34 (❌ Gagal)
- Sapi 24 + Sapi 15 = 39 (❌ Gagal)
- Sapi 16 + Sapi 19 = 35 (✅ COCOK)
- Sapi 16 + Sapi 10 = 26 (❌ Gagal)
- Sapi 16 + Sapi 15 = 31 (❌ Gagal)
- Sapi 19 + Sapi 10 = 29 (❌ Gagal)
- Sapi 19 + Sapi 15 = 34 (❌ Gagal)
- Sapi 10 + Sapi 15 = 25 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 232**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[24, 16, 19, 3, 18]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 50."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 2 pasang
C. 4 pasang
D. 0 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 24 + Sapi 16 = 40 (❌ Gagal)
- Sapi 24 + Sapi 19 = 43 (❌ Gagal)
- Sapi 24 + Sapi 3 = 27 (❌ Gagal)
- Sapi 24 + Sapi 18 = 42 (❌ Gagal)
- Sapi 16 + Sapi 19 = 35 (❌ Gagal)
- Sapi 16 + Sapi 3 = 19 (❌ Gagal)
- Sapi 16 + Sapi 18 = 34 (❌ Gagal)
- Sapi 19 + Sapi 3 = 22 (❌ Gagal)
- Sapi 19 + Sapi 18 = 37 (❌ Gagal)
- Sapi 3 + Sapi 18 = 21 (❌ Gagal)

Total pasangan yang bernilai 50 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 233**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 18, 21, 5, 22]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 48."*

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
- Sapi 19 + Sapi 18 = 37 (❌ Gagal)
- Sapi 19 + Sapi 21 = 40 (❌ Gagal)
- Sapi 19 + Sapi 5 = 24 (❌ Gagal)
- Sapi 19 + Sapi 22 = 41 (❌ Gagal)
- Sapi 18 + Sapi 21 = 39 (❌ Gagal)
- Sapi 18 + Sapi 5 = 23 (❌ Gagal)
- Sapi 18 + Sapi 22 = 40 (❌ Gagal)
- Sapi 21 + Sapi 5 = 26 (❌ Gagal)
- Sapi 21 + Sapi 22 = 43 (❌ Gagal)
- Sapi 5 + Sapi 22 = 27 (❌ Gagal)

Total pasangan yang bernilai 48 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 234**
Sebuah robot bola diletakkan di lantai 122. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 61 detik
B. 60 detik
C. 58 detik
D. 59 detik
E. 62 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (59 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 122 (Garis Start)
- Detik 1: Genap, turun 7 -> 122 - 7 = 115
- Detik 2: Ganjil, naik 3 -> 115 + 3 = 118
- Detik 3: Genap, turun 7 -> 118 - 7 = 111
- Detik 4: Ganjil, naik 3 -> 111 + 3 = 114
- Detik 5: Genap, turun 7 -> 114 - 7 = 107
- Detik 6: Ganjil, naik 3 -> 107 + 3 = 110
- Detik 7: Genap, turun 7 -> 110 - 7 = 103
- Detik 8: Ganjil, naik 3 -> 103 + 3 = 106
- Detik 9: Genap, turun 7 -> 106 - 7 = 99
- Detik 10: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 11: Genap, turun 7 -> 102 - 7 = 95
- Detik 12: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 13: Genap, turun 7 -> 98 - 7 = 91
- Detik 14: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 15: Genap, turun 7 -> 94 - 7 = 87
- Detik 16: Ganjil, naik 3 -> 87 + 3 = 90
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 59: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 235**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[20, 5, 11, 8, 12]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 3 pasang
C. 2 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 20 + Sapi 5 = 25 (❌ Gagal)
- Sapi 20 + Sapi 11 = 31 (❌ Gagal)
- Sapi 20 + Sapi 8 = 28 (❌ Gagal)
- Sapi 20 + Sapi 12 = 32 (❌ Gagal)
- Sapi 5 + Sapi 11 = 16 (❌ Gagal)
- Sapi 5 + Sapi 8 = 13 (❌ Gagal)
- Sapi 5 + Sapi 12 = 17 (❌ Gagal)
- Sapi 11 + Sapi 8 = 19 (❌ Gagal)
- Sapi 11 + Sapi 12 = 23 (❌ Gagal)
- Sapi 8 + Sapi 12 = 20 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 236**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBUTSTSUTU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 2 unit langkah
C. 6 unit langkah
D. 4 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 4 (`T`): Koordinat kini `(0, 2)`
- Instruksi 5 (`S`): Koordinat kini `(0, 1)`
- Instruksi 6 (`T`): Koordinat kini `(1, 1)`
- Instruksi 7 (`S`): Koordinat kini `(1, 0)`
- Instruksi 8 (`U`): Koordinat kini `(1, 1)`
- Instruksi 9 (`T`): Koordinat kini `(2, 1)`
- Instruksi 10 (`U`): Koordinat kini `(2, 2)`

Posisi akhir robot adalah di titik `(2, 2)`.
Jarak Manhattan = Murni $|2| + |2|$ = 2 + 2 = **4 unit**.
Opsi valid: **D**.</details>

---
**Soal 237**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBBSTSSSST`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 6 unit langkah
C. 5 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 4 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 5 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 8 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 9 (`S`): Koordinat kini `(-1, -4)`
- Instruksi 10 (`T`): Koordinat kini `(0, -4)`

Posisi akhir robot adalah di titik `(0, -4)`.
Jarak Manhattan = Murni $|0| + |-4|$ = 0 + 4 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 238**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[16, 14, 2, 23, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 43."*

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
- Sapi 16 + Sapi 14 = 30 (❌ Gagal)
- Sapi 16 + Sapi 2 = 18 (❌ Gagal)
- Sapi 16 + Sapi 23 = 39 (❌ Gagal)
- Sapi 16 + Sapi 5 = 21 (❌ Gagal)
- Sapi 14 + Sapi 2 = 16 (❌ Gagal)
- Sapi 14 + Sapi 23 = 37 (❌ Gagal)
- Sapi 14 + Sapi 5 = 19 (❌ Gagal)
- Sapi 2 + Sapi 23 = 25 (❌ Gagal)
- Sapi 2 + Sapi 5 = 7 (❌ Gagal)
- Sapi 23 + Sapi 5 = 28 (❌ Gagal)

Total pasangan yang bernilai 43 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 239**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[21, 4, 19, 7, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 35."*

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
- Sapi 21 + Sapi 4 = 25 (❌ Gagal)
- Sapi 21 + Sapi 19 = 40 (❌ Gagal)
- Sapi 21 + Sapi 7 = 28 (❌ Gagal)
- Sapi 21 + Sapi 5 = 26 (❌ Gagal)
- Sapi 4 + Sapi 19 = 23 (❌ Gagal)
- Sapi 4 + Sapi 7 = 11 (❌ Gagal)
- Sapi 4 + Sapi 5 = 9 (❌ Gagal)
- Sapi 19 + Sapi 7 = 26 (❌ Gagal)
- Sapi 19 + Sapi 5 = 24 (❌ Gagal)
- Sapi 7 + Sapi 5 = 12 (❌ Gagal)

Total pasangan yang bernilai 35 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 240**
Sebuah robot bola diletakkan di lantai 61. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 19 detik
B. 15 detik
C. 18 detik
D. 16 detik
E. 17 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (16 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 61 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 61 + 3 = 64
- Detik 2: Genap, turun 11 -> 64 - 11 = 53
- Detik 3: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 4: Genap, turun 11 -> 56 - 11 = 45
- Detik 5: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 6: Genap, turun 11 -> 48 - 11 = 37
- Detik 7: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 8: Genap, turun 11 -> 40 - 11 = 29
- Detik 9: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 10: Genap, turun 11 -> 32 - 11 = 21
- Detik 11: Ganjil, naik 3 -> 21 + 3 = 24
- Detik 12: Genap, turun 11 -> 24 - 11 = 13
- Detik 13: Ganjil, naik 3 -> 13 + 3 = 16
- Detik 14: Genap, turun 11 -> 16 - 11 = 5
- Detik 15: Ganjil, naik 3 -> 5 + 3 = 8
- Detik 16: Genap, turun 11 -> 8 - 11 = -3
</details>

---
**Soal 241**
Sebuah robot bola diletakkan di lantai 93. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 51 detik
B. 48 detik
C. 47 detik
D. 49 detik
E. 50 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (48 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 93 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 93 + 5 = 98
- Detik 2: Genap, turun 9 -> 98 - 9 = 89
- Detik 3: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 4: Genap, turun 9 -> 94 - 9 = 85
- Detik 5: Ganjil, naik 5 -> 85 + 5 = 90
- Detik 6: Genap, turun 9 -> 90 - 9 = 81
- Detik 7: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 8: Genap, turun 9 -> 86 - 9 = 77
- Detik 9: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 10: Genap, turun 9 -> 82 - 9 = 73
- Detik 11: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 12: Genap, turun 9 -> 78 - 9 = 69
- Detik 13: Ganjil, naik 5 -> 69 + 5 = 74
- Detik 14: Genap, turun 9 -> 74 - 9 = 65
- Detik 15: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 16: Genap, turun 9 -> 70 - 9 = 61
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 48: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 242**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUUTTTTT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 10 unit langkah
B. 9 unit langkah
C. 6 unit langkah
D. 7 unit langkah
E. 8 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (8 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`U`): Koordinat kini `(0, 3)`
- Instruksi 4 (`T`): Koordinat kini `(1, 3)`
- Instruksi 5 (`T`): Koordinat kini `(2, 3)`
- Instruksi 6 (`T`): Koordinat kini `(3, 3)`
- Instruksi 7 (`T`): Koordinat kini `(4, 3)`
- Instruksi 8 (`T`): Koordinat kini `(5, 3)`

Posisi akhir robot adalah di titik `(5, 3)`.
Jarak Manhattan = Murni $|5| + |3|$ = 5 + 3 = **8 unit**.
Opsi valid: **E**.</details>

---
**Soal 243**
Sebuah robot bola diletakkan di lantai 137. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 150 detik
B. 149 detik
C. 148 detik
D. 147 detik
E. 151 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (148 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 137 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 137 + 5 = 142
- Detik 2: Genap, turun 7 -> 142 - 7 = 135
- Detik 3: Ganjil, naik 5 -> 135 + 5 = 140
- Detik 4: Genap, turun 7 -> 140 - 7 = 133
- Detik 5: Ganjil, naik 5 -> 133 + 5 = 138
- Detik 6: Genap, turun 7 -> 138 - 7 = 131
- Detik 7: Ganjil, naik 5 -> 131 + 5 = 136
- Detik 8: Genap, turun 7 -> 136 - 7 = 129
- Detik 9: Ganjil, naik 5 -> 129 + 5 = 134
- Detik 10: Genap, turun 7 -> 134 - 7 = 127
- Detik 11: Ganjil, naik 5 -> 127 + 5 = 132
- Detik 12: Genap, turun 7 -> 132 - 7 = 125
- Detik 13: Ganjil, naik 5 -> 125 + 5 = 130
- Detik 14: Genap, turun 7 -> 130 - 7 = 123
- Detik 15: Ganjil, naik 5 -> 123 + 5 = 128
- Detik 16: Genap, turun 7 -> 128 - 7 = 121
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 148: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 244**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUSSTUTBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 2 unit langkah
C. 4 unit langkah
D. 1 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`S`): Koordinat kini `(1, 0)`
- Instruksi 4 (`S`): Koordinat kini `(1, -1)`
- Instruksi 5 (`T`): Koordinat kini `(2, -1)`
- Instruksi 6 (`U`): Koordinat kini `(2, 0)`
- Instruksi 7 (`T`): Koordinat kini `(3, 0)`
- Instruksi 8 (`B`): Koordinat kini `(2, 0)`
- Instruksi 9 (`S`): Koordinat kini `(2, -1)`

Posisi akhir robot adalah di titik `(2, -1)`.
Jarak Manhattan = Murni $|2| + |-1|$ = 2 + 1 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 245**
Sebuah robot bola diletakkan di lantai 86. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 44 detik
B. 48 detik
C. 46 detik
D. 45 detik
E. 47 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (45 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 86 (Garis Start)
- Detik 1: Genap, turun 9 -> 86 - 9 = 77
- Detik 2: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 3: Genap, turun 9 -> 82 - 9 = 73
- Detik 4: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 5: Genap, turun 9 -> 78 - 9 = 69
- Detik 6: Ganjil, naik 5 -> 69 + 5 = 74
- Detik 7: Genap, turun 9 -> 74 - 9 = 65
- Detik 8: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 9: Genap, turun 9 -> 70 - 9 = 61
- Detik 10: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 11: Genap, turun 9 -> 66 - 9 = 57
- Detik 12: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 13: Genap, turun 9 -> 62 - 9 = 53
- Detik 14: Ganjil, naik 5 -> 53 + 5 = 58
- Detik 15: Genap, turun 9 -> 58 - 9 = 49
- Detik 16: Ganjil, naik 5 -> 49 + 5 = 54
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 45: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 246**
Sebuah robot bola diletakkan di lantai 73. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 23 detik
B. 25 detik
C. 22 detik
D. 21 detik
E. 24 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (22 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 73 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 2: Genap, turun 13 -> 78 - 13 = 65
- Detik 3: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 4: Genap, turun 13 -> 70 - 13 = 57
- Detik 5: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 6: Genap, turun 13 -> 62 - 13 = 49
- Detik 7: Ganjil, naik 5 -> 49 + 5 = 54
- Detik 8: Genap, turun 13 -> 54 - 13 = 41
- Detik 9: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 10: Genap, turun 13 -> 46 - 13 = 33
- Detik 11: Ganjil, naik 5 -> 33 + 5 = 38
- Detik 12: Genap, turun 13 -> 38 - 13 = 25
- Detik 13: Ganjil, naik 5 -> 25 + 5 = 30
- Detik 14: Genap, turun 13 -> 30 - 13 = 17
- Detik 15: Ganjil, naik 5 -> 17 + 5 = 22
- Detik 16: Genap, turun 13 -> 22 - 13 = 9
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 22: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 247**
Sebuah robot bola diletakkan di lantai 121. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 25 detik
B. 26 detik
C. 29 detik
D. 28 detik
E. 27 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (26 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 121 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 121 + 1 = 122
- Detik 2: Genap, turun 11 -> 122 - 11 = 111
- Detik 3: Ganjil, naik 1 -> 111 + 1 = 112
- Detik 4: Genap, turun 11 -> 112 - 11 = 101
- Detik 5: Ganjil, naik 1 -> 101 + 1 = 102
- Detik 6: Genap, turun 11 -> 102 - 11 = 91
- Detik 7: Ganjil, naik 1 -> 91 + 1 = 92
- Detik 8: Genap, turun 11 -> 92 - 11 = 81
- Detik 9: Ganjil, naik 1 -> 81 + 1 = 82
- Detik 10: Genap, turun 11 -> 82 - 11 = 71
- Detik 11: Ganjil, naik 1 -> 71 + 1 = 72
- Detik 12: Genap, turun 11 -> 72 - 11 = 61
- Detik 13: Ganjil, naik 1 -> 61 + 1 = 62
- Detik 14: Genap, turun 11 -> 62 - 11 = 51
- Detik 15: Ganjil, naik 1 -> 51 + 1 = 52
- Detik 16: Genap, turun 11 -> 52 - 11 = 41
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 26: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 248**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[14, 19, 6, 16, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 43."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 3 pasang
C. 1 pasang
D. 0 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 14 + Sapi 19 = 33 (❌ Gagal)
- Sapi 14 + Sapi 6 = 20 (❌ Gagal)
- Sapi 14 + Sapi 16 = 30 (❌ Gagal)
- Sapi 14 + Sapi 5 = 19 (❌ Gagal)
- Sapi 19 + Sapi 6 = 25 (❌ Gagal)
- Sapi 19 + Sapi 16 = 35 (❌ Gagal)
- Sapi 19 + Sapi 5 = 24 (❌ Gagal)
- Sapi 6 + Sapi 16 = 22 (❌ Gagal)
- Sapi 6 + Sapi 5 = 11 (❌ Gagal)
- Sapi 16 + Sapi 5 = 21 (❌ Gagal)

Total pasangan yang bernilai 43 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 249**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 21, 3, 8, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

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
- Sapi 23 + Sapi 21 = 44 (❌ Gagal)
- Sapi 23 + Sapi 3 = 26 (❌ Gagal)
- Sapi 23 + Sapi 8 = 31 (❌ Gagal)
- Sapi 23 + Sapi 19 = 42 (❌ Gagal)
- Sapi 21 + Sapi 3 = 24 (❌ Gagal)
- Sapi 21 + Sapi 8 = 29 (❌ Gagal)
- Sapi 21 + Sapi 19 = 40 (❌ Gagal)
- Sapi 3 + Sapi 8 = 11 (❌ Gagal)
- Sapi 3 + Sapi 19 = 22 (❌ Gagal)
- Sapi 8 + Sapi 19 = 27 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 250**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTSUSTBSUU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. 2 unit langkah
C. 4 unit langkah
D. 3 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`S`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(1, 0)`
- Instruksi 6 (`T`): Koordinat kini `(2, 0)`
- Instruksi 7 (`B`): Koordinat kini `(1, 0)`
- Instruksi 8 (`S`): Koordinat kini `(1, -1)`
- Instruksi 9 (`U`): Koordinat kini `(1, 0)`
- Instruksi 10 (`U`): Koordinat kini `(1, 1)`

Posisi akhir robot adalah di titik `(1, 1)`.
Jarak Manhattan = Murni $|1| + |1|$ = 1 + 1 = **2 unit**.
Opsi valid: **B**.</details>

---
