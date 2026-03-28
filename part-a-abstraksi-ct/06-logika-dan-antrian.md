# 06. Logika Dasar dan Antrian (Logic & Queue)

> "Komputer tidak pernah bingung, ia hanya mengikuti logika yang kamu berikan. Jika hasilnya salah, periksa logikanya, bukan komputernya."

Selamat! Kamu sudah mempelajari 4 pilar utama Computational Thinking. Sekarang, kita akan masuk ke dua konsep teknis yang sangat sering muncul di soal OSN-K Informatika: **Logika Boolean** dan **Struktur Data Antrian (Queue)**.

---

## 🧠 Bagian 1: Logika Boolean (Gerbang Logika)

Dalam dunia komputer, segala sesuatu hanya bernilai **TRUE** (Benar/1) atau **FALSE** (Salah/0). Logika ini digunakan untuk mengambil keputusan.

### 1. Operator Logika Dasar & Lanjutan

Ada beberapa operator yang sering muncul di OSN-K:

| Operator | Simbol | Penjelasan Sederhana |
| :--- | :--- | :--- |
| **AND** | `&&` / `DAN` | Bernilai BENAR hanya jika **SEMUA** syarat terpenuhi. |
| **OR** | `||` / `ATAU` | Bernilai BENAR jika **SALAH SATU** saja syarat terpenuhi. |
| **NOT** | `!` / `TIDAK` | Membalikkan nilai (Benar jadi Salah, Salah jadi Benar). |
| **XOR** | `^` / `EKS-OR` | Bernilai BENAR jika **HANYA SATU** yang benar (Beda nilai = Benar, Sama nilai = Salah). |
| **NAND** | `!AND` | Kebalikan dari AND (Bernilai SALAH hanya jika semua BENAR). |
| **NOR** | `!OR` | Kebalikan dari OR (Bernilai BENAR hanya jika semua SALAH). |

### 2. Analogi Kehidupan Nyata (Lebih Detail)

*   **AND**: Syarat lulus ujian: (Hadir > 75% **AND** Nilai > 70).
*   **OR**: Diskon member: (Punya Kartu Member **OR** Belanja > 1 Juta).
*   **XOR**: Saklar lampu hotel (dua saklar untuk satu lampu): Jika saklar A dan B posisinya sama, lampu mati. Jika beda posisi, lampu nyala.
*   **NOT**: Tombol "Mute" di TV: (NOT Suara Aktif).

### 3. Tabel Kebenaran Lengkap

| A | B | AND | OR | XOR | NAND |
| :--- | :--- | :---: | :---: | :---: | :---: |
| T | T | **T** | **T** | F | F |
| T | F | F | **T** | **T** | **T** |
| F | T | F | **T** | **T** | **T** |
| F | F | F | F | F | **T** |

### 4. Hukum Logika Penting (De Morgan)

Seringkali kita perlu membalikkan sebuah logika yang kompleks. Gunakan aturan sederhana ini:
*   **NOT (A AND B)** sama dengan **(NOT A) OR (NOT B)**
*   **NOT (A OR B)** sama dengan **(NOT A) AND (NOT B)**

*Analogi:* "Saya TIDAK (makan nasi DAN minum teh)" berarti "Saya TIDAK makan nasi ATAU saya TIDAK minum teh".

### 5. Relasi dengan Kehidupan & Informatika

#### A. Logika dalam Informatika:
*   **Mesin Pencari (Google)**: Saat kamu mencari `Kucing AND Lapar`, Google hanya menampilkan hasil yang ada kedua kata tersebut. Jika `Kucing OR Anjing`, Google menampilkan salah satu atau keduanya.
*   **Sistem Login**: Kamu bisa masuk JIKA (Username Benar **AND** Password Benar). Salah satu salah, kamu ditolak.
*   **Filter Belanja**: Menampilkan barang yang (Kategori: Elektronik **AND** Harga < 1 Juta).

#### B. Logika dalam Kehidupan:
*   **Lampu Lalu Lintas**: Lampu Hijau menyala JIKA (Arah lawan Merah **AND** Tidak ada kereta lewat).
*   **Resep Masakan**: Jika tidak ada Mentega, gunakan Catatan: (Mentega **OR** Margarin).

