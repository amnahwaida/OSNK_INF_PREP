# 07. Graf Sederhana - Latihan Soal Bagian 2 (Soal 51-100)
## Topik: Rumus Jabat Tangan, Derajat, dan Perhitungan Edge

[< Bagian 1 (1-50)](./07-graf-soal-part-1.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 3 (101-150) >](./07-graf-soal-part-3.md)

---

### Soal #51: Rumus Jabat Tangan - Dasar
Sebuah graf punya 4 edge. Berapa total derajat semua vertex?
A. 4
B. 6
C. 8
D. 10

<details><summary>💡 Hint</summary>Total derajat = 2 × jumlah edge.</details>
<details><summary>✅ Jawaban</summary>**C. 8.** 2 × 4 = 8.</details>

### Soal #52: Mencari Jumlah Edge
Total derajat semua vertex = 14. Berapa jumlah edge?
A. 5
B. 6
C. 7
D. 14

<details><summary>💡 Hint</summary>Jumlah edge = total derajat ÷ 2.</details>
<details><summary>✅ Jawaban</summary>**C. 7.** 14 ÷ 2 = 7.</details>

### Soal #53: Mencari Derajat yang Hilang
Derajat vertex: 3, 2, ?, 1, 2. Jumlah edge = 5. Berapa derajat yang hilang?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Total derajat harus = 2×5 = 10. Sudah ada: 3+2+1+2 = 8.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** 10 - 8 = 2.</details>

### Soal #54: Vertex Ganjil
6 vertex dengan derajat: 3, 1, 2, 3, 1, 2. Berapa vertex yang berderajat ganjil?
A. 2
B. 3
C. 4
D. 6

<details><summary>💡 Hint</summary>Ganjil: 3, 1, 3, 1. Genap: 2, 2.</details>
<details><summary>✅ Jawaban</summary>**C. 4.** Ada 4 vertex dengan derajat ganjil.</details>

### Soal #55: Kemungkinan Derajat
Mungkinkah sebuah graf punya tepat 3 vertex berderajat ganjil?
A. Mungkin
B. Tidak mungkin
C. Tergantung jumlah edge
D. Hanya jika directed

<details><summary>💡 Hint</summary>Jumlah vertex berderajat ganjil selalu GENAP.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak mungkin.** 3 adalah bilangan ganjil, sehingga tidak mungkin.</details>

### Soal #56: Complete Graph K3
Berapa total derajat semua vertex di K3 (segitiga)?
A. 3
B. 4
C. 6
D. 9

<details><summary>💡 Hint</summary>K3 punya 3 edge. Total derajat = 2 × 3.</details>
<details><summary>✅ Jawaban</summary>**C. 6.** Setiap vertex berderajat 2, total = 3 × 2 = 6.</details>

### Soal #57: Pesta Jabat Tangan
Di sebuah pesta, 6 orang saling berjabat tangan. Setiap orang jabat tangan dengan tepat 3 orang lain. Berapa total jabat tangan?
A. 6
B. 9
C. 12
D. 18

<details><summary>💡 Hint</summary>Total derajat = 6 × 3 = 18. Jabat tangan = edge = 18/2.</details>
<details><summary>✅ Jawaban</summary>**B. 9.** 18 ÷ 2 = 9 jabat tangan.</details>

### Soal #58: Mencari Vertex
Sebuah graf punya 10 edge. Setiap vertex berderajat 4. Berapa jumlah vertex?
A. 4
B. 5
C. 8
D. 10

<details><summary>💡 Hint</summary>Total derajat = 2 × 10 = 20. Jumlah vertex = 20 ÷ 4.</details>
<details><summary>✅ Jawaban</summary>**B. 5.** 20 ÷ 4 = 5 vertex.</details>

### Soal #59: Derajat Rata-rata
Graf punya 6 vertex dan 9 edge. Berapa derajat rata-rata?
A. 1.5
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Total derajat = 18. Rata-rata = 18 ÷ 6.</details>
<details><summary>✅ Jawaban</summary>**C. 3.** Rata-rata = 18/6 = 3.</details>

