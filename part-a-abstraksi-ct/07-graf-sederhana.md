# 07. Graf Sederhana (Simple Graphs)

> "Dunia ini adalah sebuah jaringan raksasa. Setiap orang, setiap kota, setiap komputer terhubung oleh sebuah hubungan. Dalam informatika, kita menyebutnya: **Graf**."

Selamat datang di modul terakhir Part A! Di sini, kamu akan belajar tentang **Teori Graf**, salah satu topik paling keren dan paling sering muncul di soal OSN-K Informatika. Jangan khawatir, konsepnya sebenarnya sangat dekat dengan kehidupan sehari-hari!

---

## 🧠 Bagian 1: Apa Itu Graf?

### Definisi Sederhana
Graf adalah kumpulan **titik-titik** (disebut **Vertex/Node**) yang dihubungkan oleh **garis-garis** (disebut **Edge/Sisi**).

Bayangkan peta kota:
*   **Titik (Vertex)** = Kota-kota (Jakarta, Bandung, Surabaya).
*   **Garis (Edge)** = Jalan yang menghubungkan kota-kota tersebut.

```
     Jakarta
      / \
     /   \
  Bandung--Surabaya
```

Gambar di atas adalah sebuah **graf** dengan 3 vertex dan 3 edge.

### Istilah Penting (Wajib Hafal untuk OSN-K!)

| Istilah | Penjelasan | Analogi |
| :--- | :--- | :--- |
| **Vertex (V)** / Node | Titik dalam graf | Kota, Orang, Komputer |
| **Edge (E)** / Sisi | Garis penghubung antar vertex | Jalan, Pertemanan, Kabel |
| **Degree (Derajat)** | Jumlah edge yang terhubung ke sebuah vertex | Jumlah jalan keluar dari sebuah kota |
| **Adjacent (Bertetangga)** | Dua vertex yang langsung terhubung oleh edge | Jakarta bertetangga dengan Bandung |
| **Path (Jalur)** | Urutan vertex yang dilalui dari satu titik ke titik lain | Rute perjalanan: Jakarta → Bandung → Surabaya |
| **Cycle (Siklus)** | Path yang kembali ke titik awal | Jakarta → Bandung → Surabaya → Jakarta |

---

## 🚶 Bagian 2: Jenis-Jenis Graf

### 1. Graf Tak Berarah (Undirected Graph)
Edge-nya **tidak punya arah**. Jika ada jalan dari A ke B, maka jalan dari B ke A juga ada.

**Analogi:** Jalan dua arah. Pertemanan di Facebook (jika kamu berteman dengan Budi, maka Budi juga berteman denganmu).

```
  A --- B
  |     |
  C --- D
```

### 2. Graf Berarah (Directed Graph / Digraph)
Setiap edge memiliki **arah** (panah). Jalan dari A ke B belum tentu berarti ada jalan dari B ke A.

**Analogi:** Jalan satu arah. Follow di Instagram (kamu bisa follow artis, tapi artis belum tentu follow kamu balik).

```
  A --> B
  |     |
  v     v
  C --> D
```

### 3. Graf Berbobot (Weighted Graph)
Setiap edge memiliki **nilai/bobot**, biasanya mewakili jarak, biaya, atau waktu.

**Analogi:** Peta GPS. Jalan dari Jakarta ke Bandung = 150 km, Jakarta ke Surabaya = 800 km.

```
  Jakarta --150km-- Bandung
      \               /
     800km         200km
        \           /
        Surabaya
```

### 4. Tree (Pohon)
Graf yang **terhubung** dan **tidak punya siklus**. Setiap node punya tepat 1 jalur ke node lainnya.

**Analogi:** Silsilah keluarga (Family Tree). Setiap anak hanya punya satu garis ke ayah/ibunya, tidak ada lingkaran.

```
        Kakek
       /     \
    Ayah     Paman
   /    \      |
  Kamu  Adik  Sepupu
```

### Perbandingan Jenis Graf

| Jenis | Arah? | Bobot? | Siklus? | Contoh Dunia Nyata |
| :--- | :---: | :---: | :---: | :--- |
| Undirected | ❌ | ❌ | Bisa | Pertemanan Facebook |
| Directed | ✅ | ❌ | Bisa | Follower Instagram |
| Weighted | Bisa | ✅ | Bisa | Peta GPS (jarak) |
| Tree | ❌ | ❌ | ❌ | Struktur folder komputer |

---

## 📐 Bagian 3: Konsep Matematika Graf (Penting untuk OSN-K!)

### 1. Derajat Vertex (Degree)
**Derajat** sebuah vertex adalah jumlah edge yang terhubung ke vertex tersebut.

