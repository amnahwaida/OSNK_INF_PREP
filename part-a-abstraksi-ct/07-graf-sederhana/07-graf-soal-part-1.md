🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Latihan Soal Bagian 1 (Soal 1-50)
## Topik: Dasar-Dasar Graf, Vertex, Edge, Degree, Jenis Graf

[< Kembali ke Indeks Materi](../07-graf-sederhana.md) | [Bagian 2 (51-100) >](./07-graf-soal-part-2.md)

---

### Soal #1: Definisi Vertex
Dalam sebuah graf peta kota, apa yang diwakili oleh "vertex"?
A. Jalan
B. Kota
C. Jarak
D. Arah mata angin

<details><summary>💡 Hint</summary>Vertex = titik = "benda" atau "tempat".</details>
<details><summary>✅ Jawaban</summary>**B. Kota.** Vertex mewakili objek/lokasi, sedangkan jalan adalah edge.</details>

### Soal #2: Definisi Edge
Di media sosial, jika vertex adalah akun pengguna, maka edge adalah...
A. Jumlah foto
B. Hubungan pertemanan
C. Jumlah likes
D. Tanggal lahir

<details><summary>💡 Hint</summary>Edge = garis = "hubungan" antara dua vertex.</details>
<details><summary>✅ Jawaban</summary>**B. Hubungan pertemanan.** Edge menghubungkan dua vertex.</details>

### Soal #3: Menghitung Vertex
Sebuah graf memiliki titik: A, B, C, D, E. Berapa jumlah vertex?
A. 3
B. 4
C. 5
D. 6

<details><summary>💡 Hint</summary>Hitung saja jumlah huruf/titiknya.</details>
<details><summary>✅ Jawaban</summary>**C. 5.**</details>

### Soal #4: Menghitung Edge
```
A --- B
|     |
C --- D
```
Berapa jumlah edge pada graf di atas?
A. 3
B. 4
C. 5
D. 6

<details><summary>💡 Hint</summary>Hitung setiap garis: A-B, A-C, B-D, C-D.</details>
<details><summary>✅ Jawaban</summary>**B. 4.** Ada 4 garis penghubung.</details>

### Soal #5: Degree (Derajat)
```
A --- B --- C
```
Berapa derajat vertex B?
A. 1
B. 2
C. 3
D. 0

<details><summary>💡 Hint</summary>Hitung berapa garis yang "menempel" ke B.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** B terhubung ke A dan C.</details>

### Soal #6: Adjacent (Bertetangga)
```
A --- B --- C
```
Apakah A dan C bertetangga (adjacent)?
A. Ya
B. Tidak
C. Mungkin
D. Tergantung arah

<details><summary>💡 Hint</summary>Bertetangga = langsung terhubung oleh satu edge.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** A dan C tidak langsung terhubung, harus lewat B.</details>

### Soal #7: Jenis Graf - Facebook
Pertemanan di Facebook (jika kamu berteman dengan Budi, maka Budi juga berteman denganmu) adalah contoh dari...
A. Directed Graph
B. Undirected Graph
C. Weighted Graph
D. Tree

<details><summary>💡 Hint</summary>Hubungan dua arah = tidak ada panah.</details>
<details><summary>✅ Jawaban</summary>**B. Undirected Graph.** Pertemanan bersifat dua arah.</details>

### Soal #8: Jenis Graf - Instagram
Follow di Instagram (kamu bisa follow artis, tapi artis belum tentu follow balik) adalah contoh dari...
A. Undirected Graph
B. Directed Graph
C. Tree
D. Weighted Graph

<details><summary>💡 Hint</summary>Hubungan satu arah = ada panah.</details>
<details><summary>✅ Jawaban</summary>**B. Directed Graph.** Following bersifat satu arah.</details>

### Soal #9: Jenis Graf - Peta GPS
Peta yang menunjukkan jarak antar kota (Jakarta-Bandung: 150km) adalah contoh dari...
A. Undirected Graph
B. Tree
C. Weighted Graph
D. Directed Graph

<details><summary>💡 Hint</summary>Ada angka/bobot di setiap edge.</details>
<details><summary>✅ Jawaban</summary>**C. Weighted Graph.** Setiap edge memiliki bobot (jarak).</details>

