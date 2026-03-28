🔙 **[Kembali ke Daftar Soal](./README.md)**

---

# Latihan Soal Part C - Modul 02 - Set 12

### Soal 276 (Boolean Logic Flip)
```cpp
int x = -7;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **-7**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=-7] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=-7. Syarat `!x` (NOT x). Jika x=-7 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 277 (Short-Circuit AND)
```cpp
int a = 1; int b = 0;
int visit = 0;
if (a == 1 && ++visit > 0) { /* visited */ }
// Note: ++visit adds 1 to visit
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai true?
2. Berapakah nilai akhir variabel `visit`?
3. Mengapa `visit` bisa tetap bernilai 0 meskipun ada perintah `++visit`?

**Jawaban & Diagnosis:**
1. **Ya**
2. **1**
3. **Karena sifat Short-Circuit AND: Jika syarat pertama sudah FALSE, C++ malas dan tidak akan mengecek/mengeksekusi syarat kedua.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"True"| B{"Lanjut cek ++visit"}
    B -->|"visit = 1"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=1. Cek `a == 1`. Hasil: True. Karena True, lanjat cek ++visit (visit jadi 1).

---
### Soal 278 (Nested If-Else)
```cpp
bool pagi = false;
bool hujan = false;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Makan**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=0, Hujan=0. Masuk blok else terluar (Makan). 

---
### Soal 279 (Boolean Logic Flip)
```cpp
int x = 4;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **4**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=4] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=4. Syarat `!x` (NOT x). Jika x=4 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 280 (Short-Circuit OR)
```cpp
int a = 1;
int visit = 0;
if (a == 1 || ++visit > 0) { /* logic */ }
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai benar?
2. Berapakah nilai akhir variabel `visit`?
3. Apa yang terjadi pada `++visit` jika `a` bernilai 1?

**Jawaban & Diagnosis:**
1. **Benar**
2. **0**
3. **Jika `a == 1` (True), maka syarat kedua tidak akan pernah dibaca (Short-Circuit OR).**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"True"| B{"STOP: Sudah True"}
    B -->|"visit = 0"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=1. Cek `a == 1`. Hasil: True. Karena True, syarat kedua di-skip. visit tetap 0.

---
### Soal 281 (Short-Circuit AND)
```cpp
int a = 0; int b = 0;
int visit = 0;
if (a == 1 && ++visit > 0) { /* visited */ }
// Note: ++visit adds 1 to visit
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai true?
2. Berapakah nilai akhir variabel `visit`?
3. Mengapa `visit` bisa tetap bernilai 0 meskipun ada perintah `++visit`?

**Jawaban & Diagnosis:**
1. **Tidak**
2. **0**
3. **Karena sifat Short-Circuit AND: Jika syarat pertama sudah FALSE, C++ malas dan tidak akan mengecek/mengeksekusi syarat kedua.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"STOP: Sirkuit Pendek"}
    B -->|"visit = 0"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, syarat kedua (++visit) DIABAIKAN. visit tetap 0.

---
### Soal 282 (Short-Circuit OR)
```cpp
int a = 0;
int visit = 0;
if (a == 1 || ++visit > 0) { /* logic */ }
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai benar?
2. Berapakah nilai akhir variabel `visit`?
3. Apa yang terjadi pada `++visit` jika `a` bernilai 1?

**Jawaban & Diagnosis:**
1. **Salah**
2. **1**
3. **Jika `a == 1` (True), maka syarat kedua tidak akan pernah dibaca (Short-Circuit OR).**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"Lanjut cek ++visit"}
    B -->|"visit = 1"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, baru lanjut cek ++visit. visit jadi 1.

---
### Soal 283 (Boolean Logic Flip)
```cpp
int x = 2;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **2**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=2] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=2. Syarat `!x` (NOT x). Jika x=2 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 284 (Boolean Logic Flip)
```cpp
int x = -4;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **-4**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=-4] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=-4. Syarat `!x` (NOT x). Jika x=-4 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 285 (Nested If-Else)
```cpp
bool pagi = true;
bool hujan = false;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Lari**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=1, Hujan=0. Masuk blok if(pagi). Cek hujan: Lari.

---
### Soal 286 (Boolean Logic Flip)
```cpp
int x = 8;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **8**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=8] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=8. Syarat `!x` (NOT x). Jika x=8 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 287 (Short-Circuit OR)
```cpp
int a = 0;
int visit = 0;
if (a == 1 || ++visit > 0) { /* logic */ }
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai benar?
2. Berapakah nilai akhir variabel `visit`?
3. Apa yang terjadi pada `++visit` jika `a` bernilai 1?

**Jawaban & Diagnosis:**
1. **Salah**
2. **1**
3. **Jika `a == 1` (True), maka syarat kedua tidak akan pernah dibaca (Short-Circuit OR).**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"Lanjut cek ++visit"}
    B -->|"visit = 1"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, baru lanjut cek ++visit. visit jadi 1.

---
### Soal 288 (Short-Circuit AND)
```cpp
int a = 0; int b = 1;
int visit = 0;
if (a == 1 && ++visit > 0) { /* visited */ }
// Note: ++visit adds 1 to visit
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai true?
2. Berapakah nilai akhir variabel `visit`?
3. Mengapa `visit` bisa tetap bernilai 0 meskipun ada perintah `++visit`?

**Jawaban & Diagnosis:**
1. **Tidak**
2. **0**
3. **Karena sifat Short-Circuit AND: Jika syarat pertama sudah FALSE, C++ malas dan tidak akan mengecek/mengeksekusi syarat kedua.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"STOP: Sirkuit Pendek"}
    B -->|"visit = 0"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, syarat kedua (++visit) DIABAIKAN. visit tetap 0.

---
### Soal 289 (Boolean Logic Flip)
```cpp
int x = 9;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **9**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=9] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=9. Syarat `!x` (NOT x). Jika x=9 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 290 (Nested If-Else)
```cpp
bool pagi = false;
bool hujan = false;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Makan**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=0, Hujan=0. Masuk blok else terluar (Makan). 

---
### Soal 291 (Nested If-Else)
```cpp
bool pagi = false;
bool hujan = true;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Makan**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=0, Hujan=1. Masuk blok else terluar (Makan). 

