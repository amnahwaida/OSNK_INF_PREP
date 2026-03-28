# 4. Dynamic Programming Dasar (Seni Mengingat Masa Lalu)

Kalau kamu mendengar kakak tingkat Olimpiade menyebutkan mantra sakti: *"Ah gampang, di-DP-in aja!"*, mereka sedang merujuk pada **Dynamic Programming** (Pemrograman Dinamis).

Terdengar sangat seram dan ilmiah, bukan? Padahal konsep intinya hanya satu: **JANGAN PERNAH MENGHITUNG DUA KALI HAL YANG SAMA.**

Ya, DP hanyalah seni mencatat/menyimpan ingatan masa lalu ke dalam "buku catatan" (sebuah *Array/Tabel*), supaya kalau di masa depan kita ditanya rahasia pertanyaan yang sama, kita tinggal contek langsung bukunya tanpa perlu *ngotret* hitung-hitungan lagi!

Mari kita bedah sihir ini.

---

## ⏳ A. Kenapa Komputer Bisa Bodoh? (Tragedi Rekursi Fibonacci)

Ingat kembali deret Fibonacci di Part A: `1, 1, 2, 3, 5, 8, 13, 21, ...`
Jika Pak Dengklek menyuruh programmer pemula menghitung $Fibo(6)$ (Mencari Suku ke-6), si pemula akan menggunakan rumusnya memecah mundur (Rekursi mundur):
$F(6) = F(5) + F(4)$

Lalu si komputer akan kelelahan memecah lagi ke anak tirinya di bawah:
- Untuk menghitung $F(5) \rightarrow$ Dia pecah lagi mikir $F(4) + F(3)$
- Untuk menghitung $F(4) \rightarrow$ Dia pecah lagi mikir $F(3) + F(2)$

**Penyakit Kanker Otak Pemula:** 
Lihat bagaimana Si $F(4)$ ditanya berkali-kali secara rakus bercabang mendalam layaknya dahan raksasa keluarga cemara pohon yang terlahir bodoh. Komputer menghabiskan miliaran hitungan hanya untuk *menjawab pertanyaan bodoh yang hasil akhirnya sebenarnya sama* berulang-ulang dari kanan dan sisi dahan kiri ke turunan anaknya. Hal ini membuat komputermu bakalan hang total alias *Time Limit Exceeded (TLE)* hanya untuk menghitung suku ke $F(40)$. 

---

## 📖 B. Penawar Racun: *Memoization* (Mencatat Tabel Jejak)

Di sinilah Pahlawan *Dynamic Programming* turun tangan membawa sehelai "Buku Tabungan / Array Kosong".
Dia mengomeli komputer: *"HEH! Kalau kamu udah capek-capek ngitung hasil $F(4) = 3$, TOLONG DITULIS PAKE SPIDOL DI BUKU! Biar nanti kalau si dahan kanan nanya 'Hei Bang Berapa F(4)?', kamu nggak usah nurunin akar pohon lagi ngitung sedari dasar! Langsung aja buka buku halamannya, copas nilainya INSTAN!"*

**(Satu Detik Eksekusi OSN-K):**
Metode "Tulis ke dalam array kalau udah pernah dihitung" ini disebut **Memoization** (Mengingat masa lalu secara sakti dan ajaib, *Top-Down*). Dengan satu pencerahan array ini, algoritma yang tadinya mengeksekusi miliaran cabang serabutan, ciut langsung melibas lurus memendek seperti peluru. Pohon raksasa pingsan digergaji tebang habis efisiensinya sampai tak tersisa jejak keringat komputer OSN mu! Perhitungan $F(100)$ bisa kelar kurang dari seperseribu millisecond.

Ini adalah bentuk penyelesaian **Dynamic Programming yang Paling Murni Fundamental**. 

---

## 🎒 C. DP Sebagai Dewa Pilihan (Tragedi Knapsack Ransel Emas)

Ingat kejadian **Algoritma Greedy** yang gagal fatal di Bab 02 saat memecah kombinasi koin siluman aneh di Planet Namec? Kenapa Greedy gagal? Karena dia mengambil langsung uang nominal besar tanpa mensimulasikan masa depan.

Dynamic Programming datang menyempurnakan kegagalan *Greedy* itu!
Jika *Greedy* itu Si Buta yang nekat maju melangkah merampok, maka **DP itu adalah Dewa Dr. Strange yang mensimulasikan (Mengintip) semua cabang alternatif kemungkinan takdir masa depan di alam semesta secara bersamaan, Sembari menyimpan catatan di Tabel Matriks Mana Yang Paling Berhasil.**

