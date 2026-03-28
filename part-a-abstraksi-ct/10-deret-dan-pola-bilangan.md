# 10. Model Matematis, Deret & Pola Bilangan (Trik Sakti Matematika)

> "Programmer level dewa itu pemalas. Mereka ogah ngitung manual 1+2+3+...+100. Mereka lebih suka putar otak 5 menit buat nyari rumus/pola rahasianya, biar komputer bisa ngerjain sisanya dalam 0.001 detik. Inilah kekuatan asli dari Abstraksi Matematika!"

Sering banget di soal OSN-K, kamu disuruh menghitung sesuatu yang angkanya jutaan atau miliaran. Kalau kamu hitung manual satu-satu (atau dibayangin pakai *looping* biasa), waktunya pasti habis atau komputernya *nge-lag* (Time Limit Exceeded). 

Solusinya? Temukan **Pola Rahasianya (Model Matematis)**! 

---

## 🔢 1. Ilmu Titen: Insting Membaca Pola Bilangan

Kadang-kadang, deret angka di OSN-K itu sengaja dibikin aneh dan nggak masuk ke rumus standar mana pun di buku sekolah. Kamu diuji murni pakai **naluri detektif (Ilmu Titen / Pattern Recognition)**.

**Kasus 1: Barisan Sang Legenda (Fibonacci)**
> `1, 1, 2, 3, 5, 8, 13, ... ` (Tebak angka selanjutnya apa?)

Jangan cari selisihnya, karena pasti berantakan. Coba perhatikan baik-baik:
Setiap angka yang muncul adalah hasil **PENGGABUNGAN (Jumlahan) DUA ANGKA SEBELUMNYA!**
- 1 + 1 = 2
- 1 + 2 = 3
- 2 + 3 = 5
- Berarti selanjutnya pasti: $8 + 13 = 21$. Gampang kan?

**Kasus 2: Kuadrat yang Menyamar**
> `2, 5, 10, 17, 26, ...` (Berapa Suku ke-10?)

Kalau kamu pusing nyari bedanya, coba ingat-ingat deret bilangan kuadrat (pangkat dua) yang normal: `1, 4, 9, 16, 25...`
Eh, angkanya mirip banget! Ternyata deret di soal itu **cuma deret kuadrat biasa yang ditambah angka 1 tiap sukunya**.
- Suku ke-1 $\rightarrow 1^2 + 1 = 2$
- Suku ke-2 $\rightarrow 2^2 + 1 = 5$
- Suku ke-3 $\rightarrow 3^2 + 1 = 10$
- Maka, Suku ke-10 pasti $\rightarrow 10^2 + 1 = 101$. BOOM! Selesai tanpa ngurutin panjang-panjang.

---

## 📈 2. Deret Aritmetika Biasa (Naik Tangga Konstan)

Deret Aritmetika itu semacam **Anak Tangga yang adil**. Tiap kamu melangkah naik, jarak naiknya selalu sama persis (selalu nambah 3, atau selalu kurang 5, polanya konstan).

**Pondasi Dasar:**
Contoh anak tangga: `2, 5, 8, 11, 14, ...`
- **Suku Pertama / Start ($a$)** = Angka 2 (Kamu lagi nongkrong di tinggi 2 meter).
- **Langkah / Beda ($b$)** = +3 (Sekali melangkah, tinggi kamu nyepruut naik 3 meter terus).

### A. Nebak Langkah ke-$n$ ($U_n$)
Kalau kamu melangkah sampai 10 kali (Suku ke-10 / $U_{10}$), tinggi kamu sekarang berapa?
Daripada ngitung manual melangkah di otak, bayangin aja: *Dari tempat awal (a), kamu sudah naik sebanyak 9 langkah (karena yang pertama kamu udah numpang diam di atasnya).*

> **Rumus Ketinggian:** $U_n = a + (n - 1)b$
> *Jawab:* $U_{10} = 2 + (9 \times 3) = 2 + 27 = 29$. Tinggimu 29 meter.

### B. Trik Pemalas Jenius ala C.F. Gauss ($S_n$)
Bagaimana kalau ditanya: **Tolong JUMLAHKAN semua angka anak tangga tadi dari langkah 1 sampai 100?**

Ratusan tahun lalu, ada anak SD jenius bernama Carl Friedrich Gauss. Gurunya yang galak nyuruh murid-muridnya ngitung:
$1 + 2 + 3 + ... + 99 + 100 = ?$ 
Niat gurunya biar anak-anak repot berjam-jam, eh si Gauss cuma butuh 10 detik! Ini rahasianya:

Gauss masangin angka dari ujung depan sama ujung belakang:
- $1 + 100 = 101$
- $2 + 99 = 101$
- $3 + 98 = 101$

Wah, semuanya kalau dipasangkan ujung-ke-ujung hasilnya SELALU 101! 
Kalau total ada 100 angka, berarti ada **50 Pasang** (karena dibagi 2).
Yaudah, tinggal kalikan aja: **$50 \times 101 = 5050$**. Super cepat!

> **Rumus Jumlah ala Gauss ($S_n$):**
> $S_n = \frac{\text{Banyak Angkanya}}{2} \times (\text{Angka Awal} + \text{Angka Akhir})$
> *Atau bahasa resminya:* $S_n = \frac{n}{2} (a + U_n)$

---

## Σ 3. Menguliti Notasi Sigma (Simbool Seram, Aslinya Cuma For-Loop!)

Kadang OSN-K Matematika/Informatika sengaja ngasih simbol Yunani $\Sigma$ (Sigma) aneh kayak gini buat menjatuhkan mental peserta:

$$\sum_{i=1}^{5} (2i)$$

