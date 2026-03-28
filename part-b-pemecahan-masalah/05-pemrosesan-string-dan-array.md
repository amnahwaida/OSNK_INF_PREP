# 5. Pemrosesan String & Array (Bedah Silabus Asli OSN-K 2025)

Di bagian terakhir ini, kita akan langsung membedah contoh soal *Pemecahan Masalah Komputasional* yang secara **spesifik di-spill oleh pembuat soal pusat di silabus OSN-K 2025**.

Tadi kita sudah bahas angka dan graf, lalu bagaimana dengan operasi *teks* (String)? 

Sebelum masuk ke algoritma silabus asli berspesifikasi dewa bernama *"Menghitung Subsekuens"*... mari kita pahami dulu perbedaan mendikte nyawa String di OSN Informatika.

---

## ✂️ A. Beda Kasta Teks: *Substring* vs *Subsequence*

Banyak peserta gagal OSN karena menyamakan dua arti mahluk string ini.

Misalkan kita punya String Murni Induk:
`T X S A X J E U R K N K`

1. **Substring (Potongan Utuh Lurus dan Harus Dempet Tersetiai)**
   - Aturan: Harus berjejer rapat di kata aslinya, tak boleh ada sela jeda putus.
   - Contoh Valid: `T X S` atau `A X J`
   - Contoh Haram (Tidak Diakui): `T A U` (Karena dari T loncat ke A itu ngelewatin rintangan huruf X dan S yang kepotong dibuang).

2. **Subsekuens / Subsequence (Potongan Melompat Genit Tetap Urut)**
   - Aturan: Hurufnya BOLEH LONCAT JAUH asalkan posisinya **tetap wajib dari Kiri ke Kanan** di huruf aslinya (Jangan putar balik urutan!).
   - Contoh Subsekuens Valid dari kalimat di atas:
     - `T U K` (Didapat dari ambil `T`-x-s-a-x-j-e-`U`-r-`K`-n-k)
     - `S A J U N K`
     - `X X R K`
   - Contoh Subsekuens Haram (Menyalahi Takdir Waktu Belakang):
     - `K U J` (Karena huruf K letaknya udah mentok di belakangan, eh dia mundur maksa ngambil huruf U. Itu DILARANG oleh algoritma mesin).

Memahami hukum **Subsekuens** adalah nyawa penting OSN-K! Mari buktikan dengan bedah soal OSN-K asli di silabus.

---

## 🧩 B. Membedah Silabus Asli OSN-K: Soal Subsekuens "OSN"

Tengok kembali Silabus resmi OSN-K Informatika 2025 Anda. Pembuat soal menampilkan *Mockup* studi kasus seperti ini:
> **Soal Pemanasan:** "Diberikan sebuah string hanya berisi huruf O, S, dan N. Hitung berapa banyak kombinasi memetik/mencabut huruf O, S, dan N sedemikian rupa sehingga tetap merangkai kata `OSN` dalam kaidah Subsekuens Lurus Kiri ke Kanan."
> *Contoh dari panitia*: `SONOSONO`. Di kalimat ini ada **2** kemunculan Subsekuens OSN.
> Yakni: `(O ke-2, S ke-5, N ke-7)` dan `(O ke-4, S ke-5, N ke-7)`. 

### Siksaan Manual Brute Force (Gagal)
"Ah gampang min, cacah manual aja pakai bolpen!".
Misalkan teks yang diperiksa panjang banget: `NONONONONON`. 
Kapan kamu kelar mencocokkan kemungkinannya? Ini murni jebakan.

### Jurus Pemrosesan Teks & Array Pintar Berjalur (Simulasi Array Variabel)

Kamu tidak butuh coding C++ betulan! Tarik napas, dan amati logika Sang OSN-K Developer. 
Agar kita bisa menciptakan Subsekuensi utuh `O-S-N`:
- Kita butuh mencatat ada berapa **huruf 'O'** yang pernah lewat (sejarah stok 'O').
- Kalau kita kejatuhan nemu huruf **'S'**, si huruf S ini bisa langsung mengawinkan dirinya berlipat ganda dengan SEMUA STOK huruf 'O' di baris memori kirinya. Perkawinan ini kita jadikan sebagai panen pabrik mencetak paket pasangan kata `OS`!
- Terakhir, kalau tiba-tiba di depan kita ketabrak huruf **'N'**, semua stok paketan kata `OS` yang pernah jadi di sejarah array bakal dikawinkan meledak secara kumulatif melahirkan produk utuh kata `OSN`!!