### Studi Kasus: Pencuri Ransel Terbatas (0/1 Knapsack Problem)
Pak Dengklek menerobos masuk ke rumah Firaun yang penuh Emas, ditangannya dia menggenggam Karung Ransel berkapasitas bobot Murni mentok menahan berat *Maksimal 10 Kg*. 
Ada 3 pilihan barang mewah yang terpampang:
1. **Patung** (7 Kg) $\rightarrow$ Harga Rp 10 Juta
2. **Pedang** (4 Kg) $\rightarrow$ Harga Rp 6 Juta
3. **Piring Emas** (6 Kg) $\rightarrow$ Harga Rp 8 Juta

- Pemain **Brute Force** akan stres kombinasi berjam-jam mencoba satu-satu (Bisa saja meledak kelamaan kalau barangnya ada ratusan).
- Pemain **Greedy Egois Biasa** akan silau mata dan langsung sabet si *Patung* (Karena paling mahal 10 Juta). Sayangnya, tasnya kini sisa muat 3 Kg. Gak ada barang sisa seberat 3Kg. Peluang kandas. Dia kabur hanya bawa 10 Juta!

**Sang Jawara Dynamic Programming Datang Beraksi:**
Dia mengeluarkan Tabel sakti baris-kolom dengan nama variabel kapasitas sisa (`Kg Tersisa`) dan list barang (`Barang Ke-i`).

- *"Oh santai, Dr. Strange ku akan mengkomputasi masa depan! Kalau aku ambil si Patung (7kg), berarti aku dapet sisa bagasi 3 kg.* (Dicatat pelan di otak tabel bahwa state *Tinggal 3Kg* ngasilin duit Rp10jt maksimal). 
- *EH TUNGGU! Kalau Patungnya kutinggalkan abaikan... Tas ku masih utuh 10kg!*
- *Yaudah gaskan coba ambil sisi pararel 'Pedang' + 'Piring' yang bobot gandanya aja (4+6=10kg) Pas masuk pas di kantong ludes.*
- *Wah nilainya total = Pedang (Rp6jt) + Piring (Rp8jt) = **14 JUTA!***

Setelah seluruh semesta paralel simulasi tercatat dalam tabelnya, DP dengan pasti tanpa ragu akan memilih secara murni komputasi mutlak untuk MENGABAIKAN PATUNG. 
Rekor **Rp 14 Juta** adalah global optimal sejati. Di sanalah kemalasan *Memoization DP* menaklukkan dunia! 

---

## D. Apa yang Diinginkan Soal OSN-K darimu di Soal DP?

Di atas kertas OSN-K, soal DP tidak meminta kamu ngoding Array DP C++ Multi Dimensi nan ribet.
Soal OSN-K hanya memintamu **Paham Konsep Sub-Masalah Ketergantungan**:
- *Kalau aku tau cara terbaik bayar uang Rp 3.000, aku bisa mencari cara terbaik memecah jumlah recehan Rp 4.000 dengan ngobok ngintip sisa nominal masa laluku itu (Tinggal tambah sekeping 1.000!).*

Biasanya wujud modifikasinya adalah:
> "Bebras ingin menuju Puncak Tangga ke 10. Tiap langkah, dia cuma boleh loncat 1 anak tangga ATAU loncat membelah langsung ke anak tangga ke 2. Ada berapa banyak jalur rute kaki beda mutlak kemungkinan si Bebras mencapai puncak atas tangga itu?"

*Penyelesaian Compiler Manusia-mu:*
Jangan coba digambar garis rute bercabang-cabang manual di kertasmu! (Bisa abis gila waktu!). Berlakulah seperti anak DP:
- Kalau dia lagi jongkok di lantai 3.
  Kemungkinannya pasti cuma ada dua cara ia bisa sampai ke sini dong secara harfiah? 
  *Ya dari anak tangga 2 (loncat 1 langkah)* ATAU *Tiba-tiba ngeloncat terbang dari lantai 1 (loncat ganda 2 langkah)*!
- Berarti murni hitungannya: `Total Jalan menuju L3 = Total Jalan menuju L2 + Total Jalan menuju L1`.
- Tunggu! Ingat pola deret babak Part A kemarin?! Wah ternyata **Sama persis gila menyentuh nyawa Hukum Fibonacci!** Tabulasikan dengan enteng senyum dan melibas menjawabnya dalam detik OSN-K!

---

Kita sudah memahami mesin inti algoritma. Sekarang di bab terakhir Part B ini, mari kita asah pedang terakhir yang berfokus ke manipulasi Text dan Alfabet Huruf dengan kecepatan otak dewa. 

Mari meluncur ke **[Modul 05: Pemrosesan String & Array Murni OSN-K!](./05-pemrosesan-string-dan-array.md)**

---
[< Modul Part B Sebelumnya: Pencarian & Pengurutan Manual Algoritma](./03-pencarian-dan-pengurutan.md)
[< Kembali ke Indeks Part B](./README.md)
