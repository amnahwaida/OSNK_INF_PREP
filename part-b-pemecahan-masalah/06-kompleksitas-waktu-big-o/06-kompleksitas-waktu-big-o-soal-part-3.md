🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal: Time Complexity Big O (Part 3 / 6)

Berikut adalah masterclass bank soal simulasi OSN-K untuk materi **Time Complexity Big O**. Pastikan melacaknya dengan ketelitian Compiler Manusia!

---

**Soal 101**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(log N) Sang Penebas
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(N) Sang Pejalan Kaki
D. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
E. Mutlak menggunakan O(1) Sang Instan Mutlak

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: C (Mutlak menggunakan O(N) Sang Pejalan Kaki)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000**, maka:
N = 1.000.000 mentok mentok cuma bisa diproses Loop Tunggal.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N) Sang Pejalan Kaki**. Opsi tervalid: **C**.
</details>

---
**Soal 102**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
B. Mutlak menggunakan O(N) Sang Pejalan Kaki
C. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
D. Mutlak menggunakan O(log N) Sang Penebas
E. Mutlak menggunakan O(1) Sang Instan Mutlak

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: A (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **A**.
</details>

---
**Soal 103**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 5;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(N)
C. O(2^N)
D. O(N^2)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **B**.
</details>

---
**Soal 104**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(N^2)
C. O(2^N)
D. O(1)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **E**.
</details>

---
**Soal 105**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 2;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(1)
C. O(N^2)
D. O(N log N)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **E**.
</details>

---
**Soal 106**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(log N) Sang Penebas
B. Mutlak menggunakan O(N) Sang Pejalan Kaki
C. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
D. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
E. Mutlak menggunakan O(1) Sang Instan Mutlak

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: B (Mutlak menggunakan O(N) Sang Pejalan Kaki)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000**, maka:
N = 1.000.000 mentok mentok cuma bisa diproses Loop Tunggal.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N) Sang Pejalan Kaki**. Opsi tervalid: **B**.
</details>

---
**Soal 107**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(log N)
C. O(1)
D. O(N)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **B**.
</details>

