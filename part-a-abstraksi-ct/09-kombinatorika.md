# 09. Kombinatorika (Seni Berhitung Super Cepat)

> "Pernah iseng ngitung berapa banyak kombinasi password yang bisa kamu bikin dari namamu? Atau pusing mikirin ada berapa cara milih ketua dan wakil kelas dari 30 orang? Nah, Kombinatorika adalah **Seni Berhitung Tanpa Mendaftar Satu-Satu** yang bakal menyelamatkan hidupmu!"

Kalau teori Graf itu "tamu VIP" di OSN-K, maka Kombinatorika ini adalah **Rajanya!** Topik ini dijamin 100% selalu keluar tiap tahun. Menguasai ini bikin kamu jago memprediksi *"ada berapa banyak kemungkinan"* di dunia komputer.

Yuk, kita bedah pakai logika warung kopi biar gampang!

---

## 🎲 1. Aturan Dasar (Kapan Harus nambah, Kapan Harus ngali?)

Ini adalah kesalahan paling fatal anak OSN pemula. Kapan sih angka peluangnya ditambah, dan kapan dikali?

### A. Aturan Penjumlahan (Aturan "ATAU")
Kamu pakai ini saat kamu **HANYA BISA MEMILIH SATU HAL** dari dua pilihan yang **nggak bisa digabung**. (Anggap saja ini kayak percabangan `IF ... ELSE`).

**Contoh (Kasus Dompet Tipis):**
Kamu lagi di kantin. Uangmu sisa 10 ribu. Di kantin ada **3 jenis nasi** dan **4 jenis mie**. Karena uangmu mepet, kamu **HARUS PILIH: Makan Nasi ATAU Makan Mie**. Nggak bisa dua-duanya!
Berapa banyak pilihan makanan yang bisa kamu tunjuk ke ibu kantin?
> **Jawab:** Ada $3 + 4 = 7$ pilihan berbeda.
> **Logika:** Kejadian A (makan nasi) dan Kejadian B (mandi mie) terpisah dan saling jegal.

### B. Aturan Perkalian (Aturan "DAN")
Kamu pakai ini saat kegiatan harus dilakukan secara **berturut-turut** atau **harus komplit jadi satu paket bundle**. (Anggap saja ini kayak dua `For-Loop` yang bersarang / *nested loop*).

**Contoh (Kasus Anak Sultan):**
Hari ini kamu ditraktir kepsek makan *Paket Komplit*. Kamu HARUS MEMILIH **1 Makanan (dari 3 nasi)** DAN **1 Minuman (dari 4 es)**.
Berapa kemungkinan paket makan siang yang ada di mejamu?
> **Jawab:** $3 \times 4 = 12$ paket kombinasi unik.
> **Logika:** Nasi Goreng bisa dipasangin sama (Es Teh, Jeruk, Sirup, Air putih). Nasi Uduk juga gitu. Jadi tinggal kalikan saja!

---

## 🔄 2. Permutasi (Yang Penting Pangkat & Jabatan!)

**Permutasi** itu ibarat main "Kursi Jabatan". Cara menyusun benda/orang, di mana **URUTAN ITU SANGAT BERPENGARUH KE HASIL.**

> **Kata Kunci Permutasi:**
> Pemilihan Ketua/Wakil, Susun Password, Kartu ATM, Nomor Antrian, Plat Nomor Motor.
> **Mikirnya Gini:** Kalau Budi jadi Ketua & Anton jadi Wakil... itu **BEDA BANGET** dengan situasi Anton jadi Ketua & Budi jadi Wakil (Budi pasti protes kalau diturunin jabatannya!).

### A. Permutasi Biasa (Strategi "Slot Kosong")
Daripada hapal rumus, anak OSN pro biasanya pakai teknik **Slot Kosong (Filling Slots)**.

**Kasus:** Ada 5 orang kandidat mantap mau dipilih jadi Ketua, Wakil, dan Bendahara (Ada 3 kursi panas). Berapa cara nyusun kabinetnya?
**Cara Ngerjain (Bayangin 3 Kursi Kosong):**
- **Kursi 1 (Ketua):** "Siapa yang mau duduk?" Ada 5 orang berebut, jadi ada **5 pilihan**. (Misal Budi kepilih dan langsung duduk).
- **Kursi 2 (Wakil):** "Budi udah duduk, nah sisa berapa orang yang berdiri?" Tersisa **4 orang**.
- **Kursi 3 (Bendahara):** Sisa berapa orang? Tinggal **3 orang**.
> **Total Cara:** Tinggal kalikan semua peluang slotnya! $5 \times 4 \times 3 = 60$ cara/kabinet yang berbeda.

*(Buat yang maksa mau pamer rumus resmi: $P(5, 3) = \frac{5!}{(5-3)!} = \frac{5!}{2!} = 5 \times 4 \times 3 = 60$. Sama aja kan?!)*

