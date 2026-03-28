# 6. Kompleksitas Waktu (Membaca Bahasa O-Besar / Big O)

> *"Wah jagoan nih kodingannya jalan! Tapi kok pas di-submit ke *grader* (robot juri) OSN, tulisannya **TLE (Time Limit Exceeded)** ya?"*

Kalau di sekolah biasa, program yang penting *"bisa ngeluarin jawaban benar"*. 
Tapi di OSN-K, jawaban benar saja belum cukup. Programmu **dijegal dengan Timer Bom Waktu (Maksimal 1 Detik)**. Jika dalam 1 detik komputermu belum selesai menghitung, lembar jawabanmu akan dicoret hangus.

Di sinilah **Kompleksitas Waktu (Time Complexity)** dan Notasi **Big O ($O$)** menjadi penggaris saktimu. Notasi ini bukan satuan waktu detik/menit, melainkan **ukuran seberapa parah programmu akan melambat kalau beban datanya ($N$) ditambah.**

Mari kita bedah 5 tingkat "Kengerian" algoritma yang wajib kamu kenali di OSN tanpa harus kehilangan esensi keilmuan aslinya.

---

## 🏎️ 1. $O(1)$ — Sang Instan Mutlak (Constant Time)

Bayangkan kamu punya laci berisi 1.000 kaos kaki. Tapi sahabatmu bilang: *"Bro, kaos kaki merah gue taruh **persis di urutan ke-5**"*.
Berapa lama waktu yang kamu butuhkan untuk menjangkaunya? Ya gampang, langsung buka laci dan sabet kaos kaki ke-5! 

Mau isi lacinya ada 1.000 kaos kaki, sejuta kaos kaki, atau sehancur apapun dunia ini... karena kamu SUDAH TAHU pasti indeks lokasinya, kamu hanya butuh **1 KALI GERAKAN**.

- **Wujud di Kodingan:** Pengambilan nilai dari array (`data[4]`), rumus matematika langsung (misal Rumus Trik Gauss $S_n$), operasi tambah/kurang/kali biasa.
- **Karakter:** Kebal terhadap ukuran data. Mau datanya besar atau kecil, kecepatannya selalu instan.

---

## 🦅 2. $O(\log N)$ — Sang Penebas Setengah (Logarithmic Time)

Ingat **Binary Search** di *Modul 03*? Saat Pak Dengklek mencari buku resep di antara 1.000 buku yang sudah urut.
Alih-alih mengecek satu-satu, beliau menebas tumpukannya jadi dua ($500$). Lalu dibelah dua lagi jadi $250$. Lalu $125 \dots \, 62 \dots \, 31 \dots$ dan seterusnya sampai sisa 1.

Jika datanya $1.000$, dia cuma butuh $10$ langkah.
Jika datanya ekstrem $1.000.000$ (Satu Juta), dia cuma butuh **$20$ langkah**! 
Sangat tidak masuk akal cepatnya! Karena setiap perulangan, dia membuang separuh masalah ke tong sampah.

- **Wujud di Kodingan:** `Binary Search`, `Divide and Conquer`.
- **Karakter:** Raja efisiensi OSN-K. Biasanya ditandai dengan *Looping* yang nilai geraknya `dikali 2` atau `dibagi 2` (`i *= 2` atau `i /= 2`).

---

## 🚶‍♂️ 3. $O(N)$ — Sang Pejalan Kaki (Linear Time)

Ini adalah algoritma paling pasaran yang sangat wajar (Modul 01: Simulasi Linear). 
Bayangkan kamu disuruh menyalami 100 orang tamu satu per satu. Pasti kamu harus bersalaman tepat 100 kali. Kalau tamunya besok digandakan jadi 10.000 orang, kamu harus jabat tangan 10.000 kali.

Beban pekerjaanmu **tumbuh lurus seimbang** dengan jumlah datanya ($N$). Makin banyak $N$, makin lama tunggunya dengan porsi garis lurus.

- **Wujud di Kodingan:** *For-Looping* biasa bertingkat satu dari $0$ sampai $N$. Pencarian murni (*Linear Search*).
- **Karakter:** Sangat memadai untuk jumlah data sampai 100.000.000 elemen. Komputer modern (termasuk server grader OSN) bisa mengeksekusi $10^8$ iterasi murni dalam **~1 Detik**.

---

## 🐢 4. $O(N^2)$ — Sang Mimpi Buruk Kuadrat (Quadratic Time)

Hati-hati, ini adalah pembunuh masal peserta olimpiade pemula!
Bayangkan kamu ada di ruangan berisi 100 orang. Instruksinya bukan "kamu salaman dengan semua orang". Tetapi: **"TIAP-TIAP SATU ORANG saling cekokin salaman dengan KESELURUHAN ORANG LAINNYA di ruangan ini"**.

