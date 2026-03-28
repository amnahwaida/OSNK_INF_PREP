		🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal Part C - Modul 05 - Set 01 (Premium Edition)

> [!IMPORTANT]
> Dalam Rekursi, perhatikan dua hal: **Base Case** (kapan berhenti) dan **Recursive Step** (kapan memanggil diri sendiri). Jangan sampai lupas Base Case atau kamu akan terkena *Stack Overflow*!

---

### Soal 1: Penjumlahan Berantai (Sum Recursion)
```cpp
int hitung(int n) {
    if (n == 0) return 0;
    return n + hitung(n - 1);
}

int main() {
    int x = hitung(3);
}
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Berapa kali fungsi `hitung` dipanggil secara total (termasuk panggilan awal)?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["hitung(3)"] --> B["hitung(2)"]
B --> C["hitung(1)"]
C --> D["hitung(0) [Base Case]"]
D -- "return 0" --> C
C -- "return 1 + 0 = 1" --> B
B -- "return 2 + 1 = 3" --> A
A -- "return 3 + 3 = 6" --> Main["x = 6"]
```

**Jawaban:**
1. **6** (3 + 2 + 1 + 0)
2. **4 kali** (panggilan untuk n=3, 2, 1, dan 0).
</details>

---

### Soal 2: Faktorial Sederhana (Factorial Trace)
```cpp
int faktorial(int n) {
    if (n <= 1) return 1;
    return n * faktorial(n - 1);
}

int main() {
    int hasil = faktorial(4);
}
```
**Pertanyaan:**
1. Berapakah nilai `hasil`?
2. Apa yang dikembalikan oleh `faktorial(1)`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["faktorial(4)"] --> B["faktorial(3)"]
B --> C["faktorial(2)"]
C --> D["faktorial(1) [Base Case]"]
D -- "1" --> C
C -- "2 * 1 = 2" --> B
B -- "3 * 2 = 6" --> A
A -- "4 * 6 = 24" --> Main["hasil = 24"]
```

**Jawaban:**
1. **24** (4 * 3 * 2 * 1)
2. **1**
</details>

---

### Soal 3: Urutan Cetak A (Pre-order Print)
```cpp
void cetak(int n) {
    if (n < 1) return;
    cout << n;
    cetak(n - 1);
}

int main() {
    cetak(3);
}
```
**Pertanyaan:**
1. Apa output program tersebut?
2. Apakah `cout` dijalankan **sebelum** atau **sesudah** fungsi memanggil dirinya sendiri?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["cetak(3): cout 3"] --> B["cetak(2): cout 2"]
B --> C["cetak(1): cout 1"]
C --> D["cetak(0): return"]
```

**Jawaban:**
1. **321**
2. **Sebelum.** Karena `cout` berada di atas baris `cetak(n-1)`. Ini disebut *Pre-order traversal* dalam rekursi.
</details>

---

### Soal 4: Urutan Cetak B (Post-order Print)
```cpp
void cetak(int n) {
    if (n < 1) return;
    cetak(n - 1);
    cout << n;
}

int main() {
    cetak(3);
}
```
**Pertanyaan:**
1. Apa output program tersebut?
2. Mengapa outputnya terbalik dibanding Soal 3?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["cetak(3)"] --> B["cetak(2)"]
B --> C["cetak(1)"]
C --> D["cetak(0): return"]
D -- "selesai" --> C["cout 1"]
C -- "selesai" --> B["cout 2"]
B -- "selesai" --> A["cout 3"]
```

**Jawaban:**
1. **123**
2. Karena `cout` berada **di bawah** panggilan rekursif. Program "masuk" dulu sampai ke dasar (n=0), baru saat perjalanan "pulang" (backtracking), ia mencetak angkanya.
</details>

---

### Soal 5: Kelipatan Dua (Power of 2)
```cpp
int dua_pangkat(int n) {
    if (n == 0) return 1;
    return 2 * dua_pangkat(n - 1);
}

