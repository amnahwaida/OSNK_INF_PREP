		🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal Part C - Modul 03 - Set 03 (Premium Edition)

---

### Soal 21: Sensor Keamanan (Break Logic)
```cpp
// Skenario: Cari angka 13 di antara 1-20
int target = 0;
for (int i = 1; i <= 20; i++) {
    if (i == 13) {
        target = i;
        break;
    }
}
```
**Pertanyaan:**
1. Berapakah nilai `target` akhir?
2. Berapa kali loop ini berputar?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart (Pre-Break Sequence):**
```mermaid
graph LR
A["i=1...12: (F)"] --> B["i=13: target=13"]
B --> C["Kondisi: if(13==13) (T)"]
C --> D["PERINTAH: break!"]
D --> E["STOP (i=14...20 dilewati)"]
```

**Jawaban:**
1. **13**
2. **13 kali**

**📖 Analisis Mendalam:**
`break` menghentikan loop seketika. Meskipun batasnya sampai 20, mesin berhenti tepat saat menemukan angka 13. Sisa angka (14, 15, dst) tidak pernah disentuh oleh komputer.
</details>

---

### Soal 22: Antrian Ganjil (Continue Logic)
```cpp
// Skenario: Lewati angka genap, jumlahkan ganjil 1-5
int total = 0;
for (int i = 1; i <= 5; i++) {
    if (i % 2 == 0) continue;
    total += i;
}
```
**Pertanyaan:**
1. Berapakah nilai `total`?
2. Apa perbedaan `continue` dengan `break`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart (Skip Sequence):**
```mermaid
graph TD
I1["i=1 (Ganjil) --> total=1"] --> I2["i=2 (Genap) --> CONTINUE (Skip)"]
I2 --> I3["i=3 (Ganjil) --> total=1+3=4"]
I4["i=4 (Genap) --> CONTINUE (Skip)"] --> I5["i=5 (Ganjil) --> total=4+5=9"]
I3 --> I4
I5 --> End["Hasil: 9"]
```

**Jawaban:**
1. **9** (1 + 3 + 5)
2. `break` keluar dari loop selamanya, `continue` hanya melewati iterasi saat ini dan lanjut ke angka berikutnya.
</details>

---

### Soal 23: ⚠️ Jebakan Urutan (Break Before Change)
```cpp
int x = 0;
for (int i = 1; i <= 3; i++) {
    if (i == 2) break;
    x += i;
}
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apakah angka **2** sempat dijumlahkan ke `x`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart (The Wall):**
```mermaid
graph LR
A["i=1"] --> B["x = 0 + 1 = 1"]
B --> C["i=2"] --> D{"if (2 == 2)? (T)"}
D -- T --> E["BREAK!"]
E -- "x+=2 dilewati" --> End["Hasil x: 1"]
```

**Jawaban:**
1. **1**
2. **Tidak.** Karena perintah `break` berada di atas `x += i`. Begitu `i == 2`, mesin langsung kabur sebelum sempat menjumlahkan angka tersebut.
</details>

---

### Soal 24: Pencarian Linier (Flag Simulation)
```cpp
int data[] = {5, 8, 10, 2};
bool ketemu = false;
for (int i = 0; i < 4; i++) {
    if (data[i] == 10) {
        ketemu = true;
        break;
    }
}
```
**Pertanyaan:**
1. Berapakah nilai `ketemu` (true/false)?
2. Pada indeks ke berapa mesin berhenti mencari?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["i=0 (5)"] --> B["i=1 (8)"]
B --> C["i=2 (10)"]
C --> D["ketemu=T, break"]
```

**Jawaban:**
1. **true**
2. **Indeks 2.**
</details>

---

