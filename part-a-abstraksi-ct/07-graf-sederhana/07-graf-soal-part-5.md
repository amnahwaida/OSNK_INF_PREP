🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Latihan Soal Bagian 5 (Soal 201-250)
## Topik: Spanning Tree, MST, dan Aplikasi Graf

[< Bagian 4 (151-200)](./07-graf-soal-part-4.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 6 (251-300) >](./07-graf-soal-part-6.md)

---

### Soal #201: Spanning Tree - Definisi
Spanning Tree adalah subgraph yang...
A. Menghubungkan semua vertex, tanpa cycle, punya V-1 edge
B. Menghubungkan sebagian vertex
C. Punya cycle
D. Punya V edge

<details><summary>💡 Hint</summary>Spanning = mencakup semua. Tree = tanpa cycle.</details>
<details><summary>✅ Jawaban</summary>**A.**</details>

### Soal #202: Jumlah Edge di Spanning Tree
Graf punya 10 vertex. Spanning tree-nya punya berapa edge?
A. 8
B. 9
C. 10
D. 11

<details><summary>💡 Hint</summary>E = V - 1 = 10 - 1.</details>
<details><summary>✅ Jawaban</summary>**B. 9.**</details>

### Soal #203: MST - Definisi
Minimum Spanning Tree (MST) adalah spanning tree dengan...
A. Jumlah edge terbanyak
B. Total bobot terkecil
C. Total bobot terbesar
D. Jumlah vertex terbanyak

<details><summary>💡 Hint</summary>Minimum = paling kecil. Bobot = angka di edge.</details>
<details><summary>✅ Jawaban</summary>**B. Total bobot terkecil.**</details>

### Soal #204: MST - Analogi PLN
PLN ingin pasang kabel ke semua rumah dengan biaya kabel paling murah. Ini adalah masalah...
A. Euler Path
B. Hamilton Circuit
C. Minimum Spanning Tree
D. BFS

<details><summary>💡 Hint</summary>Hubungkan semua (spanning) + biaya minimum = MST.</details>
<details><summary>✅ Jawaban</summary>**C. Minimum Spanning Tree.**</details>

### Soal #205: MST - Hitung
```
A --3-- B
|     / |
5   2   4
|  /    |
C --6-- D
```
Edge: A-B(3), A-C(5), B-C(2), B-D(4), C-D(6). MST = ?
A. B-C(2), A-B(3), B-D(4) = 9
B. A-B(3), B-C(2), C-D(6) = 11
C. A-C(5), B-D(4), B-C(2) = 11
D. A-B(3), A-C(5), B-D(4) = 12

<details><summary>💡 Hint</summary>Ambil edge termurah dulu: 2, 3, 4. Cek tidak ada cycle. 3 edge = V-1 = 3. ✓</details>
<details><summary>✅ Jawaban</summary>**A. Total bobot = 9.**</details>

### Soal #206: MST - Kruskal
Algoritma Kruskal mencari MST dengan cara...
A. Ambil vertex termurah dulu
B. Urutkan semua edge dari terkecil, ambil satu per satu asal tidak membuat cycle
C. BFS dari vertex terkecil
D. Hapus edge termahal satu per satu

<details><summary>💡 Hint</summary>Kruskal = greedy, ambil edge terkecil yang aman.</details>
<details><summary>✅ Jawaban</summary>**B.**</details>

### Soal #207: MST - Prim
Algoritma Prim mencari MST dengan cara...
A. Mulai dari satu vertex, terus tambahkan edge termurah yang menghubungkan vertex baru
B. Urutkan semua edge
C. DFS biasa
D. Hamilton Path

<details><summary>💡 Hint</summary>Prim = tumbuh dari satu titik, selalu pilih edge terkecil ke vertex baru.</details>
<details><summary>✅ Jawaban</summary>**A.**</details>

### Soal #208: MST - Unique?
Jika semua bobot edge BERBEDA, berapa MST yang mungkin?
A. Bisa banyak
B. Tepat 1
C. 0
D. Tergantung vertex