### Soal #10: Jenis Graf - Folder Komputer
Struktur folder di komputer (Folder → Subfolder → File) tanpa lingkaran adalah contoh dari...
A. Directed Graph
B. Weighted Graph
C. Cycle Graph
D. Tree (Pohon)

<details><summary>💡 Hint</summary>Terhubung semua, tidak ada siklus.</details>
<details><summary>✅ Jawaban</summary>**D. Tree.** Folder komputer membentuk struktur pohon.</details>

### Soal #11: Degree Maksimum
```
    A
   /|\
  B C D
```
Berapa derajat vertex A?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Hitung garis yang menempel ke A.</details>
<details><summary>✅ Jawaban</summary>**C. 3.** A terhubung ke B, C, dan D.</details>

### Soal #12: Vertex Terisolasi
Vertex yang tidak terhubung ke vertex manapun disebut vertex terisolasi. Berapa derajatnya?
A. 1
B. 0
C. -1
D. Tidak terdefinisi

<details><summary>💡 Hint</summary>Tidak ada garis yang menempel.</details>
<details><summary>✅ Jawaban</summary>**B. 0.** Tidak ada edge yang terhubung.</details>

### Soal #13: Path (Jalur)
```
A --- B --- C --- D
```
Manakah yang merupakan path dari A ke D?
A. A → C → D
B. A → B → C → D
C. A → D → B → C
D. D → C → B → A → D

<details><summary>💡 Hint</summary>Path harus melalui edge yang ada.</details>
<details><summary>✅ Jawaban</summary>**B. A → B → C → D.** Hanya ini yang melalui edge yang benar-benar ada.</details>

### Soal #14: Cycle (Siklus)
```
A --- B
|     |
C --- D
```
Manakah yang merupakan cycle?
A. A → B → D → C → A
B. A → B → C
C. A → B → D
D. B → D → C

<details><summary>💡 Hint</summary>Cycle = jalur yang kembali ke titik awal.</details>
<details><summary>✅ Jawaban</summary>**A. A → B → D → C → A.** Satu-satunya yang kembali ke titik awal.</details>

### Soal #15: Tree vs Graf Biasa
Apa perbedaan utama antara Tree dan graf biasa?
A. Tree punya lebih banyak edge
B. Tree tidak punya siklus
C. Tree harus berarah
D. Tree hanya punya 2 vertex

<details><summary>💡 Hint</summary>Pohon = terhubung + tanpa lingkaran.</details>
<details><summary>✅ Jawaban</summary>**B. Tree tidak punya siklus.** Tree adalah graf connected tanpa cycle.</details>

### Soal #16: Edge di Tree
Sebuah tree punya 8 vertex. Berapa jumlah edge-nya?
A. 6
B. 7
C. 8
D. 9

<details><summary>💡 Hint</summary>Rumus tree: E = V - 1.</details>
<details><summary>✅ Jawaban</summary>**B. 7.** Tree selalu punya edge = vertex - 1.</details>

### Soal #17: Directed Graph
```
A --> B --> C
```
Apakah C bisa langsung ke A?
A. Bisa
B. Tidak bisa
C. Tergantung bobot
D. Selalu bisa

<details><summary>💡 Hint</summary>Panah hanya menunjuk satu arah.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak bisa.** Di directed graph, arah panah menentukan akses.</details>

### Soal #18: Weighted Graph
```
A --5-- B --3-- C
```
Berapa total bobot jalur A → B → C?
A. 5
B. 3
C. 8
D. 15

<details><summary>💡 Hint</summary>Jumlahkan bobot setiap edge yang dilewati.</details>
<details><summary>✅ Jawaban</summary>**C. 8.** 5 + 3 = 8.</details>

### Soal #19: Adjacency Matrix
```
A --- B
|
C
```
Berapa nilai matrix[B][C]?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>B dan C tidak terhubung langsung.</details>
<details><summary>✅ Jawaban</summary>**A. 0.** Tidak ada edge antara B dan C.</details>

### Soal #20: Adjacency List
```
A --- B
|     |
C --- D
```
Apa isi adjacency list vertex D?
A. [A, B]
B. [B, C]
C. [C, D]
D. [A, C]

<details><summary>💡 Hint</summary>Daftar semua tetangga langsung D.</details>
<details><summary>✅ Jawaban</summary>**B. [B, C].** D terhubung langsung ke B dan C.</details>

### Soal #21: Self-Loop
Sebuah edge yang menghubungkan vertex ke dirinya sendiri disebut...
A. Cycle
B. Self-loop
C. Bridge
D. Tree

