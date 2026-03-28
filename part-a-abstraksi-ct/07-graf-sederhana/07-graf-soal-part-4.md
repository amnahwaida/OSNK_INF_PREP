🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Latihan Soal Bagian 4 (Soal 151-200)
## Topik: BFS, DFS, dan Traversal Graf

[< Bagian 3 (101-150)](./07-graf-soal-part-3.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 5 (201-250) >](./07-graf-soal-part-5.md)

---

### Soal #151: BFS - Definisi
BFS menjelajahi graf secara...
A. Mendalam (depth-first)
B. Melebar (breadth-first, layer by layer)
C. Acak
D. Terbalik

<details><summary>💡 Hint</summary>Breadth = lebar.</details>
<details><summary>✅ Jawaban</summary>**B. Melebar (layer by layer).**</details>

### Soal #152: DFS - Definisi
DFS menjelajahi graf secara...
A. Melebar dulu
B. Mendalam dulu (sedalam mungkin, lalu mundur)
C. Layer by layer
D. Semua sekaligus

<details><summary>�� Hint</summary>Depth = kedalaman.</details>
<details><summary>✅ Jawaban</summary>**B. Mendalam dulu.**</details>

### Soal #153: BFS pakai apa?
BFS menggunakan struktur data...
A. Stack
B. Queue
C. Array
D. Tree

<details><summary>💡 Hint</summary>BFS = melebar = FIFO = antrian.</details>
<details><summary>✅ Jawaban</summary>**B. Queue.**</details>

### Soal #154: DFS pakai apa?
DFS menggunakan struktur data...
A. Queue
B. Stack (atau Rekursi)
C. Linked List
D. Matrix

<details><summary>💡 Hint</summary>DFS = mendalam = LIFO = tumpukan.</details>
<details><summary>✅ Jawaban</summary>**B. Stack (atau Rekursi).**</details>

### Soal #155: BFS Layer 1
```
    A
   / \
  B   C
 / \   \
D   E   F
```
BFS dari A. Vertex mana yang ada di Layer 1?
A. A
B. B dan C
C. D, E, dan F
D. Semua

<details><summary>💡 Hint</summary>Layer 0 = A. Layer 1 = tetangga langsung A.</details>
<details><summary>✅ Jawaban</summary>**B. B dan C.**</details>

### Soal #156: BFS - Urutan Kunjungan
Dari soal #155, urutan kunjungan BFS dari A adalah...
A. A, B, D, E, C, F
B. A, B, C, D, E, F
C. A, C, F, B, D, E
D. F, E, D, C, B, A

<details><summary>💡 Hint</summary>Layer 0: A. Layer 1: B, C. Layer 2: D, E, F.</details>
<details><summary>✅ Jawaban</summary>**B. A, B, C, D, E, F.**</details>

### Soal #157: DFS - Urutan Kunjungan
Dari soal #155, salah satu urutan DFS dari A (pilih kiri dulu) adalah...
A. A, B, C, D, E, F
B. A, B, D, E, C, F
C. A, C, F, B, D, E
D. D, E, B, F, C, A

<details><summary>💡 Hint</summary>DFS: A → B (kiri dulu) → D (sedalam mungkin) → mundur → E → mundur → C → F.</details>
<details><summary>✅ Jawaban</summary>**B. A, B, D, E, C, F.**</details>

### Soal #158: BFS - Jarak Terpendek
```
    A
   / \
  B   C
 / \   \
D   E   F
```
Berapa jarak terpendek (jumlah edge) dari A ke F?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>BFS: A → C → F = 2 langkah.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #159: BFS vs DFS - Kapan BFS?
Kamu ingin mencari jarak TERPENDEK (jumlah langkah minimum). Pakai apa?
A. DFS
B. BFS
C. Keduanya sama
D. Tidak bisa

<details><summary>💡 Hint</summary>BFS menjelajah layer by layer, jadi layer pertama ketemu = terpendek.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

### Soal #160: BFS vs DFS - Kapan DFS?
Kamu ingin mencari SEMUA kemungkinan jalur dari A ke Z. Pakai apa?
A. BFS
B. DFS
C. Keduanya
D. Spanning Tree

<details><summary>💡 Hint</summary>DFS menelusuri sedalam mungkin, cocok untuk eksplorasi semua jalur.</details>
<details><summary>✅ Jawaban</summary>**B. DFS.**</details>

