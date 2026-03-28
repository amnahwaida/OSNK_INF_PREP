🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Latihan Soal Bagian 3 (Soal 101-150)
## Topik: Euler Path/Circuit, Hamilton Path/Circuit

[< Bagian 2 (51-100)](./07-graf-soal-part-2.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 4 (151-200) >](./07-graf-soal-part-4.md)

---

### Soal #101: Euler Path - Syarat Dasar
Euler Path bisa ada jika graf punya berapa vertex berderajat ganjil?
A. 0
B. 0 atau 2
C. 2 atau 4
D. Bebas

<details><summary>💡 Hint</summary>Euler Path: 0 atau 2 ganjil. Euler Circuit: 0 ganjil.</details>
<details><summary>✅ Jawaban</summary>**B. 0 atau 2.**</details>

### Soal #102: Euler Circuit - Syarat
Euler Circuit bisa ada jika...
A. Ada 2 vertex ganjil
B. Semua vertex genap
C. Semua vertex ganjil
D. Minimal 1 vertex genap

<details><summary>💡 Hint</summary>Euler Circuit = kembali ke awal. Semua harus genap.</details>
<details><summary>✅ Jawaban</summary>**B. Semua vertex genap.**</details>

### Soal #103: Cek Euler - Graf Persegi
```
A --- B
|     |
C --- D
```
Derajat: A=2, B=2, C=2, D=2. Ada Euler apa?
A. Euler Path saja
B. Euler Circuit
C. Tidak ada Euler Path
D. Hamilton saja

<details><summary>💡 Hint</summary>0 vertex ganjil → Euler Circuit!</details>
<details><summary>✅ Jawaban</summary>**B. Euler Circuit.** Semua genap → bisa kembali ke awal!</details>

### Soal #104: Cek Euler - Rumah
```
A --- B
|\ /|
| X  |
|/ \|
C --- D
```
Derajat: A=3, B=3, C=3, D=3. Ada Euler?
A. Euler Path
B. Euler Circuit
C. Tidak ada
D. Keduanya

<details><summary>💡 Hint</summary>4 vertex ganjil → lebih dari 2.</details>
<details><summary>✅ Jawaban</summary>**C. Tidak ada.** 4 vertex ganjil → tidak ada Euler Path maupun Circuit.</details>

### Soal #105: Euler Path - Titik Awal
Jika graf punya 2 vertex ganjil (B dan D), Euler Path harus dimulai dari mana?
A. Vertex manapun
B. B atau D
C. Harus dari B
D. Harus dari vertex genap

<details><summary>💡 Hint</summary>Mulai di satu vertex ganjil, selesai di yang lain.</details>
<details><summary>✅ Jawaban</summary>**B. B atau D.** Mulai dari salah satu yang ganjil.</details>

### Soal #106: Jembatan Königsberg
Jembatan Königsberg punya 4 daratan dengan derajat: 3, 3, 3, 5. Berapa vertex ganjil?
A. 0
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>3, 3, 3, 5 — semua ganjil!</details>
<details><summary>✅ Jawaban</summary>**D. 4.** Semua 4 vertex berderajat ganjil → tidak ada Euler Path.</details>

### Soal #107: Euler di Segitiga
```
A --- B --- C --- A
```
Apakah ada Euler Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Derajat: A=2, B=2, C=2. Semua genap.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Misalnya: A→B→C→A.</details>

### Soal #108: Euler di Path Linear
```
A --- B --- C --- D --- E
```
Ada Euler Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Derajat: A=1, B=2, C=2, D=2, E=1. Tepat 2 ganjil.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Mulai dari A, selesai di E (atau sebaliknya).</details>

### Soal #109: Menggambar Tanpa Mengangkat Pena
Bisakah menggambar bentuk ini tanpa mengangkat pena dan tanpa mengulang garis?
```
A --- B
|   /|
|  / |
| /  |
C --- D
```
A. Bisa
B. Tidak bisa

<details><summary>💡 Hint</summary>Hitung derajat: A=2, B=3, C=3, D=2. Tepat 2 ganjil → ada Euler Path!</details>
<details><summary>✅ Jawaban</summary>**A. Bisa.** Mulai dari B atau C, selesai di yang lain.</details>

