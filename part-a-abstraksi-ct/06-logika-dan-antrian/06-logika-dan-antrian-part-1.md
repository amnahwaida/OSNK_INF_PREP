🔙 **Kembali ke Materi:** [Materi 06 Logika Dan Antrian](../06-logika-dan-antrian.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 06. Logika & Antrian - Latihan Soal Bagian 1 (1-50)

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

### Soal #41: Logika Berjenjang (3 Variabel)
Lampu menyala JIKA (A AND B) OR (C). 
Jika A = Benar, B = Salah, C = Benar. Status lampu adalah?
A. Nyala
B. Mati
C. Berkedip
D. Error

<details>
<summary>💡 Hint</summary>
Kerjakan (A AND B) dulu, lalu hasilkan OR dengan C.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Nyala.**
(Benar AND Salah) = Salah. Lalu (Salah OR Benar) = **Benar**.
</details>

### Soal #42: Antrian Supermarket (Enqueue 3, Dequeue 1)
Antrian Kasir: [Andi, Budi, Citra]. 
Masuk Doni, Eka, Fani. Lalu Andi selesai membayar. 
Siapa yang berada tepat di belakang Budi?
A. Andi
B. Citra
C. Doni
D. Eka

<details>
<summary>💡 Hint</summary>
Urutan tidak berubah, hanya orang paling depan yang keluar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Citra.**
Antrian menjadi [Budi, Citra, Doni, Eka, Fani]. Di belakang Budi tetap Citra.
</details>

### Soal #43: Tumpukan Pakaian (Stack)
Tumpukan: [Bawah: Kaos, Kemeja, Jaket :Atas].
Kamu menaruh Sweater, lalu mengambil 2 pakaian. Pakaian apa yang tersisa?
A. Kaos dan Kemeja
B. Jaket dan Sweater
C. Kaos dan Jaket
D. Kemeja dan Sweater

<details>
<summary>💡 Hint</summary>
LIFO: Sweater dan Jaket adalah yang paling atas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kaos dan Kemeja.**
Tumpukan: [Kaos, Kemeja, Jaket, Sweater]. Ambil 2: Sweater dan Jaket keluar.
</details>

### Soal #44: Logika XOR Majemuk
Hasil dari (1 XOR 0) XOR 1 adalah... (1 = Benar, 0 = Salah)
A. 1
B. 0
C. 2
D. Error

<details>
<summary>💡 Hint</summary>
(1 XOR 0) = 1. Lalu 1 XOR 1 = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0.**
XOR bernilai 0 jika kedua input SAMA.
</details>

### Soal #45: Antrian Pesan Antar (Queue)
Pesanan: [Pizza, Burger, Sushi].
Tiba-tiba Burger dibatalkan oleh pembeli. Urutan antar sekarang adalah...
A. [Pizza, Sushi]
B. [Sushi, Pizza]
C. [Burger, Pizza]
D. [Sushi]

<details>
<summary>💡 Hint</summary>
Data di tengah dihapus, sisanya tetap sesuai urutan kedatangan.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Pizza, Sushi].**
Pizza tetap pertama, Sushi tetap setelah Pizza.
</details>

### Soal #46: Logika NAND (3 Input)
NAND bernilai SALAH hanya jika SEMUA input BENAR.
A=T, B=T, C=F. Maka (A AND B AND C) NAND T adalah...
A. Benar
B. Salah
C. Kosong
D. Error

<details>
<summary>💡 Hint</summary>
Cek hasil AND dulu, baru NAND-kan dengan T.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
(T AND T AND F) = F. Lalu F NAND T = NOT (F AND T) = NOT F = **Benar**.
</details>

### Soal #47: Stack "Undo" Gambar
Aksi: [Gambar Garis, Warnai Merah, Hapus Garis].
Undo 1 kali akan mengembalikan kondisi ke...
A. Gambar Garis saja
B. Gambar Garis dan Warnai Merah
C. Kosong
D. Warnai Merah saja

<details>
<summary>💡 Hint</summary>
Aksi terakhir (Hapus Garis) dibatalkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gambar Garis dan Warnai Merah.**
Membatalkan penghapusan berarti mengembalikan apa yang ada sebelum dihapus.
</details>

### Soal #48: Antrian Mobil di Lampu Merah
Mobil: [M1, M2, M3, M4].
Lampu hijau menyala cukup lama untuk 3 mobil. Mobil mana yang masih tertahan?
A. M1
B. M2
C. M3
D. M4