### Soal #161: BFS Queue - Step by Step
```
A --- B
|     |
C --- D
```
BFS dari A. Isi Queue setelah memproses A?
A. [B, C]
B. [C, D]
C. [A, B]
D. [D]

<details><summary>💡 Hint</summary>A dikeluarkan, tetangganya (B, C) dimasukkan.</details>
<details><summary>✅ Jawaban</summary>**A. [B, C].**</details>

### Soal #162: BFS Queue - Lanjutan
Dari soal #161, isi Queue setelah memproses B (B keluar)?
A. [C]
B. [C, D]
C. [D, C]
D. [C, A]

<details><summary>💡 Hint</summary>B keluar. Tetangga B: A(sudah dikunjungi), D(baru). Queue: C masih ada, D masuk.</details>
<details><summary>✅ Jawaban</summary>**B. [C, D].**</details>

### Soal #163: DFS Stack - Step by Step
```
A --- B --- C
      |
      D
```
DFS dari A (pakai Stack). Isi Stack setelah push A?
A. [A]
B. [B]
C. [A, B]
D. Kosong

<details><summary>💡 Hint</summary>Awal: push titik start.</details>
<details><summary>✅ Jawaban</summary>**A. [A].**</details>

### Soal #164: DFS - Backtrack
```
A --- B
|
C --- D
```
DFS dari A (pilih B dulu): A → B. B buntu (semua tetangga sudah dikunjungi). Apa yang terjadi?
A. Berhenti
B. Backtrack ke A, lalu ke C
C. Lompat ke D
D. Restart

<details><summary>💡 Hint</summary>DFS: buntu → mundur ke persimpangan terakhir.</details>
<details><summary>✅ Jawaban</summary>**B. Backtrack ke A, lalu ke C.**</details>

### Soal #165: BFS - Analogi Riak Air
BFS diibaratkan seperti...
A. Labirin (jalan terus sampai buntu)
B. Riak air (menyebar merata dari pusat)
C. Anak tangga (naik satu per satu)
D. Pohon terbalik

<details><summary>💡 Hint</summary>Breadth = melebar = menyebar ke segala arah.</details>
<details><summary>✅ Jawaban</summary>**B. Riak air.**</details>

### Soal #166: DFS - Analogi Labirin
DFS diibaratkan seperti...
A. Riak air
B. Orang tersesat di labirin (jalan terus lalu mundur jika buntu)
C. Antrian bank
D. Lift naik turun

<details><summary>💡 Hint</summary>Depth = mendalam = terus ke satu arah sebisa mungkin.</details>
<details><summary>✅ Jawaban</summary>**B. Orang tersesat di labirin.**</details>

### Soal #167: BFS - Level/Lapisan
```
      1
     /|\
    2 3 4
   /|   |
  5 6   7
```
BFS dari 1. Vertex 5, 6, 7 ada di lapisan ke-berapa?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>Layer 0: 1. Layer 1: 2,3,4. Layer 2: 5,6,7.</details>
<details><summary>✅ Jawaban</summary>**C. 2.**</details>

### Soal #168: BFS - Jumlah Langkah
Dari soal #167, berapa langkah dari vertex 1 ke vertex 7?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>1 → 4 → 7 = 2 langkah.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #169: DFS - Urutan di Tree
```
      1
     / \
    2   3
   / \
  4   5
```
DFS dari 1 (pilih kiri dulu): ?
A. 1, 2, 4, 5, 3
B. 1, 2, 3, 4, 5
C. 1, 3, 2, 4, 5
D. 4, 5, 2, 3, 1

<details><summary>💡 Hint</summary>1 → 2 (kiri) → 4 (kiri, buntu) → 5 (mundur, kanan) → 3 (mundur ke 1, kanan).</details>
<details><summary>✅ Jawaban</summary>**A. 1, 2, 4, 5, 3.**</details>

### Soal #170: BFS - Connected Check
Jika BFS dari vertex manapun mengunjungi SEMUA vertex, maka graf tersebut...
A. Punya Euler Path
B. Connected (terhubung)
C. Punya Hamilton Path
D. Adalah Tree

<details><summary>💡 Hint</summary>BFS menjangkau semua = semua bisa dijangkau = connected.</details>
<details><summary>✅ Jawaban</summary>**B. Connected.**</details>

### Soal #171: DFS - Cycle Detection
Jika saat DFS kamu menemukan vertex yang SUDAH dikunjungi (bukan parent), apa artinya?
A. Graf adalah tree
B. Ada cycle (siklus)
C. Graf disconnected
D. BFS lebih baik

