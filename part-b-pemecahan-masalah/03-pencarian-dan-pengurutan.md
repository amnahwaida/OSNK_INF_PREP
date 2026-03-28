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

### 1. Bubble Sort (Hukuman Baris Upacara Bendera)
Bayangkan kamu sedang baris upacara bendera hari Senin, tapi acak-acakan tinggi badannya. Guru BP menyuruh kalian berbaris urut dari pendek ke tinggi.
- **Konsep:** Guru mengecek 2 anak bersebelahan dari baris paling depan. *"Eh, lu kan lebih tinggi dari temen lu, minggir ganti posisi ke belakang dia!"*. Begitu terus, si guru mukul pundak pelan "Tukaran... Tukaran...".
- **Tanda Tangan Visual (Ciri Khas Tracing):** Sadar tidak sadar, setelah Guru BP jalan dari ujung depan sampai 1 putaran mentok, **Siswa yang PALING TINGGI se-angkatan pasti otomatis sudah 'terdorong' mentok nongkrong di barisan paling belakang**. Gembok! Barisan buntut nggak perlu dicek lagi.

### 2. Selection Sort (Pak RT Milih Bantuan Siswa Miskin)
Berlawanan dengan Bubble yang repot nukar-nukar anak sebelahan tiap detik, *Selection* ini gayanya mirip Pak RT yang kalem tapi jeli.
- **Konsep:** Jangan buru-buru ngusir orang sebelahan! Pak RT diam sejenak picingkan mata sepanjang sisa deretan, dari ujung ke ujung. Dia cari: *"Siapa nih anak yang sepatunya paling bolong (Nilai paling kecil/Cebol) di lapangan ini?"* Oh si Dodo! Sini Do, kamu kutarik paksa baris di bangku VVIP paling depan (Kiri).
- **Tanda Tangan Visual (Ciri Khas Tracing):** Di iterasi-1, langsung **1 ANAK PALING KECIL MENDARAT ABADI DI SAYAP KIRI**. Putaran kedua, cari paling cebol selanjutnya di kerumunan sisa, pindahkan ke nomor urut 2. Tembok keamanan stabil mengunci satu per satu dari sayap kiri.

### 3. Insertion Sort (Momen Main Kartu Remi/Uno Waktu Istirahat)
Pernah main capsa, uno, atau remi pas jam istirahat pakai tangan kiri?
Awalnya tangan kirimu kosong. Lalu kamu jongkok memegang jemput kartu yang dibagikan satu per satu.
- **Konsep:** Tangan kirimu udah pegang 2 kartu cakep urut. Eh dapet kartu ketiga (angka 7). Pikiranmu langsung jalan: *"Wah, 7 ini harus kusisipkan di sela-sela angka 5 dan 9 yang udah kupegang nih!"*. Kamu mendorong (Insert) paksa kartu 7 itu nyempil ke tengah.
- **Tanda Tangan Visual (Ciri Khas Tracing):** Kartu yang dipegang tangan kirimu "Selalu terlihat seolah-olah udah urut" (Padahal kartu di tumpukan tengah meja masih kacau meronta). Lama-lama "tembok kartu Tangan Kiri" ini makan semua tumpukan meja, ngelebar sampai lunas.

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

## ⚔️ Simulasi Tarung: Bedah 300 Soal Pencarian & Pengurutan

Untuk menguji telunjuk dan matamu menyimulasikan gerak-gerik array dari *Bubble, Selection, dan Binary Search*, hajar uji nyali 300 soal ini:

1. **[Latihan Soal Part 1 (Soal 1-50)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-1.md)**
2. **[Latihan Soal Part 2 (Soal 51-100)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-2.md)**
3. **[Latihan Soal Part 3 (Soal 101-150)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-3.md)**
4. **[Latihan Soal Part 4 (Soal 151-200)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-4.md)**
5. **[Latihan Soal Part 5 (Soal 201-250)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-5.md)**
6. **[Latihan Soal Part 6 (Soal 251-300)](./03-pencarian-dan-pengurutan/03-pencarian-dan-pengurutan-soal-part-6.md)**

---

Lanjut kita menuju level terkeras dalam memecahkan masalah. Kalau soalnya nggak bisa pakai Greedy, dan nggak bisa dibabat pakai Sorting... kita hanya punya satu senjata nuklir terakhir. Selamat datang di negeri Dynamic Programming!

⏩ **[Modul 04: Dynamic Programming Dasar (Metode Seni Mengingat Memo)](./04-dynamic-programming-dasar.md)**

---
[< Modul Part B Sebelumnya: Algoritma Greedy](./02-algoritma-greedy.md)
[< Kembali ke Indeks Part B](./README.md)
