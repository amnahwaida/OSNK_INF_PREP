# 05. Algorithm Design (Perancangan Algoritma)

> "Algoritma bukan hanya tentang kode, tapi tentang cara kita memberikan instruksi yang presisi untuk menyelesaikan masalah."

Selamat! Kamu telah sampai di pilar terakhir dari Computational Thinking: **Algorithm Design** (Perancang Algoritma). Jika Decomposition memecah masalah, Pattern Recognition mencari kesamaan, dan Abstraction membuang detail, maka Algorithm Design adalah **penyusun langkah demi langkah** untuk mencapai solusi akhir.

---

## 🚀 Apa itu Algorithm Design?

**Algorithm Design** adalah kemampuan untuk menyusun langkah-langkah logis, terurut, dan detail untuk menyelesaikan sebuah masalah atau menjalankan sebuah tugas.

Bayangkan kamu adalah seorang arsitek yang memberikan instruksi kepada pekerja bangunan. Jika instruksimu tidak jelas, bangunan bisa rubuh. Begitu juga dengan komputer; ia hanya melakukan apa yang kamu perintahkan secara persis.

---

## 🍕 Analogi 1: Resep Membuat Pizza
Bayangkan kamu ingin mengajari adikmu membuat pizza. Kamu tidak bisa hanya bilang "buat pizza". Kamu harus memberikan algoritma:
1. Siapkan adonan roti.
2. Oleskan saus tomat di atas adonan.
3. Taburkan keju mozzarella dan topping lainnya.
4. Panggang di dalam oven pada suhu 200°C selama 15 menit.
5. Keluarkan dari oven dan potong menjadi 8 bagian.

Langkah-langkah di atas adalah sebuah **Algoritma**. Jika urutannya ditukar (misal: potong pizza dulu baru panggang), hasilnya akan kacau!

---

## 📦 Analogi 2: Rakit Lemari IKEA
Pernahkah kamu melihat buku instruksi merakit mainan atau lemari?
*   Ada daftar bahan (Input).
*   Ada langkah demi langkah gambar (Langkah Algoritma).
*   Ada hasil akhir lemari yang berdiri tegak (Output).

Buku instruksi tersebut adalah bentuk fisik dari sebuah desain algoritma.

---

## 💻 Kenapa Penting dalam Informatika?