```
  A --- B --- C
  |         /
  D ------/
```
*   Derajat A = 2 (terhubung ke B dan D)
*   Derajat B = 3 (terhubung ke A, C, dan D... tunggu, B-D tidak ada di gambar ini)

Mari kita perjelas:
```
  A --- B --- C
  |         /
  D -------
```
*   Derajat A = 2 (terhubung ke B, D)
*   Derajat B = 2 (terhubung ke A, C)
*   Derajat C = 2 (terhubung ke B, D)
*   Derajat D = 2 (terhubung ke A, C)

### 2. Rumus Jabat Tangan (Handshaking Lemma) ⭐

> **Jumlah semua derajat vertex = 2 × Jumlah Edge**

Atau dalam rumus: $\sum \text{deg}(v) = 2|E|$

**Mengapa?** Karena setiap edge menghubungkan **tepat 2 vertex**, jadi setiap edge "dihitung" 2 kali (sekali di masing-masing ujungnya).

**Contoh:**
```
  A --- B
  |   / |
  | /   |
  C --- D
```
*   Edge: A-B, A-C, B-C, B-D, C-D = **5 edge**
*   Derajat: A=2, B=3, C=3, D=2
*   Total Derajat: 2+3+3+2 = **10**
*   Cek: 2 × 5 = **10** ✅

**Tips OSN-K:** Jika soal bilang "ada 6 vertex masing-masing berderajat 3", maka jumlah edge = (6×3)/2 = **9 edge**.

### 3. Euler Path dan Euler Circuit

Ini adalah konsep klasik yang sering muncul di OSN-K!

#### Euler Path (Jalur Euler)
Sebuah jalur yang **melewati setiap edge tepat satu kali** (boleh melewati vertex berkali-kali).

**Syarat:** Graf memiliki **tepat 0 atau 2 vertex berderajat ganjil**.

#### Euler Circuit (Sirkuit Euler)
Euler Path yang **kembali ke titik awal** (membentuk siklus).

**Syarat:** **Semua vertex** berderajat **genap**.

**Analogi Kehidupan:**
Bayangkan kamu seorang pengantar surat. Kamu ingin melewati SEMUA jalan di kompleks perumahan **tepat satu kali** tanpa mengulang jalan yang sama. Bisakah? Itu adalah pertanyaan Euler Path!

**Cerita Jembatan Königsberg:**
Ini adalah masalah yang membuat Teori Graf lahir! Di kota Königsberg (sekarang Kaliningrad, Rusia), ada 7 jembatan yang menghubungkan 4 daratan. Seorang matematikawan bernama **Leonhard Euler** bertanya: "Bisakah seseorang berjalan melewati SEMUA 7 jembatan tepat 1 kali dan kembali ke titik awal?" Jawabnya: **TIDAK BISA**, karena keempat vertex punya derajat ganjil.

**Contoh Soal:**
```
Graf 1:          Graf 2:
A --- B          A --- B
|     |          |   / |
C --- D          C --- D
```
*   **Graf 1:** Semua vertex berderajat 2 (genap) → ✅ Ada **Euler Circuit**.
*   **Graf 2:** Vertex A=2, B=3, C=2, D=3 → Ada 2 vertex ganjil → ✅ Ada **Euler Path** (mulai dari B atau D).

### 4. Hamilton Path dan Hamilton Circuit

#### Hamilton Path
Jalur yang **melewati setiap vertex tepat satu kali**.

#### Hamilton Circuit
Hamilton Path yang **kembali ke titik awal**.

**Perbedaan dengan Euler:**
*   **Euler** = Lewati setiap **EDGE** tepat 1 kali.
*   **Hamilton** = Lewati setiap **VERTEX** tepat 1 kali.

**Analogi:** Traveling Salesman Problem. Seorang sales ingin mengunjungi semua kota tepat satu kali lalu pulang. Rute tersingkat mana yang harus ia ambil?

---

## 🌐 Bagian 4: Representasi Graf dalam Komputer

Bagaimana komputer menyimpan data graf? Ada 2 cara utama:

### 1. Adjacency Matrix (Matriks Ketetanggaan)
Sebuah tabel (matriks) berukuran V×V. Jika ada edge antara vertex i dan j, maka `matrix[i][j] = 1`. Jika tidak, `matrix[i][j] = 0`.

**Contoh:**
```
Graf:
A --- B
|     |
C --- D

Matriks:
    A  B  C  D
A [ 0, 1, 1, 0 ]
B [ 1, 0, 0, 1 ]
C [ 1, 0, 0, 1 ]
D [ 0, 1, 1, 0 ]
```

**Kelebihan:** Mudah mengecek apakah dua vertex terhubung (O(1)).
**Kekurangan:** Boros memori jika graf besar tapi edge-nya sedikit (sparse graph).

