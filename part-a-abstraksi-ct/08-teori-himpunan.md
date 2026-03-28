# 08. Teori Himpunan (Set Theory)

> "Di sekolah ada ekskul Basket dan Kodir. Ada yang ikut Basket saja, ada yang ikut Kodir saja, ada yang ikut KEDUANYA, dan ada yang rebahan di rumah (tidak ikut keduanya). Selamat datang di dunia **Himpunan**!"

Teori himpunan adalah fondasi dari logika matematika dan database komputer. Di soal OSN-K (terutama soal cerita/Bebras), konsep ini sering digunakan untuk memecahkan masalah pengelompokan data dan **Prinsip Inklusi-Eksklusi**.

---

## 📦 1. Apa Itu Himpunan?

**Himpunan (Set)** adalah kumpulan benda, obyek, atau angka yang didefinisikan dengan jelas. Benda-benda di dalam himpunan disebut **anggota (elemen)**.

**Contoh:**
- Himpunan $A$ = {Budi, Siti, Anton}
- Himpunan $B$ = {1, 3, 5, 7, 9} (Himpunan bilangan ganjil < 10)

### Aturan Main Himpunan:
1. **Tidak Boleh Ada Duplikat:** {1, 2, 2, 3} ditulis sebagai {1, 2, 3}. Komputer membuang paksa data kembar.
2. **Urutan Tidak Penting:** {A, B, C} sama persis dengan {C, A, B}.

**Istilah Penting:**
- **Kardinalitas** (dilambangkan $|A|$ atau $n(A)$) = **Berapa banyak anggota yang ada di dalam himpunan A**.
  - Contoh: $A = \{1, 3, 5\}$. Maka $|A| = 3$.
- **Himpunan Semesta ($S$)** = Seluruh obyek yang sedang kita bicarakan. Misal: Seluruh siswa di kelasmu.
- **Himpunan Kosong ($\emptyset$ atau $\{\}$)** = Himpunan yang tidak punya anggota sama sekali. Kardinalitasnya 0.

---

## 🎨 2. Operasi Himpunan (Cara Menyatukan atau Memisahkan)

Bayangkan ada 2 ekskul:
- $A$ = Himpunan anak Basket = {Budi, Siti, Andi}
- $B$ = Himpunan anak Paskibra = {Andi, Cici, Dedi}

### A. Gabungan / Union ($\cup$)
Semua anak yang ikut Basket **ATAU** Paskibra (atau keduanya).
- Kata kunci: **ATAU**. Ini seperti operator OR (`||`) di pemrograman.
- Digabung semua, tapi nama yang dobel cukup ditulis sekali!
- $A \cup B$ = {Budi, Siti, Andi, Cici, Dedi}

### B. Irisan / Intersection ($\cap$)
Anak yang ikut Basket **DAN** Paskibra sekaligus. Cuma yang ada di kedua ekskul!
- Kata kunci: **DAN**. Ini seperti operator AND (`&&`) di pemrograman.
- Siapa yang ada di A dan juga di B? Andi!
- $A \cap B$ = {Andi}

### C. Selisih / Difference ($-$ atau $\setminus$)
Anak yang **HANYA** ikut Basket, tapi **TIDAK** ikut Paskibra.
- $A - B$ = Orang di A, tapi kurangi yang juga ada di B.
- Budi dan Siti cuma ikut Basket. Andi ikut Paskibra, jadi Andi dicoret.
- $A - B$ = {Budi, Siti}
- *Perhatikan: $A - B$ tidak sama dengan $B - A$!* ($B - A$ = {Cici, Dedi})

### D. Komplemen ($A^c$ atau $A'$)
Semua anak di sekolah ($S$) yang **TIDAK** ikut Basket.
- Kata kunci: **SELAIN** / **BUKAN**. Ini seperti operator NOT (`!`) di pemrograman.

---

## 📊 3. Diagram Venn (Senjata Utama OSN-K!)

Kalau soal himpunan berbentuk cerita panjang, **JANGAN DIHAWAL, GAMBAR DIAGRAM VENN-NYA!**

Diagram Venn menggunakan lingkaran untuk mewakili himpunan, dan kotak besar untuk Semesta ($S$).

```
       SEMESTA (S) = Semua siswa di kelas
 _______________________________________
|                                       |
|  (BASKET)               (PASKIBRA)    |
|    ______               ______        |
|   /      \             /      \       |
|  /  Budi  \   ANDI    /  Cici  \      |
| |   Siti   |---------|   Dedi   |     |
|  \        / (Irisan)  \        /      |
|   \______/             \______/       |
|                                       |
|          Eka, Fajar (Tidak ikut apa-apa)
|_______________________________________|
```

### Cara Membaca Area:
- Kiri saja (Budi, Siti) = HANYA Basket ($A - B$)
- Kanan saja (Cici, Dedi) = HANYA Paskibra ($B - A$)
- Tengah (Andi) = KEDUANYA ($A \cap B$)
- Luar (Eka, Fajar) = TIDAK KEDUANYA ($(A \cup B)^c$)

---

## 🧮 4. Prinsip Inklusi-Eksklusi (RUMUS WAJIB!)

Ini adalah rumus **PALING SERING KELUAR** di soal OSN-K untuk menghitung jumlah (kardinalitas) gabungan himpunan.

### Kasus 2 Himpunan
Ada berapa total anak yang ikut Basket **ATAU** Paskibra ($|A \cup B|$)?
Apakah $|A| + |B|$? **TIDAK!** Karena kalau kita jumlahkan total Basket dan total Paskibra, anak yang ikut **keduanya** (Andi) akan dihitung **dua kali**. 