<details><summary>💡 Hint</summary>Bayangkan garis yang kedua ujungnya di titik yang sama.</details>
<details><summary>✅ Jawaban</summary>**B. Self-loop.**</details>

### Soal #22: Complete Graph
Graf lengkap (complete graph) K4 memiliki 4 vertex yang semuanya saling terhubung. Berapa jumlah edge-nya?
A. 4
B. 5
C. 6
D. 8

<details><summary>💡 Hint</summary>Rumus: V×(V-1)/2 = 4×3/2.</details>
<details><summary>✅ Jawaban</summary>**C. 6.** Setiap pasangan vertex terhubung: AB, AC, AD, BC, BD, CD.</details>

### Soal #23: Derajat di Complete Graph
Di complete graph K5 (5 vertex semua saling terhubung), berapa derajat setiap vertex?
A. 3
B. 4
C. 5
D. 10

<details><summary>💡 Hint</summary>Setiap vertex terhubung ke semua vertex lainnya.</details>
<details><summary>✅ Jawaban</summary>**B. 4.** Setiap vertex terhubung ke 4 vertex lainnya.</details>

### Soal #24: Graf Bipartit
Dalam sebuah turnamen catur, pemain hanya bertanding melawan pemain dari tim lawan. Jenis graf ini disebut...
A. Complete Graph
B. Bipartite Graph
C. Tree
D. Directed Graph

<details><summary>💡 Hint</summary>Vertex bisa dibagi 2 kelompok, edge hanya antar kelompok.</details>
<details><summary>✅ Jawaban</summary>**B. Bipartite Graph.** Vertex terbagi dua grup, edge hanya antar grup.</details>

### Soal #25: Subgraph
Jika graf G punya vertex {A,B,C,D} dan edge {A-B, B-C, C-D, A-D}, manakah yang BUKAN subgraph G?
A. {A,B} dengan edge {A-B}
B. {B,C,D} dengan edge {B-C, C-D}
C. {A,C} dengan edge {A-C}
D. {A,B,C} dengan edge {A-B, B-C}

<details><summary>💡 Hint</summary>Subgraph harus hanya menggunakan edge yang ada di graf asli.</details>
<details><summary>✅ Jawaban</summary>**C. {A,C} dengan edge {A-C}.** Edge A-C tidak ada di graf asli G.</details>

### Soal #26: Connected Graph
```
A --- B    D --- E
      |
      C
```
Apakah graf di atas "connected" (terhubung)?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Connected = ada jalur dari setiap vertex ke vertex lainnya.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** D dan E terpisah dari A,B,C. Tidak ada jalur dari A ke D.</details>

### Soal #27: Component
Dari soal #26, berapa jumlah komponen (connected component) graf tersebut?
A. 1
B. 2
C. 3
D. 5

<details><summary>💡 Hint</summary>Komponen = kelompok vertex yang saling terhubung.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** Komponen 1: {A,B,C}. Komponen 2: {D,E}.</details>

### Soal #28: Degree di Directed Graph
```
A --> B
A --> C
B --> C
```
Berapa out-degree (derajat keluar) vertex A?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>Out-degree = jumlah panah yang KELUAR dari A.</details>
<details><summary>✅ Jawaban</summary>**C. 2.** A punya panah keluar ke B dan C.</details>

### Soal #29: In-Degree
Dari soal #28, berapa in-degree (derajat masuk) vertex C?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>In-degree = jumlah panah yang MASUK ke C.</details>
<details><summary>✅ Jawaban</summary>**C. 2.** C menerima panah dari A dan B.</details>

### Soal #30: Analogi Graf - WhatsApp
Grup WhatsApp di mana semua anggota bisa saling chat adalah contoh dari...
A. Directed Graph
B. Weighted Graph
C. Complete Undirected Graph
D. Tree

<details><summary>💡 Hint</summary>Semua bisa chat ke semua, dua arah.</details>
<details><summary>✅ Jawaban</summary>**C. Complete Undirected Graph.** Semua anggota saling terhubung dua arah.</details>

### Soal #31: Path Length
```
A --2-- B --3-- C --1-- D
```
Berapa panjang (total bobot) path dari A ke D?
A. 3
B. 5
C. 6
D. 7