### B. Permutasi Huruf Kembar (Anagram KTP)
**Kasus:** Berapa susunan kata aneh yang bisa dibikin dari ngacak huruf di kata **"KATAK"**?

**Logika Orang Awam:**
Ada 5 huruf nih! Kalau diacak pakai logika slot kosong: $5 \times 4 \times 3 \times 2 \times 1 = 120$ kata. Selesai!

**TAPI TUNGGU DULU!** 🛑
Huruf K di depan sama huruf K di belakang itu **BENTUKNYA PERSIS SAMA**. Kalau kamu nukar posisi K depan dan K belakang, mata manusia nggak akan ngenalin bedanya (Kata "KATAK" dibalik bakal tetep kebaca "KATAK").
Artinya, ada susunan yang dobel / kembar. Kita harus membuang si kembaran ini dengan cara **Membagi totalnya dengan Faktorial huruf yang kembar.**

**Cara Jawab Cerdas:**
- Total abjad ($n$) = 5 huruf (Total semesta: $5!$)
- Abjad kembar: K ada 2 buah (Bagi $2!$). A ada 2 buah (Bagi $2!$). T cuma 1 (Bagi $1!$, nggak usah ditulis nggak apa-apa).
- **Total Kata Unik:** $\frac{5!}{2! \times 2!} = \frac{120}{(2 \times 1) \times (2 \times 1)} = \frac{120}{4} = 30$ kata aja.

### C. Permutasi Siklis (Melingkar di Meja Makan)
**Kasus:** 5 Bos Mafia lagi rapat duduk melingkar di satu meja bundar. Ada berapa formasi tempat duduk?

Masalah di meja bundar adalah: **Nggak ada Ujung dan Pangkalnya!**
Kalau semua orang geser kursinya satu langkah ke kanan searah jarum jam, formasinya (siapa di sebelah kiri dan kananmu) **nggak berubah sama sekali!** 

Biar nggak muter-muter bikin pusing, strateginya adalah **PAKU SALAH SATU ORANG (Biarin dia diem jadi patokan), sisa temannya biarin muter**.
Karena 1 orang udah dipaku, berarti orang yang pindah-pindah sisa $(n - 1)$.

> **Rumus Meja Bundar:** $(n - 1)!$
> **Jawab:** 5 bos dikurang 1 bos yang di-paku = $4! = 4 \times 3 \times 2 \times 1 = 24$ formasi duduk.

---

## 🤝 3. Kombinasi (Cuek, "Yang Penting Kepilih!")

**Kombinasi** itu ibarat masukin belanjaan ke dalam tas kresek. Kamu **MENGAMBIL/MEMILIH** kelompok, di mana **URUTAN PENGAMBILAN SAMA SEKALI NGGAK PENTING**. 

> **Kata Kunci Kombinasi:**
> Pilih Tim Cerdas Cermat, Ngambil Kelereng di Dalam Toples, Berjabat Tangan, Bikin Segitiga dari titik, Campur Warna Cat.
> **Mikirnya Gini:** Kalau Kepsek manggil "Budi dan Anton ke ruang guru (Masuk Tim)", itu sama efeknya kalau Kepsek manggil "Anton dan Budi ke ruang guru (Masuk Tim)". Nasibnya tetep sama: Mereka berdua kepilih!

Karena di Kombinasi kita nggak peduli urutan (banyak susunan yang dianggap "sama aja"), logikanya: **Hasil kombinasi PASTI SELALU LEBIH KECIL / SEDIKIT jumlahnya dibanding Permutasi.**

**Kasus:**
Dari 5 murid unggulan, Bapak Guru ingin narik 3 anak secara acak untuk disuruh lomba. Berapa banyak komposisi tim yang mungkin terbentuk?

**Rumus Kombinasi (C):**
$$C(n, r) = \frac{n!}{r! \times (n - r)!}$$
*(Lihat pembaginya! Di Kombinasi, pembaginya ada tambahan $r!$ di bawah biar angka kembarannya kebuang)*

**Cara Jawab:**
- Total murid ($n$) = 5. Yang diambil ($r$) = 3.
- $C(5, 3) = \frac{5!}{3! \times (5 - 3)!}$
- $C(5, 3) = \frac{5!}{3! \times 2!}$
- Biar gampang nulisnya: $\frac{5 \times 4 \times 3!}{3! \times 2 \times 1}$ *(Coret angka 3! di atas dan di bawah)*
- $\frac{5 \times 4}{2} = \frac{20}{2} = 10$ tim yang berbeda.

---

## 🕊️ 4. Pigeonhole Principle (Prinsip Hukum Alam Paling Sial)

Ini adalah prinsip logika matematika yang namanya lucu (Prinsip Sarang Burung Merpati / PHP), tapi dipakai untuk ngejawab soal OSN-K bertipe *"Skenario Terburuk (Worst-case)"*.