<details><summary>💡 Hint</summary>Jika semua bobot unik, MST pasti unik.</details>
<details><summary>✅ Jawaban</summary>**B. Tepat 1.** Jika semua bobot berbeda, MST unik.</details>

### Soal #209: MST - Cycle Property
Jika ada cycle di graf, edge dengan bobot TERBESAR di cycle itu pasti...
A. Masuk MST
B. TIDAK masuk MST
C. Mungkin masuk
D. Harus dihapus dari graf

<details><summary>💡 Hint</summary>Di cycle, kita selalu bisa buang edge terberat dan tetap connected.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak masuk MST.**</details>

### Soal #210: Spanning Tree - Jumlah Kemungkinan
```
A --- B
|     |
C --- D
```
Berapa spanning tree berbeda yang mungkin dari graf ini?
A. 2
B. 3
C. 4
D. 6

<details><summary>💡 Hint</summary>4 edge, perlu 3 (V-1). Buang 1 dari 4 edge, asal tetap connected. Tapi buang A-B: masih connected? Ya. Buang A-C: Ya. Buang B-D: Ya. Buang C-D: Ya. Semua 4 cara valid!</details>
<details><summary>✅ Jawaban</summary>**C. 4.** (Setiap edge bisa dibuang dan sisanya tetap spanning tree.)</details>

### Soal #211: Analogi - Jaringan WiFi
Menghubungkan semua ruangan kantor dengan WiFi repeater, pakai kabel sesedikit mungkin. Masalah...
A. BFS
B. MST
C. Euler
D. Hamilton

<details><summary>💡 Hint</summary>Hubungkan semua + minimum biaya = MST.</details>
<details><summary>✅ Jawaban</summary>**B. MST.**</details>

### Soal #212: Spanning Tree - Apakah Unique?
Sebuah graf bisa punya LEBIH DARI SATU spanning tree?
A. Ya
B. Tidak
C. Hanya jika weighted
D. Hanya jika tree

<details><summary>💡 Hint</summary>Banyak cara untuk menghubungkan semua vertex tanpa cycle.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Bisa ada banyak spanning tree berbeda.</details>

### Soal #213: MST - Total Bobot
```
A--1--B--4--C
|           |
2           3
|           |
D----5-----E
```
MST-nya adalah...
A. A-B(1), A-D(2), C-E(3), B-C(4) = 10
B. A-B(1), A-D(2), B-C(4), C-E(3) = 10
C. A-B(1), A-D(2), C-E(3), D-E(5) = 11
D. A dan B sama saja, total 10

<details><summary>💡 Hint</summary>5 vertex butuh 4 edge. Urut: 1, 2, 3, 4, 5. Ambil 1(A-B), 2(A-D), 3(C-E), 4(B-C). Cek connected & no cycle ✓.</details>
<details><summary>✅ Jawaban</summary>**D. Total bobot = 10.** (Opsi A dan B = cara tulis berbeda tapi sama).</details>

### Soal #214: MST - Menolak Edge
Saat membangun MST dengan Kruskal, kapan sebuah edge DITOLAK?
A. Jika bobotnya genap
B. Jika menambahkannya akan membuat cycle
C. Jika vertex sudah ada di tree
D. Jika bobotnya lebih dari rata-rata

<details><summary>💡 Hint</summary>Tree = tidak boleh ada cycle.</details>
<details><summary>✅ Jawaban</summary>**B. Jika menambahkannya akan membuat cycle.**</details>

### Soal #215: Aplikasi - Peta Kota
Vertex = persimpangan, Edge = jalan, Bobot = waktu tempuh. Mencari rute tercepat dari rumah ke sekolah adalah masalah...
A. MST
B. Shortest Path
C. Euler Path
D. Spanning Tree

<details><summary>💡 Hint</summary>Rute tercepat = shortest path (jalur terpendek).</details>
<details><summary>✅ Jawaban</summary>**B. Shortest Path.**</details>