---

## 🚶 Bagian 2: Antrian (Queue) & Tumpukan (Stack)

Dalam informatika, kita menyebut ini sebagai **Struktur Data**.

### 1. Antrian (Queue) - FIFO

#### A. Relasi dengan Informatika:
*   **Web Server**: Jika 100 orang membuka website bersamaan, server akan melayani orang yang klik-nya sampai ke server paling awal (Antrian Request).
*   **Sistem Operasi**: Komputer mengatur jalannya aplikasi yang banyak menggunakan antrian agar semua aplikasi kebagian waktu proses (CPU Scheduling).

#### B. Relasi dengan Kehidupan:
*   **Eskalator**: Orang yang naik duluan akan sampai di atas/bawah duluan.
*   **Pipa Air**: Air yang masuk ke ujung pipa pertama kali adalah yang keluar dari keran pertama kali.

### 2. Tumpukan (Stack) - LIFO

#### A. Relasi dengan Informatika:
*   **Tag HTML/Coding**: Jika kamu menulis `<b><i>Teks</i></b>`, kamu harus menutup `<i>` dulu baru `<b>`. Tag yang terakhir dibuka (i) harus ditutup pertama kali (LIFO).
*   **Fungsi Rekursif**: Saat sebuah fungsi memanggil dirinya sendiri, komputer menyimpan posisi fungsi sebelumnya dalam sebuah "Stack".

#### B. Relasi dengan Kehidupan:
*   **Pez Dispenser**: Permen yang kamu masukkan terakhir ke dalam wadah adalah yang akan keluar pertama kali saat kamu menekan kepalanya.
*   **Baju dalam Koper**: Baju yang kamu taruh paling atas saat packing adalah baju yang pertama kali kamu ambil saat sampai di hotel.

---

## 💻 Bagian 3: Contoh Gabungan (Simulasi Robot)

### Soal #01: Syarat Beasiswa
Budi akan mendapat beasiswa jika: (Nilai Matematika > 80) **DAN** (Penghasilan Orang Tua < 3 Juta).
Data Budi: Nilai Matematika = 85, Penghasilan Orang Tua = 4 Juta.
Apakah Budi mendapat beasiswa?
A. Ya
B. Tidak
C. Mungkin
D. Data tidak cukup

<details>
<summary>💡 Hint</summary>
Gunakan logika AND. Kedua syarat harus BENAR agar hasilnya BENAR.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Syarat 1 (85 > 80) bernilai BENAR. 
Syarat 2 (4 Juta < 3 Juta) bernilai SALAH. 
BENAR AND SALAH = **SALAH**.
</details>

### Soal #02: Logika "Atau"
Lampu akan menyala jika: (Tombol A ditekan) **OR** (Tombol B ditekan).
Jika Tombol A TIDAK ditekan, tapi Tombol B ditekan, bagaimana status lampu?
A. Mati
B. Menyala
C. Berkedip
D. Meledak

<details>
<summary>💡 Hint</summary>
Logika OR hanya butuh satu syarat BENAR untuk menghasilkan BENAR.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyala.**
Karena salah satu tombol (Tombol B) ditekan, maka kondisi OR terpenuhi.
</details>

### Soal #03: Antrian Tiket Bioskop
Ada antrian: Budi, Ani, Cici (Budi paling depan).
Lalu datang Dedi masuk ke antrian. Kemudian 2 orang paling depan selesai membeli tiket dan pergi.
Siapakah yang sekarang berada di urutan paling depan?
A. Ani
B. Cici
C. Dedi
D. Budi

<details>
<summary>💡 Hint</summary>
Gunakan prinsip FIFO. Enqueue(Dedi), lalu Dequeue(), Dequeue().
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Cici.**
1. Awal: (Budi, Ani, Cici)
2. Dedi datang: (Budi, Ani, Cici, Dedi)
3. Keluar 1 (Budi): (Ani, Cici, Dedi)
4. Keluar 2 (Ani): (Cici, Dedi)
Paling depan sekarang adalah Cici.
</details>

