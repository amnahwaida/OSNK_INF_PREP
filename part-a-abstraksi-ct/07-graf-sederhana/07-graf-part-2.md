🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Bagian 2: Rumus & Trik Penting untuk OSN-K

[< Bagian 1: Kenalan Dulu](./07-graf-part-1.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 3: Algoritma Jelajah Graf >](./07-graf-part-3.md)

---

## 🤝 Rumus Jabat Tangan (Handshaking Lemma)

Ini adalah **rumus paling penting** di teori graf. Hampir pasti muncul di OSN-K!

### Rumusnya:
> **Total semua derajat = 2 × Jumlah Garis**

Dalam simbol: $\sum \text{deg}(v) = 2 \times E$

### Kenapa Begitu? (Penjelasan Super Simpel)

Setiap garis punya **2 ujung**. Jadi, setiap garis "menyumbang" 1 derajat ke masing-masing ujungnya. Maka setiap garis dihitung 2 kali.

**Bayangkan jabat tangan:** Kalau 2 orang jabat tangan, ada 1 jabatan tangan tapi 2 tangan yang terlibat.

### Contoh:
```
  A --- B
  |   / |
  | /   |
  C --- D
```

**Langkah 1: Hitung derajat tiap titik**
- A terhubung ke B dan C → Derajat A = **2**
- B terhubung ke A, C, dan D → Derajat B = **3**
- C terhubung ke A, B, dan D → Derajat C = **3**
- D terhubung ke B dan C → Derajat D = **2**

**Langkah 2: Jumlahkan semua derajat**
2 + 3 + 3 + 2 = **10**

**Langkah 3: Cek dengan rumus**
Jumlah garis = A-B, A-C, B-C, B-D, C-D = **5 garis**
2 × 5 = **10** ✅ Cocok!

### Trik Cepat untuk Soal OSN-K:

**Soal:** "Ada 6 titik, masing-masing berderajat 3. Berapa jumlah garisnya?"

**Jawab:** Total derajat = 6 × 3 = 18. Jumlah garis = 18 ÷ 2 = **9 garis**. Selesai!

**Soal:** "Ada graf dengan 7 garis. Derajat titiknya: 2, 3, ?, 3, 2. Berapa derajat titik ketiga?"

**Jawab:** Total derajat harus = 2 × 7 = 14. Sudah terkumpul: 2+3+3+2 = 10. Maka derajat titik ketiga = 14 - 10 = **4**.

### Fakta Bonus:
> **Jumlah titik yang berderajat ganjil pasti SELALU genap.**

Artinya, kalau ada 3 titik berderajat ganjil, itu **TIDAK MUNGKIN** terjadi. Harus 0, 2, 4, 6, dst.

---

## 🚶 Euler Path & Euler Circuit

Ini topik favorit soal OSN-K! Konsepnya lahir dari cerita nyata yang sangat terkenal.

### Cerita Jembatan Königsberg (Biar Paham Konteksnya)

Pada tahun 1736, di kota Königsberg (sekarang Rusia), ada sebuah sungai dengan **4 daratan** yang dihubungkan oleh **7 jembatan**.

Warga kota bertanya: **"Bisakah kita jalan-jalan melewati SEMUA 7 jembatan, masing-masing tepat SATU kali, lalu balik ke titik awal?"**

Matematikawan jenius bernama **Leonhard Euler** menjawab: **TIDAK BISA**, dan ia membuktikannya dengan teori graf. Dari sinilah teori graf lahir!

### Apa Itu Euler Path?

**Euler Path** = Jalur yang **melewati setiap GARIS tepat satu kali**. Boleh lewat titik yang sama berkali-kali, tapi setiap garis cuma boleh dilewati sekali.

**Analogi:** Kamu seorang tukang pos. Kamu ingin melewati **semua jalan** di kompleks perumahan **tepat sekali** (tidak ada jalan yang dilewati dua kali). Bisakah?

### Apa Itu Euler Circuit?

**Euler Circuit** = Euler Path yang **titik awalnya sama dengan titik akhirnya** (kamu balik ke rumah).

### Syaratnya (INI YANG SERING DITANYAKAN!)

| Pertanyaan | Syarat | Penjelasan Simpel |
| :--- | :--- | :--- |
| Ada Euler **Path**? | Punya **0 atau 2** titik berderajat ganjil | Kalau 2 ganjil: mulai dari salah satu, selesai di yang lain |
| Ada Euler **Circuit**? | **Semua** titik berderajat **genap** | Karena harus balik ke awal, setiap masuk harus bisa keluar |

### Cara Cepat Mengerjakan Soal:

**Langkah 1:** Hitung derajat setiap titik.
**Langkah 2:** Hitung berapa titik yang punya derajat **ganjil**.
**Langkah 3:** Cocokkan:
- 0 titik ganjil → **Ada Euler Circuit** (dan otomatis ada Euler Path juga)
- 2 titik ganjil → **Ada Euler Path** (tapi bukan Circuit)
- Lebih dari 2 → **Tidak ada** Euler Path maupun Circuit