<details>
<summary>💡 Hint</summary>
FIFO: Mobil pertama yang sampai lampu merah yang jalan duluan.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. M4.**
M1, M2, dan M3 berhasil lewat. M4 harus menunggu lampu hijau berikutnya.
</details>

### Soal #49: Logika NOR (A OR B)
Pernyataan: "Tidak (Kaya ATAU Pintar)" identik dengan...
A. Tidak Kaya DAN Tidak Pintar
B. Tidak Kaya ATAU Tidak Pintar
C. Kaya DAN Pintar
D. Miskin ATAU Bodoh

<details>
<summary>💡 Hint</summary>
De Morgan: NOT (A OR B) = (NOT A) AND (NOT B).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Tidak Kaya DAN Tidak Pintar.**
Keduanya harus bernilai salah agar pernyataan awal benar.
</details>

### Soal #50: Stack Simbol Matematika
Ekspresi: $3 + (4 \times 5)$.
Dalam komputer, kurung `(` dimasukkan ke Stack. Kapan kurung `(` tersebut dikeluarkan (Pop)?
A. Saat angka 4 muncul.
B. Saat simbol `\times` muncul.
C. Saat kurung tutup `)` muncul.
D. Saat hasil akhir didapat.

<details>
<summary>💡 Hint</summary>
Stack digunakan untuk menjaga pasangan simbol.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Saat kurung tutup ) muncul.**
Kurung tutup adalah tanda untuk menyelesaikan apa yang ada di dalam kurung tersebut.
</details>

### Soal #51: Logika "Izin Keluar"
Siswa boleh keluar JIKA (Istirahat=T) **OR** (Sakit=T **AND** Ada Surat Dokter=T).
Data: Istirahat=F, Sakit=T, Ada Surat Dokter=F. Bolehkah keluar?
A. Boleh
B. Tidak Boleh
C. Tanya Guru
D. Tergantung Satpam

<details>
<summary>💡 Hint</summary>
Sakit saja tidak cukup tanpa surat doktor (karena AND).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Boleh.**
(T AND F) = F. Lalu (F OR F) = F.
</details>

### Soal #52: Antrian Tiket Ludes
Antrian: [A, B, C, D, E]. Tiket sisa 2.
Siapakah orang pertama yang TIDAK kebagian tiket?
A. B
B. C
C. D
D. E

<details>
<summary>💡 Hint</summary>
A dan B dilayani, sisanya gagal.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. C.**
A = Tiket 1, B = Tiket 2. C adalah orang urutan ke-3 yang sudah kehabisan stok.
</details>

### Soal #53: Stack Piring Pecah
Tumpukan: [P1, P2, P3].
Kamu mengambil P3, tapi terpeleset dan P3 pecah. Lalu kamu mengambil P2.
Urutan piring yang masih utuh di tanganmu (dari bawah ke atas) adalah?
A. P3, P2
B. P1, P2
C. P2 saja
D. Kosong

<details>
<summary>💡 Hint</summary>
P3 sudah tidak ada (pecah). P1 masih di meja.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. P2 saja.**
P3 pecah, P1 belum diambil. Hanya P2 yang berhasil diambil dan utuh.
</details>

### Soal #54: Logika XOR pada Lampu 3 Saklar
Lampu menyala JIKA jumlah saklar yang "ON" adalah GANJIL.
Saklar: A=ON, B=ON, C=OFF. Apakah lampu menyala?
A. Ya
B. Tidak
C. Berkedip
D. Error

<details>
<summary>💡 Hint</summary>
Hitung jumlah yang ON. 1+1+0 = 2.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
Jumlah saklar ON adalah 2 (Genap). Sesuai aturan XOR majemuk, hasilnya SALAH.
</details>

### Soal #55: Antrian Kereta Api (Masuk vs Keluar)
Gerbong: [G1, G2, G3].
Kereta masuk ke stasiun buntu (harus mundur untuk keluar). Prinsip apa yang terjadi?
A. FIFO (Queue)
B. LIFO (Stack)
C. Random
D. Circular

<details>
<summary>💡 Hint</summary>
Gerbong terakhir yang masuk akan menjadi yang pertama keluar saat mundur.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. LIFO (Stack).**
Stasiun buntu memaksa urutan keluar menjadi kebalikan dari urutan masuk.
</details>

### Soal #56: Logika NAND Identitas
Pernyataan (A NAND A) sama dengan...
A. A
B. NOT A
C. Benar
D. Salah

<details>
<summary>💡 Hint</summary>
Cek jika A=T: (T AND T) = T, NOT T = F. Cek jika A=F: (F AND F) = F, NOT F = T.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. NOT A.**
Hasilnya selalu kebalikan dari nilai A itu sendiri.
</details>

