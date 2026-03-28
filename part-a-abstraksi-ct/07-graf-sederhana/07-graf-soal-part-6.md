# 07. Graf Sederhana - Latihan Soal Bagian 6 (Soal 251-300)
## Topik: Soal Campuran & Komprehensif

[< Bagian 5 (201-250)](./07-graf-soal-part-5.md) | [< Kembali ke Indeks](../07-graf-sederhana.md)

---

### Soal #251: Campuran - Identifikasi
```
A --- B
|   / |
| /   |
C --- D --- E
```
Berapa vertex, edge, dan total derajat?
A. V=5, E=6, Total=12
B. V=5, E=5, Total=10
C. V=4, E=5, Total=10
D. V=5, E=6, Total=10

<details><summary>💡 Hint</summary>Edge: A-B, A-C, B-C, B-D, C-D, D-E = 6. Total = 2×6 = 12.</details>
<details><summary>✅ Jawaban</summary>**A. V=5, E=6, Total Derajat=12.**</details>

### Soal #252: Campuran - Euler Check
Dari soal #251, ada Euler Path?
A. Ya (Euler Circuit)
B. Ya (Euler Path, bukan Circuit)
C. Tidak ada

<details><summary>💡 Hint</summary>Derajat: A=2, B=3, C=3, D=3, E=1. Vertex ganjil: B(3), C(3), D(3), E(1) = 4 ganjil.</details>
<details><summary>✅ Jawaban</summary>**C. Tidak ada.** 4 vertex ganjil > 2.</details>

### Soal #253: Campuran - Tree Check
```
A --- B --- C
      |
      D
```
Apakah ini tree?
A. Ya (connected, 4 vertex, 3 edge, no cycle)
B. Tidak (ada cycle)

<details><summary>💡 Hint</summary>V=4, E=3 (V-1). Connected? Ya. Cycle? Tidak.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Memenuhi semua syarat tree.</details>

### Soal #254: Campuran - BFS
```
1 --- 2 --- 5
|     |
3 --- 4
```
BFS dari 1. Di layer berapa vertex 5?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Layer 0: {1}. Layer 1: {2, 3}. Layer 2: {4, 5}.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #255: Campuran - MST
```
A --2-- B
|     / |
4   1   3
| /     |
C --5-- D
```
MST = ?
A. B-C(1), A-B(2), B-D(3) = 6
B. A-B(2), B-C(1), C-D(5) = 8
C. A-C(4), B-C(1), B-D(3) = 8
D. Semua edge = 15

<details><summary>💡 Hint</summary>Urut: 1, 2, 3, 4, 5. Ambil 1(B-C), 2(A-B), 3(B-D). 3 edge = V-1 ✓, no cycle ✓.</details>
<details><summary>✅ Jawaban</summary>**A. Total = 6.**</details>

### Soal #256: Analogi - Kereta
Stasiun = vertex, Rel = edge. Jika sebuah stasiun dihapus dan jaringan kereta terputus, stasiun itu disebut...
A. Bridge
B. Cut Vertex
C. Leaf
D. Hub

<details><summary>💡 Hint</summary>Vertex yang dipotong = cut vertex.</details>
<details><summary>✅ Jawaban</summary>**B. Cut Vertex.**</details>

### Soal #257: K4 - Semua Sifat
K4: V=4, E=6, Derajat=3, Total Derajat=12. Euler?
A. Ada Euler Circuit (semua genap)
B. Ada Euler Path (2 ganjil)
C. Tidak ada (4 ganjil)
D. Tidak ada (3 ganjil)

<details><summary>💡 Hint</summary>Derajat setiap vertex = 3 (ganjil). 4 vertex ganjil.</details>
<details><summary>✅ Jawaban</summary>**C. Tidak ada.** 4 vertex ganjil.</details>