### Soal #60: Tree Edge
Tree dengan 15 vertex punya berapa edge?
A. 13
B. 14
C. 15
D. 16

<details><summary>💡 Hint</summary>Tree: E = V - 1.</details>
<details><summary>✅ Jawaban</summary>**B. 14.** 15 - 1 = 14.</details>

### Soal #61: Apakah Tree?
Graf punya 5 vertex, 4 edge, dan terhubung (connected). Apakah ini tree?
A. Ya
B. Tidak
C. Belum tentu
D. Perlu info lebih

<details><summary>💡 Hint</summary>Tree punya V-1 edge dan connected. 5-1=4 ✓, connected ✓.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Memenuhi kedua syarat tree.</details>

### Soal #62: Bukan Tree
Graf punya 5 vertex, 5 edge, dan connected. Apakah ini tree?
A. Ya
B. Tidak
C. Mungkin
D. Error

<details><summary>💡 Hint</summary>Tree harus punya V-1 = 4 edge. Ini punya 5.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Tree harus punya tepat V-1 edge. Ini punya cycle.</details>

### Soal #63: Edge Minimum Connected
Berapa edge minimum agar graf dengan 7 vertex bisa connected?
A. 5
B. 6
C. 7
D. 8

<details><summary>💡 Hint</summary>Edge minimum = tree = V - 1.</details>
<details><summary>✅ Jawaban</summary>**B. 6.** Minimal edge untuk connected = V - 1 = 6.</details>

### Soal #64: Reguler Graph
Graf reguler berderajat 3 punya 8 vertex. Berapa edge-nya?
A. 8
B. 10
C. 12
D. 24

<details><summary>💡 Hint</summary>Total derajat = 8 × 3 = 24. Edge = 24/2.</details>
<details><summary>✅ Jawaban</summary>**C. 12.**</details>

### Soal #65: Degree Sequence
Diberikan urutan derajat: [3, 2, 2, 1]. Berapa edge dalam graf ini?
A. 3
B. 4
C. 5
D. 8

<details><summary>💡 Hint</summary>Total = 3+2+2+1 = 8. Edge = 8/2.</details>
<details><summary>✅ Jawaban</summary>**B. 4.**</details>

### Soal #66: Degree Sequence Valid?
Apakah urutan derajat [3, 3, 3] valid untuk sebuah graf?
A. Ya
B. Tidak
C. Hanya jika multigraph
D. Tergantung

<details><summary>💡 Hint</summary>Total = 9 (ganjil). Seharusnya genap!</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Total derajat harus genap (2×E), tapi 9 ganjil.</details>

### Soal #67: Petersen Graph
Petersen Graph terkenal punya 10 vertex dan 15 edge. Berapa derajat tiap vertex?
A. 2
B. 3
C. 4
D. 5

<details><summary>💡 Hint</summary>Total derajat = 2×15 = 30. Per vertex = 30/10.</details>
<details><summary>✅ Jawaban</summary>**B. 3.** Graf reguler berderajat 3.</details>

### Soal #68: Handshaking di Rapat
10 orang di rapat. Setiap orang jabat tangan dengan tepat 1 orang lain. Berapa total jabat tangan?
A. 5
B. 10
C. 15
D. 20

<details><summary>💡 Hint</summary>Total derajat = 10 × 1 = 10. Edge = 10/2.</details>
<details><summary>✅ Jawaban</summary>**A. 5.**</details>

### Soal #69: Maximum Edge
Berapa edge maksimum graf sederhana (tanpa self-loop, tanpa multi-edge) dengan 6 vertex?
A. 6
B. 10
C. 15
D. 30

<details><summary>💡 Hint</summary>Maks = complete graph = V(V-1)/2 = 6×5/2.</details>
<details><summary>✅ Jawaban</summary>**C. 15.**</details>

### Soal #70: Penduduk dan Jabat Tangan
7 orang di suatu ruangan. Total jabat tangan = 21. Berarti setiap orang jabat tangan dengan...
A. 3 orang lain
B. 4 orang lain
C. 5 orang lain
D. 6 orang lain (semua orang lain)