### Soal #57: Stack Undo-Redo
Aksi: [A, B]. 
1. Undo -> [A].
2. Redo -> [A, B].
3. Undo -> [A].
4. Tambah C -> [A, C].
Apa yang terjadi jika sekarang dilakukan Redo?
A. Menjadi [A, C, B]
B. Menjadi [A, B]
C. Tidak terjadi apa-apa (Redo hilang)
D. Menjadi [A, C, C]

<details>
<summary>💡 Hint</summary>
Menambah aksi baru setelah Undo akan menghapus sejarah Redo yang lama.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Tidak terjadi apa-apa.**
Dalam kebanyakan aplikasi, menulis aksi baru (C) akan memutus jalur Redo ke aksi lama (B).
</details>

### Soal #58: Antrian Download (Prioritas)
Antrian biasa: [File_Kecil, File_Besar].
Tiba-tiba ada "File_Penting" ditandai sebagai VIP (langsung ke urutan depan).
Urutan download sekarang adalah...
A. [File_Penting, File_Kecil, File_Besar]
B. [File_Kecil, File_Penting, File_Besar]
C. [File_Kecil, File_Besar, File_Penting]
D. [File_Penting, File_Besar]

<details>
<summary>💡 Hint</summary>
Priority Queue menempatkan data penting di paling depan antrian.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [File_Penting, File_Kecil, File_Besar].**
Data VIP memotong antrian dan menjadi yang pertama dilayani.
</details>

### Soal #59: Logika "Syarat Masuk Bioskop"
Masuk JIKA (Umur >= 17) **OR** (Bawa Orang Tua=T).
Andi umur 15, bawa orang tua. Apakah boleh masuk?
A. Boleh
B. Tidak Boleh
C. Harus bayar lebih
D. Tunggu 2 tahun lagi

<details>
<summary>💡 Hint</summary>
Logika OR: Salah satu syarat terpenuhi sudah cukup.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Boleh.**
Meskipun umurnya kurang, tapi syarat "Bawa Orang Tua" bernilai BENAR.
</details>

### Soal #60: Stack "History" Browser 
Buka: FB -> IG -> WA.
Kamu klik "Back" 2 kali, lalu klik "Youtube". 
Sekarang isi tumpukan historymu (dari awal) adalah...
A. [FB, IG, WA, Youtube]
B. [FB, Youtube]
C. [FB, IG, Youtube]
D. [Youtube]

<details>
<summary>💡 Hint</summary>
Back membuang WA dan IG. Youtube ditambahkan di atas FB.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. [FB, Youtube].**
Back 2x: IG dan WA hilang. Kamu kembali di FB. Lalu buka Youtube: [FB, Youtube].
</details>

### Soal #61: Logika "Lampu Otomatis"
Lampu OFF JIKA (Hari Terang) **XOR** (Saklar Rusak).
Data: Hari Terang=T, Saklar Baik=F. Apakah lampu menyala (ON)?
A. Ya (Lampu ON)
B. Tidak (Lampu OFF)
C. Berkedip
D. Meledak

<details>
<summary>💡 Hint</summary>
T XOR F = T (Output Lampu OFF adalah T). Jadi Lampu OFF?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak (Lampu OFF).**
Hasil XOR adalah BENAR, yang berarti kondisi "Lampu OFF" adalah benar.
</details>

### Soal #62: Antrian Toko Roti
Antrian: [A, B, C].
Toko Roti tutup sementara untuk istirahat. Saat tutup, datang D dan E mengantri.
Setelah buka, C memutuskan pulang (keuar antrian). Siapa yang dilayani pertama?
A. A
B. D
C. B
D. E

<details>
<summary>💡 Hint</summary>
A tetap di depan karena datang paling awal.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. A.**
Meskipun toko tutup atau ada yang pulang, urutan depan (A) tidak berubah selama A tetap di sana.
</details>

### Soal #63: Stack Wadah CD
Wadah CD (tabung): [Bawah: Game, Musik, Film :Atas].
Kamu ambil Film, lalu masukkan CD Foto. Jika kamu ambil CD lagi, CD apa yang kamu dapat?
A. Game
B. Musik
C. Foto
D. Kosong

<details>
<summary>�� Hint</summary>
Foto adalah yang terakhir dimasukkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Foto.**
Tumpukan: [Game, Musik] -> +Foto: [Game, Musik, Foto]. Teratas adalah Foto.
</details>
---
[< Kembali ke Indeks Materi](../06-logika-dan-antrian.md) |  | [Bagian Selanjutnya >](./06-logika-dan-antrian-part-2.md)