### Soal #04: Tumpukan Buku (Stack)
Sebuah tumpukan buku berisi: Matematika (bawah), Fisika (tengah), Kimia (atas).
Budi menaruh buku Biologi di atas Kimia. Lalu Budi mengambil 2 buku dari tumpukan paling atas.
Buku apa yang tersisa di tumpukan?
A. Matematika dan Fisika
B. Kimia dan Biologi
C. Matematika dan Kimia
D. Fisika dan Kimia

<details>
<summary>💡 Hint</summary>
Stack menggunakan LIFO. Yang terakhir masuk adalah yang pertama diambil.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Matematika dan Fisika.**
1. Tumpukan: [Mat, Fis, Kim]
2. Tambah Bio: [Mat, Fis, Kim, Bio]
3. Ambil 1 (Bio): [Mat, Fis, Kim]
4. Ambil 2 (Kim): [Mat, Fis]
Buku yang tersisa adalah Matematika dan Fisika.
</details>

### Soal #05: Negasi (NOT)
Jika pernyataan $P$ adalah "Hari ini hujan", maka pernyataan **NOT (NOT P)** sama dengan...
A. Hari ini cerah
B. Hari ini hujan
C. Hari ini mendung
D. Tidak mungkin hujan

<details>
<summary>💡 Hint</summary>
Double Negation: Negasi yang dibatalkan oleh negasi lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hari ini hujan.**
NOT P = "Hari ini tidak hujan".
NOT (NOT P) = TIDAK (Tidak hujan) = "Hari ini hujan".
</details>

### Soal #11: Logika "Lampu Malam"
Lampu taman otomatis menyala JIKA (Waktu > 18:00) **AND** (NOT Ada Cahaya Matahari).
Jika jam menunjukkan 19:00 tapi ada lampu sorot terang yang mengenai sensor cahaya, apakah lampu taman menyala?
A. Ya
B. Tidak
C. Kadang-kadang
D. Tergantung saklar

<details>
<summary>💡 Hint</summary>
(19:00 > 18:00) adalah BENAR. (Ada Cahaya) adalah BENAR, maka (NOT Ada Cahaya) adalah SALAH.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
BENAR AND SALAH = SALAH. Sensor cahaya mendeteksi terang, sehingga kondisi "tidak ada cahaya" menjadi salah.
</details>

### Soal #12: Antrian Bank yang Sibuk
Antrian: [A, B, C]. 
1. Masuk D. 
2. A keluar. 
3. Masuk E. 
4. B keluar.
Siapakah dua orang terdepan sekarang?
A. C dan D
B. D dan E
C. C dan E
D. E dan D

<details>
<summary>💡 Hint</summary>
Ikuti urutan FIFO dengan teliti.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. C dan D.**
Awal: [A, B, C] -> +D: [A, B, C, D] -> -A: [B, C, D] -> +E: [B, C, D, E] -> -B: [C, D, E].
Terdepan adalah C, urutan kedua adalah D.
</details>

### Soal #13: Tumpukan Piring (Stack)
Tumpukan: [Bawah: Piring Merah, Piring Biru, Piring Hijau :Atas].
Kamu menambah Piring Kuning, lalu mengambil 3 piring dari atas. Piring warna apa yang tersisa?
A. Kuning
B. Hijau
C. Biru
D. Merah

<details>
<summary>💡 Hint</summary>
LIFO: Terakhir masuk (Kuning) adalah yang pertama keluar.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Merah.**
Awal: [M, B, H] -> +K: [M, B, H, K]. 
Ambil 3: K keluar, H keluar, B keluar. Sisa: M (Merah).
</details>

### Soal #14: Logika XOR pada Saklar
Dua saklar (A dan B) mengontrol satu lampu. Lampu NYALA jika A **XOR** B bernilai BENAR.
Jika A = 0 (Off) dan B = 1 (On), status lampu adalah?
A. Nyala (1)
B. Mati (0)
C. Berkedip
D. Konslet

<details>
<summary>💡 Hint</summary>
XOR bernilai benar jika inputnya BERBEDA.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Nyala (1).**
Karena 0 dan 1 berbeda, maka output XOR adalah 1 (Benar/Nyala).
</details>