### Soal #110: Amplop
Bisakah menggambar amplop ini tanpa mengangkat pena?
```
  A --- B
  |\ /|
  | X  |
  |/ \|
  C --- D
      |
      E
```
Hitung derajat: A=3, B=3, C=3, D=4, E=1.

A. Bisa (Euler Path)
B. Tidak bisa

<details><summary>💡 Hint</summary>Vertex ganjil: A(3), B(3), C(3), E(1) = 4 vertex ganjil.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak bisa.** Lebih dari 2 vertex ganjil.</details>

### Soal #111: Hamilton vs Euler
"Mengunjungi setiap KOTA tepat satu kali" adalah masalah...
A. Euler Path
B. Hamilton Path
C. BFS
D. DFS

<details><summary>💡 Hint</summary>Kota = Vertex. Setiap VERTEX tepat 1 kali = Hamilton.</details>
<details><summary>✅ Jawaban</summary>**B. Hamilton Path.**</details>

### Soal #112: Hamilton Path Sederhana
```
A --- B --- C --- D
```
Apakah A → B → C → D adalah Hamilton Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Setiap vertex dikunjungi tepat 1 kali? ✓</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #113: Hamilton Circuit
```
A --- B
|     |
C --- D
```
A → B → D → C → A. Apakah ini Hamilton Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua vertex dikunjungi 1 kali dan kembali ke awal?</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Semua vertex tepat 1 kali, dan kembali ke A.</details>

### Soal #114: Bukan Hamilton Path
```
A --- B --- C
      |
      D
```
A → B → D → B → C. Apakah ini Hamilton Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Vertex B dilewati 2 kali!</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** B dikunjungi 2 kali, melanggar aturan Hamilton.</details>

### Soal #115: Traveling Salesman
4 kota dengan jarak:
```
A-B:10, A-C:15, A-D:20
B-C:35, B-D:25, C-D:30
```
Hamilton Circuit terpendek mulai dari A?
A. A→B→D→C→A (total: 10+25+30+15 = 80)
B. A→B→C→D→A (total: 10+35+30+20 = 95)
C. A→C→B→D→A (total: 15+35+25+20 = 95)
D. A→D→B→C→A (total: 20+25+35+15 = 95)

<details><summary>💡 Hint</summary>Bandingkan total bobot setiap rute.</details>
<details><summary>✅ Jawaban</summary>**A. Total 80.** Ini yang terpendek.</details>

### Soal #116: Euler vs Hamilton - Perbedaan
Euler Path melewati setiap __ tepat 1 kali, Hamilton Path melewati setiap __ tepat 1 kali.
A. vertex; edge
B. edge; vertex
C. edge; edge
D. vertex; vertex

<details><summary>💡 Hint</summary>Euler = edge (garis). Hamilton = vertex (titik).</details>
<details><summary>✅ Jawaban</summary>**B. edge; vertex.**</details>

### Soal #117: Euler + Hamilton?
Bisakah sebuah graf memiliki Euler Circuit DAN Hamilton Circuit sekaligus?
A. Ya
B. Tidak pernah
C. Hanya di tree
D. Hanya di K5

<details><summary>💡 Hint</summary>C3 (segitiga) punya keduanya! A→B→C→A.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Contoh: segitiga C3.</details>

### Soal #118: Euler Path di K4
K4 (4 vertex semua saling terhubung). Derajat setiap vertex = 3 (ganjil). Berapa vertex ganjil?
A. 0
B. 2
C. 4
D. 1

<details><summary>💡 Hint</summary>Semua 4 vertex berderajat 3.</details>
<details><summary>✅ Jawaban</summary>**C. 4.** → Tidak ada Euler Path di K4!</details>

### Soal #119: Euler circuit di K5
K5: Derajat setiap vertex = 4 (genap). Ada Euler Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua vertex berderajat genap → syarat terpenuhi.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** K5 memiliki Euler Circuit.</details>

### Soal #120: Hamilton di Complete Graph
Apakah setiap complete graph Kn (n ≥ 3) memiliki Hamilton Circuit?
A. Ya
B. Tidak
C. Hanya genap
D. Hanya ganjil

<details><summary>💡 Hint</summary>Semua vertex saling terhubung, jadi selalu bisa kunjungi semua tepat 1 kali dan kembali.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #121: Peta Tukang Pos
Tukang pos ingin melewati semua jalan di kompleks tepat sekali. Ini adalah masalah...
A. Hamilton Path
B. Euler Path
C. BFS
D. Spanning Tree

