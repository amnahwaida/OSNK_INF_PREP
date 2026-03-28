🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latian Soal: Simulasi & Brute Force (Part 2 / 6)

Berikut adalah kompilasi simulasi soal OSN untuk materi **Simulasi & Brute Force**. Setiap nomor dibekali Kunci Jawaban "Diagnosis Mesin" di balik tirai tersembunyi.

---

**Soal 51**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSTBTSBSSUBTTUS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 7 unit langkah
B. 4 unit langkah
C. 5 unit langkah
D. 6 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (5 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`T`): Koordinat kini `(1, -2)`
- Instruksi 4 (`B`): Koordinat kini `(0, -2)`
- Instruksi 5 (`T`): Koordinat kini `(1, -2)`
- Instruksi 6 (`S`): Koordinat kini `(1, -3)`
- Instruksi 7 (`B`): Koordinat kini `(0, -3)`
- Instruksi 8 (`S`): Koordinat kini `(0, -4)`
- Instruksi 9 (`S`): Koordinat kini `(0, -5)`
- Instruksi 10 (`U`): Koordinat kini `(0, -4)`
- Instruksi 11 (`B`): Koordinat kini `(-1, -4)`
- Instruksi 12 (`T`): Koordinat kini `(0, -4)`
- Instruksi 13 (`T`): Koordinat kini `(1, -4)`
- Instruksi 14 (`U`): Koordinat kini `(1, -3)`
- Instruksi 15 (`S`): Koordinat kini `(1, -4)`

Posisi akhir robot adalah di titik `(1, -4)`.
Jarak Manhattan = Murni $|1| + |-4|$ = 1 + 4 = **5 unit**.
Opsi valid: **C**.</details>

---
**Soal 52**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UTSTBSTTUUUUTUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 7 unit langkah
B. 9 unit langkah
C. 11 unit langkah
D. 8 unit langkah
E. 10 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: B (9 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`T`): Koordinat kini `(1, 1)`
- Instruksi 3 (`S`): Koordinat kini `(1, 0)`
- Instruksi 4 (`T`): Koordinat kini `(2, 0)`
- Instruksi 5 (`B`): Koordinat kini `(1, 0)`
- Instruksi 6 (`S`): Koordinat kini `(1, -1)`
- Instruksi 7 (`T`): Koordinat kini `(2, -1)`
- Instruksi 8 (`T`): Koordinat kini `(3, -1)`
- Instruksi 9 (`U`): Koordinat kini `(3, 0)`
- Instruksi 10 (`U`): Koordinat kini `(3, 1)`
- Instruksi 11 (`U`): Koordinat kini `(3, 2)`
- Instruksi 12 (`U`): Koordinat kini `(3, 3)`
- Instruksi 13 (`T`): Koordinat kini `(4, 3)`
- Instruksi 14 (`U`): Koordinat kini `(4, 4)`
- Instruksi 15 (`T`): Koordinat kini `(5, 4)`

Posisi akhir robot adalah di titik `(5, 4)`.
Jarak Manhattan = Murni $|5| + |4|$ = 5 + 4 = **9 unit**.
Opsi valid: **B**.</details>