### Soal #216: Dijkstra vs BFS
Dijkstra digunakan untuk shortest path di graf __ , sedangkan BFS di graf __ .
A. berbobot; tak berbobot
B. tak berbobot; berbobot
C. keduanya berbobot
D. keduanya tak berbobot

<details><summary>💡 Hint</summary>BFS menghitung langkah (tanpa bobot). Dijkstra menghitung total bobot.</details>
<details><summary>✅ Jawaban</summary>**A. berbobot; tak berbobot.**</details>

### Soal #217: Aplikasi - PageRank
Google menentukan ranking website berdasarkan graf website. Vertex = website, Edge = link. Semakin banyak website lain yang mengarah (link) ke sebuah website, maka rankingnya...
A. Semakin rendah
B. Semakin tinggi (in-degree tinggi)
C. Tidak berpengaruh
D. Website dihapus

<details><summary>💡 Hint</summary>In-degree tinggi = banyak "rekomendasi" = informasi penting.</details>
<details><summary>✅ Jawaban</summary>**B. Semakin tinggi.**</details>

### Soal #218: Coloring Problem
Mewarnai peta agar negara bertetangga punya warna berbeda. Ini adalah masalah...
A. Euler
B. Graph Coloring
C. MST
D. Hamilton

<details><summary>💡 Hint</summary>Warnai vertex (negara) agar tetangga beda warna.</details>
<details><summary>✅ Jawaban</summary>**B. Graph Coloring.**</details>

### Soal #219: Four Color Theorem
Berapa warna minimum yang pasti cukup untuk mewarnai peta apapun?
A. 2
B. 3
C. 4
D. 5

<details><summary>💡 Hint</summary>Teorema 4 warna: setiap peta planar cukup dengan 4 warna.</details>
<details><summary>✅ Jawaban</summary>**C. 4.**</details>

### Soal #220: Chromatic Number - C3
Berapa warna minimum untuk mewarnai cycle C3 (segitiga)?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>3 vertex saling bertetangga → butuh 3 warna berbeda.</details>
<details><summary>✅ Jawaban</summary>**C. 3.**</details>

### Soal #221: Chromatic Number - Bipartite
Berapa warna minimum untuk graf bipartite?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Bipartite = 2 grup, edge hanya antar grup. Warnai tiap grup 1 warna.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #222: Matching Problem
Mencocokkan siswa dengan tutor agar setiap siswa punya tepat 1 tutor. Ini adalah masalah...
A. Euler Path
B. Maximum Matching di bipartite graph
C. MST
D. DFS

<details><summary>💡 Hint</summary>Mencocokkan 1-1 = matching di bipartite graph.</details>
<details><summary>✅ Jawaban</summary>**B. Maximum Matching.**</details>

### Soal #223: Network Flow
Air mengalir dari sumber ke tujuan melalui pipa dengan kapasitas berbeda. Berapa aliran maksimum? Ini masalah...
A. MST
B. Maximum Flow (Network Flow)
C. Euler Circuit
D. Hamilton Path

<details><summary>💡 Hint</summary>Aliran maksimum = max flow.</details>
<details><summary>✅ Jawaban</summary>**B. Maximum Flow.**</details>

### Soal #224: Aplikasi - Jadwal Ujian
Mata pelajaran = vertex. Edge jika ada siswa yang mengambil kedua mapel (tidak boleh ujian bersamaan). Warnai graf agar tetangga beda warna. Setiap WARNA = 1 slot ujian. Minimumkan warna = minimumkan...
A. Jumlah ujian
B. Jumlah slot waktu ujian
C. Jumlah siswa
D. Jumlah ruangan

<details><summary>💡 Hint</summary>Warna = slot waktu ujian yang tidak bentrok.</details>
<details><summary>✅ Jawaban</summary>**B. Jumlah slot waktu ujian.**</details>

