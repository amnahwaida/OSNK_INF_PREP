# Latian Soal: Simulasi & Brute Force (Part 3 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 101**
Sebuah robot bola diletakkan di lantai 68. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 15 detik
B. 14 detik
C. 13 detik
D. 12 detik
E. 16 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (13 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 68 (Garis Start)
- Detik 1: Genap, turun 13 -> 68 - 13 = 55
- Detik 2: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 3: Genap, turun 13 -> 58 - 13 = 45
- Detik 4: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 5: Genap, turun 13 -> 48 - 13 = 35
- Detik 6: Ganjil, naik 3 -> 35 + 3 = 38
- Detik 7: Genap, turun 13 -> 38 - 13 = 25
- Detik 8: Ganjil, naik 3 -> 25 + 3 = 28
- Detik 9: Genap, turun 13 -> 28 - 13 = 15
- Detik 10: Ganjil, naik 3 -> 15 + 3 = 18
- Detik 11: Genap, turun 13 -> 18 - 13 = 5
- Detik 12: Ganjil, naik 3 -> 5 + 3 = 8
- Detik 13: Genap, turun 13 -> 8 - 13 = -5
Simulasi berakhir pada detik ke-13. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 102**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSBBUTSSSUTUUTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 3 unit langkah
C. 4 unit langkah
D. 5 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`B`): Koordinat kini `(-1, -2)`
- Instruksi 4 (`B`): Koordinat kini `(-2, -2)`
- Instruksi 5 (`U`): Koordinat kini `(-2, -1)`
- Instruksi 6 (`T`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 8 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 9 (`S`): Koordinat kini `(-1, -4)`
- Instruksi 10 (`U`): Koordinat kini `(-1, -3)`
- Instruksi 11 (`T`): Koordinat kini `(0, -3)`
- Instruksi 12 (`U`): Koordinat kini `(0, -2)`
- Instruksi 13 (`U`): Koordinat kini `(0, -1)`
- Instruksi 14 (`T`): Koordinat kini `(1, -1)`
- Instruksi 15 (`S`): Koordinat kini `(1, -2)`

Posisi akhir robot adalah di titik `(1, -2)`.
Jarak Manhattan = Murni $|1| + |-2|$ = 1 + 2 = **3 unit**.
Opsi valid: **B**.</details>

---
**Soal 103**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 16, 20, 9, 23]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 0 pasang
C. 1 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 10 + Sapi 16 = 26 (❌ Gagal)
- Sapi 10 + Sapi 20 = 30 (✅ COCOK)
- Sapi 10 + Sapi 9 = 19 (❌ Gagal)
- Sapi 10 + Sapi 23 = 33 (❌ Gagal)
- Sapi 16 + Sapi 20 = 36 (❌ Gagal)
- Sapi 16 + Sapi 9 = 25 (❌ Gagal)
- Sapi 16 + Sapi 23 = 39 (❌ Gagal)
- Sapi 20 + Sapi 9 = 29 (❌ Gagal)
- Sapi 20 + Sapi 23 = 43 (❌ Gagal)
- Sapi 9 + Sapi 23 = 32 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 104**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUBTBBUSUT`.
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
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 4 (`T`): Koordinat kini `(0, 2)`
- Instruksi 5 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`B`): Koordinat kini `(-2, 2)`
- Instruksi 7 (`U`): Koordinat kini `(-2, 3)`
- Instruksi 8 (`S`): Koordinat kini `(-2, 2)`
- Instruksi 9 (`U`): Koordinat kini `(-2, 3)`
- Instruksi 10 (`T`): Koordinat kini `(-1, 3)`

Posisi akhir robot adalah di titik `(-1, 3)`.
Jarak Manhattan = Murni $|-1| + |3|$ = 1 + 3 = **4 unit**.
Opsi valid: **D**.</details>

---
**Soal 105**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BTSSBBTUSTBSU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 5 unit langkah
C. 3 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(0, 0)`
- Instruksi 3 (`S`): Koordinat kini `(0, -1)`
- Instruksi 4 (`S`): Koordinat kini `(0, -2)`
- Instruksi 5 (`B`): Koordinat kini `(-1, -2)`
- Instruksi 6 (`B`): Koordinat kini `(-2, -2)`
- Instruksi 7 (`T`): Koordinat kini `(-1, -2)`
- Instruksi 8 (`U`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 10 (`T`): Koordinat kini `(0, -2)`
- Instruksi 11 (`B`): Koordinat kini `(-1, -2)`
- Instruksi 12 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 13 (`U`): Koordinat kini `(-1, -2)`

Posisi akhir robot adalah di titik `(-1, -2)`.
Jarak Manhattan = Murni $|-1| + |-2|$ = 1 + 2 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 106**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBTUTUTUB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 3 unit langkah
C. 7 unit langkah
D. 4 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(2, 1)`
- Instruksi 6 (`U`): Koordinat kini `(2, 2)`
- Instruksi 7 (`T`): Koordinat kini `(3, 2)`
- Instruksi 8 (`U`): Koordinat kini `(3, 3)`
- Instruksi 9 (`B`): Koordinat kini `(2, 3)`

Posisi akhir robot adalah di titik `(2, 3)`.
Jarak Manhattan = Murni $|2| + |3|$ = 2 + 3 = **5 unit**.
Opsi valid: **E**.</details>

---
**Soal 107**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[8, 14, 20, 19, 3]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 34."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 0 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 8 + Sapi 14 = 22 (❌ Gagal)
- Sapi 8 + Sapi 20 = 28 (❌ Gagal)
- Sapi 8 + Sapi 19 = 27 (❌ Gagal)
- Sapi 8 + Sapi 3 = 11 (❌ Gagal)
- Sapi 14 + Sapi 20 = 34 (✅ COCOK)
- Sapi 14 + Sapi 19 = 33 (❌ Gagal)
- Sapi 14 + Sapi 3 = 17 (❌ Gagal)
- Sapi 20 + Sapi 19 = 39 (❌ Gagal)
- Sapi 20 + Sapi 3 = 23 (❌ Gagal)
- Sapi 19 + Sapi 3 = 22 (❌ Gagal)

Total pasangan yang bernilai 34 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 108**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 13, 23, 11, 24]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 28."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 3 pasang
D. 2 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 13 = 35 (❌ Gagal)
- Sapi 22 + Sapi 23 = 45 (❌ Gagal)
- Sapi 22 + Sapi 11 = 33 (❌ Gagal)
- Sapi 22 + Sapi 24 = 46 (❌ Gagal)
- Sapi 13 + Sapi 23 = 36 (❌ Gagal)
- Sapi 13 + Sapi 11 = 24 (❌ Gagal)
- Sapi 13 + Sapi 24 = 37 (❌ Gagal)
- Sapi 23 + Sapi 11 = 34 (❌ Gagal)
- Sapi 23 + Sapi 24 = 47 (❌ Gagal)
- Sapi 11 + Sapi 24 = 35 (❌ Gagal)

Total pasangan yang bernilai 28 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 109**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TTSUUBTBBUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 5 unit langkah
C. 2 unit langkah
D. 1 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(2, 0)`
- Instruksi 3 (`S`): Koordinat kini `(2, -1)`
- Instruksi 4 (`U`): Koordinat kini `(2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(2, 1)`
- Instruksi 6 (`B`): Koordinat kini `(1, 1)`
- Instruksi 7 (`T`): Koordinat kini `(2, 1)`
- Instruksi 8 (`B`): Koordinat kini `(1, 1)`
- Instruksi 9 (`B`): Koordinat kini `(0, 1)`
- Instruksi 10 (`U`): Koordinat kini `(0, 2)`
- Instruksi 11 (`T`): Koordinat kini `(1, 2)`

Posisi akhir robot adalah di titik `(1, 2)`.
Jarak Manhattan = Murni $|1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 110**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[5, 20, 22, 17, 8]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 4 pasang
C. 0 pasang
D. 2 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 5 + Sapi 20 = 25 (❌ Gagal)
- Sapi 5 + Sapi 22 = 27 (❌ Gagal)
- Sapi 5 + Sapi 17 = 22 (❌ Gagal)
- Sapi 5 + Sapi 8 = 13 (❌ Gagal)
- Sapi 20 + Sapi 22 = 42 (❌ Gagal)
- Sapi 20 + Sapi 17 = 37 (❌ Gagal)
- Sapi 20 + Sapi 8 = 28 (❌ Gagal)
- Sapi 22 + Sapi 17 = 39 (❌ Gagal)
- Sapi 22 + Sapi 8 = 30 (❌ Gagal)
- Sapi 17 + Sapi 8 = 25 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 111**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[4, 3, 8, 9, 23]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 38."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 3 pasang
C. 2 pasang
D. 0 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 4 + Sapi 3 = 7 (❌ Gagal)
- Sapi 4 + Sapi 8 = 12 (❌ Gagal)
- Sapi 4 + Sapi 9 = 13 (❌ Gagal)
- Sapi 4 + Sapi 23 = 27 (❌ Gagal)
- Sapi 3 + Sapi 8 = 11 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 23 = 26 (❌ Gagal)
- Sapi 8 + Sapi 9 = 17 (❌ Gagal)
- Sapi 8 + Sapi 23 = 31 (❌ Gagal)
- Sapi 9 + Sapi 23 = 32 (❌ Gagal)

Total pasangan yang bernilai 38 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 112**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SBBBTUST`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. 3 unit langkah
C. 1 unit langkah
D. 2 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`B`): Koordinat kini `(-3, -1)`
- Instruksi 5 (`T`): Koordinat kini `(-2, -1)`
- Instruksi 6 (`U`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`S`): Koordinat kini `(-2, -1)`
- Instruksi 8 (`T`): Koordinat kini `(-1, -1)`

Posisi akhir robot adalah di titik `(-1, -1)`.
Jarak Manhattan = Murni $|-1| + |-1|$ = 1 + 1 = **2 unit**.
Opsi valid: **D**.</details>

---
**Soal 113**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[18, 12, 15, 7, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 48."*

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
- Sapi 18 + Sapi 12 = 30 (❌ Gagal)
- Sapi 18 + Sapi 15 = 33 (❌ Gagal)
- Sapi 18 + Sapi 7 = 25 (❌ Gagal)
- Sapi 18 + Sapi 6 = 24 (❌ Gagal)
- Sapi 12 + Sapi 15 = 27 (❌ Gagal)
- Sapi 12 + Sapi 7 = 19 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 15 + Sapi 7 = 22 (❌ Gagal)
- Sapi 15 + Sapi 6 = 21 (❌ Gagal)
- Sapi 7 + Sapi 6 = 13 (❌ Gagal)

Total pasangan yang bernilai 48 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 114**
Sebuah robot bola diletakkan di lantai 77. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 20 detik
B. 17 detik
C. 18 detik
D. 19 detik
E. 21 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (18 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 77 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 77 + 3 = 80
- Detik 2: Genap, turun 13 -> 80 - 13 = 67
- Detik 3: Ganjil, naik 3 -> 67 + 3 = 70
- Detik 4: Genap, turun 13 -> 70 - 13 = 57
- Detik 5: Ganjil, naik 3 -> 57 + 3 = 60
- Detik 6: Genap, turun 13 -> 60 - 13 = 47
- Detik 7: Ganjil, naik 3 -> 47 + 3 = 50
- Detik 8: Genap, turun 13 -> 50 - 13 = 37
- Detik 9: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 10: Genap, turun 13 -> 40 - 13 = 27
- Detik 11: Ganjil, naik 3 -> 27 + 3 = 30
- Detik 12: Genap, turun 13 -> 30 - 13 = 17
- Detik 13: Ganjil, naik 3 -> 17 + 3 = 20
- Detik 14: Genap, turun 13 -> 20 - 13 = 7
- Detik 15: Ganjil, naik 3 -> 7 + 3 = 10
- Detik 16: Genap, turun 13 -> 10 - 13 = -3
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 18: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 115**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBTUSBTU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 4 unit langkah
C. 0 unit langkah
D. 3 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(1, 0)`
- Instruksi 6 (`B`): Koordinat kini `(0, 0)`
- Instruksi 7 (`T`): Koordinat kini `(1, 0)`
- Instruksi 8 (`U`): Koordinat kini `(1, 1)`

Posisi akhir robot adalah di titik `(1, 1)`.
Jarak Manhattan = Murni $|1| + |1|$ = 1 + 1 = **2 unit**.
Opsi valid: **A**.</details>

---
**Soal 116**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UBSUBUSBTSTUUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 3 unit langkah
C. 0 unit langkah
D. 4 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`S`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`U`): Koordinat kini `(-2, 2)`
- Instruksi 7 (`S`): Koordinat kini `(-2, 1)`
- Instruksi 8 (`B`): Koordinat kini `(-3, 1)`
- Instruksi 9 (`T`): Koordinat kini `(-2, 1)`
- Instruksi 10 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 11 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 12 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 13 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 14 (`S`): Koordinat kini `(-1, 1)`

