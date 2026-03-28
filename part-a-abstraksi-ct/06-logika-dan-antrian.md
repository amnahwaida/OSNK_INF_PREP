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

> **Tips OSN-K**: Jika ada kurung, kerjakan yang di dalam kurung dulu. Urutan pengerjaan standar: **NOT** -> **AND** -> **OR**.

---

## 🚶 Bagian 2: Antrian (Queue) & Tumpukan (Stack)

Dalam informatika, kita menyebut ini sebagai **Struktur Data**.

### 1. Antrian (Queue) - FIFO
**Analogi Tambahan:**
*   **Customer Service**: Orang yang ambil nomor antrian duluan pasti dipanggil duluan.
*   **E-Commerce Flash Sale**: Pesanan yang masuk server sepermili-detik lebih cepat akan diproses duluan sebelum stok habis.
*   **Chat Message**: Pesan WhatsApp yang kamu kirim jam 08.00 akan muncul di atas pesan jam 08.01.

### 2. Tumpukan (Stack) - LIFO
**Analogi Tambahan:**
*   **Browser History (Tombol Back)**: Halaman terakhir yang kamu buka adalah yang muncul pertama kali saat kamu klik "Back".
*   **Aplikasi Edit Foto (Undo)**: Filter terakhir yang kamu pasang adalah yang akan dihapus pertama kali saat kamu klik "Undo".
*   **Tumpukan Kursi**: Kursi yang ditaruh paling atas saat merapikan adalah yang pertama diambil saat akan digunakan.

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

---

## 🚀 Kesimpulan untuk OSN-K
*   **Logika** digunakan untuk memfilter data dan membuat percabangan (IF-ELSE).
*   **Queue** digunakan untuk mensimulasikan proses yang adil (siapa cepat dia dapat).
*   **Stack** digunakan untuk proses yang mendalam (seperti tombol 'Back' di browser atau fitur 'Undo').

---
[< Materi Sebelumnya: Algorithm Design](./05-algorithm-design.md) | [Materi Selanjutnya: Graf Sederhana](./07-graf-sederhana.md)
[< Kembali ke Beranda Materi](../README.md)