<details><summary>💡 Hint</summary>Total derajat = 2×21 = 42. Per orang = 42/7 = 6. Semua saling jabat tangan!</details>
<details><summary>✅ Jawaban</summary>**D. 6 orang lain.** Complete graph K7.</details>

### Soal #71: Bipartite Degree
Graf bipartite K3,3 punya 3 vertex di grup A dan 3 di grup B. Semua vertex grup A terhubung ke semua vertex grup B. Berapa edge?
A. 3
B. 6
C. 9
D. 12

<details><summary>💡 Hint</summary>Setiap vertex di A terhubung ke 3 vertex di B. 3 × 3.</details>
<details><summary>✅ Jawaban</summary>**C. 9.**</details>

### Soal #72: In-Degree + Out-Degree
Di directed graph, total semua in-degree = total semua out-degree = jumlah edge. Jika total in-degree = 8, berapa edge?
A. 4
B. 8
C. 16
D. Tidak bisa ditentukan

<details><summary>💡 Hint</summary>Di directed graph, setiap edge punya 1 in-degree dan 1 out-degree.</details>
<details><summary>✅ Jawaban</summary>**B. 8.**</details>

### Soal #73: Menghitung dari Matrix
```
    A  B  C
A [ 0  1  1 ]
B [ 1  0  1 ]
C [ 1  1  0 ]
```
Berapa derajat vertex A?
A. 1
B. 2
C. 3
D. 0

<details><summary>💡 Hint</summary>Jumlahkan baris A: 0+1+1 = 2.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** A terhubung ke B dan C.</details>

### Soal #74: Edge dari Matrix
Dari soal #73, berapa total edge?
A. 2
B. 3
C. 4
D. 6

<details><summary>💡 Hint</summary>Hitung 1 di atas diagonal: (A,B), (A,C), (B,C).</details>
<details><summary>✅ Jawaban</summary>**B. 3.** Graf ini adalah K3 (segitiga).</details>

### Soal #75: Diameter Graf
Diameter graf = path terpanjang dari semua shortest path antar vertex. 
```
A --- B --- C --- D
```
Berapa diameter graf ini?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Shortest path A ke D = 3 edge. Ini yang terpanjang.</details>
<details><summary>✅ Jawaban</summary>**C. 3.**</details>

### Soal #76: Degree dan Tetangga
Jika vertex A punya derajat 5 di graf undirected, berapa tetangga yang dimiliki A?
A. 4
B. 5
C. 6
D. 10

<details><summary>💡 Hint</summary>Derajat = jumlah tetangga (di graf simpel).</details>
<details><summary>✅ Jawaban</summary>**B. 5.**</details>

### Soal #77: Forest
Hutan (forest) adalah kumpulan tree yang terpisah. Jika sebuah forest punya 12 vertex dan 3 komponen, berapa edge?
A. 8
B. 9
C. 10
D. 11

<details><summary>💡 Hint</summary>Setiap komponen tree: edge = vertex-1. Total edge = V - jumlah komponen.</details>
<details><summary>✅ Jawaban</summary>**B. 9.** 12 - 3 = 9.</details>

### Soal #78: Pendant Vertex
Vertex berderajat 1 disebut pendant vertex (daun). Jika tree punya 10 vertex dan 4 pendant, berapa vertex yang berderajat > 1?
A. 4
B. 5
C. 6
D. 7

<details><summary>💡 Hint</summary>10 - 4 = 6 vertex bukan pendant.</details>
<details><summary>✅ Jawaban</summary>**C. 6.**</details>

### Soal #79: Cycle vs Path
Apa perbedaan cycle C5 dan path P5?
A. C5 punya 5 edge, P5 punya 4 edge
B. C5 punya 4 edge, P5 punya 5 edge
C. Sama saja
D. C5 punya arah, P5 tidak

