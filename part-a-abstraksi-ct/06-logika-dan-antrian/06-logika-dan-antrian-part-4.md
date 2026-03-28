# 06. Logika & Antrian - Latihan Soal Bagian 4 (151-200)

### Soal #164: Logika NAND (NOT AND)
$(F \text{ NAND } F) \text{ NAND } T = \dots$
A. Benar
B. Salah
C. Kosong
D. Error

<details>
<summary>💡 Hint</summary>
(F NAND F) = T. T NAND T = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
</details>

### Soal #165: Antrian "Download" (Parallel)
Komputer mengunduh 3 file [F1, F2, F3] bersamaan. 
Koneksi stabil. Jika F1 sizenya 10MB, F2 50MB, F3 5MB. 
Siapa yang SELESAI pertama kali (Enqueue ke Galeri)?
A. F1
B. F2
C. F3
D. F1 dan F3

<details>
<summary>💡 Hint</summary>
File paling kecil (F3) selesai paling cepat.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. F3.**
</details>

### Soal #166: Logika "Login Admin"
Bisa login jika: (Username="admin") **AND** (Password="123"). 
Username="Admin" (huruf besar), Password="123". (Case Sensitive). Dapat login?
A. Bisa
B. Tidak Bisa
C. Bisa jika lupa password
D. Error

<details>
<summary>💡 Hint</summary>
"admin" != "Admin" dalam sistem informatika.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Bisa.**
</details>

### Soal #167: Stack "Tumpukan Surat"
Surat datang: [Dari Bank, Dari Sekolah, Dari Teman]. 
Kamu mengambil surat Dari Sekolah tanpa mengambil surat Dari Teman. 
Apakah mungkin dalam prinsip Stack murni?
A. Mungkin
B. Tidak Mungkin
C. Mungkin jika suratnya tipis
D. Tergantung Pak Pos

<details>
<summary>💡 Hint</summary>
Stack hanya boleh mengambil yang teratas (Dari Teman).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Mungkin.**
</details>

### Soal #168: Logika "Lampu Sensor Gerak"
Lampu Nyala JIKA (Ada Gerak) **AND** (NOT Ada Cahaya Matahari). 
Siang hari terik, ada orang menari di depan sensor. Lampu Nyala?
A. Ya
B. Tidak
C. Berkedip
D. Rusak