<details><summary>💡 Hint</summary>Sudah dikunjungi + bukan parent = ada jalan "memutar".</details>
<details><summary>✅ Jawaban</summary>**B. Ada cycle.**</details>

### Soal #172: BFS - Social Media
Fitur "Orang yang mungkin kamu kenal" di Facebook menggunakan konsep...
A. DFS
B. BFS (teman dari teman = layer 2)
C. Euler Path
D. MST

<details><summary>💡 Hint</summary>Teman kamu = Layer 1. Teman dari teman = Layer 2.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

### Soal #173: DFS - File Explorer
Membuka folder → subfolder → sub-subfolder secara mendalam mirip dengan...
A. BFS
B. DFS
C. Euler Path
D. Hamilton

<details><summary>💡 Hint</summary>Masuk sedalam mungkin ke folder, baru mundur ke folder lain.</details>
<details><summary>✅ Jawaban</summary>**B. DFS.**</details>

### Soal #174: BFS - Virus Spread
Memodelkan penyebaran virus (hari 1: pasien pertama menulari tetangga, hari 2: tetangga menulari tetangga mereka) mirip...
A. DFS
B. BFS (layer = hari)
C. Hamilton
D. MST

<details><summary>💡 Hint</summary>Setiap "hari" = 1 layer BFS.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.** Layer 0: pasien 0. Layer 1: orang yang tertular hari 1. Dst.</details>

### Soal #175: DFS - Maze Solver
Robot yang menjelajahi labirin (jalan terus, buntu → putar balik) menggunakan...
A. BFS
B. DFS
C. MST
D. Euler

<details><summary>💡 Hint</summary>Jalan terus sedalam mungkin + backtrack = DFS.</details>
<details><summary>✅ Jawaban</summary>**B. DFS.**</details>

### Soal #176: BFS - Bipartite Check
BFS bisa digunakan untuk mengecek apakah graf adalah bipartite. Caranya: warnai vertex bergantian 2 warna saat BFS. Jika ada konflik warna, berarti...
A. Graf bipartite
B. Graf BUKAN bipartite
C. Graf connected
D. Ada Euler Path

<details><summary>💡 Hint</summary>Konflik = dua tetangga punya warna sama = tidak bisa dibagi 2 grup.</details>
<details><summary>✅ Jawaban</summary>**B. Graf BUKAN bipartite.**</details>

### Soal #177: BFS dari Vertex Berbeda
```
A --- B --- C
|         /
D -------
```
BFS dari D. Urutan?
A. D, A, C, B
B. D, A, B, C
C. D, C, A, B
D. Bisa D,A,C,B atau D,C,A,B (tergantung urutan tetangga)

<details><summary>💡 Hint</summary>D terhubung ke A dan C (layer 1). Lalu B (layer 2). Tapi urutan A dulu atau C dulu tergantung implementasi.</details>
<details><summary>✅ Jawaban</summary>**D.** Bisa variasi, yang penting layer benar.</details>

### Soal #178: DFS - Multiple Path
```
A --- B
|     |
C --- D
```
Ada berapa jalur (tanpa mengulang vertex) dari A ke D?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>A→B→D dan A→C→D.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #179: BFS Tree
Saat BFS dijalankan, edge yang digunakan untuk menemukan vertex baru membentuk sebuah...
A. Cycle
B. Spanning Tree (BFS Tree)
C. Complete Graph
D. Bipartite Graph

<details><summary>💡 Hint</summary>BFS mengunjungi semua vertex tanpa cycle → tree!</details>
<details><summary>✅ Jawaban</summary>**B. Spanning Tree (BFS Tree).**</details>

### Soal #180: DFS - Pre-order
Dalam DFS di tree, urutan "pre-order" berarti...
A. Kunjungi root terakhir
B. Kunjungi root DULUAN, baru anak-anaknya
C. Kunjungi anak-anak dulu, baru root
D. Kunjungi dari kanan

<details><summary>💡 Hint</summary>Pre = sebelum = root dikunjungi SEBELUM anaknya.</details>
<details><summary>✅ Jawaban</summary>**B. Kunjungi root duluan.**</details>

### Soal #181: BFS - Diameter
Diameter graf bisa dihitung dengan BFS dari vertex manapun. Diameter = ...
A. Jarak terpendek antara 2 vertex terdekat
B. Jarak terpendek terpanjang antara semua pasangan vertex
C. Jumlah vertex
D. Jumlah edge