Untuk 100 orang, terjadi: $100 \times 100 = 10.000$ total salaman.
Kalau di ronde dua jumlah manusianya cuma ditambah dikit jadi 1.000 orang... total salamannya BUKAN nambah dikit, tapi meledak kuadrat menjadi $1.000 \times 1.000 = 1.000.000$ kali (Satu Juta salaman!).

*Kenaikan bebannya bengis.* Data nambah 10 kali lipat, waktu tunggu meledak 100 kali lipat.

- **Wujud di Kodingan:** *Nested Loop* ganda! (Ada `for` tunggal yang melingkupi `for` kedua di perutnya). Algoritma pengurutan jadul macam `Bubble Sort`, `Insertion Sort`, dan `Selection Sort`.
- **Karakter Terbatas:** Kalau limitnya 1 Detik, algoritma ini cuma kuat menghandle maksimal $N = 10.000$. Jika rentang soal melebar tembus $N = 100.000$... Komputermu dijamin mati terkapar (Time Limit Exceeded). Saat kamu dapat TLE di sini, kamu terpaksa harus menggunakan kecerdasan mencari cara lain (*Sorting* level Lanjut) buat nurunin ia jadi $O(N \log N)$ atau lebih baik.

---

## ☠️ 5. $O(2^N)$ — Sang Kiamat Mesin (Exponential Time)

Ini adalah tingkatan horor yang tak terbayangkan. Menggandakan diri dengan sangat biadab.
Kisah legendarisnya: Raja penemu catur meminta hadiah beras yang digandakan di setiap kotaknya.
- Kotak 1: $1$ beras ($2^0$)
- Kotak 2: $2$ beras ($2^1$)
- Kotak 3: $4$ beras ($2^2$)
- Kotak 4: $8$ beras ($2^3$)

Baru sampai Kotak catur ke-64 ($2^{64}$), jumlah berasnya ludes seisi panen planet Bumi ratusan abad ke depan tidak akan sanggup membayarnya. Komputer paling super (NASA) pun hancur lebur kalau dipaksa iterasi eksponensial dalam limit 1 Detik untuk skala $N > 40$.

- **Wujud di Kodingan:** **Rekursi Murni Tanpa Catatan** (Brute force percabangan ekstrem seperti contoh Tragedi Pohon Fibonacci di Modul 04).
- **Karakter:** Mati seketika untuk tebakan nilai $N = 40$. Inilah mengapa kita **WAJIB menggunakan Dynamic Programming (DP)** untuk mencambuk kiamat $O(2^N)$ agar menciut turun kasta kembali ke pejalan kaki yang lucu $O(N)$.

---

## 🏁 Rahasia Cepat: Rumus "Meteran 1 Detik" OSN-K 

Jika di soal ada batasan **Batas Waktu Eksekusi 1.0 Detik**, gunakan penggaris patokan dari juri ini di kepalamu:
Komputer juri mampu menjalankan sekitar **$10^8$ operasi sederhana** dalam 1 detik. 
(Artinya maksimal $100.000.000$ kali putaran iterasi).

Lihat nilai maksimal variabel $N$ di Lembar Soalmu:
1. Jika $N = 10 \dots 20 \rightarrow$ Gaskan aman sentosa pakai Brute Force cabang Eksponensial $O(2^N)$.
2. Jika $N = 1.000 \dots 10.000 \rightarrow$ Aman pakai *Nested loop ganda* (Kodingan barbar dobel `for` bersarang loop dalam loop) / $O(N^2)$.
3. Jika $N = 100.000 \implies 10^5 \rightarrow$ Jangan berani-berani pakai $O(N^2)$ karena ntar meledak jadi $10^{10}$ (Lebihi 10 pangkat 8 kan?). Segera ubah taktik pakai algoritma *Sorting modern* atau rumusan pintar Binary Search $O(N \log N)$.
4. Jika $N = 1.000.000$ (Satu Juta+) $\rightarrow$ Wajib mutlak Linear saja $O(N)$. Hanya boleh pakai 1 loop sejajar! (Atau cari trik *array prefix sum*, *greedy*, DP Tabulasi 1D).
5. Jika $N = 1.000.000.000$ (Satu Miliar) $\rightarrow$ Wah keterlaluan, 100% ini soal Teori Matematika (Ingat ilmu Rumus Gauss Part A?!). Ini wajib diselesaikan dengan Instan $O(1)$! Cari apanya yang bisa diformulasikan jadi rumus matematika mati (Aritmetika/Pigeonhole) tanpa nulis perulangan 1 pun!

*(Nah, materi Big O ini yang akan sering membuat logikamu tersenyum dan mengeliminasi jebakan-jebakan naif di ujian tertulis OSN-K nanti!)*.