### Soal #258: Menambah Edge untuk Euler
Dari K4 (4 vertex ganjil), berapa edge yang perlu ditambah agar ada Euler Circuit?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Setiap edge baru bisa mengubah 2 vertex ganjil jadi genap. Butuh 4/2 = 2 edge.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #259: Directed Graph - BFS
```
A --> B --> D
|         ^
v        /
C ------
```
BFS dari A. Urutan?
A. A, B, C, D
B. A, C, B, D
C. Bisa keduanya (tergantung urutan tetangga)
D. D, C, B, A

<details><summary>💡 Hint</summary>A → B dan C (layer 1). B → D dan C → D (layer 2).</details>
<details><summary>✅ Jawaban</summary>**C.** Bisa A,B,C,D atau A,C,B,D tergantung urutan.</details>

### Soal #260: Degree Sequence Problem
Urutan derajat [4, 3, 2, 2, 1] valid untuk graf sederhana?
A. Ya (total = 12, genap)
B. Tidak (total = 12, tapi tidak bisa dibuat graf)
C. Ya (total genap = syarat cukup)
D. Tidak (total = 11, ganjil)

<details><summary>💡 Hint</summary>Total = 4+3+2+2+1 = 12 (genap ✓). Tapi vertex berderajat 4 butuh 4 tetangga, padahal hanya ada 4 vertex lain. Cek apakah realisable.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Total genap, dan urutan ini bisa diwujudkan sebagai graf.</details>

### Soal #261: Campuran - Hamilton
```
A --- B --- C
|         |
D --------
```
A → B → C → D → A. Hamilton Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua vertex dikunjungi tepat 1 kali dan kembali ke awal. Cek edge ada: A-D? Ya (D--------A).</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #262: Labirin dan DFS
Robot di labirin. Strategi: jalan terus ke depan sampai mentok, lalu putar balik dan coba jalan lain. Strategi ini mirip...
A. BFS
B. DFS
C. MST
D. Euler

<details><summary>💡 Hint</summary>Terus ke depan (depth) + putar balik (backtrack) = DFS.</details>
<details><summary>✅ Jawaban</summary>**B. DFS.**</details>

### Soal #263: Social Distance
Di BFS dari pasien COVID pertama, layer 1 = orang yang kontak langsung. Layer 2 = ?
A. Kontak dari kontak (indirect contact)
B. Orang yang sehat
C. Dokter
D. Perawat

<details><summary>💡 Hint</summary>BFS layer 2 = tetangga dari tetangga.</details>
<details><summary>✅ Jawaban</summary>**A. Kontak dari kontak.**</details>

### Soal #264: Campuran - Handshaking
10 komputer di jaringan. Total kabel = 20. Berapa rata-rata koneksi per komputer?
A. 2
B. 3
C. 4
D. 5

<details><summary>💡 Hint</summary>Total derajat = 2×20 = 40. Rata-rata = 40/10 = 4.</details>
<details><summary>✅ Jawaban</summary>**C. 4.**</details>

### Soal #265: Bipartite Matching
5 siswa dan 5 proyek. Setiap siswa harus dipasangkan dengan 1 proyek. Ini masalah...
A. MST
B. Perfect Matching di Bipartite Graph
C. Euler Circuit
D. DFS

<details><summary>💡 Hint</summary>1-1 assignment = matching di bipartite graph.</details>
<details><summary>✅ Jawaban</summary>**B. Perfect Matching.**</details>

### Soal #266: Graph Complement
Graf G: A-B, B-C. Complement G punya edge apa saja? (V = {A,B,C})
A. A-C saja
B. A-B saja
C. B-C saja
D. Tidak ada edge

<details><summary>💡 Hint</summary>Complement = edge yang TIDAK ada di G. Kemungkinan: A-B(ada), A-C(tidak ada), B-C(ada). Yang tidak ada = A-C.</details>
<details><summary>✅ Jawaban</summary>**A. A-C saja.**</details>

### Soal #267: Cycle Detection
Sebuah graf punya V vertex dan E edge. Jika E ≥ V, apakah PASTI ada cycle?
A. Ya (jika connected)
B. Tidak selalu
C. Hanya di directed graph
D. Tidak pernah