### Soal #15: Antrian Berhenti (Dequeue Error)
Ada antrian: [Kopi].
1. Dequeue dilakukan (Kopi keluar).
2. Dequeue dilakukan lagi.
Apa yang terjadi pada sistem jika antrian kosong tapi dipaksa keluar?
A. Sistem menunggu sampai ada data baru.
B. Terjadi error (Underflow).
C. Data terakhir keluar lagi.
D. Sistem meledak.

<details>
<summary>💡 Hint</summary>
Dalam komputer, mengambil data dari tempat yang kosong disebut "Underflow".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terjadi error (Underflow).**
Kita tidak bisa mengambil benda dari kotak yang sudah kosong.
</details>

### Soal #16: Logika NAND (Not AND)
Gerbang NAND: Hasilnya SALAH hanya jika kedua input BENAR.
Jika Ani belajar (T) dan Ani lulus (T), maka (Belajar NAND Lulus) adalah...
A. Benar
B. Salah
C. Mungkin
D. Tidak relevan

<details>
<summary>💡 Hint</summary>
T NAND T = NOT (T AND T).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
AND menghasilkan Benar, lalu NOT membalikkannya jadi Salah.
</details>

### Soal #17: Stack "Undo" Berlapis
Aksi: [Tulis A, Tulis B, Hapus B, Tulis C].
Jika dilakukan "Undo" sebanyak 2 kali, kondisi akhir adalah...
A. [Tulis A, Tulis B]
B. [Tulis A]
C. [Tulis A, Tulis B, Hapus B]
D. Kosong

<details>
<summary>💡 Hint</summary>
Undo membatalkan aksi TERAKHIR.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Tulis A, Tulis B].**
Aksi terakhir: Tulis C (di-Undo -> Hilang). 
Aksi sebelumnya: Hapus B (di-Undo -> B kembali ada).
</details>

### Soal #18: Antrian Pesan Chat
Pesan masuk: [P1, P2, P3].
Server hanya bisa memproses 1 pesan per detik. Pada detik ke-1.5, pesan mana yang sudah selesai diproses?
A. P1
B. P2
C. P3
D. P1 dan P2

<details>
<summary>💡 Hint</summary>
FIFO: P1 diproses detik ke-1, P2 detik ke-2.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. P1.**
Karena baru 1.5 detik, P2 masih dalam proses atau sedang menunggu.
</details>

### Soal #19: Logika NOR (Not OR)
Hasil NOR adalah BENAR jika **SEMUA** inputnya SALAH.
A = Salah, B = Salah. Maka A NOR B adalah...
A. Benar
B. Salah
C. Mungkin
D. Tergantung C

<details>
<summary>💡 Hint</summary>
F NOR F = NOT (F OR F).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
F OR F = Salah. NOT Salah = Benar.
</details>

### Soal #20: Kombinasi Queue dan Stack
Sebuah sistem menerima data: 1, 2, 3.
1. Masukkan ke Queue -> [1, 2, 3].
2. Keluarkan 1 data dari Queue (diambil 1), lalu masukkan hasil itu ke Stack.
3. Masukkan data 4 ke Queue.
Daftar di dalam Queue sekarang adalah?
A. [2, 3, 4]
B. [1, 2, 3]
C. [4, 3, 2]
D. [1, 4]

<details>
<summary>💡 Hint</summary>
Queue (FIFO): yang keluar duluan adalah yang masuk duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [2, 3, 4].**
Awal: [1, 2, 3]. 1 keluar (masuk ke stack lain). Sisa Queue: [2, 3]. Lalu +4: [2, 3, 4].
</details>

### Soal #21: Logika Braket (Kurung)
Hasil dari: NOT (Benar **OR** Salah) **AND** Benar adalah...
A. Benar
B. Salah
C. Mungkin
D. Error

<details>
<summary>💡 Hint</summary>
Kerjakan kurung: (B OR S) = B. Lalu NOT B = S. Terakhir S AND B.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
S AND B = Salah.
</details>

### Soal #22: Antrian Tiket Kereta
Antrian: [Andi, Budi].
1. Andi selesai.
2. Caca datang.
3. Budi selesai.
4. Dedi datang.
Siapa yang paling belakang di antrian?
A. Caca
B. Dedi
C. Andi
D. Budi

<details>
<summary>💡 Hint</summary>
Paling belakang berarti yang terakhir masuk (Enqueue).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dedi.**
Urutan masuk: Andi, Budi, Caca, Dedi. Dedi adalah yang paling baru (paling belakang).
</details>

