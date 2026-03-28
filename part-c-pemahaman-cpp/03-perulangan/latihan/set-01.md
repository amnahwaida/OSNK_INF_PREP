		🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal Part C - Modul 03 - Set 01 (Premium Edition)

> [!IMPORTANT]
> Fokus pada **Kondisi Berhenti** dan **Perubahan Variabel**. Ingat: Satu kesalahan kecil di `i++` bisa menyebabkan loop berjalan selamanya!

---

### Soal 1: Belajar Berhitung (Basic For Loop)
```cpp
// Skenario: Cetak angka 1 sampai 5
int total = 0;
for (int i = 1; i <= 5; i++) {
    total += i;
}
```
**Pertanyaan:**
1. Berapakah nilai `total` di akhir program?
2. Berapa kali blok di dalam `for` dieksekusi?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
Start --> Init["i = 1"]
Init --> Cond{"i <= 5?"}
Cond -- T --> Body["total += i"]
Body --> Inc["i++"]
Inc --> Cond
Cond -- F --> End
```

**Jawaban:**
1. **15** (1+2+3+4+5)
2. **5 kali**

**📖 Analisis Mendalam:**
Ini adalah struktur dasar loop `for`. Iterasi berhenti tepat saat `i` menjadi 6, karena kondisi `6 <= 5` bernilai false.
</details>

---

### Soal 2: Lari Keliling Lapangan (While Loop)
```cpp
// Skenario: Lari sampai lelah (energi habis)
int energi = 15;
int putaran = 0;

while (energi > 0) {
    energi -= 5;
    putaran++;
}
```
**Pertanyaan:**
1. Berapakah nilai `putaran` di akhir?
2. Berapakah nilai `energi` terakhir?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A{"energi > 0?"} -- T --> B["Energi - 5, Putaran + 1"]
B --> A
A -- F --> End
```

**Jawaban:**
1. **3**
2. **0**

**📖 Analisis Mendalam:**
Loop `while` mengecek kondisi di awal. Putaran terjadi 3 kali: (15->10, 10->5, 5->0). Saat energi 0, kondisi `0 > 0` salah, dan loop berhenti.
</details>

---

### Soal 3: ⚠️ Batas Tipis (Off-by-One Error)
```cpp
// Skenario: Cetak pesan 5 kali?
int count = 0;
for (int i = 0; i <= 5; i++) {
    count++;
}
```
**Pertanyaan:**
1. Berapakah nilai `count`?
2. Mengapa hasilnya bukan 5?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["i: 0, 1, 2, 3, 4, 5"] --> B["6 Iterasi"]
```

**Jawaban:**
1. **6**
2. Karena loop dimulai dari **0** dan berhenti di **<= 5** (inklusif).

**📖 Analisis Mendalam:**
Ini adalah jebakan klasik *Off-by-One*. Jika ingin 5 kali iterasi, gunakan `i < 5` (jika mulai dari 0) atau `i <= 5` (jika mulai dari 1).
</details>

---

### Soal 4: Hitung Mundur Roket (Decrement Loop)
```cpp
// Skenario: Countdown peluncuran
int t = 3;
while (t > 0) {
    t--;
}
// Di sini ada baris: t += 10;
```
**Pertanyaan:**
1. Berapakah nilai `t` tepat setelah loop selesai?
2. Berapakah nilai `t` di akhir seluruh program?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A{"3 > 0?"} -- T --> B["t = 2"]
B --> C{"2 > 0?"} -- T --> D["t = 1"]
D --> E{"1 > 0?"} -- T --> F["t = 0"]
F --> G{"0 > 0? (F)"} --> End
```

**Jawaban:**
1. **0**
2. **10**
</details>

---