Posisi akhir robot adalah di titik `(-1, 1)`.
Jarak Manhattan = Murni $|-1| + |1|$ = 1 + 1 = **2 unit**.
Opsi valid: **E**.</details>

---
**Soal 117**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `USUUUTTS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 6 unit langkah
C. 3 unit langkah
D. 5 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`S`): Koordinat kini `(0, 0)`
- Instruksi 3 (`U`): Koordinat kini `(0, 1)`
- Instruksi 4 (`U`): Koordinat kini `(0, 2)`
- Instruksi 5 (`U`): Koordinat kini `(0, 3)`
- Instruksi 6 (`T`): Koordinat kini `(1, 3)`
- Instruksi 7 (`T`): Koordinat kini `(2, 3)`
- Instruksi 8 (`S`): Koordinat kini `(2, 2)`

Posisi akhir robot adalah di titik `(2, 2)`.
Jarak Manhattan = Murni $|2| + |2|$ = 2 + 2 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 118**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BBTBTSBTTUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. -1 unit langkah
C. 1 unit langkah
D. 2 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 3 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 5 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 8 (`T`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`T`): Koordinat kini `(0, -1)`
- Instruksi 10 (`U`): Koordinat kini `(0, 0)`
- Instruksi 11 (`S`): Koordinat kini `(0, -1)`

Posisi akhir robot adalah di titik `(0, -1)`.
Jarak Manhattan = Murni $|0| + |-1|$ = 0 + 1 = **1 unit**.
Opsi valid: **C**.</details>

---
**Soal 119**
Sebuah robot bola diletakkan di lantai 121. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 67 detik
B. 65 detik
C. 64 detik
D. 66 detik
E. 63 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (64 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 121 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 121 + 5 = 126
- Detik 2: Genap, turun 9 -> 126 - 9 = 117
- Detik 3: Ganjil, naik 5 -> 117 + 5 = 122
- Detik 4: Genap, turun 9 -> 122 - 9 = 113
- Detik 5: Ganjil, naik 5 -> 113 + 5 = 118
- Detik 6: Genap, turun 9 -> 118 - 9 = 109
- Detik 7: Ganjil, naik 5 -> 109 + 5 = 114
- Detik 8: Genap, turun 9 -> 114 - 9 = 105
- Detik 9: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 10: Genap, turun 9 -> 110 - 9 = 101
- Detik 11: Ganjil, naik 5 -> 101 + 5 = 106
- Detik 12: Genap, turun 9 -> 106 - 9 = 97
- Detik 13: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 14: Genap, turun 9 -> 102 - 9 = 93
- Detik 15: Ganjil, naik 5 -> 93 + 5 = 98
- Detik 16: Genap, turun 9 -> 98 - 9 = 89
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 64: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 120**
Sebuah robot bola diletakkan di lantai 137. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 38 detik
B. 39 detik
C. 37 detik
D. 35 detik
E. 36 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (36 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 137 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 137 + 5 = 142
- Detik 2: Genap, turun 13 -> 142 - 13 = 129
- Detik 3: Ganjil, naik 5 -> 129 + 5 = 134
- Detik 4: Genap, turun 13 -> 134 - 13 = 121
- Detik 5: Ganjil, naik 5 -> 121 + 5 = 126
- Detik 6: Genap, turun 13 -> 126 - 13 = 113
- Detik 7: Ganjil, naik 5 -> 113 + 5 = 118
- Detik 8: Genap, turun 13 -> 118 - 13 = 105
- Detik 9: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 10: Genap, turun 13 -> 110 - 13 = 97
- Detik 11: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 12: Genap, turun 13 -> 102 - 13 = 89
- Detik 13: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 14: Genap, turun 13 -> 94 - 13 = 81
- Detik 15: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 16: Genap, turun 13 -> 86 - 13 = 73
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 36: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 121**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BUTTSBSBB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 3 unit langkah
C. 1 unit langkah
D. 2 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(0, 1)`
- Instruksi 4 (`T`): Koordinat kini `(1, 1)`
- Instruksi 5 (`S`): Koordinat kini `(1, 0)`
- Instruksi 6 (`B`): Koordinat kini `(0, 0)`
- Instruksi 7 (`S`): Koordinat kini `(0, -1)`
- Instruksi 8 (`B`): Koordinat kini `(-1, -1)`
- Instruksi 9 (`B`): Koordinat kini `(-2, -1)`

