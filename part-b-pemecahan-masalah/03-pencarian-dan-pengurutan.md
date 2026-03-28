# 3. Pencarian & Pengurutan (Seni Menyusun Kamus Bebek)

Di dunia *Competitive Programming* (Pemrograman Kompetitif) dan OSN Informatika, **Pencarian (Searching)** dan **Pengurutan (Sorting)** adalah menu sarapan sehari-hari.

Kabar baiknya: Karena kamu sedang mengerjakan OSN-K Kertas/Teori, kamu *hampir tidak pernah* ditanya untuk menghafal barisan kodenya dari nol.
Namun kamu **DIWAJIBKAN** paham cara menyimulasikan gerak-gerik algoritmanya dari detik pertama sampai akhir (*Tracing/Tracking Variable*). Kamu harus bisa mendeteksi: *"Pada putaran ke-3, beginilah urutan susunan angka sementaranya."*

Mari kita bedah cara melacak algoritma klasik ini satu per satu.

---

## 🔍 A. Pencarian Lurus vs Pencarian Lipat Dua (Linear vs Binary)

Pak Dengklek menyimpan buku jurnal yang berisi daftar $1.000$ resep telur dadar, dideretkan di rak berdasarkan nomor ID dari $1$ sampai $1.000$. Hari ini beliau lupa di mana resep rahasia "Telor Bebek Suci" (Katakanlah resep itu ID $= 614$).

Bagaimana cara mencari benda ini dengan pola pikir beda algoritma?

### 1. Linear Search (Pencarian Saklek Brute Force)
Ini adalah insting anak kecil.
Beliau berjalan ke rak paling awal, mengecek majalah pertama (ID=1). Bukan. Dia buang.
Beliau cek buku kedua (ID=2). Bukan. Buang.
Beliau cek terus... $3, 4, 5, \dots$ sampai buku ke $614$. Hore Ketemu!

**Kinerja (Time Complexity):** 
- Kasus terburuk: Buku dicari ada di posisi 1.000. Beliau harus ngecek 1.000 kali. Waktu eksekusi ini bergerak lurus dengan jumlah total data (disebut $O(N)$ secara notasi akademis komputer). Ini terlalu lambat jika total data ada 2 miliar baris di database.

### 2. Binary Search (Seni Membelah Dunia Jadi Dua)
Pemrograman kompetitif membenci Linear Search untuk data triliunan. Makanya diciptakan dewa penyeleksi: **Binary Search**.

**Syarat Mutlak Binary Search:** Datanya HARUS, WAJIB, MUTLAK sudah diurutkan (Sorted) dari kecil ke besar. Kalau datanya acak, Binary Search itu bunuh diri konyol berantakan.
*(Untunglah daftar buku Pak Dengklek ini sudah urut ID 1 s.d 1.000!)*

Mari ber-simulasi menelusuri Binary Search Pak Dengklek dalam misinya mencari ID-$614$:
- **Langkah 1:** Beliau langsung menunjuk Titik Tengah (Median) daftar buku. Setengahnya 1000 adalah 500. Beliau ambil Majalah ke-500.
- **Pengecekan:** Ternyata isinya resep bernomor 500. Pak Dengklek membatin: *"Oh resep ini 500, padahal tujuanku nyari si 614. Karena angka resep makin besar makin ke kanan... PASTILAH resep 614 ada di sebelah kanan rentang bukuku."*
- **Sisi Pembantaian (Eliminasi):** Beliau dengan sombong **MEMBUANG 500 BUKU YANG BERADA DI SEBELAH KIRINYA**. Tak perlu dicek. Mustahil 614 ada di kumpulan 1-500. (Populasi target sisa $501$ sampai $1000$).
- **Langkah 2:** Beliau ambil titik tengah dari barisan yang tersisa ($500$ sampai $1000$). Tengahnya adalah $750$. 
- **Pengecekan:** Dilihatnya, isinya resep ke-750. *"Waduh kelabasan (750 > 614). Pasti 614 kelentisut di tumpukan Kiri dari titik ini."*
- **Sisi Pembantaian:** Buang 250 buku di sisi kanan (Dari 751 sampai 1000). 
- **Langkah 3... 4... dan seterusnya.** Beliau terus membelah tumpukan buku yang tersisa jadi dua, dua, dan dua.

Dengan teknik ini, untuk mencari 1 resep dari $1.000$ kemungkinan, beliau hanya butuh **sekitar 10 kali lompatan ngecek (karena $2^{10} = 1024$)!**
Bandingkan dengan *Linear Search* yang butuh $1.000$ kali cek. Inilah esensi kecanggihan *Tracing Looping* Binary Search. Telinga dan mata harus peka melibas rentang nilai sisa kiri dan kanan ini secara berjenjang di kertasmu saat OSN-K.

---

## 🎲 B. Memahami Anatomi 3 Serangkai Sorter Klasik

Nah, Binary Search kan rewel tuh, minta datanya biar "Diurutkan" dulu. Memangnya gimana rahasia komputer menggeser barang yang semrawut biar urut? 