Jangan kabur dulu! Programmer C++ atau Python kalau ngelihat ini malah ketawa kegirangan. Kenapa? Karena huruf M kebalik / $\Sigma$ itu hanyalah lambang primitif dari fungsi **FOR-LOOP!**

Biar nggak takut, ini terjemahan "Bahasa Dewa" itu ke dalam **"Bahasa Kodingan Manusia"**:

```cpp
int total_sigma = 0;              // Siapin celengan kosong
for (int i = 1; i <= 5; i++) {    // Mulai dari i=1, berjalan terus mentok sampai i=5
    total_sigma += (2 * i);       // Setiap jalan, masukin nilai (2 dikali i) ke celengan!
}
```

**Cara Ngerjain Manual Kalau Komputermu Mati:**
Nih, kamu kerjain layaknya masukin koin ke celengan satu-satu sesuai perintah kodingan:
- Waktu `i=1` $\rightarrow$ Kamu masukin $2 \times 1 = 2$ ke celengan.
- Waktu `i=2` $\rightarrow$ Kamu masukin $2 \times 2 = 4$ ke celengan.
- Waktu `i=3` $\rightarrow$ Kamu masukin $2 \times 3 = 6$ ke celengan.
- Waktu `i=4` $\rightarrow$ Kamu masukin $2 \times 4 = 8$ ke celengan.
- Waktu `i=5` $\rightarrow$ Kamu masukin $2 \times 5 = 10$ ke celengan (Trus Loop berhenti karena udah mentok di 5!).

Berapa isi celenganmu sekarang?
Total = $2 + 4 + 6 + 8 + 10 =$ **30**.
Selesai! Sigma ternyata sepele banget kan?

---

## 🧩 4. Jurus Detektif: Mengupas Soal "Ayam dan Kambing"

Soal "Pemodelan" di OSN-K itu intinya cuma cerita panjang (biasanya hewan-hewan Pak Dengklek) yang harus kamu terjemahkan ke bentuk rumus (Sistem Persamaan Aljabar).

**Soal Klasik Sepanjang Masa:**
Di peternakannya, Pak Dengklek melihara buanyaak Ayam dan Kambing di dalam satu kandang gelap. 
Saking gelapnya, dia cuma bisa ngeraba **Kepala** sama ngitung kaki.
- Total jumlah **Kepala** yang kepegang ada: **40 buah**.
- Total jumlah **Kaki** yang seliweran terinjak ada: **110 kaki**.
*Pertanyaan Detektif:* Ada berapa ekor AYAM di dalam kandang itu?

**Cara Ngerjain ala Hacker Matematika (Pakai Variabel/Simbol):**
Daripada nebak-nebak buah manggis, mari kita ubah kata-katanya jadi rumus:

1. Modalnya kita tahu: Ayam (A) kakinya cuma 2. Kambing (K) kakinya 4. Kepalanya mah pasti sama-sama 1 tiap ekor.
2. Bikin Rumus Kepala: $A + K = 40$ (Berarti secara logika, jumlah *Ayam sesungguhnya adalah 40 dikurangi Kambing*, atau $A = 40 - K$).
3. Bikin Rumus Kaki: $2A + 4K = 110$.
4. **Jurus Substitusi (Ganti Perabotan):**
   Ambil tulisan "A" di rumus kaki, terus tendang dan ganti pakai info kepala tadi ($40-K$).
   $2(40 - K) + 4K = 110$
   Kalian kerjain pelungkerannya:
   $80 - 2K + 4K = 110$
   $80 + 2K = 110$
   Pindah si 80 ke kanan (Jadi minus):
   $2K = 110 - 80$
   $2K = 30$
   Dapatlah **$K = 15$ ekor Kambing!**
5. Lanjut Cari Ayamnya: Tadi kata kepalanya total 40 ekor. Kalau kambingnya 15, ya Ayamnya tinggal $40 - 15 =$ **25 ekor**.

Kasus terpecahkan! Model matematika ini bikin kamu jadi dukun sakti yang bisa nebak isi dunia nyata meskipun nggak keliatan langsung.

---

## 📝 Daftar Isi Latihan (300 Soal)

Agar makin tajam insting detektif dan aljabarmu, silakan kerjakan 300 latihan soal berikut (dibagi ke 6 bagian):

1. **[Bagian 1 (Soal 1-50)](./10-deret-dan-pola-bilangan/10-deret-soal-part-1.md)** — Ilmu Titen (Mengenal Pola Fibonacci & Kuadrat).
2. **[Bagian 2 (Soal 51-100)](./10-deret-dan-pola-bilangan/10-deret-soal-part-2.md)** — Deret Aritmetika (Mencari Ketinggian Tangga / $U_n$).
3. **[Bagian 3 (Soal 101-150)](./10-deret-dan-pola-bilangan/10-deret-soal-part-3.md)** — Menjumlahkan Deret ($S_n$) dengan Trik Pasangan Gauss.
4. **[Bagian 4 (Soal 151-200)](./10-deret-dan-pola-bilangan/10-deret-soal-part-4.md)** — Mengenal Notasi Sigma & Ekuivalensinya dengan *For-loop* Koding.
5. **[Bagian 5 (Soal 201-250)](./10-deret-dan-pola-bilangan/10-deret-soal-part-5.md)** — Pemodelan Aljabar Lanjut (Detektif Ayam & Kambing/SPLDV).
6. **[Bagian 6 (Soal 251-300)](./10-deret-dan-pola-bilangan/10-deret-soal-part-6.md)** — Pola Bilangan Tingkat 2 & Substitusi Harga Barang OSN-K.

---
[< Materi Sebelumnya: Kombinatorika](./09-kombinatorika.md)
[< Kembali ke Beranda Materi](../README.md)