<details><summary>💡 Hint</summary>Cycle menghubungkan vertex terakhir kembali ke pertama (1 edge tambahan).</details>
<details><summary>✅ Jawaban</summary>**A.** C5 punya 5 edge (lingkaran tertutup), P5 punya 4 edge (terbuka).</details>

### Soal #80: Degree di Cycle
Sebutkan derajat setiap vertex di cycle graph C10!
A. 1
B. 2
C. 5
D. 10

<details><summary>💡 Hint</summary>Setiap vertex di cycle terhubung ke kiri dan kanan.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** Semua vertex berderajat 2.</details>

### Soal #81: Star Graph
Star graph S5: 1 vertex pusat terhubung ke 5 vertex lainnya. Berapa derajat vertex pusat?
A. 1
B. 3
C. 5
D. 6

<details><summary>💡 Hint</summary>Pusat terhubung ke semua 5 vertex luar.</details>
<details><summary>✅ Jawaban</summary>**C. 5.**</details>

### Soal #82: Total Edge Star Graph
Star graph S5 punya berapa edge?
A. 3
B. 4
C. 5
D. 6

<details><summary>💡 Hint</summary>Setiap vertex luar punya 1 edge ke pusat. 5 vertex luar = 5 edge.</details>
<details><summary>✅ Jawaban</summary>**C. 5.**</details>

### Soal #83: Wheel Graph
Wheel graph W5: Cycle C5 + 1 vertex pusat yang terhubung ke semua vertex cycle. Berapa total edge?
A. 5
B. 8
C. 10
D. 12

<details><summary>💡 Hint</summary>Edge cycle = 5 + edge dari pusat = 5. Total = 10.</details>
<details><summary>✅ Jawaban</summary>**C. 10.**</details>

### Soal #84: Complement Graph
Complement dari sebuah graf adalah graf yang edge-nya dibalik. Jika G punya 4 vertex dan 2 edge, complement G punya berapa edge?
A. 2
B. 3
C. 4
D. 5

<details><summary>💡 Hint</summary>Maks edge K4 = 6. Complement = 6 - 2.</details>
<details><summary>✅ Jawaban</summary>**C. 4.**</details>

### Soal #85: Degree Sum Even
Sebuah graf punya vertex berderajat: 4, 3, 3, 2, x. Nilai x yang MUNGKIN adalah...
A. 1
B. 2
C. 3
D. 5

<details><summary>💡 Hint</summary>Total harus genap. 4+3+3+2=12. 12+x harus genap.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** 12+2=14 (genap). Opsi lain: A(13, ganjil ❌), C(15 ❌), D(17 ❌).</details>

### Soal #86: Parent dan Child di Tree
```
        A
       / \
      B   C
     /
    D
```
Siapa parent dari D?
A. A
B. B
C. C
D. D sendiri

<details><summary>💡 Hint</summary>Parent = vertex langsung di atas.</details>
<details><summary>✅ Jawaban</summary>**B. B.**</details>

### Soal #87: Sibling di Tree
Dari soal #86, siapa sibling (saudara) dari B?
A. A
B. C
C. D
D. Tidak ada

<details><summary>💡 Hint</summary>Sibling = vertex yang punya parent yang sama.</details>
<details><summary>✅ Jawaban</summary>**B. C.** B dan C sama-sama anak dari A.</details>

### Soal #88: Height of Tree
Dari soal #86, berapa height (tinggi) dari tree tersebut?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Height = panjang path terpanjang dari root ke leaf. A→B→D = 2.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #89: Binary Tree
Binary tree adalah tree di mana setiap vertex punya maksimal berapa anak?
A. 1
B. 2
C. 3
D. Tidak terbatas

<details><summary>💡 Hint</summary>Binary = dua.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #90: Full Binary Tree
Full binary tree dengan depth 3 (root = depth 0) punya berapa leaf?
A. 3
B. 4
C. 7
D. 8

<details><summary>💡 Hint</summary>Leaf pada depth d = 2^d = 2^3.</details>
<details><summary>✅ Jawaban</summary>**D. 8.**</details>

