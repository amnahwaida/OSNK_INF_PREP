# 07. Graf Sederhana - Bagian 1: Kenalan Dulu Sama Graf

[< Kembali ke Indeks Materi](../07-graf-sederhana.md) | [Bagian 2: Rumus & Trik Penting >](./07-graf-part-2.md)

---

## 🤔 Apa Sih Graf Itu?

Coba bayangkan kamu buka **Google Maps**. Di sana ada:
- **Titik-titik** = Lokasi (rumahmu, sekolah, mall, dll.)
- **Garis-garis** = Jalan yang menghubungkan lokasi-lokasi itu

Nah, dalam informatika, kita menyebut kumpulan titik dan garis ini sebagai **Graf**.

Lebih formal:
- **Titik** disebut **Vertex** (jamak: Vertices) atau **Node**
- **Garis** disebut **Edge** (Sisi)

```
Contoh paling simpel:

  Rumah ---- Sekolah ---- Mall
```
Ini adalah graf dengan **3 vertex** dan **2 edge**. Gampang kan?

---

## 📖 Kosakata Wajib (Hafalin Ya!)

Sebelum lanjut, kamu harus kenal dulu istilah-istilah ini. Tenang, aku kasih analogi biar gampang.

### 1. Vertex (Titik)
Ini adalah "benda" atau "tempat" dalam graf. 

**Contoh di dunia nyata:**
- Di peta → Kota
- Di Instagram → Akun orang
- Di game → Lokasi/checkpoint

### 2. Edge (Garis)
Ini adalah "hubungan" antara dua vertex. 

**Contoh di dunia nyata:**
- Di peta → Jalan
- Di Instagram → Hubungan "following"
- Di game → Jalur antar lokasi

### 3. Degree (Derajat)
**Berapa banyak garis yang nyambung ke satu titik**. Sesimpel itu.

**Contoh:** Kamu punya 5 teman di Facebook. Artinya, **derajat kamu = 5** (ada 5 garis pertemanan yang nyambung ke kamu).

```
       Budi
        |
  Ani---KAMU---Cici
       / \
     Dedi  Eka

Derajat KAMU = 5 (terhubung ke Ani, Budi, Cici, Dedi, Eka)
```

### 4. Adjacent (Bertetangga)
Dua titik yang **langsung terhubung** oleh satu garis disebut "bertetangga".

**Contoh:** Jika ada jalan langsung dari rumahmu ke sekolah, maka Rumah dan Sekolah itu "bertetangga". Tapi kalau harus lewat perempatan dulu, berarti mereka **tidak** langsung bertetangga.

### 5. Path (Jalur)
**Rute dari satu titik ke titik lain**, lewat beberapa garis dan titik.

```
Rumah → Perempatan → Sekolah → Mall

Ini adalah "Path" dari Rumah ke Mall, yang melewati 3 edge.
```

### 6. Cycle (Siklus)
Path yang **ujungnya balik lagi ke titik awal**. Kayak jalan-jalan keliling kompleks terus balik ke rumah lagi.

```
Rumah → Toko → Masjid → Rumah    ← ini Cycle!
```

---

## 🗂️ Jenis-Jenis Graf (Ada 4 yang Penting)

### 1. 🔄 Graf Tak Berarah (Undirected Graph)

Garisnya **tidak ada panahnya**. Artinya, kalau bisa dari A ke B, pasti bisa juga dari B ke A.

**Analogi gampang:** **Pertemanan di Facebook.** Kalau kamu berteman dengan Budi, otomatis Budi juga berteman denganmu. Hubungannya dua arah.

```
  A --- B       (A bisa ke B, B bisa ke A)
  |     |
  C --- D
```

### 2. ➡️ Graf Berarah (Directed Graph / Digraph)

Setiap garisnya **ada panahnya** (menunjukkan arah). Jadi A bisa ke B, tapi B **belum tentu** bisa ke A.