---
**Soal 53**
Sebuah robot bola diletakkan di lantai 62. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 15 detik
B. 17 detik
C. 16 detik
D. 14 detik
E. 18 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (15 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 62 (Garis Start)
- Detik 1: Genap, turun 13 -> 62 - 13 = 49
- Detik 2: Ganjil, naik 5 -> 49 + 5 = 54
- Detik 3: Genap, turun 13 -> 54 - 13 = 41
- Detik 4: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 5: Genap, turun 13 -> 46 - 13 = 33
- Detik 6: Ganjil, naik 5 -> 33 + 5 = 38
- Detik 7: Genap, turun 13 -> 38 - 13 = 25
- Detik 8: Ganjil, naik 5 -> 25 + 5 = 30
- Detik 9: Genap, turun 13 -> 30 - 13 = 17
- Detik 10: Ganjil, naik 5 -> 17 + 5 = 22
- Detik 11: Genap, turun 13 -> 22 - 13 = 9
- Detik 12: Ganjil, naik 5 -> 9 + 5 = 14
- Detik 13: Genap, turun 13 -> 14 - 13 = 1
- Detik 14: Ganjil, naik 5 -> 1 + 5 = 6
- Detik 15: Genap, turun 13 -> 6 - 13 = -7
Simulasi berakhir pada detik ke-15. Jawaban yang tepat adalah opsi **A**.
</details>

---
**Soal 54**
Sebuah robot bola diletakkan di lantai 69. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 20 detik
B. 19 detik
C. 21 detik
D. 22 detik
E. 23 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (20 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 69 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 2: Genap, turun 11 -> 72 - 11 = 61
- Detik 3: Ganjil, naik 3 -> 61 + 3 = 64
- Detik 4: Genap, turun 11 -> 64 - 11 = 53
- Detik 5: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 6: Genap, turun 11 -> 56 - 11 = 45
- Detik 7: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 8: Genap, turun 11 -> 48 - 11 = 37
- Detik 9: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 10: Genap, turun 11 -> 40 - 11 = 29
- Detik 11: Ganjil, naik 3 -> 29 + 3 = 32
- Detik 12: Genap, turun 11 -> 32 - 11 = 21
- Detik 13: Ganjil, naik 3 -> 21 + 3 = 24
- Detik 14: Genap, turun 11 -> 24 - 11 = 13
- Detik 15: Ganjil, naik 3 -> 13 + 3 = 16
- Detik 16: Genap, turun 11 -> 16 - 11 = 5
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 20: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 55**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[14, 15, 19, 23, 9]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 1 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 14 + Sapi 15 = 29 (❌ Gagal)
- Sapi 14 + Sapi 19 = 33 (❌ Gagal)
- Sapi 14 + Sapi 23 = 37 (❌ Gagal)
- Sapi 14 + Sapi 9 = 23 (❌ Gagal)
- Sapi 15 + Sapi 19 = 34 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 15 + Sapi 9 = 24 (❌ Gagal)
- Sapi 19 + Sapi 23 = 42 (❌ Gagal)
- Sapi 19 + Sapi 9 = 28 (❌ Gagal)
- Sapi 23 + Sapi 9 = 32 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 56**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TUBSTUUTUBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 2 unit langkah
C. 1 unit langkah
D. 5 unit langkah
E. 4 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(1, 1)`
- Instruksi 3 (`B`): Koordinat kini `(0, 1)`
- Instruksi 4 (`S`): Koordinat kini `(0, 0)`
- Instruksi 5 (`T`): Koordinat kini `(1, 0)`
- Instruksi 6 (`U`): Koordinat kini `(1, 1)`
- Instruksi 7 (`U`): Koordinat kini `(1, 2)`
- Instruksi 8 (`T`): Koordinat kini `(2, 2)`
- Instruksi 9 (`U`): Koordinat kini `(2, 3)`
- Instruksi 10 (`B`): Koordinat kini `(1, 3)`
- Instruksi 11 (`S`): Koordinat kini `(1, 2)`

Posisi akhir robot adalah di titik `(1, 2)`.
Jarak Manhattan = Murni $|1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **A**.</details>

---
**Soal 57**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BTSTBUBBTUTSUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 3 unit langkah
B. 0 unit langkah
C. 4 unit langkah
D. 2 unit langkah
E. 1 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: D (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`T`): Koordinat kini `(0, 0)`
- Instruksi 3 (`S`): Koordinat kini `(0, -1)`
- Instruksi 4 (`T`): Koordinat kini `(1, -1)`
- Instruksi 5 (`B`): Koordinat kini `(0, -1)`
- Instruksi 6 (`U`): Koordinat kini `(0, 0)`
- Instruksi 7 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 8 (`B`): Koordinat kini `(-2, 0)`
- Instruksi 9 (`T`): Koordinat kini `(-1, 0)`
- Instruksi 10 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 11 (`T`): Koordinat kini `(0, 1)`
- Instruksi 12 (`S`): Koordinat kini `(0, 0)`
- Instruksi 13 (`U`): Koordinat kini `(0, 1)`
- Instruksi 14 (`T`): Koordinat kini `(1, 1)`

Posisi akhir robot adalah di titik `(1, 1)`.
Jarak Manhattan = Murni $|1| + |1|$ = 1 + 1 = **2 unit**.
Opsi valid: **D**.</details>

---
**Soal 58**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[17, 15, 23, 12, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 26."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 4 pasang
D. 3 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 17 + Sapi 15 = 32 (❌ Gagal)
- Sapi 17 + Sapi 23 = 40 (❌ Gagal)
- Sapi 17 + Sapi 12 = 29 (❌ Gagal)
- Sapi 17 + Sapi 19 = 36 (❌ Gagal)
- Sapi 15 + Sapi 23 = 38 (❌ Gagal)
- Sapi 15 + Sapi 12 = 27 (❌ Gagal)
- Sapi 15 + Sapi 19 = 34 (❌ Gagal)
- Sapi 23 + Sapi 12 = 35 (❌ Gagal)
- Sapi 23 + Sapi 19 = 42 (❌ Gagal)
- Sapi 12 + Sapi 19 = 31 (❌ Gagal)

Total pasangan yang bernilai 26 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 59**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `UUSBUTBTTBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. -1 unit langkah
C. 0 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (1 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`U`): Koordinat kini `(0, 1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 2)`
- Instruksi 3 (`S`): Koordinat kini `(0, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`U`): Koordinat kini `(-1, 2)`
- Instruksi 6 (`T`): Koordinat kini `(0, 2)`
- Instruksi 7 (`B`): Koordinat kini `(-1, 2)`
- Instruksi 8 (`T`): Koordinat kini `(0, 2)`
- Instruksi 9 (`T`): Koordinat kini `(1, 2)`
- Instruksi 10 (`B`): Koordinat kini `(0, 2)`
- Instruksi 11 (`S`): Koordinat kini `(0, 1)`

Posisi akhir robot adalah di titik `(0, 1)`.
Jarak Manhattan = Murni $|0| + |1|$ = 0 + 1 = **1 unit**.
Opsi valid: **A**.</details>

---
**Soal 60**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 13, 10, 9, 17]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 27."*

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
- Sapi 22 + Sapi 13 = 35 (❌ Gagal)
- Sapi 22 + Sapi 10 = 32 (❌ Gagal)
- Sapi 22 + Sapi 9 = 31 (❌ Gagal)
- Sapi 22 + Sapi 17 = 39 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)
- Sapi 13 + Sapi 9 = 22 (❌ Gagal)
- Sapi 13 + Sapi 17 = 30 (❌ Gagal)
- Sapi 10 + Sapi 9 = 19 (❌ Gagal)
- Sapi 10 + Sapi 17 = 27 (✅ COCOK)
- Sapi 9 + Sapi 17 = 26 (❌ Gagal)

Total pasangan yang bernilai 27 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 61**
Sebuah robot bola diletakkan di lantai 70. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 23 detik
B. 21 detik
C. 20 detik
D. 24 detik
E. 22 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (21 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 70 (Garis Start)
- Detik 1: Genap, turun 11 -> 70 - 11 = 59
- Detik 2: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 3: Genap, turun 11 -> 64 - 11 = 53
- Detik 4: Ganjil, naik 5 -> 53 + 5 = 58
- Detik 5: Genap, turun 11 -> 58 - 11 = 47
- Detik 6: Ganjil, naik 5 -> 47 + 5 = 52
- Detik 7: Genap, turun 11 -> 52 - 11 = 41
- Detik 8: Ganjil, naik 5 -> 41 + 5 = 46
- Detik 9: Genap, turun 11 -> 46 - 11 = 35
- Detik 10: Ganjil, naik 5 -> 35 + 5 = 40
- Detik 11: Genap, turun 11 -> 40 - 11 = 29
- Detik 12: Ganjil, naik 5 -> 29 + 5 = 34
- Detik 13: Genap, turun 11 -> 34 - 11 = 23
- Detik 14: Ganjil, naik 5 -> 23 + 5 = 28
- Detik 15: Genap, turun 11 -> 28 - 11 = 17
- Detik 16: Ganjil, naik 5 -> 17 + 5 = 22
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 21: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 62**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[8, 13, 11, 3, 4]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 32."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 3 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 8 + Sapi 13 = 21 (❌ Gagal)
- Sapi 8 + Sapi 11 = 19 (❌ Gagal)
- Sapi 8 + Sapi 3 = 11 (❌ Gagal)
- Sapi 8 + Sapi 4 = 12 (❌ Gagal)
- Sapi 13 + Sapi 11 = 24 (❌ Gagal)
- Sapi 13 + Sapi 3 = 16 (❌ Gagal)
- Sapi 13 + Sapi 4 = 17 (❌ Gagal)
- Sapi 11 + Sapi 3 = 14 (❌ Gagal)
- Sapi 11 + Sapi 4 = 15 (❌ Gagal)
- Sapi 3 + Sapi 4 = 7 (❌ Gagal)

Total pasangan yang bernilai 32 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 63**
Sebuah robot bola diletakkan di lantai 59. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 14 detik
B. 15 detik
C. 12 detik
D. 11 detik
E. 13 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (12 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 59 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 59 + 1 = 60
- Detik 2: Genap, turun 13 -> 60 - 13 = 47
- Detik 3: Ganjil, naik 1 -> 47 + 1 = 48
- Detik 4: Genap, turun 13 -> 48 - 13 = 35
- Detik 5: Ganjil, naik 1 -> 35 + 1 = 36
- Detik 6: Genap, turun 13 -> 36 - 13 = 23
- Detik 7: Ganjil, naik 1 -> 23 + 1 = 24
- Detik 8: Genap, turun 13 -> 24 - 13 = 11
- Detik 9: Ganjil, naik 1 -> 11 + 1 = 12
- Detik 10: Genap, turun 13 -> 12 - 13 = -1
- Detik 11: Ganjil, naik 1 -> -1 + 1 = 0
- Detik 12: Genap, turun 13 -> 0 - 13 = -13
Simulasi berakhir pada detik ke-12. Jawaban yang tepat adalah opsi **C**.
</details>

---
**Soal 64**
Sebuah robot bola diletakkan di lantai 142. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 33 detik
B. 32 detik
C. 31 detik
D. 34 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (31 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 142 (Garis Start)
- Detik 1: Genap, turun 11 -> 142 - 11 = 131
- Detik 2: Ganjil, naik 1 -> 131 + 1 = 132
- Detik 3: Genap, turun 11 -> 132 - 11 = 121
- Detik 4: Ganjil, naik 1 -> 121 + 1 = 122
- Detik 5: Genap, turun 11 -> 122 - 11 = 111
- Detik 6: Ganjil, naik 1 -> 111 + 1 = 112
- Detik 7: Genap, turun 11 -> 112 - 11 = 101
- Detik 8: Ganjil, naik 1 -> 101 + 1 = 102
- Detik 9: Genap, turun 11 -> 102 - 11 = 91
- Detik 10: Ganjil, naik 1 -> 91 + 1 = 92
- Detik 11: Genap, turun 11 -> 92 - 11 = 81
- Detik 12: Ganjil, naik 1 -> 81 + 1 = 82
- Detik 13: Genap, turun 11 -> 82 - 11 = 71
- Detik 14: Ganjil, naik 1 -> 71 + 1 = 72
- Detik 15: Genap, turun 11 -> 72 - 11 = 61
- Detik 16: Ganjil, naik 1 -> 61 + 1 = 62
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 31: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 65**
Sebuah robot bola diletakkan di lantai 76. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 28 detik
B. 26 detik
C. 27 detik
D. 29 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (27 detik)**

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
**Soal 66**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSUTSSSSBUTBUU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 2 unit langkah
B. 1 unit langkah
C. 4 unit langkah
D. 3 unit langkah
E. 0 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (2 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`U`): Koordinat kini `(0, -1)`
- Instruksi 4 (`T`): Koordinat kini `(1, -1)`
- Instruksi 5 (`S`): Koordinat kini `(1, -2)`
- Instruksi 6 (`S`): Koordinat kini `(1, -3)`
- Instruksi 7 (`S`): Koordinat kini `(1, -4)`
- Instruksi 8 (`S`): Koordinat kini `(1, -5)`
- Instruksi 9 (`B`): Koordinat kini `(0, -5)`
- Instruksi 10 (`U`): Koordinat kini `(0, -4)`
- Instruksi 11 (`T`): Koordinat kini `(1, -4)`
- Instruksi 12 (`B`): Koordinat kini `(0, -4)`
- Instruksi 13 (`U`): Koordinat kini `(0, -3)`
- Instruksi 14 (`U`): Koordinat kini `(0, -2)`

Posisi akhir robot adalah di titik `(0, -2)`.
Jarak Manhattan = Murni $|0| + |-2|$ = 0 + 2 = **2 unit**.
Opsi valid: **A**.</details>

---
**Soal 67**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[13, 21, 6, 24, 8]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 1 pasang
C. 2 pasang
D. 3 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 13 + Sapi 21 = 34 (❌ Gagal)
- Sapi 13 + Sapi 6 = 19 (❌ Gagal)
- Sapi 13 + Sapi 24 = 37 (❌ Gagal)
- Sapi 13 + Sapi 8 = 21 (❌ Gagal)
- Sapi 21 + Sapi 6 = 27 (❌ Gagal)
- Sapi 21 + Sapi 24 = 45 (❌ Gagal)
- Sapi 21 + Sapi 8 = 29 (❌ Gagal)
- Sapi 6 + Sapi 24 = 30 (✅ COCOK)
- Sapi 6 + Sapi 8 = 14 (❌ Gagal)
- Sapi 24 + Sapi 8 = 32 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 68**
Sebuah robot bola diletakkan di lantai 89. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 94 detik
B. 97 detik
C. 96 detik
D. 93 detik
E. 95 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (94 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 89 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 2: Genap, turun 7 -> 94 - 7 = 87
- Detik 3: Ganjil, naik 5 -> 87 + 5 = 92
- Detik 4: Genap, turun 7 -> 92 - 7 = 85
- Detik 5: Ganjil, naik 5 -> 85 + 5 = 90
- Detik 6: Genap, turun 7 -> 90 - 7 = 83
- Detik 7: Ganjil, naik 5 -> 83 + 5 = 88
- Detik 8: Genap, turun 7 -> 88 - 7 = 81
- Detik 9: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 10: Genap, turun 7 -> 86 - 7 = 79
- Detik 11: Ganjil, naik 5 -> 79 + 5 = 84
- Detik 12: Genap, turun 7 -> 84 - 7 = 77
- Detik 13: Ganjil, naik 5 -> 77 + 5 = 82
- Detik 14: Genap, turun 7 -> 82 - 7 = 75
- Detik 15: Ganjil, naik 5 -> 75 + 5 = 80
- Detik 16: Genap, turun 7 -> 80 - 7 = 73
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 94: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 69**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `TSTSSBBTBTSSTU`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 5 unit langkah
C. 6 unit langkah
D. 8 unit langkah
E. 7 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`T`): Koordinat kini `(1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(1, -1)`
- Instruksi 3 (`T`): Koordinat kini `(2, -1)`
- Instruksi 4 (`S`): Koordinat kini `(2, -2)`
- Instruksi 5 (`S`): Koordinat kini `(2, -3)`
- Instruksi 6 (`B`): Koordinat kini `(1, -3)`
- Instruksi 7 (`B`): Koordinat kini `(0, -3)`
- Instruksi 8 (`T`): Koordinat kini `(1, -3)`
- Instruksi 9 (`B`): Koordinat kini `(0, -3)`
- Instruksi 10 (`T`): Koordinat kini `(1, -3)`
- Instruksi 11 (`S`): Koordinat kini `(1, -4)`
- Instruksi 12 (`S`): Koordinat kini `(1, -5)`
- Instruksi 13 (`T`): Koordinat kini `(2, -5)`
- Instruksi 14 (`U`): Koordinat kini `(2, -4)`

Posisi akhir robot adalah di titik `(2, -4)`.
Jarak Manhattan = Murni $|2| + |-4|$ = 2 + 4 = **6 unit**.
Opsi valid: **C**.</details>

---
**Soal 70**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[9, 3, 7, 8, 20]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 27."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 4 pasang
D. 3 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 9 + Sapi 3 = 12 (❌ Gagal)
- Sapi 9 + Sapi 7 = 16 (❌ Gagal)
- Sapi 9 + Sapi 8 = 17 (❌ Gagal)
- Sapi 9 + Sapi 20 = 29 (❌ Gagal)
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 8 = 11 (❌ Gagal)
- Sapi 3 + Sapi 20 = 23 (❌ Gagal)
- Sapi 7 + Sapi 8 = 15 (❌ Gagal)
- Sapi 7 + Sapi 20 = 27 (✅ COCOK)
- Sapi 8 + Sapi 20 = 28 (❌ Gagal)

Total pasangan yang bernilai 27 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 71**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[17, 2, 19, 16, 21]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 26."*

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
- Sapi 17 + Sapi 2 = 19 (❌ Gagal)
- Sapi 17 + Sapi 19 = 36 (❌ Gagal)
- Sapi 17 + Sapi 16 = 33 (❌ Gagal)
- Sapi 17 + Sapi 21 = 38 (❌ Gagal)
- Sapi 2 + Sapi 19 = 21 (❌ Gagal)
- Sapi 2 + Sapi 16 = 18 (❌ Gagal)
- Sapi 2 + Sapi 21 = 23 (❌ Gagal)
- Sapi 19 + Sapi 16 = 35 (❌ Gagal)
- Sapi 19 + Sapi 21 = 40 (❌ Gagal)
- Sapi 16 + Sapi 21 = 37 (❌ Gagal)

Total pasangan yang bernilai 26 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 72**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SUTTUUSSTUBTTBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 1 unit langkah
B. 2 unit langkah
C. 5 unit langkah
D. 4 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 0)`
- Instruksi 3 (`T`): Koordinat kini `(1, 0)`
- Instruksi 4 (`T`): Koordinat kini `(2, 0)`
- Instruksi 5 (`U`): Koordinat kini `(2, 1)`
- Instruksi 6 (`U`): Koordinat kini `(2, 2)`
- Instruksi 7 (`S`): Koordinat kini `(2, 1)`
- Instruksi 8 (`S`): Koordinat kini `(2, 0)`
- Instruksi 9 (`T`): Koordinat kini `(3, 0)`
- Instruksi 10 (`U`): Koordinat kini `(3, 1)`
- Instruksi 11 (`B`): Koordinat kini `(2, 1)`
- Instruksi 12 (`T`): Koordinat kini `(3, 1)`
- Instruksi 13 (`T`): Koordinat kini `(4, 1)`
- Instruksi 14 (`B`): Koordinat kini `(3, 1)`
- Instruksi 15 (`S`): Koordinat kini `(3, 0)`

Posisi akhir robot adalah di titik `(3, 0)`.
Jarak Manhattan = Murni $|3| + |0|$ = 3 + 0 = **3 unit**.
Opsi valid: **E**.</details>

---
**Soal 73**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BSBBBUSUBSSB`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 6 unit langkah
B. 7 unit langkah
C. 9 unit langkah
D. 10 unit langkah
E. 8 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (8 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`S`): Koordinat kini `(-1, -1)`
- Instruksi 3 (`B`): Koordinat kini `(-2, -1)`
- Instruksi 4 (`B`): Koordinat kini `(-3, -1)`
- Instruksi 5 (`B`): Koordinat kini `(-4, -1)`
- Instruksi 6 (`U`): Koordinat kini `(-4, 0)`
- Instruksi 7 (`S`): Koordinat kini `(-4, -1)`
- Instruksi 8 (`U`): Koordinat kini `(-4, 0)`
- Instruksi 9 (`B`): Koordinat kini `(-5, 0)`
- Instruksi 10 (`S`): Koordinat kini `(-5, -1)`
- Instruksi 11 (`S`): Koordinat kini `(-5, -2)`
- Instruksi 12 (`B`): Koordinat kini `(-6, -2)`

Posisi akhir robot adalah di titik `(-6, -2)`.
Jarak Manhattan = Murni $|-6| + |-2|$ = 6 + 2 = **8 unit**.
Opsi valid: **E**.</details>

---
**Soal 74**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[12, 16, 8, 20, 14]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

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
- Sapi 12 + Sapi 16 = 28 (❌ Gagal)
- Sapi 12 + Sapi 8 = 20 (❌ Gagal)
- Sapi 12 + Sapi 20 = 32 (❌ Gagal)
- Sapi 12 + Sapi 14 = 26 (❌ Gagal)
- Sapi 16 + Sapi 8 = 24 (❌ Gagal)
- Sapi 16 + Sapi 20 = 36 (❌ Gagal)
- Sapi 16 + Sapi 14 = 30 (❌ Gagal)
- Sapi 8 + Sapi 20 = 28 (❌ Gagal)
- Sapi 8 + Sapi 14 = 22 (❌ Gagal)
- Sapi 20 + Sapi 14 = 34 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 75**
Sebuah robot bola diletakkan di lantai 86. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 44 detik
B. 42 detik
C. 45 detik
D. 46 detik
E. 43 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: E (43 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 86 (Garis Start)
- Detik 1: Genap, turun 7 -> 86 - 7 = 79
- Detik 2: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 3: Genap, turun 7 -> 82 - 7 = 75
- Detik 4: Ganjil, naik 3 -> 75 + 3 = 78
- Detik 5: Genap, turun 7 -> 78 - 7 = 71
- Detik 6: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 7: Genap, turun 7 -> 74 - 7 = 67
- Detik 8: Ganjil, naik 3 -> 67 + 3 = 70
- Detik 9: Genap, turun 7 -> 70 - 7 = 63
- Detik 10: Ganjil, naik 3 -> 63 + 3 = 66
- Detik 11: Genap, turun 7 -> 66 - 7 = 59
- Detik 12: Ganjil, naik 3 -> 59 + 3 = 62
- Detik 13: Genap, turun 7 -> 62 - 7 = 55
- Detik 14: Ganjil, naik 3 -> 55 + 3 = 58
- Detik 15: Genap, turun 7 -> 58 - 7 = 51
- Detik 16: Ganjil, naik 3 -> 51 + 3 = 54
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 43: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 76**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[23, 8, 6, 4, 5]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 34."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 3 pasang
C. 2 pasang
D. 0 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 23 + Sapi 8 = 31 (❌ Gagal)
- Sapi 23 + Sapi 6 = 29 (❌ Gagal)
- Sapi 23 + Sapi 4 = 27 (❌ Gagal)
- Sapi 23 + Sapi 5 = 28 (❌ Gagal)
- Sapi 8 + Sapi 6 = 14 (❌ Gagal)
- Sapi 8 + Sapi 4 = 12 (❌ Gagal)
- Sapi 8 + Sapi 5 = 13 (❌ Gagal)
- Sapi 6 + Sapi 4 = 10 (❌ Gagal)
- Sapi 6 + Sapi 5 = 11 (❌ Gagal)
- Sapi 4 + Sapi 5 = 9 (❌ Gagal)

Total pasangan yang bernilai 34 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 77**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[20, 7, 13, 11, 10]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 30."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 4 pasang
B. 0 pasang
C. 2 pasang
D. 1 pasang
E. 3 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 20 + Sapi 7 = 27 (❌ Gagal)
- Sapi 20 + Sapi 13 = 33 (❌ Gagal)
- Sapi 20 + Sapi 11 = 31 (❌ Gagal)
- Sapi 20 + Sapi 10 = 30 (✅ COCOK)
- Sapi 7 + Sapi 13 = 20 (❌ Gagal)
- Sapi 7 + Sapi 11 = 18 (❌ Gagal)
- Sapi 7 + Sapi 10 = 17 (❌ Gagal)
- Sapi 13 + Sapi 11 = 24 (❌ Gagal)
- Sapi 13 + Sapi 10 = 23 (❌ Gagal)
- Sapi 11 + Sapi 10 = 21 (❌ Gagal)

Total pasangan yang bernilai 30 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 78**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[3, 7, 24, 11, 16]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 33."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 1 pasang
B. 4 pasang
C. 0 pasang
D. 3 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: C (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 3 + Sapi 7 = 10 (❌ Gagal)
- Sapi 3 + Sapi 24 = 27 (❌ Gagal)
- Sapi 3 + Sapi 11 = 14 (❌ Gagal)
- Sapi 3 + Sapi 16 = 19 (❌ Gagal)
- Sapi 7 + Sapi 24 = 31 (❌ Gagal)
- Sapi 7 + Sapi 11 = 18 (❌ Gagal)
- Sapi 7 + Sapi 16 = 23 (❌ Gagal)
- Sapi 24 + Sapi 11 = 35 (❌ Gagal)
- Sapi 24 + Sapi 16 = 40 (❌ Gagal)
- Sapi 11 + Sapi 16 = 27 (❌ Gagal)

Total pasangan yang bernilai 33 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 79**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[22, 5, 13, 9, 23]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 42."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 2 pasang
C. 3 pasang
D. 4 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: A (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 22 + Sapi 5 = 27 (❌ Gagal)
- Sapi 22 + Sapi 13 = 35 (❌ Gagal)
- Sapi 22 + Sapi 9 = 31 (❌ Gagal)
- Sapi 22 + Sapi 23 = 45 (❌ Gagal)
- Sapi 5 + Sapi 13 = 18 (❌ Gagal)
- Sapi 5 + Sapi 9 = 14 (❌ Gagal)
- Sapi 5 + Sapi 23 = 28 (❌ Gagal)
- Sapi 13 + Sapi 9 = 22 (❌ Gagal)
- Sapi 13 + Sapi 23 = 36 (❌ Gagal)
- Sapi 9 + Sapi 23 = 32 (❌ Gagal)

Total pasangan yang bernilai 42 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 80**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[9, 4, 14, 12, 21]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 39."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 3 pasang
C. 1 pasang
D. 4 pasang
E. 0 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 9 + Sapi 4 = 13 (❌ Gagal)
- Sapi 9 + Sapi 14 = 23 (❌ Gagal)
- Sapi 9 + Sapi 12 = 21 (❌ Gagal)
- Sapi 9 + Sapi 21 = 30 (❌ Gagal)
- Sapi 4 + Sapi 14 = 18 (❌ Gagal)
- Sapi 4 + Sapi 12 = 16 (❌ Gagal)
- Sapi 4 + Sapi 21 = 25 (❌ Gagal)
- Sapi 14 + Sapi 12 = 26 (❌ Gagal)
- Sapi 14 + Sapi 21 = 35 (❌ Gagal)
- Sapi 12 + Sapi 21 = 33 (❌ Gagal)

Total pasangan yang bernilai 39 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 81**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SSSSSUBS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 7 unit langkah
C. 6 unit langkah
D. 8 unit langkah
E. 5 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: C (6 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`S`): Koordinat kini `(0, -2)`
- Instruksi 3 (`S`): Koordinat kini `(0, -3)`
- Instruksi 4 (`S`): Koordinat kini `(0, -4)`
- Instruksi 5 (`S`): Koordinat kini `(0, -5)`
- Instruksi 6 (`U`): Koordinat kini `(0, -4)`
- Instruksi 7 (`B`): Koordinat kini `(-1, -4)`
- Instruksi 8 (`S`): Koordinat kini `(-1, -5)`

Posisi akhir robot adalah di titik `(-1, -5)`.
Jarak Manhattan = Murni $|-1| + |-5|$ = 1 + 5 = **6 unit**.
Opsi valid: **C**.</details>

---
**Soal 82**
Sebuah robot bola diletakkan di lantai 113. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 30 detik
B. 33 detik
C. 32 detik
D. 29 detik
E. 31 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (30 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 113 (Garis Start)
- Detik 1: Ganjil, naik 5 -> 113 + 5 = 118
- Detik 2: Genap, turun 13 -> 118 - 13 = 105
- Detik 3: Ganjil, naik 5 -> 105 + 5 = 110
- Detik 4: Genap, turun 13 -> 110 - 13 = 97
- Detik 5: Ganjil, naik 5 -> 97 + 5 = 102
- Detik 6: Genap, turun 13 -> 102 - 13 = 89
- Detik 7: Ganjil, naik 5 -> 89 + 5 = 94
- Detik 8: Genap, turun 13 -> 94 - 13 = 81
- Detik 9: Ganjil, naik 5 -> 81 + 5 = 86
- Detik 10: Genap, turun 13 -> 86 - 13 = 73
- Detik 11: Ganjil, naik 5 -> 73 + 5 = 78
- Detik 12: Genap, turun 13 -> 78 - 13 = 65
- Detik 13: Ganjil, naik 5 -> 65 + 5 = 70
- Detik 14: Genap, turun 13 -> 70 - 13 = 57
- Detik 15: Ganjil, naik 5 -> 57 + 5 = 62
- Detik 16: Genap, turun 13 -> 62 - 13 = 49
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 30: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 83**
Sebuah robot bola diletakkan di lantai 94. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 49 detik
B. 46 detik
C. 47 detik
D. 50 detik
E. 48 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (47 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 94 (Garis Start)
- Detik 1: Genap, turun 7 -> 94 - 7 = 87
- Detik 2: Ganjil, naik 3 -> 87 + 3 = 90
- Detik 3: Genap, turun 7 -> 90 - 7 = 83
- Detik 4: Ganjil, naik 3 -> 83 + 3 = 86
- Detik 5: Genap, turun 7 -> 86 - 7 = 79
- Detik 6: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 7: Genap, turun 7 -> 82 - 7 = 75
- Detik 8: Ganjil, naik 3 -> 75 + 3 = 78
- Detik 9: Genap, turun 7 -> 78 - 7 = 71
- Detik 10: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 11: Genap, turun 7 -> 74 - 7 = 67
- Detik 12: Ganjil, naik 3 -> 67 + 3 = 70
- Detik 13: Genap, turun 7 -> 70 - 7 = 63
- Detik 14: Ganjil, naik 3 -> 63 + 3 = 66
- Detik 15: Genap, turun 7 -> 66 - 7 = 59
- Detik 16: Ganjil, naik 3 -> 59 + 3 = 62
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 47: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 84**
Sebuah robot bola diletakkan di lantai 99. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 56 detik
B. 55 detik
C. 58 detik
D. 57 detik
E. 59 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: A (56 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 99 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 99 + 3 = 102
- Detik 2: Genap, turun 7 -> 102 - 7 = 95
- Detik 3: Ganjil, naik 3 -> 95 + 3 = 98
- Detik 4: Genap, turun 7 -> 98 - 7 = 91
- Detik 5: Ganjil, naik 3 -> 91 + 3 = 94
- Detik 6: Genap, turun 7 -> 94 - 7 = 87
- Detik 7: Ganjil, naik 3 -> 87 + 3 = 90
- Detik 8: Genap, turun 7 -> 90 - 7 = 83
- Detik 9: Ganjil, naik 3 -> 83 + 3 = 86
- Detik 10: Genap, turun 7 -> 86 - 7 = 79
- Detik 11: Ganjil, naik 3 -> 79 + 3 = 82
- Detik 12: Genap, turun 7 -> 82 - 7 = 75
- Detik 13: Ganjil, naik 3 -> 75 + 3 = 78
- Detik 14: Genap, turun 7 -> 78 - 7 = 71
- Detik 15: Ganjil, naik 3 -> 71 + 3 = 74
- Detik 16: Genap, turun 7 -> 74 - 7 = 67
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 56: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 85**
Sebuah robot bola diletakkan di lantai 126. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 9 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 32 detik
B. 33 detik
C. 31 detik
D. 34 detik
E. 30 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (31 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 126 (Garis Start)
- Detik 1: Genap, turun 9 -> 126 - 9 = 117
- Detik 2: Ganjil, naik 1 -> 117 + 1 = 118
- Detik 3: Genap, turun 9 -> 118 - 9 = 109
- Detik 4: Ganjil, naik 1 -> 109 + 1 = 110
- Detik 5: Genap, turun 9 -> 110 - 9 = 101
- Detik 6: Ganjil, naik 1 -> 101 + 1 = 102
- Detik 7: Genap, turun 9 -> 102 - 9 = 93
- Detik 8: Ganjil, naik 1 -> 93 + 1 = 94
- Detik 9: Genap, turun 9 -> 94 - 9 = 85
- Detik 10: Ganjil, naik 1 -> 85 + 1 = 86
- Detik 11: Genap, turun 9 -> 86 - 9 = 77
- Detik 12: Ganjil, naik 1 -> 77 + 1 = 78
- Detik 13: Genap, turun 9 -> 78 - 9 = 69
- Detik 14: Ganjil, naik 1 -> 69 + 1 = 70
- Detik 15: Genap, turun 9 -> 70 - 9 = 61
- Detik 16: Ganjil, naik 1 -> 61 + 1 = 62
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 31: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 86**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[4, 12, 3, 13, 14]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 37."*

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
- Sapi 4 + Sapi 12 = 16 (❌ Gagal)
- Sapi 4 + Sapi 3 = 7 (❌ Gagal)
- Sapi 4 + Sapi 13 = 17 (❌ Gagal)
- Sapi 4 + Sapi 14 = 18 (❌ Gagal)
- Sapi 12 + Sapi 3 = 15 (❌ Gagal)
- Sapi 12 + Sapi 13 = 25 (❌ Gagal)
- Sapi 12 + Sapi 14 = 26 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 3 + Sapi 14 = 17 (❌ Gagal)
- Sapi 13 + Sapi 14 = 27 (❌ Gagal)

Total pasangan yang bernilai 37 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 87**
Sebuah robot bola diletakkan di lantai 72. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 13 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 5 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai 0 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 20 detik
B. 19 detik
C. 16 detik
D. 17 detik
E. 18 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (17 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 72 (Garis Start)
- Detik 1: Genap, turun 13 -> 72 - 13 = 59
- Detik 2: Ganjil, naik 5 -> 59 + 5 = 64
- Detik 3: Genap, turun 13 -> 64 - 13 = 51
- Detik 4: Ganjil, naik 5 -> 51 + 5 = 56
- Detik 5: Genap, turun 13 -> 56 - 13 = 43
- Detik 6: Ganjil, naik 5 -> 43 + 5 = 48
- Detik 7: Genap, turun 13 -> 48 - 13 = 35
- Detik 8: Ganjil, naik 5 -> 35 + 5 = 40
- Detik 9: Genap, turun 13 -> 40 - 13 = 27
- Detik 10: Ganjil, naik 5 -> 27 + 5 = 32
- Detik 11: Genap, turun 13 -> 32 - 13 = 19
- Detik 12: Ganjil, naik 5 -> 19 + 5 = 24
- Detik 13: Genap, turun 13 -> 24 - 13 = 11
- Detik 14: Ganjil, naik 5 -> 11 + 5 = 16
- Detik 15: Genap, turun 13 -> 16 - 13 = 3
- Detik 16: Ganjil, naik 5 -> 3 + 5 = 8
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 17: Menyentuh batas lantai <= 0. Selesai.
</details>

---
**Soal 88**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[7, 21, 16, 20, 15]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 31."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 1 pasang
C. 4 pasang
D. 0 pasang
E. 2 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 7 + Sapi 21 = 28 (❌ Gagal)
- Sapi 7 + Sapi 16 = 23 (❌ Gagal)
- Sapi 7 + Sapi 20 = 27 (❌ Gagal)
- Sapi 7 + Sapi 15 = 22 (❌ Gagal)
- Sapi 21 + Sapi 16 = 37 (❌ Gagal)
- Sapi 21 + Sapi 20 = 41 (❌ Gagal)
- Sapi 21 + Sapi 15 = 36 (❌ Gagal)
- Sapi 16 + Sapi 20 = 36 (❌ Gagal)
- Sapi 16 + Sapi 15 = 31 (✅ COCOK)
- Sapi 20 + Sapi 15 = 35 (❌ Gagal)

Total pasangan yang bernilai 31 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
**Soal 89**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `SUUUUTUTTSSTSS`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 4 unit langkah
B. 5 unit langkah
C. 6 unit langkah
D. 3 unit langkah
E. 2 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: A (4 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`S`): Koordinat kini `(0, -1)`
- Instruksi 2 (`U`): Koordinat kini `(0, 0)`
- Instruksi 3 (`U`): Koordinat kini `(0, 1)`
- Instruksi 4 (`U`): Koordinat kini `(0, 2)`
- Instruksi 5 (`U`): Koordinat kini `(0, 3)`
- Instruksi 6 (`T`): Koordinat kini `(1, 3)`
- Instruksi 7 (`U`): Koordinat kini `(1, 4)`
- Instruksi 8 (`T`): Koordinat kini `(2, 4)`
- Instruksi 9 (`T`): Koordinat kini `(3, 4)`
- Instruksi 10 (`S`): Koordinat kini `(3, 3)`
- Instruksi 11 (`S`): Koordinat kini `(3, 2)`
- Instruksi 12 (`T`): Koordinat kini `(4, 2)`
- Instruksi 13 (`S`): Koordinat kini `(4, 1)`
- Instruksi 14 (`S`): Koordinat kini `(4, 0)`

Posisi akhir robot adalah di titik `(4, 0)`.
Jarak Manhattan = Murni $|4| + |0|$ = 4 + 0 = **4 unit**.
Opsi valid: **A**.</details>

---
**Soal 90**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[17, 7, 14, 11, 16]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 25."*

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
- Sapi 17 + Sapi 7 = 24 (❌ Gagal)
- Sapi 17 + Sapi 14 = 31 (❌ Gagal)
- Sapi 17 + Sapi 11 = 28 (❌ Gagal)
- Sapi 17 + Sapi 16 = 33 (❌ Gagal)
- Sapi 7 + Sapi 14 = 21 (❌ Gagal)
- Sapi 7 + Sapi 11 = 18 (❌ Gagal)
- Sapi 7 + Sapi 16 = 23 (❌ Gagal)
- Sapi 14 + Sapi 11 = 25 (✅ COCOK)
- Sapi 14 + Sapi 16 = 30 (❌ Gagal)
- Sapi 11 + Sapi 16 = 27 (❌ Gagal)

Total pasangan yang bernilai 25 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **C**.</details>

---
**Soal 91**
Sebuah robot bola diletakkan di lantai 93. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 3 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -5 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 27 detik
B. 25 detik
C. 26 detik
D. 28 detik
E. 29 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: C (26 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 93 (Garis Start)
- Detik 1: Ganjil, naik 3 -> 93 + 3 = 96
- Detik 2: Genap, turun 11 -> 96 - 11 = 85
- Detik 3: Ganjil, naik 3 -> 85 + 3 = 88
- Detik 4: Genap, turun 11 -> 88 - 11 = 77
- Detik 5: Ganjil, naik 3 -> 77 + 3 = 80
- Detik 6: Genap, turun 11 -> 80 - 11 = 69
- Detik 7: Ganjil, naik 3 -> 69 + 3 = 72
- Detik 8: Genap, turun 11 -> 72 - 11 = 61
- Detik 9: Ganjil, naik 3 -> 61 + 3 = 64
- Detik 10: Genap, turun 11 -> 64 - 11 = 53
- Detik 11: Ganjil, naik 3 -> 53 + 3 = 56
- Detik 12: Genap, turun 11 -> 56 - 11 = 45
- Detik 13: Ganjil, naik 3 -> 45 + 3 = 48
- Detik 14: Genap, turun 11 -> 48 - 11 = 37
- Detik 15: Ganjil, naik 3 -> 37 + 3 = 40
- Detik 16: Genap, turun 11 -> 40 - 11 = 29
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 26: Menyentuh batas lantai <= -5. Selesai.
</details>

---
**Soal 92**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[17, 9, 7, 8, 12]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 38."*

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
- Sapi 17 + Sapi 9 = 26 (❌ Gagal)
- Sapi 17 + Sapi 7 = 24 (❌ Gagal)
- Sapi 17 + Sapi 8 = 25 (❌ Gagal)
- Sapi 17 + Sapi 12 = 29 (❌ Gagal)
- Sapi 9 + Sapi 7 = 16 (❌ Gagal)
- Sapi 9 + Sapi 8 = 17 (❌ Gagal)
- Sapi 9 + Sapi 12 = 21 (❌ Gagal)
- Sapi 7 + Sapi 8 = 15 (❌ Gagal)
- Sapi 7 + Sapi 12 = 19 (❌ Gagal)
- Sapi 8 + Sapi 12 = 20 (❌ Gagal)

Total pasangan yang bernilai 38 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 93**
Sebuah robot bola diletakkan di lantai 149. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 11 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 34 detik
B. 31 detik
C. 35 detik
D. 32 detik
E. 33 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: D (32 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 149 (Garis Start)
- Detik 1: Ganjil, naik 1 -> 149 + 1 = 150
- Detik 2: Genap, turun 11 -> 150 - 11 = 139
- Detik 3: Ganjil, naik 1 -> 139 + 1 = 140
- Detik 4: Genap, turun 11 -> 140 - 11 = 129
- Detik 5: Ganjil, naik 1 -> 129 + 1 = 130
- Detik 6: Genap, turun 11 -> 130 - 11 = 119
- Detik 7: Ganjil, naik 1 -> 119 + 1 = 120
- Detik 8: Genap, turun 11 -> 120 - 11 = 109
- Detik 9: Ganjil, naik 1 -> 109 + 1 = 110
- Detik 10: Genap, turun 11 -> 110 - 11 = 99
- Detik 11: Ganjil, naik 1 -> 99 + 1 = 100
- Detik 12: Genap, turun 11 -> 100 - 11 = 89
- Detik 13: Ganjil, naik 1 -> 89 + 1 = 90
- Detik 14: Genap, turun 11 -> 90 - 11 = 79
- Detik 15: Ganjil, naik 1 -> 79 + 1 = 80
- Detik 16: Genap, turun 11 -> 80 - 11 = 69
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 32: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 94**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[20, 19, 8, 10, 24]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

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
- Sapi 20 + Sapi 19 = 39 (❌ Gagal)
- Sapi 20 + Sapi 8 = 28 (❌ Gagal)
- Sapi 20 + Sapi 10 = 30 (❌ Gagal)
- Sapi 20 + Sapi 24 = 44 (❌ Gagal)
- Sapi 19 + Sapi 8 = 27 (❌ Gagal)
- Sapi 19 + Sapi 10 = 29 (✅ COCOK)
- Sapi 19 + Sapi 24 = 43 (❌ Gagal)
- Sapi 8 + Sapi 10 = 18 (❌ Gagal)
- Sapi 8 + Sapi 24 = 32 (❌ Gagal)
- Sapi 10 + Sapi 24 = 34 (❌ Gagal)

Total pasangan yang bernilai 29 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 95**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[21, 16, 12, 8, 6]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 47."*

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
- Sapi 21 + Sapi 16 = 37 (❌ Gagal)
- Sapi 21 + Sapi 12 = 33 (❌ Gagal)
- Sapi 21 + Sapi 8 = 29 (❌ Gagal)
- Sapi 21 + Sapi 6 = 27 (❌ Gagal)
- Sapi 16 + Sapi 12 = 28 (❌ Gagal)
- Sapi 16 + Sapi 8 = 24 (❌ Gagal)
- Sapi 16 + Sapi 6 = 22 (❌ Gagal)
- Sapi 12 + Sapi 8 = 20 (❌ Gagal)
- Sapi 12 + Sapi 6 = 18 (❌ Gagal)
- Sapi 8 + Sapi 6 = 14 (❌ Gagal)

Total pasangan yang bernilai 47 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **A**.</details>

---
**Soal 96**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[19, 23, 17, 7, 22]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 29."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 0 pasang
B. 4 pasang
C. 2 pasang
D. 3 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: E (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 19 + Sapi 23 = 42 (❌ Gagal)
- Sapi 19 + Sapi 17 = 36 (❌ Gagal)
- Sapi 19 + Sapi 7 = 26 (❌ Gagal)
- Sapi 19 + Sapi 22 = 41 (❌ Gagal)
- Sapi 23 + Sapi 17 = 40 (❌ Gagal)
- Sapi 23 + Sapi 7 = 30 (❌ Gagal)
- Sapi 23 + Sapi 22 = 45 (❌ Gagal)
- Sapi 17 + Sapi 7 = 24 (❌ Gagal)
- Sapi 17 + Sapi 22 = 39 (❌ Gagal)
- Sapi 7 + Sapi 22 = 29 (✅ COCOK)

Total pasangan yang bernilai 29 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **E**.</details>

---
**Soal 97**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[14, 3, 13, 15, 19]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 34."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 2 pasang
B. 0 pasang
C. 3 pasang
D. 1 pasang
E. 4 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: D (1 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 14 + Sapi 3 = 17 (❌ Gagal)
- Sapi 14 + Sapi 13 = 27 (❌ Gagal)
- Sapi 14 + Sapi 15 = 29 (❌ Gagal)
- Sapi 14 + Sapi 19 = 33 (❌ Gagal)
- Sapi 3 + Sapi 13 = 16 (❌ Gagal)
- Sapi 3 + Sapi 15 = 18 (❌ Gagal)
- Sapi 3 + Sapi 19 = 22 (❌ Gagal)
- Sapi 13 + Sapi 15 = 28 (❌ Gagal)
- Sapi 13 + Sapi 19 = 32 (❌ Gagal)
- Sapi 15 + Sapi 19 = 34 (✅ COCOK)

Total pasangan yang bernilai 34 murni ada **1 pasang**.
Oleh karena itu opsi yang tepat adalah **D**.</details>

---
**Soal 98**
Sebuah robot bola diletakkan di lantai 150. Aturan pergerakan robot setiap detiknya adalah sebagai berikut:
- Jika posisi lantai saat ini bernilai GENAP, bola akan anjlok turun 7 lantai.
- Jika posisi lantai saat ini bernilai GANJIL, bola akan memantul naik 1 lantai.
Robot akan otomatis mati (berhenti bergerak) begitu menyentuh lantai -10 atau lebih bawah dari itu.
Berapa detik waktu yang dibutuhkan hingga robot tersebut mati?

A. 56 detik
B. 53 detik
C. 54 detik
D. 55 detik
E. 52 detik

<details>
<summary><b>Klik untuk melihat kunci jawaban & pembahasan Tracing Simulasi</b></summary>

**Jawaban: B (53 detik)**

**Pembahasan (Simulasi Manual "Compiler Manusia"):**
Kita lacak pergerakan state `Detik` dan `Posisi` dari awal:
- Detik 0: Posisi = 150 (Garis Start)
- Detik 1: Genap, turun 7 -> 150 - 7 = 143
- Detik 2: Ganjil, naik 1 -> 143 + 1 = 144
- Detik 3: Genap, turun 7 -> 144 - 7 = 137
- Detik 4: Ganjil, naik 1 -> 137 + 1 = 138
- Detik 5: Genap, turun 7 -> 138 - 7 = 131
- Detik 6: Ganjil, naik 1 -> 131 + 1 = 132
- Detik 7: Genap, turun 7 -> 132 - 7 = 125
- Detik 8: Ganjil, naik 1 -> 125 + 1 = 126
- Detik 9: Genap, turun 7 -> 126 - 7 = 119
- Detik 10: Ganjil, naik 1 -> 119 + 1 = 120
- Detik 11: Genap, turun 7 -> 120 - 7 = 113
- Detik 12: Ganjil, naik 1 -> 113 + 1 = 114
- Detik 13: Genap, turun 7 -> 114 - 7 = 107
- Detik 14: Ganjil, naik 1 -> 107 + 1 = 108
- Detik 15: Genap, turun 7 -> 108 - 7 = 101
- Detik 16: Ganjil, naik 1 -> 101 + 1 = 102
... (Simulasi berlanjut mencetak pola yang sama menurun)
- Detik 53: Menyentuh batas lantai <= -10. Selesai.
</details>

---
**Soal 99**
Sebuah robot mainan Koko mendarat di titik kordinat `(0,0)`. Robot tersebut dikendalikan menggunakan remote control yang hanya mengirimkan instruksi teks satu karakter:
- `U` (Utara): Maju sumbu Y (+1)
- `S` (Selatan): Mundur sumbu Y (-1)
- `T` (Timur): Geser sumbu X (+1)
- `B` (Barat): Geser sumbu X (-1)

Robot menerima sejarah *log* instruksi beruntun: `BUTBBSUUT`.
Berapa jarak Manhattan mutlak (Total jarak langkah minimum tanpa diagonal: $|X| + |Y|$) dari Posisi Start ke Titik Berhenti robot tersebut?

A. 5 unit langkah
B. 4 unit langkah
C. 2 unit langkah
D. 1 unit langkah
E. 3 unit langkah

<details>
<summary><b>Klik untuk melihat kunci jawaban & Tracing Matriks 2D</b></summary>

**Jawaban: E (3 unit langkah)**

**Pembahasan (Simulasi Vektor Matriks O(N)):**
Mari kita lacak *State* mesin robot huruf demi huruf:
- Awal: X=0, Y=0
- Instruksi 1 (`B`): Koordinat kini `(-1, 0)`
- Instruksi 2 (`U`): Koordinat kini `(-1, 1)`
- Instruksi 3 (`T`): Koordinat kini `(0, 1)`
- Instruksi 4 (`B`): Koordinat kini `(-1, 1)`
- Instruksi 5 (`B`): Koordinat kini `(-2, 1)`
- Instruksi 6 (`S`): Koordinat kini `(-2, 0)`
- Instruksi 7 (`U`): Koordinat kini `(-2, 1)`
- Instruksi 8 (`U`): Koordinat kini `(-2, 2)`
- Instruksi 9 (`T`): Koordinat kini `(-1, 2)`

Posisi akhir robot adalah di titik `(-1, 2)`.
Jarak Manhattan = Murni $|-1| + |2|$ = 1 + 2 = **3 unit**.
Opsi valid: **E**.</details>

---
**Soal 100**
Pak Dengklek memiliki 5 ekor sapi pemerah susu bernomor dada: `[16, 8, 11, 5, 13]`.
Pak Dengklek memberikan instruksi kepada mesin pemerah: *"Tarik masuk DUA EKOR sapi berbeda sekaligus yang jika dijumlahkan nomor dadanya bernilai tepat 46."*

Berapa total pasangan sapi yang sah memenuhi syarat tersebut menggunakan evaluasi kombinasi Brute-Force?

A. 3 pasang
B. 0 pasang
C. 4 pasang
D. 2 pasang
E. 1 pasang

<details>
<summary><b>Klik untuk melihat kunci jawaban & bedah iterasi Brute Force</b></summary>

**Jawaban: B (0 pasang)**

**Pembahasan (Mengecek Semua Kemungkinan Nested Loop O(N^2)):**
Mari kita jodohkan paksa setiap elemen secara *exhaustive search*:
- Sapi 16 + Sapi 8 = 24 (❌ Gagal)
- Sapi 16 + Sapi 11 = 27 (❌ Gagal)
- Sapi 16 + Sapi 5 = 21 (❌ Gagal)
- Sapi 16 + Sapi 13 = 29 (❌ Gagal)
- Sapi 8 + Sapi 11 = 19 (❌ Gagal)
- Sapi 8 + Sapi 5 = 13 (❌ Gagal)
- Sapi 8 + Sapi 13 = 21 (❌ Gagal)
- Sapi 11 + Sapi 5 = 16 (❌ Gagal)
- Sapi 11 + Sapi 13 = 24 (❌ Gagal)
- Sapi 5 + Sapi 13 = 18 (❌ Gagal)

Total pasangan yang bernilai 46 murni ada **0 pasang**.
Oleh karena itu opsi yang tepat adalah **B**.</details>

---