int main() {
    int x = dua_pangkat(3);
}
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Berapa nilai yang dikembalikan saat `n = 0`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Jawaban:**
1. **8** ($2 \times 2 \times 2 \times 1$)
2. **1**
</details>

---

### Soal 6: Pencari FPB (Recursive GCD)
```cpp
int fpb(int a, int b) {
    if (b == 0) return a;
    return fpb(b, a % b);
}

int main() {
    int hasil = fpb(12, 8);
}
```
**Pertanyaan:**
1. Berapakah nilai `hasil`?
2. Bagaimana urutan parameter `(a, b)` pada panggilan kedua?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["fpb(12, 8)"] --> B["fpb(8, 12%8=4)"]
B --> C["fpb(4, 8%4=0)"]
C -- "return a: 4" --> B
B -- "4" --> A
A -- "4" --> Main
```

**Jawaban:**
1. **4**
2. **(8, 4)**
</details>

---

### Soal 7: Pembagi Dua (Logarithmic Stack)
```cpp
int bagi(int n) {
    if (n <= 1) return 1;
    return 1 + bagi(n / 2);
}

int main() {
    int x = bagi(8);
}
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Berapa kali fungsi ini memanggil dirinya sendiri (tidak termasuk main)?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["bagi(8)"] --> B["bagi(4)"]
B --> C["bagi(2)"]
C --> D["bagi(1) [Base Case]"]
D -- "1" --> C
C -- "1+1 = 2" --> B
B -- "1+2 = 3" --> A
A -- "1+3 = 4" --> Main
```

**Jawaban:**
1. **4**
2. **3 kali** (bagi 4, 2, dan 1).
</details>

---

### Soal 8: Jumlah Digit (Digit Sum)
```cpp
int sum_digit(int n) {
    if (n == 0) return 0;
    return (n % 10) + sum_digit(n / 10);
}

int main() {
    int s = sum_digit(123);
}
```
**Pertanyaan:**
1. Berapakah nilai `s`?
2. Apa peran `n / 10` dalam rekursi di atas?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph TD
A["sum(123)"] --> B["3 + sum(12)"]
B --> C["2 + sum(1)"]
C --> D["1 + sum(0)"]
D -- "0" --> C
```

**Jawaban:**
1. **6** (3 + 2 + 1 + 0)
2. Untuk **membuang digit terakhir** sehingga angka menjadi semakin kecil dan akhirnya mencapai 0 (Base Case).
</details>

---

### Soal 9: Misteri Parameter (Static Trap?)
```cpp
int misteri(int n) {
    if (n <= 0) return 0;
    return n + misteri(n - 2);
}

int main() {
    int x = misteri(5);
}
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apakah fungsi ini akan pernah memanggil `misteri(0)`?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Call Stack:**
```mermaid
graph LR
A["misteri(5)"] --> B["5 + mist(3)"]
B --> C["3 + mist(1)"]
C --> D["1 + mist(-1)"]
D -- "0" --> C
```

**Jawaban:**
1. **9** (5 + 3 + 1 + 0)
2. **Tidak.** Dari 1 langsung melompat ke -1 karena `n - 2`. Namun karena kondisinya `n <= 0`, maka `misteri(-1)` tetap mengembalikan 0 dan berhenti.
</details>

---

### Soal 10: Fibonacci Mini (Tree Intro)
```cpp
int fib(int n) {
    if (n <= 1) return n;
    return fib(n-1) + fib(n-2);
}

int main() {
    int hasil = fib(3);
}
```
**Pertanyaan:**
1. Berapakah nilai `hasil`?
2. Berapa kali `fib(1)` dipanggil dalam proses ini?

<details>
<summary><b>Klik untuk Lihat Jawaban & Diagnosis</b></summary>

**Mermaid Tree Trace:**
```mermaid
graph TD
A["fib(3)"] --> B["fib(2)"]
A --> C["fib(1)"]
B --> D["fib(1)"]
B --> E["fib(0)"]
```

**Jawaban:**
1. **2**
2. **2 kali.** (Sekali dari fib(3) dan sekali dari fib(2)).
</details>