Maka, kita harus menguranginya sekali.

> **Rumus 2 Himpunan:**
> $$|A \cup B| = |A| + |B| - |A \cap B|$$
> *(Gabungan = Total A + Total B - Irisannya)*

**Contoh Soal OSN-K:**
Di sebuah kelas ada 40 siswa. 25 siswa suka Nasi Goreng, 20 siswa suka Mie Goreng, dan 10 siswa suka DUA-DUANYA. Pertanyaannya:
1. Berapa siswa yang suka Nasi Goreng **ATAU** Mie Goreng?
2. Berapa siswa yang **TIDAK SUKA KEDUANYA**?

**Cara Jawab:**
- $A$ = Nasi Goreng (25)
- $B$ = Mie Goreng (20)
- Keduanya ($A \cap B$) = 10
- Total Siswa ($S$) = 40

Jawab 1: Gunakan Inklusi-Eksklusi:
$|A \cup B| = 25 + 20 - 10 = 35$ siswa.

Jawab 2: Yang tidak suka keduanya = Total Siswa dikurangi yang suka (Nasi ATAU Mie).
$40 - 35 = 5$ siswa.

Sangat mudah kalau pakai logika ini!

---

### Kasus 3 Himpunan (Agak Mengerikan Panjang Rumusnya, Tapi Polanya Jelas)

Kalau ada 3 ekskul: A, B, dan C. Bagaimana mencari total anak yang ikut minimal 1 ekskul ($|A \cup B \cup C|$)?

**Polanya (Inklusi-Eksklusi):**
1. **Tambahkan** semua yang sendiri-sendiri (+ $|A| + |B| + |C|$)
2. **Kurangi** semua irisan 2 himpunan (- $|A \cap B| - |A \cap C| - |B \cap C|$)
3. **Tambahkan lagi** irisan ketiganya (+ $|A \cap B \cap C|$)

> **Rumus 3 Himpunan:**
> $$|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |A \cap C| - |B \cap C| + |A \cap B \cap C|$$

*(Ingat polanya: Tambah yang 1, Kurangi yang ber-2, Tambah yang ber-3).*

**Trik Jitu OSN-K untuk 3 Himpunan:**
**JANGAN MENGUNGGUNAKAN RUMUS! GAMBAR DIAGRAM VENN-NYA!**
Mulailah mengisi angka dari **Tengah/Paling Dalam** (Irisan ketiga himpunan), lalu mundur pelan-pelan ke luar.

**Contoh Soal (Penyelesaian dengan Venn):**
Ada 100 siswa.
- 50 suka IPA, 40 suka IPS, 30 suka Bahasa.
- 20 suka IPA & IPS.
- 15 suka IPA & Bahasa.
- 10 suka IPS & Bahasa.
- 5 suka KETIGANYA.
Berapa yang TIDAK suka ketiganya?

**Cara Venn (Mulai dari Terdalam):**
1. Suka Ketiganya = **5**. (Isi di tengah-tengah diagram).
2. Suka (IPA & IPS) total 20. Tapi 5 sudah dihitung di tengah. Berarti yang **HANYA** (IPA & IPS) = 20 - 5 = **15**.
3. Suka (IPA & Bahasa) total 15. Yang **HANYA** (IPA & Bahasa) = 15 - 5 = **10**.
4. Suka (IPS & Bahasa) total 10. Yang **HANYA** (IPS & Bahasa) = 10 - 5 = **5**.
5. Total IPA 50. Yang sudah ada: 5 (ketiganya) + 15 (dengan IPS saja) + 10 (dengan Bahasa saja) = 30. Berarti **HANYA IPA** = 50 - 30 = **20**.
6. Total IPS 40. Sudah ada: 5 + 15 + 5 = 25. **HANYA IPS** = 40 - 25 = **15**.
7. Total Bahasa 30. Sudah ada: 5 + 10 + 5 = 20. **HANYA Bahasa** = 30 - 20 = **10**.

Sekarang, jumlahkan SEMUA DENGAN BENAR (tanpa double counting):
Total yang suka = (Hanya IPA) + (Hanya IPS) + (Hanya BHS) + (Hanya IPA-IPS) + (Hanya IPA-BHS) + (Hanya IPS-BHS) + (Ketiganya)
Total = 20 + 15 + 10 + 15 + 10 + 5 + 5 = **80**.

Maka, yang TIDAK suka ketiganya = 100 - 80 = **20 siswa.**

---

## 💻 5. Hubungan Himpunan dengan Komputer (Database SQL)

Himpunan adalah dasar dari *Database*! Saat kamu mengambil data dari server, operasi `JOIN` di SQL sebenarnya adalah teori himpunan.

Masih ingat operasi himpunan di atas?
| Teori Himpunan | Query Database SQL (Konsep) | Logika Programming |
|----------------|-----------------------------|--------------------|
| Gabungan ($A \cup B$) | `FULL OUTER JOIN` | `IF (A OR B)` |
| Irisan ($A \cap B$) | `INNER JOIN` (Data yang cocok di Keduanya) | `IF (A AND B)` |
| Selisih ($A - B$)  | `LEFT JOIN` (Cari yang di A tapi `B IS NULL`) | `IF (A AND NOT B)` |

Siswa yang menguasai Teori Himpunan akan sangat jago menganalisis kebenaran logika kode dan database!

---
[< Materi Sebelumnya: Graf Sederhana](./07-graf-sederhana.md) | [Materi Berikutnya: Kombinatorika >](./09-kombinatorika.md)
[< Kembali ke Beranda Materi](../README.md)