<details><summary>💡 Hint</summary>Jalan = edge. Setiap EDGE tepat 1 kali = Euler.</details>
<details><summary>✅ Jawaban</summary>**B. Euler Path.**</details>

### Soal #122: Kurir Antar Paket
Kurir ingin mengunjungi semua alamat tepat sekali lalu kembali ke gudang. Ini adalah masalah...
A. Euler Circuit
B. Hamilton Circuit
C. Spanning Tree
D. BFS

<details><summary>💡 Hint</summary>Alamat = vertex. Setiap VERTEX tepat 1 kali + kembali = Hamilton Circuit.</details>
<details><summary>✅ Jawaban</summary>**B. Hamilton Circuit.**</details>

### Soal #123: Euler Path - Menghitung
```
  A
 / \
B---C
|   |
D---E
```
Derajat: A=2, B=3, C=3, D=2, E=2. Ada Euler Path?
A. Ya (2 vertex ganjil)
B. Tidak (4 vertex ganjil)

<details><summary>💡 Hint</summary>Vertex ganjil: B(3) dan C(3) = 2 vertex ganjil.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Mulai dari B, selesai di C.</details>

### Soal #124: Euler di Bintang
Star graph S4 (pusat + 4 vertex). Derajat: Pusat=4, Lainnya=1. Berapa vertex ganjil?
A. 0
B. 1
C. 4
D. 5

<details><summary>💡 Hint</summary>4 vertex berderajat 1 (ganjil). Pusat berderajat 4 (genap).</details>
<details><summary>✅ Jawaban</summary>**C. 4.** → Tidak ada Euler Path di star graph.</details>

### Soal #125: Euler di Wheel
Wheel W4 (C4 + pusat). Derajat: Pusat=4, Lainnya=3. Berapa vertex ganjil?
A. 0
B. 4
C. 5
D. 1

<details><summary>💡 Hint</summary>4 vertex lingkaran berderajat 3. Pusat berderajat 4.</details>
<details><summary>✅ Jawaban</summary>**B. 4.** → Tidak ada Euler Path.</details>

### Soal #126: Semi-Euler
Graf yang punya Euler Path tapi BUKAN Euler Circuit disebut...
A. Eulerian
B. Semi-Eulerian
C. Hamiltonian
D. Non-Eulerian

<details><summary>💡 Hint</summary>Punya path tapi tidak circuit → "setengah" Eulerian.</details>
<details><summary>✅ Jawaban</summary>**B. Semi-Eulerian.**</details>

### Soal #127: Menggambar Huruf "A"
Bisakah menggambar huruf A (garis-garisnya saja) tanpa mengangkat pena?
```
    /\
   /  \
  /----\
 /      \
```
Hitung vertex dan edge lalu cek derajatnya.

A. Bisa
B. Tidak bisa

<details><summary>💡 Hint</summary>Puncak: deg 2. Kiri bawah: deg 2. Kanan bawah: deg 2. Kiri tengah: deg 3. Kanan tengah: deg 3. → 2 ganjil.</details>
<details><summary>✅ Jawaban</summary>**A. Bisa.** 2 vertex ganjil → ada Euler Path.</details>

### Soal #128: Menambah Edge
Sebuah graf punya 4 vertex ganjil. Berapa edge minimum yang harus ditambah agar ada Euler Circuit?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>Setiap edge baru bisa mengurangi 2 vertex ganjil. Butuh 4/2 = 2 edge.</details>
<details><summary>✅ Jawaban</summary>**B. 2.**</details>

### Soal #129: Euler di Directed Graph
Di directed graph, Euler Circuit ada jika...
A. Semua vertex: in-degree = out-degree
B. Semua vertex berderajat genap
C. Ada 2 vertex ganjil
D. Graf punya cycle

<details><summary>💡 Hint</summary>Setiap masuk harus bisa keluar → in = out.</details>
<details><summary>✅ Jawaban</summary>**A.** In-degree = Out-degree untuk semua vertex.</details>