<details><summary>💡 Hint</summary>Diameter = "paling jauh" di antara semua "paling dekat".</details>
<details><summary>✅ Jawaban</summary>**B.** Diameter = maximum shortest path distance.</details>

### Soal #182: BFS - Weighted Graph?
BFS menemukan jarak terpendek di graf berbobot?
A. Ya, selalu
B. Tidak (hanya benar di graf tak berbobot)
C. Hanya di tree
D. Tergantung

<details><summary>💡 Hint</summary>BFS menghitung jumlah EDGE, bukan total BOBOT. Untuk weighted gunakan Dijkstra.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** BFS hanya benar untuk shortest path di graf tak berbobot.</details>

### Soal #183: DFS - Topological Sort
Di directed acyclic graph (DAG), DFS bisa digunakan untuk mengurutkan vertex sedemikian rupa sehingga semua edge menunjuk ke arah yang sama. Ini disebut...
A. BFS
B. Topological Sort
C. Euler Path
D. Hamilton Path

<details><summary>💡 Hint</summary>Mengurutkan "dari yang paling independen ke yang paling bergantung".</details>
<details><summary>✅ Jawaban</summary>**B. Topological Sort.**</details>

### Soal #184: BFS - Shortest Path Count
```
    A
   / \
  B   C
   \ /
    D
```
BFS dari A. Berapa banyak shortest path dari A ke D?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>A→B→D dan A→C→D. Keduanya 2 langkah.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #185: DFS - Stack Kosong
Kapan DFS berhenti?
A. Stack penuh
B. Stack kosong (semua sudah dikunjungi)
C. Menemukan cycle
D. Setelah 10 langkah

<details><summary>💡 Hint</summary>DFS selesai ketika tidak ada lagi vertex yang perlu dikunjungi.</details>
<details><summary>✅ Jawaban</summary>**B. Stack kosong.**</details>

### Soal #186: BFS - Undirected Connected
BFS dari vertex A di graf connected akan mengunjungi...
A. Hanya tetangga A
B. Hanya layer 1 dan 2
C. SEMUA vertex
D. Hanya setengah vertex

<details><summary>💡 Hint</summary>Connected + BFS = semua terjangkau.</details>
<details><summary>✅ Jawaban</summary>**C. Semua vertex.**</details>

### Soal #187: DFS di Directed Graph
```
A --> B --> C
      |
      v
      D
```
DFS dari A. Urutan?
A. A, B, C, D atau A, B, D, C
B. A, C, B, D
C. D, C, B, A
D. A saja (B tidak terjangkau)

<details><summary>💡 Hint</summary>A→B (panah ada). Dari B: B→C dan B→D. Tergantung mana dulu.</details>
<details><summary>✅ Jawaban</summary>**A.** A→B→C→D atau A→B→D→C (tergantung urutan tetangga).</details>

### Soal #188: Unreachable Vertex
```
A --> B    C --> D
```
BFS dari A. Vertex mana yang TIDAK terjangkau?
A. B
B. C dan D
C. A
D. Semua terjangkau

<details><summary>💡 Hint</summary>Tidak ada panah dari komponen A-B ke komponen C-D.</details>
<details><summary>✅ Jawaban</summary>**B. C dan D.**</details>

### Soal #189: BFS Level Count
```
      1
     /|\
    2 3 4
   /|   |\
  5 6   7 8
```
BFS dari 1. Berapa vertex di Layer 2?
A. 2
B. 3
C. 4
D. 5

<details><summary>💡 Hint</summary>Layer 0: {1}. Layer 1: {2,3,4}. Layer 2: {5,6,7,8}.</details>
<details><summary>✅ Jawaban</summary>**C. 4.**</details>

### Soal #190: DFS - Numbering
DFS memberi "discovery time" pada setiap vertex. Vertex pertama yang ditemukan mendapat nomor...
A. 0 atau 1
B. V (jumlah vertex)
C. Acak
D. Negatif

<details><summary>💡 Hint</summary>Discovery dimulai dari 1 (atau 0).</details>
<details><summary>✅ Jawaban</summary>**A. 0 atau 1** (tergantung implementasi).</details>

### Soal #191: BFS - Game AI
Dalam game, NPC mencari jarak terpendek ke player. Algoritma yang cocok...
A. DFS
B. BFS (untuk graf tanpa bobot)
C. Random walk
D. Euler Path