Posisi akhir robot adalah di titik `(-2, -1)`.
Jarak Manhattan = Murni $|-2| + |-1|$ = 2 + 1 = **3 unit**.
Opsi valid: **B**.</details>

---
**Soal 122**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[12, 8, 15, 13, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 27."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 0 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 12 + Sapi 8 = 20 (❌ Gagal)
- Sapi 12 + Sapi 15 = 27 (✅ COCOK)
- Sapi 12 + Sapi 13 = 25 (❌ Gagal)
- Sapi 12 + Sapi 10 = 22 (❌ Gagal)
- Sapi 8 + Sapi 15 = 23 (❌ Gagal)
- Sapi 8 + Sapi 13 = 21 (❌ Gagal)
- Sapi 8 + Sapi 10 = 18 (❌ Gagal)
- Sapi 15 + Sapi 13 = 28 (❌ Gagal)
- Sapi 15 + Sapi 10 = 25 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)

Total pasangan yang bernilai 27 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 123**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[21, 16, 12, 11, 18]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 40."*

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
- Sapi 21 + Sapi 16 = 37 (❌ Gagal)
- Sapi 21 + Sapi 12 = 33 (❌ Gagal)
- Sapi 21 + Sapi 11 = 32 (❌ Gagal)
- Sapi 21 + Sapi 18 = 39 (❌ Gagal)
- Sapi 16 + Sapi 12 = 28 (❌ Gagal)
- Sapi 16 + Sapi 11 = 27 (❌ Gagal)
- Sapi 16 + Sapi 18 = 34 (❌ Gagal)
- Sapi 12 + Sapi 11 = 23 (❌ Gagal)
- Sapi 12 + Sapi 18 = 30 (❌ Gagal)
- Sapi 11 + Sapi 18 = 29 (❌ Gagal)