Mari bongkar array memori hitungannya simulasi ke soal silabus: `SONOSONO`

**TABEL DETEKTIF STRING MANUAL OSN-K KITA:**

Variabel Kantongan (Simpan di Ingatan):
- `Stok_O` (Jumlah O sejauh ini) = 0
- `Stok_OS` (Jumlah rakitan pasangan OS sejauh ini) = 0
- `Total_OSN` (Juara Akhir panenan murni = Puncak Jawaban) = 0

*Mari simulasi bergerak 1 Huruf, dari paling Kiri Ke Kanan...*

1. Huruf `S` $\rightarrow$ Dia butuh O dari kiri. Stok O masa lalu = 0. Tidak ada yang bisa dinikahi. Total `Stok_OS` nambah 0.
2. Huruf `O` $\rightarrow$ Mantap bang! Kantongi jadi aset sejarah. `Stok_O` = 1.
3. Huruf `N` $\rightarrow$ Datanglah huruf penyelesai misi. Apakah kita udah punya rak rakitan `OS` di masa lalu? Nggak punya (masih 0). `Total_OSN` = 0.
4. Huruf `O` $\rightarrow$ Ooo dapet panen lagi. Tambah ke aset! `Stok_O` lama(1) + 1 = 2 buah. (Kita sekarang menginjak 2 buah O berjejer).
5. Huruf `S` $\rightarrow$ Datanglah huruf genit S! Dia akan menarik KESELURUHAN stok tabungan aset O masa lalu. (Ada 2 O kan?). Boom! Berarti di detik titik ini, kita sukses memproduksi 2 jenis kombiasi silangan variasi `OS`. Simpan ke kantong OS: (`Stok_OS` = 2 paket).
6. Huruf `O` $\rightarrow$ Nambah sejarah stok O lagi. `Stok_O` = 2 + 1 = 3 buah aset O.
7. Huruf `N` $\rightarrow$ BOM ATOM! Final. Huruf ketok palu datang! Dia melihat langsung ke rak tabungan `Stok_OS` masa lalu (Ternyata sudah panen terbuat 2 jenis cetakan paket). Si `N` langsung mengklaim dan melebur dua cetakan gantung itu menjadi hasil komplit.
   `Total_OSN` dipanen = bertambah 2 poin hadiah. (Skor Total: 2 Murni).
8. Huruf `O` $\rightarrow$ Aset nambah jadi 4. 

Habis! Looping berhenti! Laporan Total = Score 2 !!

Gila bukan? Kamu tak perlu membuat garis-garis silang semrawut pakai pensil! Kamu murni pakai konsep hitungan **Tabel Tabungan Linear $O(N)$**. Kamu baru saja membuktikan betapa seramnya Pemrosesan Array + Pemotongan Teks Subsekuens dalam mengunyah kalimat `S-O-N-O-[S-O-N]-O` ini di depan mata kertas!

*(Soal OSN-P nanti memintamu menghitung String OSN pada kata ribuan huruf, kamu akan tersenyum menang setelah tahu tabel sakti silangan ini).*

---

Selesai sudah pembekalan *Algoritma Manual* kita di alam komputasi kertas Part B!
Di titik ini, insting *Compiler Manusia* milikmu sudah terbangun. Kamu paham `Array Looping`, cara serakah `Greedy`, dan *Simulasi Waktu*. 

Tapi apalah artinya memahami "maksud perulangan kata" tanpa tahu bagaimana wujud mantranya dalam bahasa C++ dewa di terminal?
Oleh karena itu, tarik napas lagi dan mari kita dobrak Pintu Babak Terakhir OSN-K:
⏩ **Bagian C: Pemahaman Potongan Algoritma Bahasa C++.**

---
[< Modul Part B Sebelumnya: Dynamic Programming (DP)](./04-dynamic-programming-dasar.md)
[< Kembali ke Indeks Part B](./README.md)