<details><summary>💡 Hint</summary>Jarak terpendek (tanpa bobot) = BFS.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

### Soal #192: DFS - Sudoku
Memecahkan puzzle Sudoku dengan mencoba angka satu per satu (jika salah → backtrack) mirip...
A. BFS
B. DFS + Backtracking
C. Euler Circuit
D. MST

<details><summary>💡 Hint</summary>Coba sedalam mungkin, salah → mundur = DFS.</details>
<details><summary>✅ Jawaban</summary>**B. DFS + Backtracking.**</details>

### Soal #193: Perbandingan Memori
Manakah yang biasanya lebih hemat memori?
A. BFS
B. DFS
C. Sama saja
D. Tergantung network

<details><summary>💡 Hint</summary>BFS menyimpan semua vertex di satu layer. DFS hanya menyimpan satu jalur.</details>
<details><summary>✅ Jawaban</summary>**B. DFS.** DFS hanya menyimpan path dari root ke node saat ini.</details>

### Soal #194: BFS - Time Complexity
Waktu eksekusi BFS pada graf dengan V vertex dan E edge adalah...
A. O(V)
B. O(E)
C. O(V + E)
D. O(V × E)

<details><summary>💡 Hint</summary>Setiap vertex dan edge dikunjungi tepat sekali.</details>
<details><summary>✅ Jawaban</summary>**C. O(V + E).**</details>

### Soal #195: DFS - Time Complexity
Waktu eksekusi DFS?
A. O(V²)
B. O(V + E)
C. O(E²)
D. O(V × E)

<details><summary>💡 Hint</summary>Sama dengan BFS.</details>
<details><summary>✅ Jawaban</summary>**B. O(V + E).**</details>

### Soal #196: BFS vs DFS - Completeness
Manakah yang PASTI menemukan vertex tujuan (jika ada)?
A. BFS saja
B. DFS saja
C. Keduanya (di graf finite)
D. Tidak ada yang pasti

<details><summary>💡 Hint</summary>Di graf yang terbatas (finite), keduanya pasti menjangkau semua vertex.</details>
<details><summary>✅ Jawaban</summary>**C. Keduanya** (di graf finite/terbatas).</details>

### Soal #197: BFS - Multi-Source
Jika BFS dimulai dari BEBERAPA vertex sekaligus (semua masuk Queue di awal), ini disebut...
A. Multi-source BFS
B. DFS  
C. Euler Path
D. Hamilton Path

<details><summary>💡 Hint</summary>Bayangkan beberapa batu dijatuhkan ke kolam bersamaan → riak dari banyak sumber.</details>
<details><summary>✅ Jawaban</summary>**A. Multi-source BFS.**</details>

### Soal #198: DFS - Strongly Connected
Di directed graph, DFS dua kali bisa digunakan untuk mencari komponen yang "strongly connected". Strongly connected artinya...
A. Semua vertex berderajat genap
B. Ada jalur dari setiap vertex ke setiap vertex lain (mengikuti arah panah)
C. Semua vertex punya self-loop
D. Graf tidak punya cycle

<details><summary>💡 Hint</summary>Strong = kuat. Dari A bisa ke B, dan dari B bisa ke A.</details>
<details><summary>✅ Jawaban</summary>**B.**</details>

### Soal #199: BFS - Shortest in Grid
Di papan catur 8×8, BFS dari kuda (knight) bisa menghitung minimum langkah ke kotak tujuan. Ini karena...
A. BFS selalu menemukan jalur terpendek di graf tak berbobot
B. Kuda hanya bisa bergerak lurus
C. Papan catur adalah tree
D. DFS lebih cocok

<details><summary>💡 Hint</summary>Setiap langkah kuda = 1 "cost". BFS = shortest path.</details>
<details><summary>✅ Jawaban</summary>**A.** BFS menjamin shortest path di graf tak berbobot.</details>

### Soal #200: Refleksi Bagian 4
Untuk soal "berapa langkah minimum dari A ke B" di graf TANPA bobot, algoritma terbaik adalah...
A. DFS
B. BFS
C. Euler Path
D. MST

<details><summary>💡 Hint</summary>Langkah minimum = shortest path = BFS!</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

---
[< Bagian 3 (101-150)](./07-graf-soal-part-3.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 5 (201-250) >](./07-graf-soal-part-5.md)