### Soal 25: Sensor Polusi (Skip Logic)
```cpp
// Skip jika nilai > 50
int sensor[] = {10, 60, 20};
int total = 0;
for (int i = 0; i < 3; i++) {
    if (sensor[i] > 50) continue;
    total += sensor[i];
}
```
**Pertanyaan:**
1. Berapakah nilai `total`?
2. Nilai mana yang dilewati oleh program?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A["10"] --> B["sum=10"]
B --> C["60 > 50?"] -- T --> D["Skip"]
D --> E["20"] --> F["sum=30"]
```

**Jawaban:**
1. **30**
2. **60**
</details>

---

### Soal 26: ⚠️ Jebakan Increment (Continue + Manual Inc)
```cpp
int n = 0, total = 0;
while (n < 3) {
    n++;
    if (n == 2) continue;
    total += 10;
}
```
**Pertanyaan:**
1. Berapakah nilai `total`?
2. Apa yang terjadi jika `n++` ditaruh di bawah `continue`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart (While-Increment Trace):**
```mermaid
graph TD
Start --> W1["n:0 -> 1"] --> T1["total = 10"]
T1 --> W2["n:1 -> 2"] --> C1{"if(2==2)? (T)"}
C1 -- T --> S1["CONTINUE (Skip total+=10)"]
S1 --> W3["n:2 -> 3"] --> T3["total = 10 + 10 = 20"]
T3 -- "n < 3? (F)" --> End["Hasil: 20"]
```

**Jawaban:**
1. **20**
2. **Infinite Loop.** Karena `n` tidak akan pernah bertambah jika ia terus menerus dilewati oleh `continue`.

**📖 Analisis Mendalam:**
Pada loop `while`, posisi increment sangat krusial jika menggunakan `continue`. Di `for`, increment sudah otomatis dilakukan di header, sehingga lebih aman dari jebakan *Infinite Loop* saat melakukan skip.
</details>

---

### Soal 27: Filter Karakter (Char Skip)
```cpp
string kata = "bana-na";
int huruf_a = 0;
for (int i = 0; i < 7; i++) {
    if (kata[i] == '-') continue;
    if (kata[i] == 'a') huruf_a++;
}
```
**Pertanyaan:**
1. Berapakah nilai `huruf_a`?
2. Berapa kali perintah `continue` dijalankan?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["'b'"] --> B["'a'*"] --> C["'n'"]
C --> D["'-' (Skip)"] --> E["'a'*"]
E --> F["'n'"] --> G["'a'*"]
```

**Jawaban:**
1. **3**
2. **1 kali** (pada karakter ke-5).
</details>

---

### Soal 28: Break Bersarang (Nested Break)
```cpp
int total = 0;
for (int i = 0; i < 2; i++) {
    for (int j = 0; j < 5; j++) {
        if (j == 2) break;
        total++;
    }
}
```
**Pertanyaan:**
1. Berapakah nilai `total`?
2. Apakah `break` menghentikan loop `i`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph TD
A["i=0: j=0, 1 (break)"] --> B["total=2"]
B --> C["i=1: j=0, 1 (break)"] --> D["total=4"]
```

**Jawaban:**
1. **4**
2. **Tidak.** `break` hanya menghancurkan loop terdalam (`j`).
</details>

---

### Soal 29: Mencari Bilangan Ganjil Pertama
```cpp
int angka[] = {2, 4, 7, 8, 9};
int ganjil = 0;
for (int x : angka) {
    if (x % 2 != 0) {
        ganjil = x;
        break;
    }
}
```
**Pertanyaan:**
1. Berapakah nilai `ganjil`?
2. Mengapa angka **9** tidak masuk ke variabel `ganjil`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart:**
```mermaid
graph LR
A["2 (G)"] --> B["4 (G)"]
B --> C["7 (O)!"]
C --> D["ganjil=7, break"]
```

**Jawaban:**
1. **7**
2. Karena mesin sudah menemukan angka ganjil pertama (7) dan langsung melakukan `break`.
</details>

---

### Soal 30: ⚠️ Total Sisa (Continue Flow)
```cpp
int sum = 0;
for (int i = 1; i <= 4; i++) {
    if (i == 3) continue;
    sum += i;
    if (sum > 5) break;
}
```
**Pertanyaan:**
1. Berapakah nilai `sum` akhir?
2. Berapakah nilai `i` terakhir saat program berhenti?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Flowchart (Double Constraint Trace):**
```mermaid
graph TD
I1["i=1: sum=1, 1>5?(F)"] --> I2["i=2: sum=3, 3>5?(F)"]
I2 --> I3["i=3: CONTINUE (Skip)"]
I3 --> I4["i=4: sum=7, 7>5?(T)"]
I4 -- T --> B["BREAK!"]
B --> End["Hasil Akhir sum: 7"]
```

**Jawaban:**
1. **7**
2. **4**
</details>
