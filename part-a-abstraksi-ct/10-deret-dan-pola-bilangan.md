# 10. Model Matematis, Deret & Pola Bilangan

> "Programmer yang hebat tidak menghitung manual 1+2+3+...+100. Mereka menggunakan otak, melihat polanya, dan langsung tahu jawabannya dalam sepersekian detik berkat Gauss!"

Masalah yang sering didapatkan pemrogram komputer adalah "Looping" (Perulangan) raksasa. Untuk menjadikannya sangat cepat, loop ini disederhanakan menjadi rumus matematis tertutup (Model). Inilah sebabnya mengapa materi ini masuk ke silabus OSN-K.

---

## 🔢 1. Melihat Pola Bilangan (Pattern Recognition tingkat dewa)

Terkadang, deret yang disajikan tidak masuk dalam rumus Aritmetika standar. Jadi kamu diuji menemukan fungsi $f(x)$ sendiri.

**Contoh 1: Barisan Fibonacci**
Berapa suku berikutnya dari: `1, 1, 2, 3, 5, 8, 13, ... ?`
Lihat polanya: Setiap angka adalah penjumlahan DUA ANGKA SEBELUMNYA.
- $1+1=2$
- $1+2=3$
- $2+3=5$
- Jadi selanjutnya: $8+13 = 21$.

**Contoh 2: Barisan Kuadrat yang Digeser**
Berapa suku ke-10 dari barisan: `2, 5, 10, 17, 26, ...` ?
- Ini susah kalau cari bedanya biasa. Tapi orang Informatika sadar bahwa:
- 2 = $1^2 + 1$
- 5 = $2^2 + 1$
- 10= $3^2 + 1$
- dst...
Jadi suku ke-10 adalah $10^2 + 1 = 101$.

---

## 📈 2. Deret Aritmetika Dasar (Tangga Setara)

Deret aritmetika adalah barisan bilangan yang punya **SELISIH (BEDA)** yang stabil dan konstan (selalu tambah atau selalu kurang dengan jumlah yang sama).

Contoh: `2, 5, 8, 11, 14, ...` (Polanya: selalu ditambah 3!)
- **Suku Pertama ($a$)** = 2
- **Beda ($b$)** = +3

### A. Rumus Mencari Suku ke-$n$ ($U_n$)
Bayangkan kamu di anak tangga ke-1 (tinggi 2m), setiap langkah kamu naik 3m. Berapa tinggi di langkah ke-10?
> $$U_n = a + (n - 1)b$$
- $U_{10} = 2 + (10 - 1) \times 3$
- $U_{10} = 2 + (9 \times 3) = 2 + 27 = 29$.

### B. Rumus Menjumlahkan Seluruh Deret ($S_n$)
Ini yang disebut trik Gauss (Carl Friedrich Gauss). Saat kecil, ia diminta menghitung jumlah $1 + 2 + 3 + ... + 100$.
Cara bodoh: hitung urut berjam-jam.
Cara jenius Gauss:
$1 + 100 = 101$
$2 + 99 = 101$
$3 + 98 = 101$
Ada berapa pasang 101? Karena total ada 100 angka, kalau dipasangkan dua-dua jadi ada **50 pasang**.
Total = $50 \times 101 = 5050$.

> **Rumus Jumlah Deret Aritmetika ($S_n$):**
> $$S_n = \frac{n}{2} \times (\text{Awal} + \text{Akhir})$$
> Atau:
> $$S_n = \frac{n}{2} \times (a + U_n)$$

**Contoh Soal OSN-K:**
Pak Dengklek menyimpan bebeknya di 50 kandang berderet. Kandang 1 berisi 5 bebek. Kandang 2 berisi 8 bebek. Kandang 3 berisi 11 bebek, dan seterusnya dengan selisih 3. Berapa total seluruh bebek Pak Dengklek dari kandang 1 sampai 50?
1. Cari dulu isi kandang 50 (Suku ke-50):
   $U_{50} = 5 + (49) \times 3 = 5 + 147 = 152$ bebek.
2. Cari total semua:
   $S_{50} = \frac{50}{2} \times (5 + 152) = 25 \times 157 = 3925$ bebek. (Dikerjakan dalam 30 detik!).

---

## Σ 3. Notasi Sigma (Cara Menyingkat Loop O(n))

Notasi angka Yunani $\Sigma$ (Sigma) adalah cara matematika untuk merepresentasikan *looping pertambahan* ala bahasa C++ `for-loop`. Kadang-kadang OSN-K memunculkannya untuk menakut-nakuti anak yang lemah matematika, padahal ini gampang!

$$\sum_{i=1}^{5} (2i)$$

**Cara baca Programmer (Pseudo-code):**
```cpp
int total = 0;
for (int i = 1; i <= 5; i++) {
    total = total + (2 * i);
}
```

**Penyelesaian Manual:**
Ganti nilai $i$ dari 1 sampai 5, lalu tambahkan semua hasilnya!
- Jika i=1 → $2 \times 1 = 2$
- Jika i=2 → $2 \times 2 = 4$
- Jika i=3 → $2 \times 3 = 6$
- Jika i=4 → $2 \times 4 = 8$
- Jika i=5 → $2 \times 5 = 10$

Totalnya = $2 + 4 + 6 + 8 + 10 = 30$.
Sangat gampang kan? Sigma hanya cara *fancy* (keren) untuk menulis deret bertambah.

---

## 🧩 4. Memodelkan Masalah Dunia Nyata (Matematika Praktis)

Selain deret baku, terkadang kamu akan berhadapan dengan soal "hitung-hitungan sawah dan bebek" (pemodelan matematis biasa) dengan Sistem Persamaan Linear (SPLDV).

**Contoh Klasik:**
Di peternakan Pak Dengklek ada kumpulan Ayam dan Kambing. Total jumlah KEPALA hewan di sana adalah 40 buah. Total jumlah KAKI hewan di sana adalah 110 kaki.
Berapa jumlah ayamnya saja?

**Cara "Informatika / Matematika Model":**
1. Ayam (A) kakinya 2. Kambing (K) kakinya 4. Kepala cuma 1 ditiap hewan.
2. Persamaan Kepala: $A + K = 40$ (Maka $A = 40 - K$)
3. Persamaan Kaki: $2A + 4K = 110$
4. Substitusi (Ganti A dengan $40-K$):
   $2(40 - K) + 4K = 110$
   $80 - 2K + 4K = 110$
   $80 + 2K = 110$
   $2K = 30$
   $K = 15$ ekor (Kambing).
5. Jumlah Ayam: $40 - 15 = 25$ ekor ayam. Selesai!

Pola berpikir: **(1) Observasi, (2) Definisikan variabel, (3) Cari persamaan, (4) Substitusi.** Itulah abstraksi matematis!

---
[< Materi Sebelumnya: Kombinatorika](./09-kombinatorika.md)
[< Kembali ke Beranda Materi](../README.md)