---
**Soal 108**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N) Sang Pejalan Kaki
B. Mutlak menggunakan O(1) Sang Instan Mutlak
C. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
D. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
E. Mutlak menggunakan O(log N) Sang Penebas

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: C (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **C**.
</details>

---
**Soal 109**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N^2)
B. O(N)
C. O(log N)
D. O(1)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: A (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **A**.
</details>

---
**Soal 110**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(N^2)
C. O(N)
D. O(log N)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **B**.
</details>

---
**Soal 111**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 3;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(log N)
C. O(N)
D. O(N log N)
E. O(N^2)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **C**.
</details>

---
**Soal 112**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 3;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(N^2)
C. O(N)
D. O(1)
E. O(log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **C**.
</details>

---
**Soal 113**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(N)
C. O(N^2)
D. O(2^N)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **B**.
</details>

---
**Soal 114**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N) Sang Pejalan Kaki
B. Mutlak menggunakan O(log N) Sang Penebas
C. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
D. Mutlak menggunakan O(1) Sang Instan Mutlak
E. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: E (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **E**.
</details>

---
**Soal 115**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(1)
C. O(log N)
D. O(N log N)
E. O(N^2)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **E**.
</details>

---
**Soal 116**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(2^N)
C. O(log N)
D. O(N^2)
E. O(1)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: D (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **D**.
</details>

---
**Soal 117**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N)
B. O(N^2)
C. O(N log N)
D. O(2^N)
E. O(log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **B**.
</details>

---
**Soal 118**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(1)
C. O(N)
D. O(2^N)
E. O(log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **C**.
</details>

---
**Soal 119**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(1)
C. O(N^2)
D. O(N)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: D (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **D**.
</details>

---
**Soal 120**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(log N)
C. O(N log N)
D. O(N^2)
E. O(1)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **B**.
</details>

---
**Soal 121**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(N log N)
C. O(N^2)
D. O(log N)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: D (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **D**.
</details>

---
**Soal 122**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N)
B. O(N^2)
C. O(log N)
D. O(N log N)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **C**.
</details>

---
**Soal 123**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(1) Sang Instan Mutlak
D. Mutlak menggunakan O(log N) Sang Penebas
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: B (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **B**.
</details>

---
**Soal 124**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 20`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(log N) Sang Penebas
B. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
C. Mutlak menggunakan O(1) Sang Instan Mutlak
D. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: B (Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 20**, maka:
N super mikroskopis = 20 ini dirancang sengaja untuk di-Brute Force rekursi penuh.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(2^N) Sang Kiamat Eksponensial**. Opsi tervalid: **B**.
</details>

---
**Soal 125**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(1) Sang Instan Mutlak
D. Mutlak menggunakan O(log N) Sang Penebas
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: E (Mutlak menggunakan O(N) Sang Pejalan Kaki)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000**, maka:
N = 1.000.000 mentok mentok cuma bisa diproses Loop Tunggal.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N) Sang Pejalan Kaki**. Opsi tervalid: **E**.
</details>

---
**Soal 126**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(N log N)
C. O(1)
D. O(N^2)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **E**.
</details>

---
**Soal 127**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(N^2)
C. O(log N)
D. O(N log N)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **C**.
</details>

---
**Soal 128**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(1) Sang Instan Mutlak
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(N) Sang Pejalan Kaki
D. Mutlak menggunakan O(log N) Sang Penebas
E. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: B (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **B**.
</details>

---
**Soal 129**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(N)
C. O(N^2)
D. O(1)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **C**.
</details>

---
**Soal 130**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 2;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N^2)
B. O(log N)
C. O(2^N)
D. O(1)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **E**.
</details>

---
**Soal 131**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(1) Sang Instan Mutlak
B. Mutlak menggunakan O(log N) Sang Penebas
C. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
D. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: A (Mutlak menggunakan O(1) Sang Instan Mutlak)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000000**, maka:
N = 1 Miliar itu gila! Mana mungkin dilooping manual di kertas? Ini pasti jebakan rumus matematika konstan mutlak murni.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(1) Sang Instan Mutlak**. Opsi tervalid: **A**.
</details>

---
**Soal 132**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 3;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(2^N)
C. O(N)
D. O(1)
E. O(N^2)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **C**.
</details>

---
**Soal 133**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 20`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(log N) Sang Penebas
D. Mutlak menggunakan O(1) Sang Instan Mutlak
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: A (Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 20**, maka:
N super mikroskopis = 20 ini dirancang sengaja untuk di-Brute Force rekursi penuh.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(2^N) Sang Kiamat Eksponensial**. Opsi tervalid: **A**.
</details>

---
**Soal 134**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N) Sang Pejalan Kaki
B. Mutlak menggunakan O(log N) Sang Penebas
C. Mutlak menggunakan O(1) Sang Instan Mutlak
D. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
E. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: C (Mutlak menggunakan O(1) Sang Instan Mutlak)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000000**, maka:
N = 1 Miliar itu gila! Mana mungkin dilooping manual di kertas? Ini pasti jebakan rumus matematika konstan mutlak murni.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(1) Sang Instan Mutlak**. Opsi tervalid: **C**.
</details>

---
**Soal 135**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(N^2)
C. O(N)
D. O(N log N)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: A (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **A**.
</details>

---
**Soal 136**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 5;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(N)
C. O(2^N)
D. O(1)
E. O(N^2)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **B**.
</details>

---
**Soal 137**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
B. Mutlak menggunakan O(N) Sang Pejalan Kaki
C. Mutlak menggunakan O(log N) Sang Penebas
D. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
E. Mutlak menggunakan O(1) Sang Instan Mutlak

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: E (Mutlak menggunakan O(1) Sang Instan Mutlak)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000000**, maka:
N = 1 Miliar itu gila! Mana mungkin dilooping manual di kertas? Ini pasti jebakan rumus matematika konstan mutlak murni.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(1) Sang Instan Mutlak**. Opsi tervalid: **E**.
</details>

---
**Soal 138**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 4;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(1)
C. O(log N)
D. O(N^2)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **E**.
</details>

---
**Soal 139**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N)
B. O(N^2)
C. O(log N)
D. O(2^N)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **B**.
</details>

---
**Soal 140**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N log N)
B. O(N^2)
C. O(log N)
D. O(1)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **B**.
</details>

---
**Soal 141**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(1) Sang Instan Mutlak
B. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
C. Mutlak menggunakan O(log N) Sang Penebas
D. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
E. Mutlak menggunakan O(N) Sang Pejalan Kaki

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: A (Mutlak menggunakan O(1) Sang Instan Mutlak)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000000**, maka:
N = 1 Miliar itu gila! Mana mungkin dilooping manual di kertas? Ini pasti jebakan rumus matematika konstan mutlak murni.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(1) Sang Instan Mutlak**. Opsi tervalid: **A**.
</details>

---
**Soal 142**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(N)
C. O(2^N)
D. O(N^2)
E. O(log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **E**.
</details>

---
**Soal 143**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 5000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
B. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
C. Mutlak menggunakan O(N) Sang Pejalan Kaki
D. Mutlak menggunakan O(1) Sang Instan Mutlak
E. Mutlak menggunakan O(log N) Sang Penebas

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: A (Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 5000**, maka:
N = 5000 dipangkat dua masih (25 Juta), amat sangat aman dieksekusi limit 100 Juta juri.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N^2) Sang Mimpi Buruk Kuadrat**. Opsi tervalid: **A**.
</details>

---
**Soal 144**
Dalam lembar soal OSN-K Provinsi, tertulis informasi batasan program:
- `Timer Eksekusi Juri: 1.0 Detik`.
- Rentang Nilai Masukan: `1 ≤ N ≤ 1000000`.

Sebagai "Compiler Manusia", insting batas **Kompleksitas Waktu Terlambat (Worst-Case Big O)** apa yang berani kamu ambil untuk merancang solusi tanpa takut meledak menabrak dinding TLE (Time Limit Exceeded)?

A. Mutlak menggunakan O(log N) Sang Penebas
B. Mutlak menggunakan O(N^2) Sang Mimpi Buruk Kuadrat
C. Mutlak menggunakan O(2^N) Sang Kiamat Eksponensial
D. Mutlak menggunakan O(N) Sang Pejalan Kaki
E. Mutlak menggunakan O(1) Sang Instan Mutlak

<details>
<summary><b>Klik untuk melihat kunci jawaban & Rahasia Rentang OSN</b></summary>

**Jawaban: D (Mutlak menggunakan O(N) Sang Pejalan Kaki)**

**Pembahasan (Hukum OSN-K 1 Detik = 10^8 Operasi):**
Patokan kaku dari Server Grader Olimpiade itu selalu konstan. Mereka hanya sanggup mengeksekusi $\approx 10^8$ perintah per detiknya.
Karena juri melemparkan beban nilai sejauh-jauhnya sampai **N = 1000000**, maka:
N = 1.000.000 mentok mentok cuma bisa diproses Loop Tunggal.

Membalap kenyataan tersebut, taktik membumi yang dijamin lolos aman adalah batas **O(N) Sang Pejalan Kaki**. Opsi tervalid: **D**.
</details>

---
**Soal 145**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  jawaban += 3;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(N)
B. O(log N)
C. O(N^2)
D. O(1)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: A (O(N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Ini adalah *Single Loop* biasa (Satu Lapis). Iterasi maju lurus persis sejalan dengan N. Pasti O(N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N)**. Opsi tervalid: **A**.
</details>

---
**Soal 146**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(log N)
C. O(N^2)
D. O(N)
E. O(2^N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **C**.
</details>

---
**Soal 147**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(1)
B. O(N log N)
C. O(log N)
D. O(2^N)
E. O(N^2)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: E (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **E**.
</details>

---
**Soal 148**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
for (int i = 1; i <= N; i++) {
  for (int x = 1; x <= i; x++) {
    bebek += 1;
  }
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(log N)
B. O(N)
C. O(N^2)
D. O(1)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: C (O(N^2))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Lihat ada *Nested Loop* (Loop di dalam Loop). Area hitungannya membentuk segitiga $N \times N / 2$, yang mengukuhkan takdir Kuadrat O(N^2).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(N^2)**. Opsi tervalid: **C**.
</details>

---
**Soal 149**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(log N)
C. O(1)
D. O(N^2)
E. O(N log N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: B (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **B**.
</details>

---
**Soal 150**
Diberikan potongan simulasi algoritma semu (*Pseudocode*) di kertas burammu sebagai berikut:

```cpp
int sisa = N;
while (sisa > 0) {
  sisa = sisa / 2;
  belah += 1;
}
```

Berapakah Kompleksitas Waktu Asimtotik (Notasi Big O) yang dianut oleh tulang punggung kode di atas?

A. O(2^N)
B. O(1)
C. O(N^2)
D. O(log N)
E. O(N)

<details>
<summary><b>Klik untuk melihat kunci jawaban & Bedah Anatomi Kode</b></summary>

**Jawaban: D (O(log N))**

**Pembahasan (Mendeteksi Kecepatan Loop):**
Sebagai *Compiler Manusia*, kita tak perlu mensimulasikan nilai aslinya, kita hanya membidik kecepatan kelipatan strukturnya.
Perhatikan operasi mutasinya! `sisa = sisa / 2`. Variabel menyusut dibagi separuh menyusut drastis membelah bumi setiap detiknya. Ini DNA dari O(log N).

Secara teknis teori Informatika, algoritma ini diklasifikasikan masuk ke dalam golongan **O(log N)**. Opsi tervalid: **D**.
</details>

---