### Soal #23: Tumpukan Kartu (Stack)
Tumpukan: [As, King, Queen].
Kamu ambil 1 (Queen), taruh Jack, taruh 10.
Jika kamu ambil 1 kartu lagi dari atas, kartu apa itu?
A. Jack
B. 10
C. King
D. As

<details>
<summary>💡 Hint</summary>
LIFO: Terakhir ditaruh adalah yang paling atas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 10.**
Tumpukan: [As, King] -> +Jack: [As, King, Jack] -> +10: [As, King, Jack, 10]. Teratas adalah 10.
</details>

### Soal #24: Logika Deteksi Banjir
Alarm bunyi JIKA (Ketinggian Air > 200cm) **OR** (Debit Air > 500L/s).
Data: Air = 150cm, Debit = 600L/s. Apakah alarm bunyi?
A. Ya
B. Tidak
C. Rusak
D. Tergantung Hujan

<details>
<summary>💡 Hint</summary>
Syarat OR: Cukup satu yang terpenuhi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
Debit air 600 sudah melebihi batas 500, sehingga alarm aktif.
</details>

### Soal #25: Antrian di Lift
Lift kapasitas 2 orang. Antrian: [A, B, C, D, E].
Lift naik pertama membawa A dan B. Lift kembali kosong. Siapa yang akan naik berikutnya?
A. C dan D
B. E saja
C. Semua sisa
D. A dan B lagi

<details>
<summary>💡 Hint</summary>
FIFO: Antrian dilayani per kelompok sesuai kapasitas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. C dan D.**
C dan D adalah urutan berikutnya setelah A dan B keluar dari antrian.
</details>

### Soal #26: Logika Berjenjang
Jika $X = 5$. Manakah logika yang bernilai BENAR?
A. $(X > 10)$ AND $(X < 2)$
B. $(X = 5)$ OR $(X = 10)$
C. NOT $(X = 5)$
D. $(X < 5)$ AND $(X > 0)$

<details>
<summary>💡 Hint</summary>
Cek satu per satu syaratnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. (X=5) OR (X=10).**
Syarat pertama (5=5) adalah BENAR. Karena ini OR, hasil akhirnya langsung BENAR.
</details>

### Soal #27: Stack "Browsing"
Kamu di Google -> Klik Wiki -> Klik Youtube. (Sekarang di Youtube).
Kamu klik "Back" 1 kali. Di mana kamu sekarang?
A. Google
B. Wiki
C. Home
D. Youtube