Total pasangan yang bernilai 40 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 124**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSBSBUUUB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 7 unit langkah
C. 3 unit langkah
D. 6 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`S`): Koordinat kini `(-2, -2)`
- Instruksi 5 (`B`): Koordinat kini `(-3, -2)`
- Instruksi 6 (`U`): Koordinat kini `(-3, -1)`
- Instruksi 7 (`U`): Koordinat kini `(-3, 0)`
- Instruksi 8 (`U`): Koordinat kini `(-3, 1)`
- Instruksi 9 (`B`): Koordinat kini `(-4, 1)`

Posisi akhir robot adalah di titik `(-4, 1)`.
Jarak Manhattan = Murni $|-4| + |1|$ = 4 + 1 = **5 unit**.
Opsi valid: **E**.</details>

---
**Soal 125**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[11, 17, 5, 7, 2]`.
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
- Sapi 11 + Sapi 17 = 28 (❌ Gagal)
- Sapi 11 + Sapi 5 = 16 (❌ Gagal)
- Sapi 11 + Sapi 7 = 18 (❌ Gagal)
- Sapi 11 + Sapi 2 = 13 (❌ Gagal)
- Sapi 17 + Sapi 5 = 22 (❌ Gagal)
- Sapi 17 + Sapi 7 = 24 (❌ Gagal)
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)
- Sapi 5 + Sapi 7 = 12 (❌ Gagal)
- Sapi 5 + Sapi 2 = 7 (❌ Gagal)
- Sapi 7 + Sapi 2 = 9 (❌ Gagal)

Total pasangan yang bernilai 49 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 126**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSSSBBBUSUTUBTB`.
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
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 4 (`S`): Koordinat kini `(-1, -3)`
- Instruksi 5 (`B`): Koordinat kini `(-2, -3)`
- Instruksi 6 (`B`): Koordinat kini `(-3, -3)`
- Instruksi 7 (`B`): Koordinat kini `(-4, -3)`
- Instruksi 8 (`U`): Koordinat kini `(-4, -2)`
- Instruksi 9 (`S`): Koordinat kini `(-4, -3)`
- Instruksi 10 (`U`): Koordinat kini `(-4, -2)`
- Instruksi 11 (`T`): Koordinat kini `(-3, -2)`
- Instruksi 12 (`U`): Koordinat kini `(-3, -1)`
- Instruksi 13 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 14 (`T`): Koordinat kini `(-3, -1)`
- Instruksi 15 (`B`): Koordinat kini `(-4, -1)`

Posisi akhir robot adalah di titik `(-4, -1)`.
Jarak Manhattan = Murni $|-4| + |-1|$ = 4 + 1 = **5 unit**.
Opsi valid: **E**.</details>