### Soal #130: Hamilton di Bipartite
Graf bipartite K2,3 (2 vertex kiri, 3 kanan). Apakah ada Hamilton Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Hamilton Circuit butuh jumlah vertex di kedua partisi sama. 2 ≠ 3.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Jumlah vertex di kedua sisi tidak sama.</details>

### Soal #131: Euler di C6
Cycle graph C6 (hexagon). Ada Euler Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua vertex berderajat 2 (genap).</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Ikuti lingkarannya saja.</details>

### Soal #132: Hamilton di C6
Ada Hamilton Circuit di C6?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>C6 sendiri sudah merupakan Hamilton Circuit!</details>
<details><summary>✅ Jawaban</summary>**A. Ya.**</details>

### Soal #133: Dirac's Theorem
Dirac: Jika graf simple punya V ≥ 3 dan setiap vertex berderajat ≥ V/2, maka...
A. Pasti ada Euler Circuit
B. Pasti ada Hamilton Circuit
C. Pasti tree
D. Pasti planar

<details><summary>💡 Hint</summary>Dirac's theorem menjamin Hamilton Circuit.</details>
<details><summary>✅ Jawaban</summary>**B. Pasti ada Hamilton Circuit.**</details>

### Soal #134: Menghitung Euler Path
```
A--B--C
|  |  |
D--E--F
```
Hitung derajat semua vertex.
A=2, B=3, C=2, D=2, E=3, F=2. Ada Euler?

A. Euler Circuit
B. Euler Path (bukan circuit)
C. Tidak ada

<details><summary>�� Hint</summary>2 vertex ganjil (B dan E). → Euler Path!</details>
<details><summary>✅ Jawaban</summary>**B. Euler Path.** Mulai dari B atau E.</details>

### Soal #135: Modifikasi Graf
Dari soal #134, jika kita tambahkan edge B-E, semua vertex akan berderajat genap. Sekarang ada apa?
A. Euler Path saja
B. Euler Circuit
C. Hamilton saja
D. Tidak ada

<details><summary>💡 Hint</summary>B jadi 4, E jadi 4. Semua genap!</details>
<details><summary>✅ Jawaban</summary>**B. Euler Circuit.**</details>

### Soal #136: Chinese Postman Problem
Tukang pos harus melewati semua jalan di graf, tapi graf punya 4 vertex ganjil. Apa yang harus dilakukan?
A. Melewati beberapa jalan 2 kali
B. Mengangkat kaki dan teleportasi
C. Mengabaikan beberapa jalan
D. Menambah vertex baru

<details><summary>💡 Hint</summary>Jika tidak ada Euler Path, beberapa edge harus diulang.</details>
<details><summary>✅ Jawaban</summary>**A. Melewati beberapa jalan 2 kali.** Ini disebut Chinese Postman Problem.</details>

### Soal #137: Hamilton di Path Graph
Path P5: A-B-C-D-E. Ada Hamilton Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>A→B→C→D→E sudah mengunjungi semua vertex tepat 1 kali.</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Path graph sendiri sudah merupakan Hamilton Path.</details>

### Soal #138: Hamilton Circuit di Path
Dari soal #137, ada Hamilton Circuit di P5?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>E tidak terhubung ke A. Tidak bisa kembali.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Tidak ada edge E-A untuk kembali ke awal.</details>

### Soal #139: Petersen Graph - Euler
Petersen Graph: 10 vertex, semua berderajat 3. Ada Euler Circuit?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua berderajat 3 (ganjil). 10 vertex ganjil > 2.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Terlalu banyak vertex ganjil.</details>

### Soal #140: K3,3 - Euler
K3,3: Setiap vertex berderajat 3. Ada Euler Path?
A. Ya (ada Euler Path)
B. Tidak

<details><summary>💡 Hint</summary>6 vertex semua ganjil → 6 > 2.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.**</details>

### Soal #141: Menggambar Bintang 5 Ujung
Bisakah menggambar ☆ tanpa mengangkat pena (5 garis, 5 titik potong)?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Semua vertex berderajat 2 → semua genap!</details>
<details><summary>✅ Jawaban</summary>**A. Ya.** Euler Circuit! (Semua vertex berderajat genap.)</details>

### Soal #142: Euler + Analogi Kehidupan
Museum punya 10 ruangan dan 15 pintu. Pengunjung ingin masuk lewat semua pintu tepat sekali. Ini adalah masalah...
A. Hamilton Path (ruangan = vertex)
B. Euler Path (pintu = edge)
C. BFS
D. DFS