<details>
<summary>💡 Hint</summary>
Sejarah browser adalah Stack. Back mengambil halaman sebelumnya (paling atas tumpukan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Wiki.**
Tumpukan: [Google, Wiki, Youtube]. Back membuang Youtube, tersisa Wiki di paling atas.
</details>

### Soal #28: Antrian Download File
File: [Besar, Sedang, Kecil]. Semuanya mulai download bersamaan (Parallel).
Ternyata koneksi lambat, hanya bisa 1 file. Sistem otomatis mengantrikan (Queue).
File mana yang paling terakhir selesai?
A. Besar
B. Sedang
C. Kecil
D. Bersamaan

<details>
<summary>💡 Hint</summary>
FIFO: Yang masuk antrian terakhir akan diproses terakhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kecil.**
Urutan antrian: Besar(1), Sedang(2), Kecil(3). Maka Kecil adalah yang paling akhir diproses.
</details>

### Soal #29: Logika Keamanan Rumah
Pintu terbuka JIKA (Punya Kunci) **AND** (NOT Alarm Aktif).
Budi punya kunci, tapi ia lupa mematikan alarm. Apakah pintu terbuka?
A. Terbuka
B. Tetap Terkunci
C. Alarm meledak
D. Kunci patah

<details>
<summary>💡 Hint</summary>
(Punya Kunci = Benar) AND (NOT Alarm Aktif = Salah).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tetap Terkunci.**
Benar AND Salah = Salah. Pintu tidak akan terbuka demi keamanan.
</details>

### Soal #30: Refleksi Computational Thinking
Setelah belajar Logika dan Antrian, apa langkah pertama yang paling tepat jika kamu ingin membuat aplikasi "Booking Tiket Pesawat"?
A. Membuat desain logo aplikasi.
B. Merancang logika antrian kursi dan sistem pembayaran (Boolean).
C. Mencari investor.
D. Membeli laptop baru.

<details>
<summary>💡 Hint</summary>
Gunakan pilar CT yang sudah kamu pelajari untuk menyelesaikan masalah inti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Merancang logika dan sistem antrian.**
Ini adalah inti teknis dari fungsionalitas aplikasi tiket yang adil dan aman.
</details>

### Soal #31: Pencarian Google (AND/NOT)
Kamu ingin mencari resep kue yang (Tanpa Telur) **AND** (Gunakan Cokelat).
Hasil pencarian mana yang akan muncul?
A. Resep Brownies Kukus (Bahan: Telur, Cokelat, Tepung)
B. Resep Dark Chocolate Cake (Bahan: Cokelat, Pisang, Tepung)
C. Resep Omelet Cokelat (Bahan: Telur, Cokelat)
D. Resep Roti Tawar (Bahan: Tepung, Ragi)

<details>
<summary>💡 Hint</summary>
Syarat 1: NOT Telur. Syarat 2: Cokelat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Resep Dark Chocolate Cake.**
Hanya pilihan B yang mengandung Cokelat tanpa menggunakan Telur.
</details>

### Soal #32: Tag HTML (Stack)
Sebuah kode web tertulis: `<div><span><b>Teks`.
Manakah urutan penutup tag yang benar sesuai prinsip Stack?
A. `</b></span></div>`
B. `</div></span></b>`
C. `</span></b></div>`
D. `</b></div></span>`

<details>
<summary>💡 Hint</summary>
LIFO: Tag yang terakhir dibuka (`<b>`) harus ditutup pertama kali.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. </b></span></div>.**
Urutan buka: div -> span -> b. Maka urutan tutup harus dibalik: b -> span -> div.
</details>

### Soal #33: CPU Scheduling (Queue)
Komputer memiliki 3 tugas: [Cetak_Dokumen, Putar_Musik, Scan_Virus].
Jika komputer menggunakan sistem Queue, dan tiba-tiba user klik "Pause" pada Putar_Musik, tugas mana yang akan diproses selanjutnya setelah Cetak_Dokumen selesai?
A. Putar_Musik
B. Scan_Virus
C. Tidak ada
D. Cetak_Dokumen lagi

<details>
<summary>💡 Hint</summary>
Jika satu tugas ditangguhkan/dikeluarkan dari antrian, tugas di belakangnya maju.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Scan_Virus.**
Urutan: [1.Cetak, 2.Musik, 3.Scan]. Karena Musik di-pause, maka urutan ke-2 yang kosong diisi oleh Scan_Virus.
</details>

### Soal #34: Hukum De Morgan (Logic)
Pernyataan: **NOT (Lapar AND Haus)** identik dengan...
A. NOT Lapar AND NOT Haus
B. NOT Lapar OR NOT Haus
C. Lapar OR Haus
D. Tetap Lapar dan Haus

<details>
<summary>💡 Hint</summary>
Hukum De Morgan: NOT (A AND B) = (NOT A) OR (NOT B).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. NOT Lapar OR NOT Haus.**
Pernyataan ini berarti "Setidaknya salah satu dari kondisi (Lapar atau Haus) tidak terjadi".
</details>

### Soal #35: Keamanan Microwave
Microwave menyala JIKA (Pintu Tertutup) **AND** (Waktu Set > 0) **AND** (Tombol Start Ditekan).
Jika pintu tertutup dan waktu sudah di-set 2 menit, tapi microwave tidak menyala, apa kemungkinan penyebabnya?
A. Pintu rusak
B. Waktu habis
C. Tombol Start belum ditekan
D. Listrik mati

<details>
<summary>💡 Hint</summary>
Syarat AND membutuhkan SEMUA kondisi bernilai BENAR.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Tombol Start belum ditekan.**
Karena dua syarat lain sudah terpenuhi (Pintu & Waktu), maka syarat ketiga yang mungkin belum aktif.
</details>

### Soal #36: Vending Machine (Queue)
Koin yang kamu masukkan ke lubang vending machine masuk ke dalam sebuah tabung penyimpanan. Jika koin yang kamu masukkan pertama kali adalah koin yang paling bawah (untuk diambil pemilik mesin), sistem penyimpanan ini menggunakan prinsip...
A. Stack
B. Queue
C. Random
D. Circular

<details>
<summary>💡 Hint</summary>
Koin pertama masuk -> Koin pertama diambil di bawah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Queue.**
Masuk dari atas (belakang), keluar dari bawah (depan). Ini adalah aliran FIFO.
</details>

### Soal #37: Pez Dispenser (Stack)
Kamu mengisi Pez dengan permen: [1.Jeruk, 2.Apel, 3.Anggur].
Manakah permen yang akan dimakan oleh adikmu pertama kali saat ia menekan kepala Pez?
A. Jeruk
B. Apel
C. Anggur
D. Semua bersamaan

<details>
<summary>💡 Hint</summary>
LIFO: Permen terakhir yang dimasukkan (Anggur) berada di posisi paling atas.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Anggur.**
Permen terakhir yang masuk adalah yang pertama kali keluar.
</details>

### Soal #38: Penumpang Eskalator (Queue)
Lima orang (1, 2, 3, 4, 5) naik eskalator berurutan. Di tengah jalan, orang nomor 3 pingsan dan harus digendong keluar eskalator oleh petugas di samping.
Siapakah orang yang sampai di lantai atas tepat setelah orang nomor 2?
A. Orang nomor 1
B. Orang nomor 4
C. Orang nomor 3
D. Orang nomor 5

<details>
<summary>💡 Hint</summary>
Jika data di tengah antrian hilang, data di belakangnya tetap maju sesuai urutan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Orang nomor 4.**
Urutan: [1, 2, 3, 4, 5]. Nomor 3 hilang, sisa: [1, 2, 4, 5]. Maka setelah nomor 2 adalah nomor 4.
</details>

### Soal #39: Panggilan Telepon Beruntun (Stack)
Kamu sedang menelepon Ibu, lalu ada panggilan masuk dari Guru yang mendesak, kamu menjawabnya. Saat bicara dengan Guru, Ayah menelepon.
Urutan penyelesaian telepon agar kamu bisa kembali bicara dengan Ibu adalah...
A. Selesaikan Guru -> Selesaikan Ayah -> Lanjut Ibu
B. Selesaikan Ayah -> Selesaikan Guru -> Lanjut Ibu
C. Selesaikan Ibu -> Selesaikan Guru -> Selesaikan Ayah
D. Matikan semua

<details>
<summary>💡 Hint</summary>
Ini seperti Interupsi/Rekursi. Panggilan terbaru (terakhir) harus diselesaikan dulu untuk kembali ke panggilan sebelumnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Selesaikan Ayah -> Selesaikan Guru -> Lanjut Ibu.**
Panggilan terakhir (Ayah) berada di puncak "Stack" perhatianmu.
</details>

### Soal #40: Logika Kontrol Game
Karakter melompat JIKA (Tombol Spasi) **AND** (Diatas Tanah **OR** Punya Skill Double Jump).
Karakter tidak di atas tanah, dan tidak punya skill Double Jump. Tapi player menekan Spasi.
Apakah karakter melompat?
A. Ya
B. Tidak
C. Karakter jatuh
D. Game Error

<details>
<summary>💡 Hint</summary>
(Spasi = T) AND (Tanah = F OR Skill = F).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
(F OR F) menghasilkan SALAH. BENAR AND SALAH menghasilkan SALAH.
</details>

---

## 🚀 Kesimpulan untuk OSN-K
*   **Logika** digunakan untuk memfilter data dan membuat percabangan (IF-ELSE).
*   **Queue** digunakan untuk mensimulasikan proses yang adil (siapa cepat dia dapat).
*   **Stack** digunakan untuk proses yang mendalam (seperti tombol 'Back' di browser atau fitur 'Undo').

---
[< Materi Sebelumnya: Algorithm Design](./05-algorithm-design.md) | [Materi Selanjutnya: Graf Sederhana](./07-graf-sederhana.md)
[< Kembali ke Beranda Materi](../README.md)