Olimpiade OSN-K sering menugaskan peserta melacak posisi susunan sementara *array* setelah `3 putaran iterasi kodingan Sort`. Mari kuasai perbedaan konsep *"Seni Berpindah Posisi"* tiga algoritma ini:

### 1. Bubble Sort (Gelembung Pemukul Tetangga)
Namanya *Bubble* (Gelembung), elemen-elemen besar perlahan akan mengapung melayang ke kanan deretan.
- **Konsep:** Dia jalan dari awal ke akhir, mengecek dirinya dengan 1 orang tetangga persis di kanannya. *"Eh bro, badanmu kan lebih kecil nih, kita tukeran bangku dong biar lu di kiri"*. Begitu terus sampai ujung barisan.
- **Tanda Tangan Visual (Ciri Khas Tracing):** Setiap kali 1 Putaran Keseluruhan Keliling (Iterasi 1) Selesai, dijamin **ANGKA PALING BESAR 100% PASTI SUDAH MENGENDAP DI POSISI PALING KANAN (UJUNG)**. 
*(Makanya putaran berikutnya nggak perlu cek elemen ujung kanan lagi).*

### 2. Selection Sort (Sang Pecari Kasta Terendah)
Berlawanan dengan Bubble. *Selection* ini algoritmanya lebih "santai dan pendiam, tapi teliti".
- **Konsep:** Jangan buru-buru menukar setiap jam! Kita picingkan mata sepanjang sisa deretan, cari siapa sih angka paling kecil / paling cebol *di seluruh deretan barisan*? Oh, si 12! Ambil si cebol 12 itu, langsung lempar/tukar bangku aja paksa bawa ke posisi paling Kiri (Garis Start iterasi).
- **Tanda Tangan Visual (Ciri Khas Tracing):** Di awal iterasi-1, langsung terbentuk **1 ELEMEN TERKECIL MENDARAT ABADI DI SISI KIRI**. Iterasi kedua, nemu anak terkecil kedua mendarat stabil di sisi kiri nomor 2... dst. Tembok keamanan stabil mengukuh dari area sisi kiri pelan-pelan ke kanan.

### 3. Insertion Sort (Bapak Pemain Kartu Remi)
Pernah menyortir setumpuk kartu Remi/Uno di tangan kiri setelah dikocok?
Anggap saja mulanya tangan kiri cuma memegang 1 kartu (otomatis urut). Tangan kanan pelan-pelan memungut kartu kedua.
- **Konsep:** Ambil satu elemen baru (misal memungut angka 7). Cek deretan yang *sudah dirapikan di sebelah kirimu*. Sisipkan (Insert) angka 7 itu pelan-pelan mendesak dan mendorong paksa elemen lain menggeser sampai 7 nangkring di posisi sah urutannya.
- **Tanda Tangan Visual (Ciri Khas Tracing):** Separuh deret dari pinggir kiri itu "Selalu terlihat urut secara temporer" (Padahal sisa yang kanan masih ngacak jelek berserakan). Seiring putaran bertambah, "Tembok area rapi" itu makin melebar memakan memfagositosis array yang acak.

---

### Siap Di Uji Tracing?
Jika pada soal OSN-K disajikan barisan bilangan mentah: `[8, 4, 1, 9, 2]`
Kemudian muncul pertanyaan: *"Jika dikenakan aturan Selection Sort Ascending, seperti apa tatanan array tepat setelah 2 kali proses penukaran angka keliling utama selesai?"*

**Jawaban Compiler Manusia-mu:**
- Putaran 1: Cari angka terminator cebol murni di area `[8, 4, 1, 9, 2]`. Ditemukan `1` (di indeks 2). Suruh tukaran lapak maksa sama posisi si pemegang Indeks 0 (yakni `8`). 
Array berubah jadi: `[`**`1`**`, 4, 8, 9, 2]` *(Elemen 1 udah gembok kekunci kebal)*.
- Putaran 2: Pandangan OSN-K menyempit, cuma mengintip sisa antrian `[4, 8, 9, 2]`. Cari paling cebol. Ditemukan `2` di pucuk. Tukar dengan gembong sisa yang paling depan (yakni `4`).
Array memutasi jadi: `[`**`1, 2`**`, 8, 9, 4]` *(Tembok kiri membentang gembok kebal berlanjut)*.

Hasil Laporan ke Pusat Pilihan Ganda = `[1, 2, 8, 9, 4]`. Berani coba algoritma Bubble / Insertion dengan teliti di atas kertas coret OSN-K mu nanti? Latihan di 1 lembar buram sangat dianjurkan!

---
Lanjut kita menuju level terkeras dalam memecahkan masalah. Kalau soalnya nggak bisa pakai Greedy, dan nggak bisa dibabat pakai Sorting... kita hanya punya satu senjata nuklir terakhir. Selamat datang di negeri Dynamic Programming!

⏩ **[Modul 04: Dynamic Programming Dasar (Metode Seni Mengingat Memo)](./04-dynamic-programming-dasar.md)**

---
[< Modul Part B Sebelumnya: Algoritma Greedy](./02-algoritma-greedy.md)
[< Kembali ke Indeks Part B](./README.md)