### Contoh Soal:

**Graf 1:**
```
A --- B
|     |
C --- D
```
Derajat: A=2, B=2, C=2, D=2 → **Semua genap** → ✅ Ada **Euler Circuit**!

**Graf 2:**
```
A --- B
|   / |
| /   |
C --- D
```
Derajat: A=2, B=3, C=3, D=2 → **2 titik ganjil** (B dan C) → ✅ Ada **Euler Path** (mulai dari B, selesai di C, atau sebaliknya).

**Graf 3:**
```
A --- B --- C
|         / |
D -------   E
```
Hitung derajatnya. Jika ada **lebih dari 2** titik ganjil → ❌ **Tidak ada** Euler Path.

---

## 🏃 Hamilton Path & Hamilton Circuit

Mirip Euler, tapi beda objek:

| | Euler | Hamilton |
| :--- | :--- | :--- |
| Yang dilewati tepat 1 kali | Setiap **GARIS** | Setiap **TITIK** |
| Boleh lewat titik berulang? | ✅ Boleh | ❌ Tidak |
| Boleh lewat garis berulang? | ❌ Tidak | ✅ Boleh (kalau perlu) |

### Apa Itu Hamilton Path?
Jalur yang **mengunjungi setiap TITIK tepat satu kali**.

### Apa Itu Hamilton Circuit?
Hamilton Path yang **balik ke titik awal**.

**Analogi:** Kamu seorang salesman. Kamu harus berkunjung ke **semua kota tepat satu kali** lalu pulang. Rute mana yang paling efisien? (Ini disebut **Traveling Salesman Problem**, salah satu masalah tersulit di ilmu komputer!)

### Contoh:
```
A --- B
|   / |
| /   |
C --- D
```
Hamilton Path: A → B → D → C ✅ (Setiap titik dikunjungi tepat 1 kali)
Hamilton Circuit: A → B → D → C → A ✅ (Kembali ke awal)

### Tips untuk OSN-K:
Tidak ada rumus cepat untuk Hamilton (tidak seperti Euler). Kamu harus **coba-coba jalurnya** satu per satu. Tapi kalau soalnya kecil (4-6 titik), itu masih bisa dikerjakan manual.

---

## 🌳 Spanning Tree (Pohon Rentang)

### Apa Itu?
Bayangkan kamu kerja di **PLN** (perusahaan listrik). Kamu harus memasang kabel ke **semua rumah** di desa. Tapi kamu mau pakai **kabel sesedikit mungkin** dan **tidak boleh ada lingkaran** (boros kabel).

Hasilnya adalah **Spanning Tree**: sebuah "pohon" yang menghubungkan semua titik dari graf asal, tanpa siklus, dan pakai garis sesedikit mungkin.

### Aturannya:
- Harus **menghubungkan semua titik**
- **Tidak boleh ada siklus** (lingkaran)
- Jumlah garisnya selalu = **V - 1** (V = jumlah titik)

### Minimum Spanning Tree (MST)

Kalau grafnya punya bobot (angka di setiap garis), MST adalah spanning tree yang **total bobotnya paling kecil**.

**Contoh:**
```
  A --5-- B
  |     / |
  3   2   4
  | /     |
  C --6-- D
```

**Pilihan edge untuk MST:**
- Ambil C-B (2) → paling murah dulu
- Ambil A-C (3) → termurah berikutnya
- Ambil B-D (4) → Total: 2 + 3 + 4 = **9** ✅ Ini MST!

**Kenapa bukan A-B (5)?** Karena A sudah terhubung ke B lewat A-C-B. Menambah A-B akan membuat siklus.

---

## 📊 Tabel Ringkasan Semua Rumus

| Konsep | Rumus / Syarat | Cara Cepat |
| :--- | :--- | :--- |
| Rumus Jabat Tangan | Total derajat = 2 × Jumlah garis | Setiap garis dihitung 2 kali |
| Garis di Pohon (Tree) | Jumlah garis = V - 1 | Pohon selalu punya garis = titik - 1 |
| Euler Path | 0 atau 2 titik berderajat ganjil | Hitung yang ganjil! |
| Euler Circuit | Semua titik berderajat genap | Tidak boleh ada ganjil |
| Titik berderajat ganjil | Selalu berjumlah **genap** | Tidak mungkin ada 1 atau 3 saja |
| Connected Graph | Ada jalur dari setiap titik ke titik lain | Cek ada yang terisolasi? |

---

> **Kamu sekarang sudah bisa mengerjakan banyak soal OSN-K tentang graf!** Di Bagian 3, kita akan belajar tentang **BFS dan DFS** — cara komputer menjelajahi graf. Ini penting banget untuk soal-soal simulasi!

---

[< Bagian 1: Kenalan Dulu](./07-graf-part-1.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 3: Algoritma Jelajah Graf >](./07-graf-part-3.md)