**Pahami Logika Sederhananya:**
"Bayangin kamu punya 10 ekor burung merpati, tapi kamu miskin dan cuma punya 9 kotak sarang kandang. Pas malam hari tiba, semua burung pulang kampung masuk ke kandang. HUKUM ALAM MENGATAKAN: Walaupun mereka coba bagi-bagi tempat serajin apapun, silakan cek aja: **PASTI ADA minimal 1 kotak sarang yang empet-empetan diisi oleh 2 merpati (atau lebih).** Nggak mungkin semuanya sanggup tidur sendirian."

> *Jika N ekor burung dipaksa masuk ke M kandang (padahal N lebih gede dari M), pasti ada kandang yang isinya double.*

**Gimana model soalnya di OSN-K?**
Biasanya soal yang tanya: *"Berapa banyak barang yang MENGGILA harus DIAMBIL ACAK dalam GELAP agar KITA PASTI 100% AMAN MENDAPATKAN..."*

**Contoh Soal (Pengambilan Kaus Kaki Random):**
Di keranjang baju kotormu ada:
- **10 kaos kaki Hitam**
- **8 kaos kaki Putih**
- **6 kaos kaki Merah**
Masalahnya lagi mati lampu (gelap gulita). Kamu harus ngambil kaos kaki secara acak satu per satu pakai tangan kosong.
**Pertanyaannya:** "Berapa buah kaos kaki *MINIMAL* yang harus kamu cabut dari keranjang, agar kamu **DIJAMIN (100% PASTI AMAN)** dapat SEPASANG (2 buah) kaos kaki berwarna HITAM?"

**Cara Jawab Pakai Logika PHP (Skenario Paling Apes):**
1. Kalau soal minta "Pasti", kamu memposisikan dirimu sebagai **orang paling sial / apes sedunia**.
2. Kamu ngarepnya ngambil warna Hitam. Kesempatan ke-1 sampai ke-8, kamu malah ngambil yang warna Putih secara beruntun. (8 Putih keambil semua, masih belum dapet sepasang Hitam). Sial banget kan?
3. Kamu ambil lagi di kesempatan ke-9 sampai ke-14 panjang, eh malah dapetnya si Merah berturut-turut. (6 Merah habis semua, masih belum dapet Hitam juga!).
4. Total kamu udah buang energi ngambil $8 + 6 = 14$ kaos kaki yang jelas-jelas gagal. Di kasurmu sekarang udah berserakan 8 Putih dan 6 Merah.
5. Dan lihat kondisi keranjangnya: sekarang HANYA ADA WARNA HITAM MURNI! (Karena putih dan merahnya udah habis keambil sama *"kesialan"* kamu tadi).
6. Maka di **ambilan ke-15**, kamu merem pun PASTI dapat Hitam! (Hitam pertama).
7. Di **ambilan ke-16**, kamu juga pasti dapat Hitam! (Hitam kedua = SEPASANG!)

**Jawaban:** $8 + 6 + 2 = 16$ kaos kaki yang harus diambil secara acak. Logika Invers yang asyik, bukan?

---

## 📝 Daftar Isi Latihan (300 Soal Pilihan Ganda)

Untuk memperkuat logikamu dalam menghitung probabilitas dan susunan, silakan kerjakan 300 latihan soal Kombinatorika (dalam format Pilihan Ganda) yang dibagi menjadi 6 bagian ini:

1. **[Bagian 1 (Soal 1-50)](./09-kombinatorika/09-kombinatorika-soal-part-1.md)** — Aturan Penjumlahan & Perkalian (Kasus "Atau" vs "Dan").
2. **[Bagian 2 (Soal 51-100)](./09-kombinatorika/09-kombinatorika-soal-part-2.md)** — Permutasi Dasar & Susunan Kursi Jabatan.
3. **[Bagian 3 (Soal 101-150)](./09-kombinatorika/09-kombinatorika-soal-part-3.md)** — Permutasi Unsur Kembar (Anagram Kata) & Siklis (Meja Bundar).
4. **[Bagian 4 (Soal 151-200)](./09-kombinatorika/09-kombinatorika-soal-part-4.md)** — Kombinasi Dasar (Memilih Tim & Jabat Tangan).
5. **[Bagian 5 (Soal 201-250)](./09-kombinatorika/09-kombinatorika-soal-part-5.md)** — Kombinasi Lanjut Bersyarat (Multigrup Pria/Wanita & Pilihan Wajib).
6. **[Bagian 6 (Soal 251-300)](./09-kombinatorika/09-kombinatorika-soal-part-6.md)** — Prinsip Sarang Merpati / *Pigeonhole Principle* (Skenario Terburuk).

---
[< Materi Sebelumnya: Teori Himpunan](./08-teori-himpunan.md) | [Materi Berikutnya: Deret & Pola Bilangan >](./10-deret-dan-pola-bilangan.md)
[< Kembali ke Beranda Materi](../README.md)