<details><summary>💡 Hint</summary>Tree punya V-1 edge. Jika E ≥ V dan connected, maka E > V-1 → ada cycle.</details>
<details><summary>✅ Jawaban</summary>**A. Ya (jika connected).** E ≥ V > V-1 → pasti ada cycle.</details>

### Soal #268: Campuran - Connected Component
```
A --- B    C --- D --- E    F
```
Berapa connected component?
A. 1
B. 2
C. 3
D. 6

<details><summary>💡 Hint</summary>Komponen: {A,B}, {C,D,E}, {F}.</details>
<details><summary>✅ Jawaban</summary>**C. 3.**</details>

### Soal #269: Weighted Shortest Path
```
A --1-- B --1-- C
|               |
10              1
|               |
D ------1----- E
```
Shortest path A ke E?
A. A→D→E (11)
B. A→B→C→E (3)
C. A→B→D→E (12)
D. Keduanya A dan B

<details><summary>💡 Hint</summary>A→B(1)→C(1)→E(1) = 3. vs A→D(10)→E(1) = 11.</details>
<details><summary>✅ Jawaban</summary>**B. 3.**</details>

### Soal #270: Topological Sort
```
A --> B --> D
|         ^
v        /
C ------
```
Topological Order yang valid?
A. A, B, C, D
B. A, C, B, D
C. D, B, C, A
D. A dan B keduanya valid

<details><summary>💡 Hint</summary>A harus sebelum B dan C. B dan C harus sebelum D.</details>
<details><summary>✅ Jawaban</summary>**D. Keduanya valid.** A,B,C,D dan A,C,B,D sama-sama valid.</details>

### Soal #271: Campuran - Euler + Handshaking
Graf punya 7 edge. Semua vertex berderajat 2. Berapa vertex?
A. 5
B. 6
C. 7
D. 8

<details><summary>💡 Hint</summary>Total derajat = 2×7 = 14. Vertex = 14 ÷ 2 = 7.</details>
<details><summary>✅ Jawaban</summary>**C. 7.** Ini graf C7 (cycle 7-simpul). Euler Circuit? Ya! (Semua genap.)</details>

### Soal #272: Graph Isomorphism
Dua graf memiliki vertex dan edge yang sama jumlahnya. Apakah mereka pasti isomorphic?
A. Ya
B. Tidak (perlu cek konektivitas juga)
C. Hanya jika weighted
D. Hanya jika directed

<details><summary>💡 Hint</summary>Jumlah sama ≠ struktur sama. Perlu cek degree sequence, dll.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Perlu cek lebih detail (degree sequence, adjacency, dll).</details>

### Soal #273: Campuran - Tree Properties
Tree punya 20 leaf dan 5 vertex berderajat 3. Berapa total vertex? (Sisanya berderajat 2.)
A. 25
B. 30
C. Perlu info jumlah edge

<details><summary>💡 Hint</summary>Total derajat = 2E = 2(V-1). 20×1 + 5×3 + x×2 = 2(20+5+x-1). Solve.</details>
<details><summary>✅ Jawaban</summary>**C.** Kita perlu menghitung: 20 + 15 + 2x = 2(24+x). 35 + 2x = 48 + 2x → 35=48? Kontradiksi! Jadi konfigurasi ini **tidak mungkin**.</details>

### Soal #274: Weighted Graph - Negatif
Apakah MST bisa ada di graf dengan bobot negatif?
A. Ya (MST tetap bisa dihitung)
B. Tidak
C. Hanya jika semua negatif
D. Hanya Dijkstra

<details><summary>💡 Hint</summary>Kruskal dan Prim tetap bekerja dengan bobot negatif.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** MST bisa dihitung meskipun ada bobot negatif.</details>

### Soal #275: Game - Pathfinding
NPC di game mengejar pemain. Grid 10×10, NPC di (0,0), Player di (9,9). Algoritma terbaik untuk menemukan jalur terpendek?
A. DFS
B. BFS
C. Random walk
D. Euler Path