### 2. Adjacency List (Daftar Ketetanggaan)
Setiap vertex menyimpan **daftar tetangganya**.

**Contoh:**
```
Graf yang sama:
A → [B, C]
B → [A, D]
C → [A, D]
D → [B, C]
```

**Kelebihan:** Hemat memori untuk graf sparse.
**Kekurangan:** Mengecek koneksi dua vertex butuh waktu lebih lama.

### Kapan Pakai Yang Mana?

| Situasi | Gunakan |
| :--- | :--- |
| Graf kecil (vertex < 100) | Adjacency Matrix |
| Graf besar, edge sedikit | Adjacency List |
| Sering cek "apakah A-B terhubung?" | Adjacency Matrix |
| Sering iterasi semua tetangga | Adjacency List |

---

## 🔍 Bagian 5: Algoritma Penelusuran Graf (Graph Traversal)

Bagaimana cara "menjelajahi" semua vertex dalam sebuah graf? Ada 2 strategi utama:

### 1. BFS (Breadth-First Search) - Pencarian Melebar

**Analogi:** Bayangkan kamu menjatuhkan batu ke kolam. Riak air menyebar ke segala arah secara **merata, layer demi layer**. BFS menjelajah seperti itu.

**Cara Kerja:**
1.  Mulai dari vertex awal, tandai sebagai "sudah dikunjungi".
2.  Kunjungi **semua tetangga** vertex awal dulu (Layer 1).
3.  Baru kemudian kunjungi tetangga dari tetangga (Layer 2).
4.  Ulangi sampai semua vertex terjelajahi.

**Menggunakan:** Queue (Antrian) - FIFO!

**Contoh:**
```
Graf:
    A
   / \
  B   C
 / \   \
D   E   F

BFS dari A: A → B, C → D, E, F
(Layer 0: A, Layer 1: B,C, Layer 2: D,E,F)
```

**Kegunaan di Dunia Nyata:**
*   **Google Maps:** Mencari rute terdekat (jumlah belokan paling sedikit).
*   **Social Media:** Fitur "Orang yang mungkin kamu kenal" (teman dari teman).
*   **Virus Spread:** Memodelkan penyebaran virus dari satu orang ke orang lain per hari.

### 2. DFS (Depth-First Search) - Pencarian Mendalam

**Analogi:** Bayangkan kamu di dalam labirin. Kamu terus berjalan **ke satu arah sedalam mungkin** sampai buntu. Baru kemudian kamu **mundur** (backtrack) dan coba jalan lain.

**Cara Kerja:**
1.  Mulai dari vertex awal, tandai sebagai "sudah dikunjungi".
2.  Langsung masuk ke **satu tetangga** dan telusuri sedalam mungkin.
3.  Jika buntu, **mundur** ke percabangan terakhir dan coba arah lain.
4.  Ulangi sampai semua vertex terjelajahi.

**Menggunakan:** Stack (Tumpukan) - LIFO! (Atau bisa pakai Rekursi)

**Contoh:**
```
Graf yang sama:
    A
   / \
  B   C
 / \   \
D   E   F

DFS dari A: A → B → D (buntu, mundur) → E (buntu, mundur) → C → F
```

**Kegunaan di Dunia Nyata:**
*   **Maze Solver:** Robot yang menjelajahi labirin.
*   **File Explorer:** Membuka folder → subfolder → sub-subfolder (sedalam mungkin).
*   **Puzzle / Game AI:** Menelusuri semua kemungkinan langkah Sudoku atau Catur.

### Perbandingan BFS vs DFS

| Aspek | BFS | DFS |
| :--- | :--- | :--- |
| Strategi | Melebar (layer demi layer) | Mendalam (sedalam mungkin) |
| Struktur Data | Queue (FIFO) | Stack (LIFO) / Rekursi |
| Cocok untuk | Jarak terpendek | Mencari semua jalur |
| Analogi | Riak air di kolam | Petualangan di labirin |
| Memori | Lebih boros (simpan semua tetangga) | Lebih hemat |

---

## 🌳 Bagian 6: Spanning Tree (Pohon Rentang)

### Definisi
Spanning Tree adalah **subgraf** dari sebuah graf yang:
1.  Menghubungkan **semua vertex**.
2.  Tidak memiliki **siklus**.
3.  Memiliki tepat **V-1 edge** (V = jumlah vertex).

**Analogi:** Bayangkan kamu adalah perusahaan listrik. Kamu harus memasang kabel ke semua rumah di desa, tapi kamu ingin menggunakan **kabel sesedikit mungkin** tanpa ada lingkaran (agar tidak boros). Itulah Spanning Tree!