### Soal #91: Cut Vertex
Vertex yang jika dihapus membuat graf menjadi tidak connected disebut...
A. Bridge
B. Cut vertex / Articulation point
C. Pendant
D. Leaf

<details><summary>💡 Hint</summary>Cut = memotong. Vertex yang "memotong" koneksi graf.</details>
<details><summary>✅ Jawaban</summary>**B. Cut vertex.**</details>

### Soal #92: Vertex dan Edge di K6
Complete graph K6 punya berapa vertex dan berapa edge?
A. V=6, E=12
B. V=6, E=15
C. V=6, E=30
D. V=6, E=6

<details><summary>💡 Hint</summary>E = 6×5/2 = 15.</details>
<details><summary>✅ Jawaban</summary>**B. V=6, E=15.**</details>

### Soal #93: Derajat Minimum
Jika graf connected sederhana punya V vertex, berapa derajat minimum setiap vertex agar pasti connected?
A. 0
B. 1
C. V/2
D. V-1

<details><summary>💡 Hint</summary>Derajat 1 cukup jika disusun dengan benar (tree).</details>
<details><summary>✅ Jawaban</summary>**B. 1.** (minimal, bukan jaminan. Tapi tree bisa connected dengan deg min 1).</details>

### Soal #94: Self-Loop dan Derajat
Self-loop menambah berapa ke derajat vertex?
A. 0
B. 1
C. 2
D. 3

<details><summary>💡 Hint</summary>Self-loop dihitung 2 karena kedua ujungnya di vertex yang sama.</details>
<details><summary>✅ Jawaban</summary>**C. 2.**</details>

### Soal #95: Adjacency Matrix Directed
```
A --> B
B --> C
C --> A
```
Berapa nilai matrix[C][A]?
A. 0
B. 1
C. 2
D. -1

<details><summary>💡 Hint</summary>C → A berarti ada panah dari C ke A.</details>
<details><summary>✅ Jawaban</summary>**B. 1.**</details>

### Soal #96: Weighted Matrix
```
A --5-- B
A --3-- C
B --2-- C
```
Berapa nilai matrix[A][B]?
A. 0
B. 1
C. 3
D. 5

<details><summary>💡 Hint</summary>Untuk weighted graph, isi matrix adalah bobot edge.</details>
<details><summary>✅ Jawaban</summary>**D. 5.** Bobot edge A-B = 5.</details>

### Soal #97: Complement Degree
Graf G punya 5 vertex. Vertex A berderajat 2 di G. Di complement G, berapa derajat A?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Maks derajat di K5 = 4. Complement = 4 - 2.</details>
<details><summary>✅ Jawaban</summary>**B. 2.** Derajat complement = (V-1) - derajat asli = 4-2 = 2.</details>

### Soal #98: Path vs Walk
Perbedaan path dan walk adalah...
A. Path boleh mengulang vertex, walk tidak
B. Walk boleh mengulang vertex, path tidak
C. Keduanya sama
D. Path punya bobot, walk tidak

<details><summary>💡 Hint</summary>Path = "bersih" (tidak ada pengulangan vertex).</details>
<details><summary>✅ Jawaban</summary>**B.** Walk boleh lewat vertex yang sama berulang kali, path tidak.</details>

### Soal #99: Eccentricity
Eccentricity vertex v = jarak maksimum dari v ke vertex terjauh. Di path A-B-C-D-E, berapa eccentricity vertex C?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>C ke A = 2, C ke E = 2. Maks = 2.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #100: Refleksi Bagian 2
Rumus yang paling sering kamu gunakan saat mengerjakan soal derajat graf adalah...
A. E = V + 1
B. Total derajat = 2 × E
C. E = V²
D. Total derajat = E / 2

<details><summary>💡 Hint</summary>Rumus Jabat Tangan!</details>
<details><summary>✅ Jawaban</summary>**B. Total derajat = 2 × E.** Rumus Jabat Tangan (Handshaking Lemma).</details>

---
[< Bagian 1 (1-50)](./07-graf-soal-part-1.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 3 (101-150) >](./07-graf-soal-part-3.md)