**Analogi gampang:** **Follow di Instagram.** Kamu bisa follow Atta Halilintar, tapi Atta belum tentu follow kamu balik. Hubungannya satu arah.

```
  A --> B       (A bisa ke B, tapi B TIDAK bisa ke A)
  |     |
  v     v
  C --> D
```

### 3. ⚖️ Graf Berbobot (Weighted Graph)

Setiap garisnya punya **angka** yang menunjukkan "harga" — bisa jarak, waktu, atau biaya.

**Analogi gampang:** **Google Maps.** Jalan dari rumah ke sekolah itu 3 km, tapi dari rumah ke mall itu 10 km. Angka km ini disebut **bobot (weight)**.

```
  Rumah --3km-- Sekolah
    \              /
    10km         5km
      \          /
       Mall
```

### 4. 🌳 Tree (Pohon)

Ini adalah graf yang **spesial banget**: semua titik terhubung, tapi **tidak ada siklus** (tidak ada jalan memutar).

**Analogi gampang:** **Silsilah Keluarga.** Kakek → Ayah → Kamu. Tidak ada yang melingkar. Atau, **Folder di komputermu:** Folder utama → Sub-folder → File.

```
        Kakek
       /     \
    Ayah     Paman
   /    \      |
  Kamu  Adik  Sepupu
```

**Fakta penting:** Jika sebuah pohon punya **V titik**, maka ia selalu punya tepat **V - 1 garis**. Contoh: 6 orang di silsilah di atas, jumlah garis = 5.

### Tabel Ringkasan

| Jenis | Ada Panah? | Ada Angka? | Boleh Memutar? | Contoh |
| :--- | :---: | :---: | :---: | :--- |
| Tak Berarah | ❌ | ❌ | ✅ | Facebook |
| Berarah | ✅ | ❌ | ✅ | Instagram |
| Berbobot | Bisa dua-duanya | ✅ | ✅ | Google Maps |
| Pohon (Tree) | ❌ | ❌ | ❌ | Folder Komputer |

---

## 🖥️ Bagaimana Komputer Menyimpan Graf?

Kita bisa gambar graf di kertas, tapi komputer tidak bisa gambar. Jadi, komputer menyimpan graf dalam bentuk **tabel** atau **daftar**.

### Cara 1: Tabel (Adjacency Matrix)

Buat tabel berukuran jumlah titik × jumlah titik. Isi angka **1** jika dua titik terhubung, angka **0** jika tidak.

**Contoh graf:**
```
A --- B
|     |
C --- D
```

**Tabelnya:**
```
      A    B    C    D
A  [  0    1    1    0  ]
B  [  1    0    0    1  ]
C  [  1    0    0    1  ]
D  [  0    1    1    0  ]
```

Cara bacanya: Baris A kolom B = 1. Artinya, A dan B **terhubung**. Baris A kolom D = 0. Artinya, A dan D **tidak langsung terhubung**.

**Kapan pakai ini?** Cocok kalau grafnya kecil (kurang dari 100 titik), atau kalau sering ditanya "apakah A dan B nyambung?"

### Cara 2: Daftar Tetangga (Adjacency List)

Tiap titik menyimpan **daftar siapa saja tetangganya**.

```
A → [B, C]
B → [A, D]
C → [A, D]
D → [B, C]
```

Cara bacanya: A punya tetangga B dan C. D punya tetangga B dan C.

**Kapan pakai ini?** Cocok kalau grafnya besar tapi garisnya sedikit (misal 1000 titik tapi cuma 50 garis). Ini lebih hemat memori.

---

> **Sampai sini paham?** Bagus! Kamu sudah mengerti dasar-dasar graf: apa itu vertex, edge, degree, jenis-jenis graf, dan cara komputer menyimpannya. Di Bagian 2, kita akan belajar **rumus-rumus penting** yang sering keluar di OSN-K!

---

[< Kembali ke Indeks Materi](../07-graf-sederhana.md) | [Bagian 2: Rumus & Trik Penting >](./07-graf-part-2.md)
