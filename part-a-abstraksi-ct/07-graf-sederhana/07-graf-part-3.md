🔙 **Kembali ke Materi:** [Materi 07 Graf Sederhana](../07-graf-sederhana.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 07. Graf Sederhana - Bagian 3: Algoritma Jelajah Graf & Tips OSN-K

[< Bagian 2: Rumus & Trik](./07-graf-part-2.md) | [< Kembali ke Indeks](../07-graf-sederhana.md)

---

## 🔍 Cara Komputer Menjelajahi Graf

Bayangkan kamu punya peta sebuah pulau dengan banyak kota. Kamu ingin **mengunjungi semua kota**. Ada 2 strategi:

1. **BFS** — Kunjungi yang **terdekat dulu**, baru yang jauh.
2. **DFS** — Langsung **masuk sedalam mungkin**, baru mundur.

Kedua cara ini sangat penting di informatika dan sering muncul secara tersirat di soal OSN-K.

---

## 🌊 BFS (Breadth-First Search) — Pencarian Melebar

### Analoginya:
Bayangkan kamu **menjatuhkan batu ke kolam yang tenang**. Riak airnya menyebar ke segala arah, lapisan demi lapisan. Riak **tidak langsung lompat ke ujung kolam**, tapi menyebar secara merata dari titik tengah.

BFS bekerja persis seperti itu!

### Cara Kerjanya (Step by Step):

```
Graf contoh:
      A
     / \
    B   C
   / \   \
  D   E   F
```

**Mulai dari A:**
1. Kunjungi **A** (Lapisan 0)
2. Kunjungi semua tetangga A → **B, C** (Lapisan 1)
3. Kunjungi semua tetangga B dan C yang belum dikunjungi → **D, E, F** (Lapisan 2)
4. Selesai! Semua titik sudah dikunjungi.

**Hasil BFS:** A → B → C → D → E → F

### BFS Pakai Apa?
BFS menggunakan **Queue (Antrian!)** — ingat materi sebelumnya? FIFO!

Cara mainnya:
1. Masukkan titik awal ke antrian: **[A]**
2. Keluarkan A, masukkan tetangganya: **[B, C]**
3. Keluarkan B, masukkan tetangganya (yang belum dikunjungi): **[C, D, E]**
4. Keluarkan C, masukkan tetangganya: **[D, E, F]**
5. Keluarkan D, E, F → Selesai!

### Kapan BFS Berguna?
- ✅ **Mencari jarak terpendek** (berapa langkah minimal dari A ke F?)
- ✅ **Fitur "Orang yang mungkin kamu kenal"** di media sosial (teman dari teman)
- ✅ **Menyebar info** — seperti memodelkan penyebaran virus, gosip, atau sinyal WiFi

### Contoh Soal Gaya OSN-K:
> "Dari titik A, berapa langkah minimum untuk sampai ke F?"

Gunakan BFS! Dari contoh di atas:
- A ke B = 1 langkah
- A ke C = 1 langkah
- A ke D = 2 langkah (lewat B)
- A ke E = 2 langkah (lewat B)
- A ke F = 2 langkah (lewat C)

Jawaban: **2 langkah.**

---

## 🏔️ DFS (Depth-First Search) — Pencarian Mendalam

### Analoginya:
Bayangkan kamu **tersesat di labirin**. Strategi kamu: jalan terus lurus **sedalam mungkin** sampai mentok tembok. Kalau buntu, **mundur ke persimpangan terakhir** lalu coba jalan lain. Ulangi sampai keluar.

DFS bekerja persis seperti itu!

### Cara Kerjanya (Step by Step):

```
Graf yang sama:
      A
     / \
    B   C
   / \   \
  D   E   F
```

**Mulai dari A:**
1. Kunjungi **A**
2. Masuk ke tetangga pertama → **B**
3. Dari B, masuk lagi ke tetangga pertama → **D**
4. D sudah buntu (tidak ada tetangga baru) → **Mundur ke B**
5. Dari B, coba tetangga lain → **E**
6. E buntu → **Mundur ke B** → **Mundur ke A**
7. Dari A, coba tetangga lain → **C**
8. Dari C → **F**
9. Selesai!

**Hasil DFS:** A → B → D → E → C → F

### DFS Pakai Apa?
DFS menggunakan **Stack (Tumpukan!)** — ingat materi sebelumnya? LIFO!

Atau lebih gampangnya, DFS bisa pakai **Rekursi** (fungsi yang memanggil dirinya sendiri — tapi ini topik pemrograman lanjutan).

### Kapan DFS Berguna?
- ✅ **Mencari semua kemungkinan jalur** (misal: ada berapa cara dari A ke F?)
- ✅ **Memecahkan puzzle** (Sudoku, 8 Queens, maze)
- ✅ **Cek apakah graf terhubung** (connected)
- ✅ **AI musuh di game** yang mengejar pemain lewat jalur tertentu

---

## ⚔️ BFS vs DFS — Perbandingan Lengkap

| Aspek | BFS | DFS |
| :--- | :--- | :--- |
| **Strategi** | Melebar dulu (layer by layer) | Mendalam dulu (sedalam mungkin) |
| **Pakai struktur data** | **Queue** (Antrian, FIFO) | **Stack** (Tumpukan, LIFO) |
| **Cocok untuk** | Jarak terpendek | Mencari semua jalur |
| **Analogi** | Riak air di kolam | Petualangan di labirin |
| **Memori** | Lebih boros (simpan banyak titik sekaligus) | Lebih hemat |
| **Urutan kunjungan** | "Selapis dulu baru lanjut" | "Sedalam mungkin baru mundur" |

### Cara Gampang Ingat:

- **BFS** = **B**readth = **B**road = **L**ebar → **Menyebar merata**
- **DFS** = **D**epth = **D**alam → **Nyemplung sedalam mungkin**

---

## 🌐 Graf di Kehidupan Nyata (Biar Makin Paham)

### Di Dunia Informatika:
| Aplikasi | Vertex (Titik) | Edge (Garis) | Jenis Graf |
| :--- | :--- | :--- | :--- |
| **Internet** | Website | Hyperlink | Directed (klik searah) |
| **Google Maps** | Persimpangan | Jalan | Weighted (ada jaraknya) |
| **Facebook** | Akun | Pertemanan | Undirected (dua arah) |
| **Instagram** | Akun | Following | Directed (satu arah) |
| **WhatsApp Group** | Anggota | Bisa chat | Undirected |
| **Wikipedia** | Artikel | Link ke artikel lain | Directed |

### Di Dunia Game:
| Aplikasi | Vertex (Titik) | Edge (Garis) | Penjelasan |
| :--- | :--- | :--- | :--- |
| **Peta Game** | Lokasi/kota | Jalur antar kota | Pathfinding NPC |
| **Skill Tree** | Skill | Garis prasyarat | Harus unlock skill A sebelum B |
| **Dialog Tree** | Pilihan dialog | Garis ke reaksi NPC | Setiap pilihan beda dampak |
| **Puzzle** | State (kondisi) | Langkah/aksi | Semua kemungkinan kondisi |

### Di Kehidupan Sehari-hari:
| Aplikasi | Vertex (Titik) | Edge (Garis) |
| :--- | :--- | :--- |
| **Rute Bus** | Halte | Jalur bus |
| **Silsilah Keluarga** | Orang | Hubungan orangtua-anak |
| **Jadwal Penerbangan** | Bandara | Rute penerbangan |
| **Jaringan Listrik** | Gardu | Kabel listrik |
| **Turnamen** | Tim | Pertandingan |

---

## 💡 Tips & Trik Menghadapi Soal Graf di OSN-K

### Tip 1: SELALU Gambar Grafnya!
Kalau soal memberikan deskripsi kata-kata, **gambar dulu** grafnya di kertas. Ini membantu otak memproses informasi visual jauh lebih cepat.

### Tip 2: Hitung Derajat Dulu
Banyak soal bisa diselesaikan hanya dengan **menghitung derajat** tiap titik dan pakai **Rumus Jabat Tangan**.

### Tip 3: Cek Euler Path/Circuit
Kalau soal bertanya "bisakah melewati semua jalan tepat sekali?", langsung:
1. Hitung derajat setiap titik
2. Hitung berapa yang **ganjil**
3. Cocokkan dengan tabel syarat!

### Tip 4: BFS = Jarak Terpendek
Kalau soal bertanya "berapa langkah minimum?", pikirkan **BFS** (lapisan demi lapisan).

### Tip 5: Perhatikan "Tepat Satu Kali"
- Lewati setiap **GARIS** tepat 1 kali → **Euler**
- Kunjungi setiap **TITIK** tepat 1 kali → **Hamilton**
Jangan sampai tertukar!

---

## 🚀 Kesimpulan Akhir

Selamat! Kamu sudah mempelajari **semua konsep dasar Teori Graf** yang diperlukan untuk OSN-K:

| Apa yang kamu pelajari | Di mana |
| :--- | :--- |
| Definisi graf, vertex, edge, degree | Bagian 1 |
| Jenis graf (undirected, directed, weighted, tree) | Bagian 1 |
| Cara komputer menyimpan graf | Bagian 1 |
| Rumus Jabat Tangan | Bagian 2 |
| Euler Path & Circuit | Bagian 2 |
| Hamilton Path & Circuit | Bagian 2 |
| Spanning Tree & MST | Bagian 2 |
| BFS & DFS | Bagian 3 |
| Aplikasi dunia nyata | Bagian 3 |

> 🎯 **Kamu sudah resmi menyelesaikan seluruh materi Part A: Abstraksi dan Computational Thinking!** Dengan pemahaman ini, kamu punya fondasi kuat untuk menghadapi soal-soal OSN-K Informatika. Terus berlatih soal ya!

---

[< Bagian 2: Rumus & Trik](./07-graf-part-2.md) | [< Kembali ke Indeks](../07-graf-sederhana.md)