### Soal #225: Shortest Path Negatif
Dijkstra TIDAK bisa digunakan jika graf punya...
A. Banyak vertex
B. Bobot negatif
C. Cycle
D. Directed edge

<details><summary>💡 Hint</summary>Dijkstra mengasumsikan semua bobot positif.</details>
<details><summary>✅ Jawaban</summary>**B. Bobot negatif.** Gunakan Bellman-Ford untuk bobot negatif.</details>

### Soal #226: MST vs Shortest Path
MST menghubungkan SEMUA vertex dengan total bobot minimum. Shortest Path mencari rute terbaik antara __ vertex.
A. Semua
B. 2 (satu pasang)
C. Hanya vertex ganjil
D. Hanya leaf

<details><summary>💡 Hint</summary>MST = semua vertex. Shortest path = dari A ke B.</details>
<details><summary>✅ Jawaban</summary>**B. 2 vertex (satu pasang).**</details>

### Soal #227: Aplikasi - Routing Internet
Router internet mengirim data melalui graf jaringan. Setiap router = vertex, kabel = edge, delay = bobot. Untuk meminimalkan delay, router menggunakan...
A. BFS
B. Shortest Path (misal Dijkstra)
C. MST
D. Euler Circuit

<details><summary>💡 Hint</summary>Minimalkan delay dari sumber ke tujuan = shortest path.</details>
<details><summary>✅ Jawaban</summary>**B. Shortest Path.**</details>

### Soal #228: Analogi - Skill Tree Game
Skill Tree di game RPG (unlock Skill A sebelum B) adalah contoh...
A. Undirected Graph
B. Directed Acyclic Graph (DAG)
C. Complete Graph
D. Cycle Graph

<details><summary>💡 Hint</summary>Ada urutan (directed), tidak boleh circular dependency (acyclic).</details>
<details><summary>✅ Jawaban</summary>**B. DAG.** Directed (ada urutan) dan Acyclic (tidak boleh memutar).</details>

### Soal #229: MST - Kruskal Step
Edge diurutkan: 1, 2, 3, 4, 5, 6. V = 4. Kruskal ambil edge berapa saja?
A. 1, 2, 3 (3 edge = V-1, tanpa cycle)
B. 4, 5, 6
C. 1, 6
D. Semua

<details><summary>💡 Hint</summary>Ambil 3 edge terkecil, asal tidak membuat cycle.</details>
<details><summary>✅ Jawaban</summary>**A. 1, 2, 3** (asumsi tidak ada cycle).</details>

### Soal #230: Topological Sort
Di DAG jadwal mata kuliah (harus ambil Matematika sebelum Fisika), urutan pengambilan yang valid disebut...
A. BFS Order
B. DFS Order
C. Topological Order
D. Euler Order

<details><summary>💡 Hint</summary>Mengurutkan agar semua prasyarat terpenuhi = topological sort.</details>
<details><summary>✅ Jawaban</summary>**C. Topological Order.**</details>

### Soal #231: Analogi - Dependency
```
Install NodeJS --> Install NPM --> Install React
```
Urutan instalasi ini membentuk...
A. Cycle
B. DAG (Directed Acyclic Graph)
C. Undirected Graph
D. Complete Graph

<details><summary>💡 Hint</summary>Ada urutan dependencies, tidak boleh circular.</details>
<details><summary>✅ Jawaban</summary>**B. DAG.**</details>

### Soal #232: Spanning Forest
Jika graf punya 3 komponen: {A,B,C}, {D,E}, {F}. Spanning forest punya berapa edge?
A. 2 + 1 + 0 = 3
B. 3 + 2 + 1 = 6
C. 5
D. 0

<details><summary>💡 Hint</summary>Tiap komponen jadi tree: (3-1)+(2-1)+(1-1) = 2+1+0.</details>
<details><summary>✅ Jawaban</summary>**A. 3 edge.**</details>

### Soal #233: MST - Tie Breaking
Jika 2 edge punya bobot SAMA saat Kruskal, mana yang dipilih?
A. Yang paling kiri
B. Bebas (keduanya valid, mungkin menghasilkan MST berbeda)
C. Yang paling kanan
D. Tidak boleh ada bobot sama