### Soal 5: Pangkat Manual (Power Simulation)
```cpp
// Skenario: Hitung 2 pangkat 4
int basis = 2;
int hasil = 1;

for (int i = 0; i < 4; i++) {
    hasil *= basis;
}
```
**Pertanyaan:**
1. Berapakah nilai `hasil`?
2. Apa guna `i < 4` dalam konteks perpangkatan ini?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["1 * 2"] --> B["2 * 2"] --> C["4 * 2"] --> D["8 * 2"]
D --> E["16"]
```

**Jawaban:**
1. **16**
2. Sebagai penentu berapa kali perkalian dengan basis dilakukan (eksponen).
</details>

---

### Soal 6: Kelipatan Genap (Step Change)
```cpp
// Skenario: Jumlahkan angka genap 2 sampai 6
int jumlah = 0;
for (int i = 2; i <= 6; i += 2) {
    jumlah += i;
}
```
**Pertanyaan:**
1. Berapakah nilai `jumlah`?
2. Berapa kali variabel `i` diubah nilainya?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A["i = 2"] --> B["jumlah = 2"]
B --> C["i = 4"] --> D["jumlah = 6"]
D --> E["i = 6"] --> F["jumlah = 12"]
F --> G["i = 8 (Stop)"]
```

**Jawaban:**
1. **12** (2 + 4 + 6)
2. **3 kali** (menjadi 4, 6, lalu 8 untuk pengecekan gagal).
</details>

---

### Soal 7: Misteri ++i vs i++ (Prefix vs Postfix)
```cpp
// Skenario: Loop dengan increment berbeda
int a = 0, b = 0;

for (int i = 0; i < 3; i++) a++;
for (int j = 0; j < 3; ++j) b++;
```
**Pertanyaan:**
1. Berapakah nilai `a`?
2. Berapakah nilai `b`?
3. Apakah ada perbedaan hasil antara `i++` dan `++i` dalam bagian ketiga perintah `for`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Jawaban:**
1. **3**
2. **3**
3. **Tidak ada.** Di dalam header `for`, post-increment dan pre-increment memberikan hasil iterasi yang sama.

**📖 Analisis Mendalam:**
Meskipun secara teori `++i` sedikit lebih cepat, compiler modern memperlakukan keduanya secara identik di dalam struktur `for`. Keduanya akan melakukan penambahan **setelah** blok kode di dalam loop selesai dikerjakan.
</details>

---

### Soal 8: Tabungan Berlipat (Compound Interest)
```cpp
// Skenario: Uang 100rb, tiap tahun naik 10% (dibulatkan ke bawah)
int uang = 100000;
for (int thn = 0; thn < 2; thn++) {
    uang += uang / 10;
}
```
**Pertanyaan:**
1. Berapakah nilai `uang` setelah 2 tahun?
2. Apa yang membedakan tahun ke-1 dan tahun ke-2?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A["Start: 100k"] --> B["Thn 1: 100k + 10k = 110k"]
B --> C["Thn 2: 110k + 11k = 121k"]
```

**Jawaban:**
1. **121000**
2. Di tahun kedua, bunga 10% dihitung dari saldo yang sudah bertambah di tahun pertama (bunga berbunga).
</details>

---

### Soal 9: ⚠️ Loop Tanpa Henti? (Inversion Trap)
```cpp
// Skenario: Salah tanda di increment/decrement
int n = 5;
while (n < 10) {
    n--; // <-- Perhatikan ini!
    if (n < 0) break; // Penyelamat darurat
}
```
**Pertanyaan:**
1. Berapakah nilai `n` terakhir sebelum program berhenti?
2. Kenapa tanpa `break`, program ini akan menjadi *Infinite Loop*?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["5"] --> B["4"] --> C["3"] --> D["..."] --> E["-1 (Break!)"]
```

**Jawaban:**
1. **-1**
2. Karena `n` terus mengecil (menjauh dari angka 10), sehingga kondisi `n < 10` akan **selalu benar** selamanya.
</details>

---

### Soal 10: Pemecah Kelompok (Skip Multiples)
```cpp
// Skenario: Jumlahkan angka dari 1 ke 5, tapi lewatkan angka 3
int total = 0;
for (int i = 1; i <= 5; i++) {
    if (i != 3) {
        total += i;
    }
}
```
**Pertanyaan:**
1. Berapakah nilai `total`?
2. Rumus matematika apa yang setara dengan `total` tersebut?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A["i: 1"] --> B["total = 1"]
B --> C["i: 2"] --> D["total = 3"]
D --> E["i: 3 (Skip)"]
E --> F["i: 4"] --> G["total = 7"]
G --> H["i: 5"] --> I["total = 12"]
```

**Jawaban:**
1. **12**
2. $(1+2+3+4+5) - 3 = 12$.
</details>