<details><summary>💡 Hint</summary>Pintu = edge. Setiap EDGE tepat 1 kali = Euler.</details>
<details><summary>✅ Jawaban</summary>**B. Euler Path.**</details>

### Soal #143: Euler Path Existence
Sebuah graf connected punya 0 vertex ganjil. Apa kesimpulannya?
A. Ada Euler Path tapi bukan Circuit
B. Ada Euler Circuit (dan otomatis ada Euler Path juga)
C. Tidak ada Euler Path
D. Ada Hamilton Circuit

<details><summary>💡 Hint</summary>0 ganjil → Euler Circuit. Circuit selalu bisa jadi Path (tanpa syarat kembali).</details>
<details><summary>✅ Jawaban</summary>**B.** Ada Euler Circuit (yang juga merupakan Euler Path).</details>

### Soal #144: Hitung Edge dari Euler Condition
Graf punya 5 vertex semua berderajat 4. Ada Euler Circuit? Berapa edge?
A. Ya, 10 edge
B. Tidak, 10 edge
C. Ya, 20 edge
D. Tidak, 5 edge

<details><summary>💡 Hint</summary>Semua genap → Euler Circuit. Edge = (5×4)/2 = 10.</details>
<details><summary>✅ Jawaban</summary>**A. Ya, 10 edge.**</details>

### Soal #145: Hamilton di Disconnected
Apakah graf disconnected bisa punya Hamilton Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Hamilton harus mengunjungi SEMUA vertex. Kalau ada yang terpisah, tidak mungkin.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** Harus connected untuk Hamilton Path.</details>

### Soal #146: Euler di Disconnected
Apakah graf disconnected bisa punya Euler Path?
A. Ya
B. Tidak

<details><summary>💡 Hint</summary>Euler Path harus melewati SEMUA edge. Kalau ada komponen yang tidak terjangkau, tidak mungkin.</details>
<details><summary>✅ Jawaban</summary>**B. Tidak.** (Kecuali komponen lain tidak punya edge.)</details>

### Soal #147: Membuat Graf Euler
Kamu punya 4 vertex. Berapa edge minimum agar ada Euler Circuit?
A. 2
B. 3
C. 4
D. 6

<details><summary>💡 Hint</summary>Cycle C4 punya 4 edge dan semua vertex berderajat 2 (genap).</details>
<details><summary>✅ Jawaban</summary>**C. 4.** Bentuk persegi (C4).</details>

### Soal #148: Perbedaan Kunci
Manakah pernyataan yang BENAR?
A. Euler Path = lewat semua vertex 1 kali
B. Hamilton Path = lewat semua edge 1 kali
C. Euler Path = lewat semua edge 1 kali
D. Keduanya sama

<details><summary>💡 Hint</summary>Euler = EDGE. Hamilton = VERTEX.</details>
<details><summary>✅ Jawaban</summary>**C.**</details>

### Soal #149: Menghitung Jalur Hamilton
```
A --- B
|     |
C --- D
```
Berapa banyak Hamilton Circuit berbeda yang mungkin (mulai dari A)?
A. 1
B. 2
C. 3
D. 4

<details><summary>💡 Hint</summary>A→B→D→C→A dan A→C→D→B→A (yang kedua = kebalikan pertama).</details>
<details><summary>✅ Jawaban</summary>**A. 1.** (Atau 2 jika arah berlawanan dihitung berbeda.)</details>

### Soal #150: Refleksi Bagian 3
Untuk mengecek Euler Path/Circuit, langkah pertama yang harus kamu lakukan adalah...
A. Menggambar graf ulang
B. Menghitung derajat setiap vertex
C. Mencari cycle
D. Menghitung jumlah vertex

<details><summary>💡 Hint</summary>Syarat Euler bergantung pada derajat vertex.</details>
<details><summary>✅ Jawaban</summary>**B. Menghitung derajat setiap vertex.** Lalu hitung yang ganjil!</details>

---
[< Bagian 2 (51-100)](./07-graf-soal-part-2.md) | [< Kembali ke Indeks](../07-graf-sederhana.md) | [Bagian 4 (151-200) >](./07-graf-soal-part-4.md)