<details><summary>💡 Hint</summary>Jika bobot sama, MST bisa tidak unik.</details>
<details><summary>✅ Jawaban</summary>**B. Bebas.** Bisa menghasilkan MST berbeda tapi total bobot tetap sama.</details>

### Soal #234: Aplikasi - Clustering
Mengelompokkan data berdasarkan "kedekatan" bisa dilakukan dengan MST lalu memotong edge terberat. Ini disebut...
A. MST-based clustering
B. BFS grouping
C. Euler partitioning
D. Hamilton splitting

<details><summary>💡 Hint</summary>Potong edge terberat di MST = pisahkan jadi cluster.</details>
<details><summary>✅ Jawaban</summary>**A. MST-based clustering.**</details>

### Soal #235: Planar & K3,3
K3,3 (complete bipartite 3,3) adalah graf yang...
A. Planar
B. Tidak planar (tidak bisa digambar tanpa crossing)
C. Tree
D. Cycle

<details><summary>💡 Hint</summary>Kuratowski: K5 dan K3,3 tidak planar.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak planar.**</details>

### Soal #236: Planar & K5
Apakah K5 planar?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>K5 = 5 vertex semua saling terhubung. Tidak bisa digambar tanpa crossing.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.**</details>

### Soal #237: Euler Formula (Planar)
Untuk graf planar connected: V - E + F = ?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>Euler's polyhedron formula. V=vertex, E=edge, F=face(region).</details>
<details><summary>✅ Jawaban</summary>**C. 2.** V - E + F = 2.</details>

### Soal #238: Faces in Planar Graf
Graf planar: V=4, E=6. Berapa faces (F)?
A. 2
B. 3
C. 4
D. 5

<details><summary>�� Hint</summary>F = 2 - V + E = 2 - 4 + 6.</details>
<details><summary>✅ Jawaban</summary>**C. 4.**</details>

### Soal #239: Analogi - Pipa Air
```
Sumber --5-- A --3-- B --4-- Tujuan
              |             |
              2             6
              |             |
              C -----7----- D
```
Berapa MST total bobot?
A. 14
B. 16
C. 20
D. 27

<details><summary>💡 Hint</summary>6 vertex, butuh 5 edge. Urutkan: 2, 3, 4, 5, 6, 7. Ambil 2+3+4+5+6=20? Cek cycle!</details>
<details><summary>✅ Jawaban</summary>**A. 14.** Ambil edge terkecil tanpa cycle: 2(A-C)+3(A-B)+4(B-Tujuan)+5(Sumber-A) = 14, lalu tambah 1 edge lagi yang connect D tanpa cycle.</details>

### Soal #240: Aplikasi - Social Network Analysis
Vertex dengan derajat tertinggi di social network disebut...
A. Influencer / Hub
B. Leaf
C. Bridge
D. Root

<details><summary>�� Hint</summary>Derajat tinggi = banyak koneksi = berpengaruh.</details>
<details><summary>✅ Jawaban</summary>**A. Influencer / Hub.**</details>

### Soal #241: Betweenness Centrality
Vertex yang PALING SERING dilewati oleh shortest path antar vertex lain punya __ tinggi.
A. Degree
B. Betweenness Centrality
C. Eccentricity
D. Weight

<details><summary>💡 Hint</summary>Between = di antara. Centrality = pusat.</details>
<details><summary>✅ Jawaban</summary>**B. Betweenness Centrality.** Vertex "persimpangan" penting.</details>

### Soal #242: MST - Analogi Jaringan Telepon
Menghubungkan 5 desa dengan kabel telepon, biaya kabel proporsional dengan jarak. Minimalkan biaya = ...
A. Shortest Path
B. MST
C. Euler Circuit
D. Hamilton Path

<details><summary>💡 Hint</summary>Hubungkan SEMUA desa + biaya minimum = MST.</details>
<details><summary>✅ Jawaban</summary>**B. MST.**</details>