Dalam dunia komputer, algoritma adalah "otak" dari setiap aplikasi.
*   **Google Maps**: Menggunakan algoritma untuk mencari rute tercepat (Dijkstra's Algorithm).
*   **Instagram**: Menggunakan algoritma untuk menentukan foto mana yang muncul paling atas di feed-mu.
*   **Sorting (Pengurutan)**: Algoritma untuk mengurutkan daftar nama dari A ke Z.

### 4 Syarat Algoritma yang Baik:
1.  **Finiteness (Terbatas)**: Harus ada titik berhenti. Jangan sampai komputer "hang" karena berputar selamanya.
2.  **Definiteness (Jelas)**: Setiap langkah tidak boleh bermakna ganda (ambigu).
3.  **Input & Output**: Harus jelas apa yang dimasukkan dan apa yang dihasilkan.
4.  **Effectiveness (Efektif)**: Langkahnya harus sederhana dan bisa dilakukan.

---

## 📝 Contoh di OSN-K Informatika

Di soal OSN-K, kamu sering diminta mengikuti jejak variabel dalam sebuah instruksi (Trace).
**Contoh sederhana:**
1. Mulai dengan angka $X = 5$.
2. Jika $X$ ganjil, tambahkan 1.
3. Jika $X$ genap, bagi dengan 2.
4. Ulangi langkah 2 & 3 sebanyak 3 kali. Berapa hasil akhirnya?

Kemampuan kamu mengikuti langkah di atas secara teliti adalah inti dari Algorithm Design.

---

## 🏗️ Latihan Soal Level: Newbie sampai Mahir

Berikut adalah bank soal latihan untuk mengasah logika algoritmamu.

### Soal #1: Algoritma Mencuci Tangan
Manakah urutan algoritma mencuci tangan yang paling logis dan benar?
1. Keringkan tangan dengan tissue.
2. Bilas dengan air mengalir.
3. Gosok tangan dengan sabun.
4. Basahi tangan dengan air.

A. 4-3-2-1
B. 3-4-2-1
C. 4-2-3-1
D. 2-3-4-1

<details>
<summary>💡 Hint</summary>
Pikirkan urutan yang paling higienis dan efektif: basahi dulu, baru sabun, baru bilas, baru keringkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4-3-2-1**
Urutan Logis: Basahi (4) -> Sabun (3) -> Bilas (2) -> Keringkan (1).
</details>

### Soal #2: Algoritma Penukaran Isi Gelas
Ada gelas A berisi Teh dan gelas B berisi Kopi. Algoritma untuk menukar isinya agar gelas A jadi Kopi dan gelas B jadi Teh membutuhkan bantuan gelas C (kosong). Urutan yang benar adalah...
1. Tuang isi B ke A.
2. Tuang isi A ke C.
3. Tuang isi C ke B.

A. 1-2-3
B. 2-1-3
C. 3-1-2
D. 2-3-1

<details>
<summary>💡 Hint</summary>
Gelas C digunakan untuk "menyimpan sementara" isi salah satu gelas agar tidak tumpah saat gelas lainnya dituangkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2-1-3**
Langkah: Pindahkan A ke C (A kosong), Pindahkan B ke A (B kosong), Pindahkan C ke B. Selesai!
</details>

### Soal #3: Algoritma "Tebak Angka"
Komputer memikirkan angka 1-100. Strategi paling cepat (Algoritma Binary Search) adalah dengan menebak angka tengah. Jika angka target adalah 75, apa tebakan pertama dan kedua komputer?
A. 1 lalu 2
B. 50 lalu 75
C. 50 lalu 25
D. 100 lalu 50

<details>
<summary>💡 Hint</summary>
Mulailah dari tengah (50). Karena 75 > 50, maka tebakan selanjutnya adalah tengah-tengah antara 51 sampai 100.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 50 lalu 75**
Langkah 1: Tengah (50). Langkah 2: Tengah antara 51-100 adalah 75 (Langsung ketemu!).
</details>

### Soal #4: Algoritma Membuat Indomie
Manakah langkah yang merupakan bagian dari "Input" dalam algoritma memasak mie instan?
A. Merebus air hingga mendidih.
B. Menyiapkan bumbu di piring.
C. Menyiapkan satu bungkus mie dan air.
D. Mengaduk mie dengan bumbu.

<details>
<summary>💡 Hint</summary>
Input adalah bahan-bahan atau persiapan awal sebelum proses dimulai.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Menyiapkan satu bungkus mie dan air.**
Bahan mentah adalah input, sedangkan memasak adalah proses.
</details>

### Soal #5: Algoritma Lampu Lalu Lintas
Sebuah algoritma mengatur lampu: Merah (30 detik) -> Hijau (20 detik) -> Kuning (5 detik) -> Ulangi. Jika sekarang detik ke-1 Hijau, warna apa yang muncul 26 detik kemudian?
A. Merah
B. Hijau
C. Kuning
D. Mati

<details>
<summary>💡 Hint</summary>
Hitung sisa waktu Hijau (20 detik total). Jika baru jalan 1 detik, sisa 19 detik Hijau. Sisa detiknya masuk ke fase berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kuning**
Sisa Hijau: 19 detik. Sisa waktu pertanyaan: 26 - 19 = 7 detik lagi. Masuk ke fase Kuning (yang berdurasi 5 detik). Karena 7 > 5, maka sebenarnya setelah 7 detik sudah masuk ke Merah awal.
*Re-kalkulasi:* Hijau (1-20), Kuning (21-25), Merah (26-55). Pada detik ke-26 dari awal Hijau, lampu sudah berubah jadi **Merah**.
*Jawaban yang tepat sesuai hitungan:* **A. Merah**.
</details>

### Soal #6: Algoritma Robot Kurir
Robot berada di koordinat (0,0). Instruksi: Maju 2 langkah, Putar Kanan 90°, Maju 3 langkah. Di koordinat mana robot sekarang (X,Y)?
A. (2, 3)
B. (3, 2)
C. (2, -3)
D. (3, -2)

<details>
<summary>💡 Hint</summary>
Asumsikan Maju menambah nilai Y. Putar Kanan mengubah arah ke X positif.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. (3, 2)** atau **(2, -3)** tergantung arah hadap awal. Jika hadap Utara (Y+), Maju 2 (0,2). Putar Kanan (Hadap X+), Maju 3 (3,2).
*Pilihan yang paling mendekati:* **A. (3, 2)** atau **B**. Kita asumsikan format (X,Y). Maju 2 (0,2) -> Kanan -> Maju 3 (3,2).
</details>

### Soal #7: Syarat "Finiteness"
Kenapa algoritma "Ulangi: Tulis 'Halo' selamanya" dianggap algoritma yang buruk?
A. Karena kata 'Halo' membosankan.
B. Karena melanggar syarat Finiteness (harus ada titik henti).
C. Karena memakan banyak tinta.
D. Karena komputer tidak suka menyapa.

<details>
<summary>💡 Hint</summary>
Algoritma harus memberikan solusi dalam waktu yang terbatas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Melanggar syarat Finiteness.**
Algoritma harus berhenti (finish) setelah mencapai tujuannya.
</details>

### Soal #8: Algoritma Mencari Kartu Terbesar
Kamu punya tumpukan 10 kartu acak. Algoritma paling benar untuk mencari kartu terbesar adalah...
A. Ambil kartu pertama, anggap itu yang terbesar. Bandingkan dengan kartu berikutnya satu per satu. Jika ada yang lebih besar, jadikan dia "terbesar sementara".
B. Kocok kartunya sampai yang terbesar muncul di atas.
C. Ambil dua kartu saja dan pakai yang lebih besar di antara keduanya.
D. Langsung tebak kartu kelima.

<details>
<summary>💡 Hint</summary>
Pikirkan proses sistematis yang menjamin kartu paling besar pasti ditemukan meskipun kartunya sangat banyak.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bandingkan satu per satu dengan "terbesar sementara".**
Ini adalah dasar dari algoritma *Linear Search* atau *Selection*.
</details>

### Soal #9: Algoritma "Lampu Tidur Otomatis"
1. Baca sensor cahaya.
2. JIKA cahaya < 10 (gelap), MAKA nyalakan lampu.
3. JIKA TIDAK, MAKA matikan lampu.
4. Tunggu 5 detik, kembali ke langkah 1.
Apa "Output" dari algoritma ini?
A. Sensor cahaya.
B. Kondisi lampu (Nyala/Mati).
C. Angka 10.
D. Waktu 5 detik.

<details>
<summary>💡 Hint</summary>
Output adalah hasil atau aksi yang dilakukan oleh sistem setelah memproses input.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kondisi lampu (Nyala/Mati).**
Aksi menyalakan/mematikan lampu adalah output yang terlihat/terasa oleh pengguna.
</details>

### Soal #10: Seleksi Algoritma (Percabangan)
"Jika hari hujan, bawa payung. Jika tidak hujan dan panas, pakai topi. Jika tidak keduanya, jangan bawa apa-apa."
Kondisi hari ini: **Cerah dan Panas**. Apa yang kamu lakukan?
A. Bawa payung.
B. Pakai topi.
C. Bawa payung dan topi.
D. Tidak bawa apa-apa.

<details>
<summary>💡 Hint</summary>
Ikuti logika "If-Else" secara bertahap. Cek kondisi pertama, jika salah, cek kondisi kedua.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pakai topi.**
Hujan? Tidak. Panas? Ya. Maka pilih instruksi "pakai topi".
</details>

### Soal #11: Algoritma Pembuatan Akun
Urutan manakah yang benar dalam mendaftar akun media sosial?
1. Verifikasi email.
2. Masukkan username dan password.
3. Klik tombol "Daftar".
4. Buka halaman registrasi.

A. 4-2-3-1
B. 4-3-2-1
C. 1-2-3-4
D. 2-3-1-4

<details>
<summary>💡 Hint</summary>
Kamu harus ada di halamannya dulu (4), isi data (2), baru kirim (3), baru cek email (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4-2-3-1**
Langkah logis pendaftaran akun digital.
</details>

### Soal #12: Algoritma "Naik Lift"
Jika kamu di lantai 1 dan ingin ke lantai 5:
1. Masuk ke lift.
2. Tekan tombol 5.
3. Tunggu lift sampai di lantai 1.
4. Tunggu sampai pintu terbuka di lantai 5 dan keluar.
5. Tekan tombol panggil lift.
Urutan yang benar adalah...
A. 5-3-1-2-4
B. 1-2-3-4-5
C. 5-1-3-2-4
D. 2-5-3-1-4

<details>
<summary>💡 Hint</summary>
Panggil dulu (5), tunggu sampai (3), masuk (1), tekan tujuan (2), sampai (4).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 5-3-1-2-4**
Urutan presisi interaksi dengan lift.
</details>

### Soal #13: Algoritma Penjumlahan Deret
Algoritma: $X = 0$, tambahkan $X$ dengan angka 1, 2, dan 3 secara berurutan. Apa isi $X$ sekarang?
A. 1
B. 3
C. 6
D. 0

<details>
<summary>💡 Hint</summary>
$(0 + 1) = 1$, lalu $(1 + 2) = 3$, lalu $(3 + 3) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 6**
Akumulasi penambahan $1+2+3 = 6$.
</details>

### Soal #14: Algoritma "Password Salah"
Sebuah sistem ATM:
1. Masukkan PIN.
2. Jika PIN benar, masuk ke menu.
3. Jika PIN salah, kurangi kesempatan sebanyak 1.
4. Jika kesempatan = 0, blokir kartu.
Jika kesempatan awal adalah 3, dan seseorang salah memasukkan PIN sebanyak 3 kali, apa status kartunya?
A. Masuk ke menu.
B. Kesempatan sisa 1.
C. Terblokir.
D. Berkurang 3.

<details>
<summary>💡 Hint</summary>
Lakukan pengurangan (3-1-1-1) dan cek kondisi di langkah 4.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Terblokir.**
Setiap salah mengurangi jatah. Setelah 3 kali salah, kesempatan menjadi 0 dan kartu diblokir.
</details>

### Soal #15: Algoritma Mencari Kata di Kamus
Cara tercepat mencari kata "Zebra" di kamus fisik adalah dengan...
A. Membuka dari halaman pertama satu per satu hingga akhir.
B. Langsung membuka area belakang kamus karena "Z" di urutan terakhir.
C. Mencari dari tengah lalu ke arah depan.
D. Menebak halaman secara acak.

<details>
<summary>💡 Hint</summary>
Gunakan pengetahuan tentang indeks alfabetis untuk mempercepat pencarian.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Membuka area belakang.**
Pemanfaatan struktur data terurut (Alphabetical) untuk efisiensi pencarian.
</details>

### Soal #16: Algoritma "Kelipatan 3"
1. Mulai dari $N = 1$.
2. Tulis $N$ jika habis dibagi 3.
3. Tambahkan $N$ dengan 1.
4. Ulangi sampai $N = 10$.
Berapa banyak angka yang ditulis?
A. 3
B. 4
C. 10
D. 1

<details>
<summary>💡 Hint</summary>
Angka antara 1-10 yang habis dibagi 3 adalah: 3, 6, 9.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 3**
Angka yang ditulis adalah 3, 6, dan 9.
</details>

### Soal #17: Efektivitas Algoritma
Dua orang ingin menghitung $10 + 10 + 10 + 10 + 10$.
- Orang A: Menambah satu-satu (10+10=20, 20+10=30, dst).
- Orang B: Menghitung $10 \times 5$.
Siapa yang menggunakan algoritma lebih efektif?
A. Orang A
B. Orang B
C. Sama saja
D. Tidak ada yang benar

<details>
<summary>💡 Hint</summary>
Efektivitas berkaitan dengan kecepatan mencapai hasil yang sama dengan langkah yang lebih ringkas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Orang B**
Operasi perkalian adalah bentuk "jalan pintas" (abstraksi matematis) yang lebih cepat daripada penjumlahan berulang.
</details>

### Soal #18: Algoritma "Cek Lulus"
Jika nilai $\ge 75$ MAKA "Lulus". Jika tidak MAKA "Remedial".
Budi mendapat nilai 74.9. Apa hasil yang muncul di layar?
A. Lulus
B. Remedial
C. 75
D. Eror

<details>
<summary>💡 Hint</summary>
Perhatikan operator perbandingannya ($\ge$). 74.9 lebih kecil dari 75.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Remedial**
Karena 74.9 < 75, maka kondisi Lulus tidak terpenuhi.
</details>

### Soal #19: Algoritma Pengurutan (Es Krim)
Urutkan rasa es krim berdasarkan harga dari yang termurah (Sorting):
- Cokelat: Rp 5.000
- Vanila: Rp 4.500
- Strawberry: Rp 6.000

A. Vanila - Cokelat - Strawberry
B. Strawberry - Cokelat - Vanila
C. Cokelat - Vanila - Strawberry
D. Vanila - Strawberry - Cokelat

<details>
<summary>💡 Hint</summary>
Bandingkan angkanya: 4.500 < 5.000 < 6.000.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Vanila - Cokelat - Strawberry**
Pengurutan berdasarkan nilai numerik terkecil ke terbesar.
</details>

### Soal #20: Algoritma Keamanan (Lockscreen)
"Geser ke atas untuk membuka". Jika kamu mengetuk layar 2 kali, apakah HP terbuka?
A. Ya, karena HP-nya pintar.
B. Tidak, karena input yang diberikan tidak sesuai dengan langkah algoritma pembukaan kunci.
C. Tergantung merk HP.
D. Ya, jika layar disentuh.

<details>
<summary>💡 Hint</summary>
Algoritma sangat kaku terhadap jenis Input. Jika minta "Geser", maka "Ketuk" tidak akan diproses.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak sesuai dengan langkah algoritma.**
Algoritma memerlukan input spesifik untuk menghasilkan output yang diinginkan.

---
[< Materi Sebelumnya: Abstraction](./04-abstraction.md) | [Materi Selanjutnya: Latihan Soal Campuran](../README.md)
[< Kembali ke Beranda Materi](../README.md)