### Minimum Spanning Tree (MST)
Jika grafnya berbobot (ada jarak/biaya di setiap edge), MST adalah spanning tree dengan **total bobot terkecil**.

**Contoh:**
```
  A --5-- B
  |     / |
  3   2   4
  | /     |
  C --6-- D

Pilihan Edge:
- A-C (3), C-B (2), B-D (4) → Total: 9 ✅ (MST)
- A-B (5), B-D (4), A-C (3) → Total: 12 ❌ (bukan minimum)
```

---

## 🏙️ Bagian 7: Relasi Graf dengan Kehidupan & Informatika

### A. Graf dalam Informatika:
*   **Internet:** Setiap website adalah vertex, setiap hyperlink adalah edge (directed). Google menggunakan graf untuk menentukan ranking website (PageRank).
*   **Social Network:** Setiap akun adalah vertex. Pertemanan = undirected edge, Following = directed edge.
*   **Database:** Relasi antar tabel dalam database bisa dimodelkan sebagai graf.
*   **Routing Jaringan:** Router internet menggunakan graf berbobot untuk menentukan jalur tercepat mengirim data.

### B. Graf dalam Kehidupan:
*   **Peta & Navigasi:** Kota = vertex, jalan = edge, jarak = bobot.
*   **Jadwal Penerbangan:** Bandara = vertex, rute penerbangan = edge.
*   **Organisasi:** Struktur organisasi perusahaan adalah sebuah Tree (pohon).
*   **Turnamen Olahraga:** Pertandingan antar tim bisa digambarkan sebagai graf. Tim = vertex, pertandingan = edge.

### C. Graf dalam Game:
*   **Peta Game Open World:** Lokasi = vertex, jalur antar lokasi = edge.
*   **Skill Tree:** Skill = vertex, prerequisite = directed edge.
*   **Pathfinding NPC:** Musuh dalam game menggunakan algoritma graf (BFS/DFS/A*) untuk mengejarmu!

---

## 📊 Bagian 8: Tabel Ringkasan Rumus & Tips OSN-K

| Konsep | Rumus / Syarat | Tips Cepat |
| :--- | :--- | :--- |
| Total Derajat | $\sum \text{deg}(v) = 2 \times E$ | Setiap edge dihitung 2 kali |
| Jumlah Edge Tree | $E = V - 1$ | Pohon selalu punya edge = vertex - 1 |
| Euler Path | Tepat 0 atau 2 vertex ganjil | Hitung vertex berderajat ganjil! |
| Euler Circuit | Semua vertex genap | Tidak boleh ada yang ganjil |
| Graph Connected | Ada jalur dari setiap vertex ke vertex lain | Cek apakah ada yang "terisolasi" |
| Vertex berderajat ganjil | Selalu berjumlah **GENAP** | Tidak mungkin ada 1 atau 3 vertex ganjil saja |

---

## 💡 Bagian 9: Tips & Trik Menghadapi Soal Graf di OSN-K

### 1. Langkah Pertama: Gambar Grafnya!
Jika soal memberikan deskripsi verbal, **SELALU gambar grafnya** di kertas. Ini akan sangat membantu visualisasi.

### 2. Hitung Derajat Setiap Vertex
Banyak soal OSN-K yang bisa diselesaikan hanya dengan menghitung derajat. Ingat Rumus Jabat Tangan!

### 3. Identifikasi Jenis Graf
Tanyakan pada diri sendiri:
*   Berarah atau tidak?
*   Ada bobot atau tidak?
*   Ada siklus atau tidak (Tree)?

### 4. Cek Euler Path/Circuit
Jika soal bertanya "bisakah melewati semua jalan tepat sekali?", langsung hitung vertex berderajat ganjil!

### 5. Gunakan BFS untuk Jarak Terpendek
Jika soal bertanya "berapa langkah minimum dari A ke B?", gunakan BFS!

---

## 🚀 Kesimpulan untuk OSN-K
*   **Graf** adalah cara merepresentasikan hubungan antar objek.
*   **Degree** dan **Handshaking Lemma** adalah alat hitung utama.
*   **Euler Path/Circuit** muncul sangat sering di soal OSN-K.
*   **BFS** dan **DFS** adalah dua cara menjelajahi graf yang wajib dipahami.
*   **Tree** adalah graf khusus tanpa siklus (sangat penting di informatika).

> **Selamat!** Kamu telah menyelesaikan seluruh materi **Part A: Abstraksi dan Computational Thinking**. Dengan pemahaman ini, kamu sudah memiliki fondasi kuat untuk menghadapi soal-soal OSN-K Informatika. Terus berlatih! 🎯

---
[< Materi Sebelumnya: Logika dan Antrian](./06-logika-dan-antrian.md)
[< Kembali ke Beranda Materi](../README.md)