<details><summary>💡 Hint</summary>Grid tanpa bobot → BFS = shortest path.</details>
<details><summary>✅ Jawaban</summary>**B. BFS.**</details>

### Soal #276: Degree dan Tree
Di tree, tidak mungkin SEMUA vertex berderajat > 1. Mengapa?
A. Karena tree punya leaf (derajat 1)
B. Karena tree memiliki self-loop
C. Karena tree selalu directed
D. Karena tree punya cycle

<details><summary>💡 Hint</summary>Tree dengan ≥ 2 vertex pasti punya minimal 2 leaf.</details>
<details><summary>✅ Jawaban</summary>**A.** Tree pasti punya leaf (vertex berderajat 1).</details>

### Soal #277: Campuran - DFS Application
Untuk mengecek apakah sebuah graf connected, cukup jalankan DFS dari vertex manapun. Jika semua vertex terkunjungi, berarti...
A. Ada Euler Path
B. Graf connected
C. Graf adalah tree
D. Ada Hamilton Circuit

<details><summary>💡 Hint</summary>DFS menjangkau semua = semua terhubung = connected.</details>
<details><summary>✅ Jawaban</summary>**B. Graf connected.**</details>

### Soal #278: Spanning Tree - Non-unique
```
A --- B
|   /|
| /  |
C ---D
```
Berapa spanning tree yang berbeda?
A. 4
B. 6
C. 8
D. 16