---
### Soal 292 (Boolean Logic Flip)
```cpp
int x = -8;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **-8**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=-8] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=-8. Syarat `!x` (NOT x). Jika x=-8 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 293 (Short-Circuit AND)
```cpp
int a = 0; int b = 0;
int visit = 0;
if (a == 1 && ++visit > 0) { /* visited */ }
// Note: ++visit adds 1 to visit
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai true?
2. Berapakah nilai akhir variabel `visit`?
3. Mengapa `visit` bisa tetap bernilai 0 meskipun ada perintah `++visit`?

**Jawaban & Diagnosis:**
1. **Tidak**
2. **0**
3. **Karena sifat Short-Circuit AND: Jika syarat pertama sudah FALSE, C++ malas dan tidak akan mengecek/mengeksekusi syarat kedua.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"STOP: Sirkuit Pendek"}
    B -->|"visit = 0"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, syarat kedua (++visit) DIABAIKAN. visit tetap 0.

---
### Soal 294 (Boolean Logic Flip)
```cpp
int x = 8;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **8**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=8] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=8. Syarat `!x` (NOT x). Jika x=8 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 295 (Short-Circuit OR)
```cpp
int a = 0;
int visit = 0;
if (a == 1 || ++visit > 0) { /* logic */ }
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai benar?
2. Berapakah nilai akhir variabel `visit`?
3. Apa yang terjadi pada `++visit` jika `a` bernilai 1?

**Jawaban & Diagnosis:**
1. **Salah**
2. **1**
3. **Jika `a == 1` (True), maka syarat kedua tidak akan pernah dibaca (Short-Circuit OR).**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"False"| B{"Lanjut cek ++visit"}
    B -->|"visit = 1"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=0. Cek `a == 1`. Hasil: False. Karena False, baru lanjut cek ++visit. visit jadi 1.

---
### Soal 296 (Nested If-Else)
```cpp
bool pagi = true;
bool hujan = true;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Tidur**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=1, Hujan=1. Masuk blok if(pagi). Cek hujan: Tidur.

---
### Soal 297 (Nested If-Else)
```cpp
bool pagi = false;
bool hujan = false;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Makan**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=0, Hujan=0. Masuk blok else terluar (Makan). 

---
### Soal 298 (Short-Circuit AND)
```cpp
int a = 1; int b = 0;
int visit = 0;
if (a == 1 && ++visit > 0) { /* visited */ }
// Note: ++visit adds 1 to visit
```
**Pertanyaan:**
1. Apakah kondisi `a == 1` bernilai true?
2. Berapakah nilai akhir variabel `visit`?
3. Mengapa `visit` bisa tetap bernilai 0 meskipun ada perintah `++visit`?

**Jawaban & Diagnosis:**
1. **Ya**
2. **1**
3. **Karena sifat Short-Circuit AND: Jika syarat pertama sudah FALSE, C++ malas dan tidak akan mengecek/mengeksekusi syarat kedua.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[Cek a == 1] -->|"True"| B{"Lanjut cek ++visit"}
    B -->|"visit = 1"| C[Selesai]
```

**📖 Cara Membaca Diagram:**
a=1. Cek `a == 1`. Hasil: True. Karena True, lanjat cek ++visit (visit jadi 1).

---
### Soal 299 (Boolean Logic Flip)
```cpp
int x = -8;
if (!x) printf("Nol");
else printf("Bukan Nol");
```
**Pertanyaan:**
1. Berapakah nilai `x`?
2. Apa output program tersebut?
3. Dalam C++, angka berapakah yang dianggap sebagai `false`?

**Jawaban & Diagnosis:**
1. **-8**
2. **Bukan Nol**
3. **Hanya angka 0. Selebihnya (positif maupun negatif) dianggap `true`.**

**Mermaid Flowchart:**
```mermaid
graph TD
    A[x=-8] --> B{x != 0?}
    B -- Ya (True) --> C["!x jadi False"]
    B -- Tidak (False) --> D["!x jadi True"]
    C --> E[Bukan Nol]
    D --> F[Nol]
```

**📖 Cara Membaca Diagram:**
x=-8. Syarat `!x` (NOT x). Jika x=-8 (bukan 0), maka x dianggap true, !x jadi false. Maka cetak 'Bukan Nol'.

---
### Soal 300 (Nested If-Else)
```cpp
bool pagi = false;
bool hujan = true;
if (pagi) {
    if (hujan) printf("Tidur");
    else printf("Lari");
} else {
    printf("Makan");
}
```
**Pertanyaan:**
1. Apa output yang muncul di layar?
2. Jika `pagi` false, apakah kondisi `hujan` akan dicek?
3. Berapa jumlah total blok `printf` yang ada dalam kode ini?

**Jawaban & Diagnosis:**
1. **Makan**
2. **Tidak, karena mesin langsung masuk ke blok `else` terluar.**
3. **3**

**Mermaid Flowchart:**
```mermaid
graph TD
    A{pagi?} -- Ya --> B{hujan?}
    A -- Tidak --> C[Makan]
    B -- Ya --> D[Tidur]
    B -- Tidak --> E[Lari]
```

**📖 Cara Membaca Diagram:**
Pagi=0, Hujan=1. Masuk blok else terluar (Makan). 

---