<details>
<summary>💡 Hint</summary>
(T) AND (NOT T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #169: Antrian "Bioskop"
Tiket sisa 5. Antrean ada 10 orang. 
Orang ke-6 di antrean akan...
A. Dapat tiket
B. Tidak dapat tiket
C. Dapat setengah harga
D. Jadi admin

<details>
<summary>💡 Hint</summary>
Tiket 1-5 untuk orang 1-5.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak dapat tiket.**
</details>

### Soal #170: Stack "Baju dalam Lemari"
Tumpukan baju: [Bawah: Celana, Kaos, Jaket :Atas]. 
Kamu mengambil Jaket, lalu menaruh Kemeja. 
Urutan baju dari atas sekarang adalah...
A. Jaket, Kaos
B. Kemeja, Kaos, Celana
C. Celana, Kaos, Kemeja
D. Kaos, Kemeja

<details>
<summary>💡 Hint</summary>
Jaket dibuang. Kemeja masuk di atas Kaos.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kemeja, Kaos, Celana.**
</details>

### Soal #171: Logika "Vending Machine"
Minuman keluar JIKA (Uang Cukup) **AND** (Stok Ada). 
Uang 10rb, Harga 5rb, Stok Habis. Keluar minuman?
A. Keluar
B. Tidak Keluar (Uang dikembalikan)
C. Keluar air saja
D. Meledak

<details>
<summary>💡 Hint</summary>
(T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Keluar.**
</details>

### Soal #172: Antrian "Print Task"
Urutan: [A, B, C]. 
Printer kehabisan kertas saat sedang mencetak B. 
Setelah kertas diisi, printer melanjutkan pekerjaan siapa?
A. A
B. B
C. C
D. Tugas Baru

<details>
<summary>💡 Hint</summary>
B belum selesai diproses (Dequeue belum komplit).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B.**
</details>

### Soal #173: Stack "Koin Tip"
Pelanggan 1 kasih 500, Pelanggan 2 kasih 1000. Kamu tumpuk. 
Kamu butuh kembalian 500. Kamu ambil koin teratas. 
Dapat koin berapa?
A. 500
B. 1000
C. 1500
D. Kosong

<details>
<summary>💡 Hint</summary>
Terakhir masuk adalah 1000.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1000.**
</details>

### Soal #174: Logika "Deteksi Banjir"
Bahaya JIKA (Air > 100cm) **OR** (Debit > 500). 
Air 50cm, Debit 600. Status?
A. Bahaya
B. Aman
C. Waspada
D. Siaga

<details>
<summary>💡 Hint</summary>
Logika OR: Salah satu terpenuhi = Bahaya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bahaya.**
</details>

### Soal #175: Antrian "Masuk Kelas"
Guru: "Anak-anak, masuk satu-satu!". 
Budi mendorong Iwan agar masuk duluan. 
Iwan sekarang berada di posisi...
A. Paling belakang
B. Paling depan
C. Luar kelas
D. Admin

<details>
<summary>💡 Hint</summary>
Masuk duluan = Depan antrean.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Paling depan.**
</details>

### Soal #176: Logika "Sinyal HP"
Internet jalan JIKA (Indosat **OR** Telkomsel) **AND** (Punya Kuota). 
Indosat ada, Telkomsel Tidak, Kuota Ada. Jalan?
A. Ya
B. Tidak
C. Kadang
D. Error

<details>
<summary>💡 Hint</summary>
(T OR F) AND (T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
</details>

### Soal #177: Stack "Kamera"
Filter: [BlackWhite, Sepia, Blur]. 
Kamu membuang Blur, lalu membuang Sepia. 
Filter mana yang masih aktif?
A. BlackWhite
B. Sepia
C. Blur
D. Tidak ada

<details>
<summary>💡 Hint</summary>
LIFO: Menghapus 2 teratas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. BlackWhite.**
</details>

### Soal #178: Logika "Mesin Cuci"
Berputar JIKA (Pintu Tertutup) **AND** (Tombol Start Ditekan) **AND** (Berat < 7kg). 
Pintu tutup, Start OK, Berat 10kg. Berputar?
A. Ya
B. Tidak
C. Air meluap
D. Meledak

<details>
<summary>💡 Hint</summary>
(T) AND (T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #179: Antrian "Chat"
Status: [Pending, Sent, Delivered]. 
Laila mengirim pesan P1 lalu P2. 
Jika P2 masuk ke HP lawan bicara duluan tapi P1 belum (karena sinyal), apakah HP lawan bicara akan mengurutkan ulang?
A. Ya, sistem akan menunggu P1 agar urut.
B. Tidak, tampil apa adanya.
C. Tergantung aplikasi.
D. HP meledak.

<details>
<summary>💡 Hint</summary>
Aplikasi chat biasanya punya "Sequencing" (Queue) agar percakapan masuk akal.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya, sistem menunggu P1.**
</details>

### Soal #180: Stack "Buku yang Dibaca"
Buku: [A, B, C]. 
Malam 1 baca A. Malam 2 baca B. Malam 3 teringat sesuatu di A dan membacanya lagi. 
Kini "Terakhir Dibaca" adalah...
A. A
B. B
C. C
D. Semua

<details>
<summary>💡 Hint</summary>
Baru saja diakses = Menjadi teratas.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. A.**
</details>

### Soal #181: Logika "Lampu Solar"
Charge JIKA (Terang) **AND** (Baterai < 100%). 
Terang sekali, Baterai 100%. Apakah men-charge?
A. Ya
B. Tidak
C. Baterai meledak
D. Lampu nyala

<details>
<summary>💡 Hint</summary>
(T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #182: Antrian "E-ticket"
Daftar: [Andi, Budi]. 
Budi membatalkan pesanan. Caca mendaftar. 
Urutan antrean sekarang:
A. [Andi, Caca]
B. [Caca, Andi]
C. [Budi, Caca]
D. [Andi, Budi, Caca]

<details>
<summary>💡 Hint</summary>
Budi dihapus, Caca masuk di belakang.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Andi, Caca].**
</details>

### Soal #183: Stack "Piring di Rak"
Tumpukan 6 piring. Kamu ambil 3 piring teratas. 
Lalu kamu taruh 1 piring baru. Berapa jumlah piring sekarang?
A. 4
B. 3
C. 7
D. 2

<details>
<summary>💡 Hint</summary>
6 - 3 + 1 = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 4.**
</details>

### Soal #184: Logika "Password & Sidik Jari"
Masuk JIKA (Password Benar) **OR** (Sidik Jari Cocok). 
Password Salah, Sidik Jari Cocok. Bisa masuk?
A. Bisa
B. Tidak Bisa
C. Harus ke Polisi
D. Bayar denda

<details>
<summary>💡 Hint</summary>
Logika OR: Salah satu Benar = Benar.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Bisa.**
</details>

### Soal #185: Antrian "Kasir"
Antrian: [A, B]. 
Kasir: "Maaf, mesin rusak, pindah ke kasir sebelah!". 
Di kasir sebelah sudah ada C. Di mana posisi A dan B?
A. Di depan C.
B. Di belakang C.
C. Pulang saja.
D. Jadi Kasir.

<details>
<summary>💡 Hint</summary>
FIFO: C sudah ada di sana lebih dulu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di belakang C.**
</details>

### Soal #186: Logika "Sensor Parkir"
Bunyi JIKA (Jarak < 50cm) **AND** (Gigi Mundur). 
Gigi Mundur, Jarak 100cm. Bunyi?
A. Ya
B. Tidak
C. Pelan
D. Rusak

<details>
<summary>💡 Hint</summary>
(F) AND (T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #187: Stack "Kartu Nama"
Tumpukan: [A, B, C]. 
Ambil 2 kartu. Siapakah yang tersisa di tumpukan?
A. C
B. B
C. A
D. Kosong

<details>
<summary>💡 Hint</summary>
LIFO: Keluar C, lalu B. Sisa A.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. A.**
</details>

### Soal #188: Logika "Sistem Siram Tanaman"
Siram JIKA (Tanah Kering) **OR** (Jam 17:00). 
Tanah Basah, Jam 17:00. Apakah menyiram?
A. Ya
B. Tidak
C. Banjir
D. Rusak

<details>
<summary>💡 Hint</summary>
(F OR T) = T.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
</details>

### Soal #189: Antrian "Struk Belanja"
Struk keluar: [Belanja1, Belanja2]. 
Printer macet. Struk Belanja 2 keluar setengah potong. 
Petugas mencetak ulang Struk Belanja 2. 
Urutan struk yang utuh adalah...
A. [Belanja1, Belanja2]
B. [Belanja2, Belanja1]
C. [Belanja1]
D. [Belanja2]

<details>
<summary>💡 Hint</summary>
FIFO: Urutan kejadian tetap Belanja1 lalu Belanja2.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Andi, Belanja2].**
</details>

### Soal #190: Stack "Batu Kali"
Susun Batu: [Dasar: Besar, Menengah, Kecil :Puncak]. 
Ambil Kecil, ganti dengan Ranting. 
Apa yang ada di Puncak tumpukan?
A. Kecil
B. Ranting
C. Menengah
D. Besar

<details>
<summary>💡 Hint</summary>
Ranting ditaruh paling akhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ranting.**
</details>

### Soal #191: Logika "Sensor Malam"
Lampu Jalan Jalan JIKA (TIDAK Siang). 
Siang = Benar. Apakah Lampu Jalan?
A. Ya
B. Tidak
C. Berkedip
D. Rusak

<details>
<summary>💡 Hint</summary>
TIDAK (T) = F.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #192: Antrian "Tiket Kereta"
Sisa Kursi: 10. Antrean 15 orang. 
Orang nomor 10 di antrean akan...
A. Dapat kursi
B. Berdiri
C. Pulang
D. Gagal

<details>
<summary>💡 Hint</summary>
Orang 1-10 dapat kursi.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Dapat kursi.**
</details>

### Soal #193: Stack "Kotak Sepatu"
Tumpukan kotak: [S1, S2, S3]. 
Budi ingin mengambil S1 karena mau kondangan. 
Minimal berapa kotak yang harus dipindah?
A. 1
B. 2
C. 3
D. 0

<details>
<summary>💡 Hint</summary>
Pindahkan S3, lalu pindahkan S2.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2.**
</details>

### Soal #194: Logika "Otomatisasi Pintu"
Kunci Terbuka JIKA (Admin Datang) **AND** (NOT Ada Tamu Asing). 
Admin Datang, Ada Tamu Asing. Kunci Terbuka?
A. Ya
B. Tidak
C. Tergantung Tamu
D. Lari

<details>
<summary>💡 Hint</summary>
(T) AND (NOT T) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #195: Antrian "Dokter Gigi"
Selesai: [Pasien A]. Antre: [Pasien B, Pasien C]. 
Masuk Pasien D. Pasien B dipanggil masuk. 
Siapa yang paling belakang di antrean sekarang?
A. C
B. D
C. B
D. A

<details>
<summary>💡 Hint</summary>
D adalah yang terakhir mendaftar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. D.**
</details>

### Soal #196: Logika "Filter Instagram"
Wajah mulus JIKA (Filter ON) **AND** (Cahaya Terang). 
Filter ON, Cahaya Redup. Wajah mulus?
A. Ya
B. Tidak
C. Berbayang
D. Error

<details>
<summary>💡 Hint</summary>
(T) AND (F) = ?
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak.**
</details>

### Soal #197: Stack "Tumpukan CD Balap"
Isi: [Game1, Game2, Game3]. 
Ambil Game3, lalu masukkan Game4, lalu ambil 1. 
Game apa yang kamu pegang?
A. Game1
B. Game2
C. Game3
D. Game4

<details>
<summary>💡 Hint</summary>
[G1, G2] -> +G4: [G1, G2, G4] -> Ambil 1: G4.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Game4.**
</details>

### Soal #198: Logika "Kelayakan Makan"
Makan JIKA (Lapar) **OR** (Makanan Enak). 
Tidak Lapar, Makanan Enak. Makan?
A. Ya
B. Tidak
C. Nanti
D. Buat Besok

<details>
<summary>💡 Hint</summary>
(F OR T) = T.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya.**
</details>

### Soal #199: Antrian "Pintu Masuk Sekolah"
Antrean: [A, B, C]. 
Pak Guru: "Yang pakai sepatu hitam duluan!". 
Hanya C yang pakai sepatu hitam. Urutan masuk menjadi:
A. [C, A, B]
B. [A, B, C]
C. [C, B, A]
D. [B, A, C]

<details>
<summary>💡 Hint</summary>
C memotong antrean (Priority Queue).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [C, A, B].**
</details>

### Soal #200: Refleksi Akhir
Computational Thinking mengajarkan kita bahwa masalah sulit bisa diselesaikan dengan...
A. Logika yang tepat dan pengorganisasian data yang baik.
B. Membeli robot mahal.
C. Bertanya pada teman saat ujian.
D. Berdoa saja.

<details>
<summary>💡 Hint</summary>
Pilihlah jawaban yang paling bijak.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Logika yang tepat dan pengorganisasian data.**
Selamat! Kamu sudah menyelesaikan 200 soal Logika dan Antrian!
</details>
---
[< Kembali ke Indeks Materi](../06-logika-dan-antrian.md) | [< Bagian Sebelumnya](./06-logika-dan-antrian-part-3.md) | 