<details><summary>💡 Hint</summary>5 edge, perlu 3 (V-1=3). Buang 2 dari 5. C(5,2)=10, tapi tidak semua valid (harus connected).</details>
<details><summary>✅ Jawaban</summary>**C. 8.** (Dihitung dengan Kirchhoff's theorem atau bruteforce.)</details>

### Soal #279: Analogi - Folder dan File
Folder yang berisi subfolder berisi file. Ini adalah contoh...
A. Cycle Graph
B. Complete Graph
C. Tree
D. Bipartite Graph

<details><summary>💡 Hint</summary>Hierarki tanpa lingkaran = tree.</details>
<details><summary>✅ Jawaban</summary>**C. Tree.**</details>

### Soal #280: Binary Tree - Max Nodes
Binary tree dengan tinggi 4 (root = tinggi 0) punya maksimal berapa node?
A. 15
B. 16
C. 31
D. 32

<details><summary>💡 Hint</summary>Maks node = 2^(h+1) - 1 = 2^5 - 1 = 31.</details>
<details><summary>✅ Jawaban</summary>**C. 31.**</details>

### Soal #281: Graph Coloring - Cycle
Berapa warna minimum untuk C4 (persegi)?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>C4 jumlah vertex genap → bipartite → 2 warna cukup.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** Cycle genap = bipartite = 2 warna.</details>

### Soal #282: Graph Coloring - Odd Cycle
Berapa warna minimum untuk C5 (pentagon)?
A. 1
B. 2
C. 3
D. 5

<details><summary>💡 Hint</summary>C5 jumlah vertex ganjil → BUKAN bipartite → butuh 3 warna.</details>
<details><summary>✅ Jawaban</summary>**C. 3.** Cycle ganjil butuh 3 warna.</details>

### Soal #283: Campuran - Connected dan Euler
Graf connected punya 8 vertex dan 10 edge. 4 vertex berderajat ganjil. Ada Euler Path?
A. Ya (Euler Circuit)
B. Ya (Euler Path)
C. Tidak ada

<details><summary>💡 Hint</summary>4 vertex ganjil > 2 → tidak ada Euler.</details>
<details><summary>✅ Jawaban</summary>**C. Tidak ada.**</details>

### Soal #284: MST - Edge Terberat
Di MST, jika ada edge dengan bobot 100 dan semua edge lain bobotnya < 10, apakah edge 100 bisa masuk MST?
A. Ya (jika itu satu-satunya edge yang menghubungkan ke vertex tertentu)
B. Tidak pernah
C. Selalu masuk
D. Tergantung DFS

<details><summary>💡 Hint</summary>Jika menghapus edge 100 memutuskan koneksi, maka edge itu wajib masuk MST.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Bridge selalu masuk MST apapun bobotnya.</details>

### Soal #285: BFS - Bipartite Test
Saat BFS, kamu mewarnai vertex alternating 2 warna. Jika kamu menemukan edge antara 2 vertex WARNA SAMA, berarti...
A. Graf connected
B. Graf bipartite
C. Graf BUKAN bipartite
D. Ada Euler Circuit

<details><summary>💡 Hint</summary>Bipartite = 2 grup warna berbeda. Warna sama bertetangga = konflik.</details>
<details><summary>✅ Jawaban</summary>**C. Bukan bipartite.**</details>

### Soal #286: Campuran - Degree Sequence
Urutan derajat: [5, 3, 3, 3, 2]. Valid?
A. Ya (total = 16, genap)
B. Tidak (vertex berderajat 5 tapi hanya ada 4 vertex lain → dia butuh 5 tetangga padahal cuma ada 4)
C. Mungkin
D. Tergantung weighted atau tidak

<details><summary>💡 Hint</summary>Maks derajat = V-1 = 4. Tapi ada vertex berderajat 5!</details>
<details><summary>✅ Jawaban</summary>**B. Tidak valid.** Derajat maks di graf 5 vertex = 4. Tidak mungkin ada derajat 5.</details>

### Soal #287: Campuran - Forest
Forest punya 15 vertex dan 10 edge. Berapa komponen?
A. 3
B. 4
C. 5
D. 6

<details><summary>💡 Hint</summary>Di forest: E = V - komponen. 10 = 15 - k. k = 5.</details>
<details><summary>✅ Jawaban</summary>**C. 5.**</details>

### Soal #288: DFS - Topological
Topological sort hanya bisa dilakukan di graf yang...
A. Undirected dan connected
B. Directed dan acyclic (DAG)
C. Weighted
D. Complete

<details><summary>💡 Hint</summary>Topological = urutan dependency = harus directed + tanpa cycle.</details>
<details><summary>✅ Jawaban</summary>**B. DAG (Directed Acyclic Graph).**</details>

### Soal #289: Analogi - Antrian BFS
BFS menggunakan Queue karena...
A. Vertex yang ditemukan dulu harus dijelajahi dulu (FIFO)
B. Vertex terakhir dijelajahi dulu (LIFO)
C. Queue lebih cepat
D. Kebetulan saja

<details><summary>💡 Hint</summary>BFS = layer by layer. Layer 1 selesai dulu baru layer 2 = FIFO.</details>
<details><summary>✅ Jawaban</summary>**A.** FIFO menjamin tetangga yang ditemukan lebih dulu diproses lebih dulu.</details>

### Soal #290: Analogi - Tumpukan DFS
DFS menggunakan Stack karena...
A. Vertex yang ditemukan terakhir harus dijelajahi dulu (LIFO)
B. Stack lebih kecil
C. Stack lebih cepat
D. Kebetulan saja

<details><summary>💡 Hint</summary>DFS = masuk sedalam mungkin = yang baru ditemukan langsung dijelajahi = LIFO.</details>
<details><summary>✅ Jawaban</summary>**A.** LIFO menjamin vertex terbaru langsung dijelajahi (depth-first).</details>

### Soal #291: Campuran - Complete Bipartite
K4,4 (4 kiri, 4 kanan). Berapa edge?
A. 8
B. 12
C. 16
D. 24

<details><summary>💡 Hint</summary>Setiap vertex kiri terhubung ke 4 kanan. 4 × 4 = 16.</details>
<details><summary>✅ Jawaban</summary>**C. 16.**</details>

### Soal #292: Euler di K4,4
K4,4: derajat setiap vertex = 4 (genap). Ada Euler Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua genap dan connected → Euler Circuit!</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #293: Hamilton di K4,4
K4,4 ada Hamilton Circuit?
A. Ya (jumlah vertex sama di kedua partisi)
B. Tidak

<details><summary>💡 Hint</summary>K(n,n) selalu punya Hamilton Circuit jika n ≥ 2.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #294: Campuran - Multi Konsep
Sebuah graf connected punya 6 vertex, semua berderajat 2. Apakah ini cycle graph C6?
A. Ya
B. Tidak
C. Mungkin

<details><summary>�� Hint</summary>Connected + semua derajat 2 → pasti cycle graph.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Connected graph di mana semua vertex berderajat 2 = cycle.</details>

### Soal #295: Shortest Path - Tidak Ada
```
A --- B    C --- D
```
Berapa shortest path dari A ke D?
A. 1
B. 2
C. Tidak ada (disconnected)
D. 0

<details><summary>💡 Hint</summary>A dan D ada di komponen berbeda.</details>
<details><summary>✅ Jawaban</summary>**C. Tidak ada.** A dan D tidak terhubung.</details>

### Soal #296: Campuran - MST di K3
K3 (segitiga) dengan bobot: A-B(3), B-C(1), A-C(2). MST?
A. B-C(1), A-C(2) = 3
B. A-B(3), B-C(1) = 4
C. A-B(3), A-C(2) = 5
D. Semua edge = 6

<details><summary>💡 Hint</summary>3 vertex, butuh 2 edge. Terkecil: 1, 2. Cek connected: B-C + A-C → semua terhubung ✓.</details>
<details><summary>✅ Jawaban</summary>**A. Total = 3.**</details>

### Soal #297: Analogi Final - Internet
Internet adalah contoh graf yang...
A. Kecil dan sederhana
B. Sangat besar, directed, weighted, dan dynamis
C. Hanya tree
D. Tidak punya cycle

<details><summary>💡 Hint</summary>Miliaran website saling terhubung dengan link berarah.</details>
<details><summary>✅ Jawaban</summary>**B.** Internet = graf raksasa yang terus berubah.</details>

### Soal #298: Self-Assessment
Apa langkah PERTAMA yang harus kamu lakukan saat mengerjakan soal graf di OSN-K?
A. Langsung jawab
B. Gambar grafnya di kertas
C. Menghafal rumus
D. Melewatkan soal

<details><summary>💡 Hint</summary>Visualisasi membantu otak memproses informasi.</details>
<details><summary>✅ Jawaban</summary>**B. Gambar grafnya di kertas!** Selalu jadi langkah pertama.</details>

### Soal #299: Rumus Terpenting
Rumus yang PALING SERING berguna di soal derajat graf OSN-K adalah...
A. E = V²
B. V - E + F = 2
C. Total Derajat = 2 × E (Handshaking Lemma)
D. E = V!

<details><summary>💡 Hint</summary>Rumus Jabat Tangan.</details>
<details><summary>✅ Jawaban</summary>**C. Total Derajat = 2 × E.**</details>

### Soal #300: Refleksi Akhir 🎉
Setelah mengerjakan 300 soal graf, kamu sekarang memahami bahwa graf adalah...
A. Cara merepresentasikan berbagai hubungan dunia nyata dalam informatika
B. Hanya tentang "titik dan garis"
C. Topik yang tidak pernah muncul di OSN-K
D. Hal yang sangat membosankan

<details><summary>💡 Hint</summary>Pikirkan semua aplikasi graf yang sudah kamu pelajari!</details>
<details><summary>✅ Jawaban</summary>**A. Cara merepresentasikan berbagai hubungan dunia nyata.**

🎉 **SELAMAT!** Kamu telah menyelesaikan seluruh 300 soal latihan Graf Sederhana! Dengan latihan ini, kamu sudah jauh lebih siap menghadapi soal-soal OSN-K Informatika tentang teori graf. Terus berlatih dan semangat! 💪</details>

---
[< Bagian 5 (201-250)](./07-graf-soal-part-5.md) | [< Kembali ke Indeks](../07-graf-sederhana.md)