---
**Soal 127**
Sebuah robot bola diletakkan di lantai 108. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 39 detik
B. 37 detik
C. 38 detik
D. 36 detik
E. 40 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (37 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 108 (Garis Start)
- Detik 1: Genap, turun 11 -> 108 - 11 = 97
- Detik 2: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 3: Genap, turun 11 -> 102 - 11 = 91
- Detik 4: Ganjil, naik 5 -> 91 + 5 = 96
- Detik 5: Genap, turun 11 -> 96 - 11 = 85
- Detik 6: Ganjil, naik 5 -> 85 + 5 = 90
- Detik 7: Genap, turun 11 -> 90 - 11 = 79
- Detik 8: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 9: Genap, turun 11 -> 84 - 11 = 73
- Detik 10: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 11: Genap, turun 11 -> 78 - 11 = 67
- Detik 12: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 13: Genap, turun 11 -> 72 - 11 = 61
- Detik 14: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 15: Genap, turun 11 -> 66 - 11 = 55
- Detik 16: Ganjil, naik 5 -> 55 + 5 = 60
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 37: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 128**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[10, 4, 6, 12, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 44."*

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
- Sapi 10 + Sapi 4 = 14 (❌ Gagal)
- Sapi 10 + Sapi 6 = 16 (❌ Gagal)
- Sapi 10 + Sapi 12 = 22 (❌ Gagal)
- Sapi 10 + Sapi 19 = 29 (❌ Gagal)
- Sapi 4 + Sapi 6 = 10 (❌ Gagal)
- Sapi 4 + Sapi 12 = 16 (❌ Gagal)
- Sapi 4 + Sapi 19 = 23 (❌ Gagal)
- Sapi 6 + Sapi 12 = 18 (❌ Gagal)
- Sapi 6 + Sapi 19 = 25 (❌ Gagal)
- Sapi 12 + Sapi 19 = 31 (❌ Gagal)

Total pasangan yang bernilai 44 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 129**
Sebuah robot bola diletakkan di lantai 111. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 115 detik
B. 118 detik
C. 116 detik
D. 117 detik
E. 119 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (116 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 111 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 111 + 5 = 116
- Detik 2: Genap, turun 7 -> 116 - 7 = 109
- Detik 3: Ganjil, naik 5 -> 109 + 5 = 114
- Detik 4: Genap, turun 7 -> 114 - 7 = 107
- Detik 5: Ganjil, naik 5 -> 107 + 5 = 112
- Detik 6: Genap, turun 7 -> 112 - 7 = 105
- Detik 7: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 8: Genap, turun 7 -> 110 - 7 = 103
- Detik 9: Ganjil, naik 5 -> 103 + 5 = 108
- Detik 10: Genap, turun 7 -> 108 - 7 = 101
- Detik 11: Ganjil, naik 5 -> 101 + 5 = 106
- Detik 12: Genap, turun 7 -> 106 - 7 = 99
- Detik 13: Ganjil, naik 5 -> 99 + 5 = 104
- Detik 14: Genap, turun 7 -> 104 - 7 = 97
- Detik 15: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 16: Genap, turun 7 -> 102 - 7 = 95
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 116: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 130**
Sebuah robot bola diletakkan di lantai 126. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 42 detik
B. 43 detik
C. 45 detik
D. 46 detik
E. 44 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (43 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 126 (Garis Start)
- Detik 1: Genap, turun 7 -> 126 - 7 = 119
- Detik 2: Ganjil, naik 1 -> 119 + 1 = 120
- Detik 3: Genap, turun 7 -> 120 - 7 = 113
- Detik 4: Ganjil, naik 1 -> 113 + 1 = 114
- Detik 5: Genap, turun 7 -> 114 - 7 = 107
- Detik 6: Ganjil, naik 1 -> 107 + 1 = 108
- Detik 7: Genap, turun 7 -> 108 - 7 = 101
- Detik 8: Ganjil, naik 1 -> 101 + 1 = 102
- Detik 9: Genap, turun 7 -> 102 - 7 = 95
- Detik 10: Ganjil, naik 1 -> 95 + 1 = 96
- Detik 11: Genap, turun 7 -> 96 - 7 = 89
- Detik 12: Ganjil, naik 1 -> 89 + 1 = 90
- Detik 13: Genap, turun 7 -> 90 - 7 = 83
- Detik 14: Ganjil, naik 1 -> 83 + 1 = 84
- Detik 15: Genap, turun 7 -> 84 - 7 = 77
- Detik 16: Ganjil, naik 1 -> 77 + 1 = 78
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 43: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 131**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSUUTSBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 0 unit langkah
B. 2 unit langkah
C. 1 unit langkah
D. 4 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`U`): Koordinat kini `(-1, 0)`
- Instruksi 4 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`T`): Koordinat kini `(0, 1)`
- Instruksi 6 (`S`): Koordinat kini `(0, 0)`
- Instruksi 7 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 8 (`S`): Koordinat kini `(-1, -1)`

Posisi akhir robot adalah di titik `(-1, -1)`.
Jarak Manhattan = Murni $|-1| + |-1|$ = 1 + 1 = **2 unit**.
Opsi valid: **B**.</details>

---
**Soal 132**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSUTUUBTTTTU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 8 unit langkah
B. 5 unit langkah
C. 6 unit langkah
D. 4 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`U`): Koordinat kini `(0, -1)`
- Instruksi 4 (`T`): Koordinat kini `(1, -1)`
- Instruksi 5 (`U`): Koordinat kini `(1, 0)`
- Instruksi 6 (`U`): Koordinat kini `(1, 1)`
- Instruksi 7 (`B`): Koordinat kini `(0, 1)`
- Instruksi 8 (`T`): Koordinat kini `(1, 1)`
- Instruksi 9 (`T`): Koordinat kini `(2, 1)`
- Instruksi 10 (`T`): Koordinat kini `(3, 1)`
- Instruksi 11 (`T`): Koordinat kini `(4, 1)`
- Instruksi 12 (`U`): Koordinat kini `(4, 2)`

Posisi akhir robot adalah di titik `(4, 2)`.
Jarak Manhattan = Murni $|4| + |2|$ = 4 + 2 = **6 unit**.
Opsi valid: **C**.</details>

---
**Soal 133**
Sebuah robot bola diletakkan di lantai 88. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 86 detik
B. 85 detik
C. 82 detik
D. 83 detik
E. 84 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (83 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 88 (Garis Start)
- Detik 1: Genap, turun 7 -> 88 - 7 = 81
- Detik 2: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 3: Genap, turun 7 -> 86 - 7 = 79
- Detik 4: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 5: Genap, turun 7 -> 84 - 7 = 77
- Detik 6: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 7: Genap, turun 7 -> 82 - 7 = 75
- Detik 8: Ganjil, naik 5 -> 75 + 5 = 80
- Detik 9: Genap, turun 7 -> 80 - 7 = 73
- Detik 10: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 11: Genap, turun 7 -> 78 - 7 = 71
- Detik 12: Ganjil, naik 5 -> 71 + 5 = 76
- Detik 13: Genap, turun 7 -> 76 - 7 = 69
- Detik 14: Ganjil, naik 5 -> 69 + 5 = 74
- Detik 15: Genap, turun 7 -> 74 - 7 = 67
- Detik 16: Ganjil, naik 5 -> 67 + 5 = 72
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 83: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 134**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTBUSUUUBUSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 2 unit langkah
C. 4 unit langkah
D. 5 unit langkah
E. 6 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(0, 1)`
- Instruksi 4 (`U`): Koordinat kini `(0, 2)`
- Instruksi 5 (`S`): Koordinat kini `(0, 1)`
- Instruksi 6 (`U`): Koordinat kini `(0, 2)`
- Instruksi 7 (`U`): Koordinat kini `(0, 3)`
- Instruksi 8 (`U`): Koordinat kini `(0, 4)`
- Instruksi 9 (`B`): Koordinat kini `(-1, 4)`
- Instruksi 10 (`U`): Koordinat kini `(-1, 5)`
- Instruksi 11 (`S`): Koordinat kini `(-1, 4)`
- Instruksi 12 (`S`): Koordinat kini `(-1, 3)`

Posisi akhir robot adalah di titik `(-1, 3)`.
Jarak Manhattan = Murni $|-1| + |3|$ = 1 + 3 = **4 unit**.
Opsi valid: **C**.</details>

---
**Soal 135**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[18, 23, 3, 9, 22]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 26."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 3 pasang
D. 2 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 18 + Sapi 23 = 41 (❌ Gagal)
- Sapi 18 + Sapi 3 = 21 (❌ Gagal)
- Sapi 18 + Sapi 9 = 27 (❌ Gagal)
- Sapi 18 + Sapi 22 = 40 (❌ Gagal)
- Sapi 23 + Sapi 3 = 26 (✅ COCOK)
- Sapi 23 + Sapi 9 = 32 (❌ Gagal)
- Sapi 23 + Sapi 22 = 45 (❌ Gagal)
- Sapi 3 + Sapi 9 = 12 (❌ Gagal)
- Sapi 3 + Sapi 22 = 25 (❌ Gagal)
- Sapi 9 + Sapi 22 = 31 (❌ Gagal)

Total pasangan yang bernilai 26 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 136**
Sebuah robot bola diletakkan di lantai 74. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 80 detik
B. 78 detik
C. 82 detik
D. 81 detik
E. 79 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (79 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 74 (Garis Start)
- Detik 1: Genap, turun 7 -> 74 - 7 = 67
- Detik 2: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 3: Genap, turun 7 -> 72 - 7 = 65
- Detik 4: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 5: Genap, turun 7 -> 70 - 7 = 63
- Detik 6: Ganjil, naik 5 -> 63 + 5 = 68
- Detik 7: Genap, turun 7 -> 68 - 7 = 61
- Detik 8: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 9: Genap, turun 7 -> 66 - 7 = 59
- Detik 10: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 11: Genap, turun 7 -> 64 - 7 = 57
- Detik 12: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 13: Genap, turun 7 -> 62 - 7 = 55
- Detik 14: Ganjil, naik 5 -> 55 + 5 = 60
- Detik 15: Genap, turun 7 -> 60 - 7 = 53
- Detik 16: Ganjil, naik 5 -> 53 + 5 = 58
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 79: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 137**
Sebuah robot bola diletakkan di lantai 137. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 39 detik
B. 38 detik
C. 40 detik
D. 41 detik
E. 37 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (38 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 137 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 137 + 5 = 142
- Detik 2: Genap, turun 13 -> 142 - 13 = 129
- Detik 3: Ganjil, naik 5 -> 129 + 5 = 134
- Detik 4: Genap, turun 13 -> 134 - 13 = 121
- Detik 5: Ganjil, naik 5 -> 121 + 5 = 126
- Detik 6: Genap, turun 13 -> 126 - 13 = 113
- Detik 7: Ganjil, naik 5 -> 113 + 5 = 118
- Detik 8: Genap, turun 13 -> 118 - 13 = 105
- Detik 9: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 10: Genap, turun 13 -> 110 - 13 = 97
- Detik 11: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 12: Genap, turun 13 -> 102 - 13 = 89
- Detik 13: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 14: Genap, turun 13 -> 94 - 13 = 81
- Detik 15: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 16: Genap, turun 13 -> 86 - 13 = 73
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 38: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 138**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[9, 12, 8, 24, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 4 pasang
D. 0 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 9 + Sapi 12 = 21 (❌ Gagal)
- Sapi 9 + Sapi 8 = 17 (❌ Gagal)
- Sapi 9 + Sapi 24 = 33 (❌ Gagal)
- Sapi 9 + Sapi 4 = 13 (❌ Gagal)
- Sapi 12 + Sapi 8 = 20 (❌ Gagal)
- Sapi 12 + Sapi 24 = 36 (❌ Gagal)
- Sapi 12 + Sapi 4 = 16 (❌ Gagal)
- Sapi 8 + Sapi 24 = 32 (❌ Gagal)
- Sapi 8 + Sapi 4 = 12 (❌ Gagal)
- Sapi 24 + Sapi 4 = 28 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 139**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUTBUUUUUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 8 unit langkah
B. 9 unit langkah
C. 6 unit langkah
D. 7 unit langkah
E. 10 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (8 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`T`): Koordinat kini `(1, 2)`
- Instruksi 4 (`B`): Koordinat kini `(0, 2)`
- Instruksi 5 (`U`): Koordinat kini `(0, 3)`
- Instruksi 6 (`U`): Koordinat kini `(0, 4)`
- Instruksi 7 (`U`): Koordinat kini `(0, 5)`
- Instruksi 8 (`U`): Koordinat kini `(0, 6)`
- Instruksi 9 (`U`): Koordinat kini `(0, 7)`
- Instruksi 10 (`T`): Koordinat kini `(1, 7)`

Posisi akhir robot adalah di titik `(1, 7)`.
Jarak Manhattan = Murni $|1| + |7|$ = 1 + 7 = **8 unit**.
Opsi valid: **A**.</details>

---
**Soal 140**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[6, 15, 24, 11, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 45."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 4 pasang
C. 2 pasang
D. 0 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 6 + Sapi 15 = 21 (❌ Gagal)
- Sapi 6 + Sapi 24 = 30 (❌ Gagal)
- Sapi 6 + Sapi 11 = 17 (❌ Gagal)
- Sapi 6 + Sapi 17 = 23 (❌ Gagal)
- Sapi 15 + Sapi 24 = 39 (❌ Gagal)
- Sapi 15 + Sapi 11 = 26 (❌ Gagal)
- Sapi 15 + Sapi 17 = 32 (❌ Gagal)
- Sapi 24 + Sapi 11 = 35 (❌ Gagal)
- Sapi 24 + Sapi 17 = 41 (❌ Gagal)
- Sapi 11 + Sapi 17 = 28 (❌ Gagal)

Total pasangan yang bernilai 45 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 141**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TBSUBSSBBUBTBT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 6 unit langkah
C. 4 unit langkah
D. 2 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`B`): Koordinat kini `(0, 0)`
- Instruksi 3 (`S`): Koordinat kini `(0, -1)`
- Instruksi 4 (`U`): Koordinat kini `(0, 0)`
- Instruksi 5 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(-1, -2)`
- Instruksi 8 (`B`): Koordinat kini `(-2, -2)`
- Instruksi 9 (`B`): Koordinat kini `(-3, -2)`
- Instruksi 10 (`U`): Koordinat kini `(-3, -1)`
- Instruksi 11 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 12 (`T`): Koordinat kini `(-3, -1)`
- Instruksi 13 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 14 (`T`): Koordinat kini `(-3, -1)`

Posisi akhir robot adalah di titik `(-3, -1)`.
Jarak Manhattan = Murni $|-3| + |-1|$ = 3 + 1 = **4 unit**.
Opsi valid: **C**.</details>

---
**Soal 142**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSTSUBTSSB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 4 unit langkah
C. 6 unit langkah
D. 5 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(2, -1)`
- Instruksi 4 (`S`): Koordinat kini `(2, -2)`
- Instruksi 5 (`U`): Koordinat kini `(2, -1)`
- Instruksi 6 (`B`): Koordinat kini `(1, -1)`
- Instruksi 7 (`T`): Koordinat kini `(2, -1)`
- Instruksi 8 (`S`): Koordinat kini `(2, -2)`
- Instruksi 9 (`S`): Koordinat kini `(2, -3)`
- Instruksi 10 (`B`): Koordinat kini `(1, -3)`

Posisi akhir robot adalah di titik `(1, -3)`.
Jarak Manhattan = Murni $|1| + |-3|$ = 1 + 3 = **4 unit**.
Opsi valid: **B**.</details>

---
**Soal 143**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[13, 2, 10, 23, 14]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 42."*

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
- Sapi 13 + Sapi 2 = 15 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)
- Sapi 13 + Sapi 23 = 36 (❌ Gagal)
- Sapi 13 + Sapi 14 = 27 (❌ Gagal)
- Sapi 2 + Sapi 10 = 12 (❌ Gagal)
- Sapi 2 + Sapi 23 = 25 (❌ Gagal)
- Sapi 2 + Sapi 14 = 16 (❌ Gagal)
- Sapi 10 + Sapi 23 = 33 (❌ Gagal)
- Sapi 10 + Sapi 14 = 24 (❌ Gagal)
- Sapi 23 + Sapi 14 = 37 (❌ Gagal)

Total pasangan yang bernilai 42 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 144**
Sebuah robot bola diletakkan di lantai 57. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 34 detik
B. 32 detik
C. 33 detik
D. 31 detik
E. 35 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (32 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 57 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 57 + 3 = 60
- Detik 2: Genap, turun 7 -> 60 - 7 = 53
- Detik 3: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 4: Genap, turun 7 -> 56 - 7 = 49
- Detik 5: Ganjil, naik 3 -> 49 + 3 = 52
- Detik 6: Genap, turun 7 -> 52 - 7 = 45
- Detik 7: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 8: Genap, turun 7 -> 48 - 7 = 41
- Detik 9: Ganjil, naik 3 -> 41 + 3 = 44
- Detik 10: Genap, turun 7 -> 44 - 7 = 37
- Detik 11: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 12: Genap, turun 7 -> 40 - 7 = 33
- Detik 13: Ganjil, naik 3 -> 33 + 3 = 36
- Detik 14: Genap, turun 7 -> 36 - 7 = 29
- Detik 15: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 16: Genap, turun 7 -> 32 - 7 = 25
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 32: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 145**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[21, 17, 10, 6, 12]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 33."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 2 pasang
C. 1 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 21 + Sapi 17 = 38 (❌ Gagal)
- Sapi 21 + Sapi 10 = 31 (❌ Gagal)
- Sapi 21 + Sapi 6 = 27 (❌ Gagal)
- Sapi 21 + Sapi 12 = 33 (✅ COCOK)
- Sapi 17 + Sapi 10 = 27 (❌ Gagal)
- Sapi 17 + Sapi 6 = 23 (❌ Gagal)
- Sapi 17 + Sapi 12 = 29 (❌ Gagal)
- Sapi 10 + Sapi 6 = 16 (❌ Gagal)
- Sapi 10 + Sapi 12 = 22 (❌ Gagal)
- Sapi 6 + Sapi 12 = 18 (❌ Gagal)

Total pasangan yang bernilai 33 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 146**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSSTSSTBBB`.
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
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`T`): Koordinat kini `(1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(1, -1)`
- Instruksi 7 (`S`): Koordinat kini `(1, -2)`
- Instruksi 8 (`T`): Koordinat kini `(2, -2)`
- Instruksi 9 (`B`): Koordinat kini `(1, -2)`
- Instruksi 10 (`B`): Koordinat kini `(0, -2)`
- Instruksi 11 (`B`): Koordinat kini `(-1, -2)`

Posisi akhir robot adalah di titik `(-1, -2)`.
Jarak Manhattan = Murni $|-1| + |-2|$ = 1 + 2 = **3 unit**.
Opsi valid: **C**.</details>

---
**Soal 147**
Sebuah robot bola diletakkan di lantai 62. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 13 detik
B. 10 detik
C. 11 detik
D. 14 detik
E. 12 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (11 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 62 (Garis Start)
- Detik 1: Genap, turun 13 -> 62 - 13 = 49
- Detik 2: Ganjil, naik 1 -> 49 + 1 = 50
- Detik 3: Genap, turun 13 -> 50 - 13 = 37
- Detik 4: Ganjil, naik 1 -> 37 + 1 = 38
- Detik 5: Genap, turun 13 -> 38 - 13 = 25
- Detik 6: Ganjil, naik 1 -> 25 + 1 = 26
- Detik 7: Genap, turun 13 -> 26 - 13 = 13
- Detik 8: Ganjil, naik 1 -> 13 + 1 = 14
- Detik 9: Genap, turun 13 -> 14 - 13 = 1
- Detik 10: Ganjil, naik 1 -> 1 + 1 = 2
- Detik 11: Genap, turun 13 -> 2 - 13 = -11
Simulasi berakhir pada detik ke-11. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 148**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[12, 19, 16, 4, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 32."*

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
- Sapi 12 + Sapi 19 = 31 (❌ Gagal)
- Sapi 12 + Sapi 16 = 28 (❌ Gagal)
- Sapi 12 + Sapi 4 = 16 (❌ Gagal)
- Sapi 12 + Sapi 17 = 29 (❌ Gagal)
- Sapi 19 + Sapi 16 = 35 (❌ Gagal)
- Sapi 19 + Sapi 4 = 23 (❌ Gagal)
- Sapi 19 + Sapi 17 = 36 (❌ Gagal)
- Sapi 16 + Sapi 4 = 20 (❌ Gagal)
- Sapi 16 + Sapi 17 = 33 (❌ Gagal)
- Sapi 4 + Sapi 17 = 21 (❌ Gagal)

Total pasangan yang bernilai 32 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 149**
Sebuah robot bola diletakkan di lantai 90. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 31 detik
B. 28 detik
C. 29 detik
D. 30 detik
E. 32 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (29 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 90 (Garis Start)
- Detik 1: Genap, turun 11 -> 90 - 11 = 79
- Detik 2: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 3: Genap, turun 11 -> 84 - 11 = 73
- Detik 4: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 5: Genap, turun 11 -> 78 - 11 = 67
- Detik 6: Ganjil, naik 5 -> 67 + 5 = 72
- Detik 7: Genap, turun 11 -> 72 - 11 = 61
- Detik 8: Ganjil, naik 5 -> 61 + 5 = 66
- Detik 9: Genap, turun 11 -> 66 - 11 = 55
- Detik 10: Ganjil, naik 5 -> 55 + 5 = 60
- Detik 11: Genap, turun 11 -> 60 - 11 = 49
- Detik 12: Ganjil, naik 5 -> 49 + 5 = 54
- Detik 13: Genap, turun 11 -> 54 - 11 = 43
- Detik 14: Ganjil, naik 5 -> 43 + 5 = 48
- Detik 15: Genap, turun 11 -> 48 - 11 = 37
- Detik 16: Ganjil, naik 5 -> 37 + 5 = 42
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 29: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 150**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 20, 23, 16, 13]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 34."*

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
- Sapi 22 + Sapi 20 = 42 (❌ Gagal)
- Sapi 22 + Sapi 23 = 45 (❌ Gagal)
- Sapi 22 + Sapi 16 = 38 (❌ Gagal)
- Sapi 22 + Sapi 13 = 35 (❌ Gagal)
- Sapi 20 + Sapi 23 = 43 (❌ Gagal)
- Sapi 20 + Sapi 16 = 36 (❌ Gagal)
- Sapi 20 + Sapi 13 = 33 (❌ Gagal)
- Sapi 23 + Sapi 16 = 39 (❌ Gagal)
- Sapi 23 + Sapi 13 = 36 (❌ Gagal)
- Sapi 16 + Sapi 13 = 29 (❌ Gagal)

Total pasangan yang bernilai 34 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