<details><summary>💡 Hint</summary>Jumlahkan semua bobot edge yang dilewati.</details>
<details><summary>✅ Jawaban</summary>**C. 6.** 2 + 3 + 1 = 6.</details>

### Soal #32: Shortest Path
```
     B
    / \
   2   3
  /     \
A --10-- C
```
Jalur terpendek dari A ke C adalah...
A. A → C (bobot 10)
B. A → B → C (bobot 5)
C. Keduanya sama
D. Tidak ada jalur

<details><summary>💡 Hint</summary>Bandingkan total bobot tiap jalur.</details>
<details><summary>✅ Jawaban</summary>**B. A → B → C (bobot 5).** 2 + 3 = 5 < 10.</details>

### Soal #33: Degree Minimum
Jika semua vertex sebuah graf punya derajat minimal 1, apa artinya?
A. Graf pasti connected
B. Tidak ada vertex yang terisolasi
C. Graf punya cycle
D. Graf adalah tree

<details><summary>💡 Hint</summary>Derajat 0 = terisolasi. Derajat ≥ 1 = pasti punya tetangga.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak ada vertex yang terisolasi.** Tapi belum tentu connected.</details>

### Soal #34: Analogi - Jadwal Penerbangan
Dalam graf jadwal penerbangan, vertex mewakili bandara. Apa yang diwakili oleh edge berarah?
A. Jarak tempuh
B. Rute penerbangan satu arah
C. Harga tiket
D. Nama maskapai

<details><summary>💡 Hint</summary>Berarah = ada arah dari kota asal ke kota tujuan.</details>
<details><summary>✅ Jawaban</summary>**B. Rute penerbangan satu arah.**</details>

### Soal #35: Matrix Simetris
Adjacency matrix graf tak berarah selalu bersifat...
A. Identitas
B. Simetris
C. Diagonal
D. Nol semua

<details><summary>💡 Hint</summary>Jika A-B = 1, maka B-A juga = 1.</details>
<details><summary>✅ Jawaban</summary>**B. Simetris.** matrix[i][j] selalu = matrix[j][i].</details>

### Soal #36: Adjacency List vs Matrix
Graf punya 1000 vertex tapi hanya 10 edge. Representasi mana yang lebih hemat memori?
A. Adjacency Matrix
B. Adjacency List
C. Sama saja
D. Tidak bisa disimpan

<details><summary>�� Hint</summary>Matrix butuh 1000×1000 = 1 juta sel. List cukup 10 entri.</details>
<details><summary>✅ Jawaban</summary>**B. Adjacency List.** Jauh lebih hemat untuk graf sparse.</details>

### Soal #37: Tree Depth
```
        A
       / \
      B   C
     / \
    D   E
```
Berapa kedalaman (depth) vertex D jika A adalah root?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>Depth = jarak dari root. A=0, B=1, D=2.</details>
<details><summary>✅ Jawaban</summary>**C. 2.** A(0) → B(1) → D(2).</details>

### Soal #38: Leaf Node
Dari soal #37, vertex mana saja yang merupakan "leaf" (daun)?
A. A dan B
B. C, D, dan E
C. A saja
D. B saja

<details><summary>💡 Hint</summary>Leaf = vertex yang tidak punya anak (derajat 1 di tree, kecuali root).</details>
<details><summary>✅ Jawaban</summary>**B. C, D, dan E.** Mereka tidak punya anak lagi.</details>

### Soal #39: Planar Graph
Graf yang bisa digambar di kertas TANPA ada garis yang bersilangan disebut...
A. Complete Graph
B. Planar Graph
C. Bipartite Graph
D. Weighted Graph

<details><summary>💡 Hint</summary>Planar = "rata" = bisa digambar tanpa crossing.</details>
<details><summary>✅ Jawaban</summary>**B. Planar Graph.**</details>

### Soal #40: Multigraph
Jika antara dua kota ada 2 jalan berbeda (misal tol dan non-tol), graf ini disebut...
A. Simple Graph
B. Multigraph
C. Complete Graph
D. Tree

<details><summary>💡 Hint</summary>Multi = banyak edge antara dua vertex yang sama.</details>
<details><summary>✅ Jawaban</summary>**B. Multigraph.** Ada lebih dari satu edge antara pasangan vertex yang sama.</details>

### Soal #41: Degree Sum
```
A --- B --- C
      |
      D
```
Berapa total derajat semua vertex?
A. 4
B. 5
C. 6
D. 8