### Soal #243: Biconnected Component
Graf biconnected adalah graf connected yang tetap connected meskipun satu vertex manapun dihapus. Artinya, graf ini TIDAK punya...
A. Edge
B. Cycle
C. Cut vertex (articulation point)
D. Spanning tree

<details><summary>💡 Hint</summary>Biconnected = tidak ada titik yang jika dihapus memutuskan graf.</details>
<details><summary>✅ Jawaban</summary>**C. Cut vertex.**</details>

### Soal #244: MST Kruskal - Implementasi
Untuk mengecek apakah menambahkan edge akan membuat cycle, Kruskal biasanya menggunakan struktur data...
A. Queue
B. Stack
C. Union-Find (Disjoint Set)
D. Linked List

<details><summary>💡 Hint</summary>Union-Find mengelompokkan vertex yang sudah terhubung.</details>
<details><summary>✅ Jawaban</summary>**C. Union-Find.**</details>

### Soal #245: Graph vs Digraph Edge Count
Undirected graph K4 punya 6 edge. Jika diubah jadi directed (setiap edge jadi 2 panah), berapa directed edge?
A. 6
B. 8
C. 12
D. 24

<details><summary>💡 Hint</summary>Setiap undirected edge → 2 directed edge (A→B dan B→A).</details>
<details><summary>✅ Jawaban</summary>**C. 12.** 6 × 2 = 12.</details>

### Soal #246: Analogi - DNA Sequencing
Dalam bioinformatika, potongan DNA dimodelkan sebagai vertex, overlap = edge. Merangkai DNA lengkap = menemukan...
A. Euler Path (melewati semua edge)
B. Hamilton Path (melewati semua vertex)
C. MST
D. BFS

<details><summary>💡 Hint</summary>Setiap potongan harus dirangkai tepat 1 kali = setiap vertex 1 kali.</details>
<details><summary>✅ Jawaban</summary>**B. Hamilton Path.**</details>

### Soal #247: Degree Centrality
Vertex A punya derajat 8 di graf dengan 20 vertex. Degree centrality A = ?
A. 8/20 = 0.4
B. 8/19 ≈ 0.42
C. 8
D. 20

<details><summary>💡 Hint</summary>Degree Centrality = deg(v) / (V-1). Maks kemungkinan tetangga = V-1.</details>
<details><summary>✅ Jawaban</summary>**B. 8/19 ≈ 0.42.**</details>

### Soal #248: Analogi - Maze Game
Peta labirin game: kotak = vertex, dinding terbuka = edge. Mencari jalan keluar tercepat menggunakan...
A. DFS
B. BFS
C. MST
D. Euler Path

<details><summary>💡 Hint</summary>Tercepat = shortest path = BFS.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

### Soal #249: Weighted Shortest Path
```
A --1-- B --10-- D
|               /
5             3
|           /
C ----2----
```
Shortest path A ke D?
A. A→B→D (11)
B. A→C→D (7)
C. A→B→C→D (terlalu panjang)
D. Tidak ada jalur

<details><summary>💡 Hint</summary>A→C(5)→D via C→D(2)... Cek koneksi. A-B(1), B-D(10), A-C(5), C-D(2).</details>
<details><summary>✅ Jawaban</summary>**B. A→C→D = 5+2 = 7.** Lebih pendek dari A→B→D = 11.</details>

### Soal #250: Refleksi Bagian 5
Untuk menghubungkan SEMUA titik dengan biaya paling murah, gunakan...
A. BFS
B. DFS
C. MST (Minimum Spanning Tree)
D. Euler Circuit

<details><summary>💡 Hint</summary>Hubungkan semua + minimum = MST.</details>
<details><summary>✅ Jawaban</summary>**C. MST.**</details>

---
[< Bagian 4 (151-200)](./07-graf-soal-part-4.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 6 (251-300) >](./07-graf-soal-part-6.md)