<details><summary>💡 Hint</summary>A=1, B=3, C=1, D=1. Atau pakai rumus: 2 × jumlah edge.</details>
<details><summary>✅ Jawaban</summary>**C. 6.** Jumlah edge = 3. Total derajat = 2×3 = 6.</details>

### Soal #42: Analogi - Turnamen
Dalam turnamen sepak bola, setiap tim bertanding melawan semua tim lain tepat sekali. Jika ada 5 tim, berapa total pertandingan?
A. 5
B. 10
C. 15
D. 20

<details><summary>💡 Hint</summary>Ini sama dengan jumlah edge di complete graph K5 = V(V-1)/2.</details>
<details><summary>✅ Jawaban</summary>**B. 10.** 5×4/2 = 10.</details>

### Soal #43: Directed Cycle
```
A --> B --> C --> A
```
Apakah graf di atas memiliki cycle?
A. Ya
B. Tidak
C. Hanya jika undirected
D. Tergantung bobot

<details><summary>💡 Hint</summary>A ke B ke C kembali ke A mengikuti arah panah.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Ada directed cycle: A → B → C → A.</details>

### Soal #44: Bridge (Jembatan)
Edge yang jika dihapus membuat graf menjadi tidak connected disebut...
A. Cycle
B. Bridge
C. Loop
D. Chain

<details><summary>💡 Hint</summary>Bridge = satu-satunya "jembatan" penghubung dua bagian graf.</details>
<details><summary>✅ Jawaban</summary>**B. Bridge.**</details>

### Soal #45: Isomorfisme
Dua graf yang bentuknya beda tapi strukturnya sama (jumlah vertex, edge, dan koneksi yang sama) disebut...
A. Symmetric
B. Isomorphic
C. Identical
D. Parallel

<details><summary>💡 Hint</summary>Iso = sama, morph = bentuk. Sama secara struktur.</details>
<details><summary>✅ Jawaban</summary>**B. Isomorphic.**</details>

### Soal #46: Degree Vertex di Cycle Graph
Cycle graph C6 memiliki 6 vertex yang membentuk lingkaran. Berapa derajat setiap vertex?
A. 1
B. 2
C. 3
D. 6

<details><summary>💡 Hint</summary>Setiap vertex terhubung ke tetangga kiri dan kanan.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** Di cycle, setiap vertex punya tepat 2 tetangga.</details>

### Soal #47: Analogi - Rangkaian Listrik
Dalam rangkaian listrik, komponen (lampu, resistor) adalah vertex. Apa yang menjadi edge?
A. Arus listrik
B. Kabel penghubung
C. Tegangan
D. Watt

<details><summary>💡 Hint</summary>Yang "menghubungkan" komponen satu ke lainnya.</details>
<details><summary>✅ Jawaban</summary>**B. Kabel penghubung.**</details>

### Soal #48: Sparse vs Dense Graph
Graf dengan 100 vertex dan 10 edge disebut...
A. Dense Graph
B. Sparse Graph
C. Complete Graph
D. Null Graph

<details><summary>💡 Hint</summary>Sparse = jarang (edge sedikit dibanding vertex).</details>
<details><summary>✅ Jawaban</summary>**B. Sparse Graph.** Sangat sedikit edge dibandingkan kemungkinan maksimum.</details>

### Soal #49: Null Graph
Graf yang hanya punya vertex tanpa edge sama sekali disebut...
A. Complete Graph
B. Empty/Null Graph
C. Tree
D. Cycle

<details><summary>💡 Hint</summary>Null = kosong. Tidak ada garis sama sekali.</details>
<details><summary>✅ Jawaban</summary>**B. Empty/Null Graph.**</details>

### Soal #50: Refleksi Bagian 1
Manakah pernyataan yang BENAR tentang graf?
A. Semua graf punya siklus
B. Edge selalu punya arah
C. Graf bisa merepresentasikan berbagai hubungan dunia nyata
D. Tree selalu punya siklus

<details><summary>💡 Hint</summary>Pikirkan semua contoh graf yang sudah kamu pelajari.</details>
<details><summary>✅ Jawaban</summary>**C.** Graf adalah cara universal merepresentasikan berbagai jenis hubungan.</details>

---
[< Kembali ke Indeks Materi](../07-graf-sederhana.md) | [Bagian 2 (51-100) >](./07-graf-soal-part-2.md)
