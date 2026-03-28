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
| **OR** | `\|\|` / `ATAU` | Bernilai BENAR jika **SALAH SATU** saja syarat terpenuhi. |
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

## 📝 Daftar Isi Latihan (200 Soal)

Untuk menjaga performa halaman, 200 soal latihan telah dibagi menjadi 4 bagian berikut:

1.  **[Bagian 1 (Soal 1 - 50)](./06-logika-dan-antrian/06-logika-dan-antrian-part-1.md)** - Dasar Logika & Dasar Queue/Stack.
2.  **[Bagian 2 (Soal 51 - 100)](./06-logika-dan-antrian/06-logika-dan-antrian-part-2.md)** - Logika XOR/NAND & Variasi Antrean Dunia Nyata.
3.  **[Bagian 3 (Soal 101 - 150)](./06-logika-dan-antrian/06-logika-dan-antrian-part-3.md)** - Logika De Morgan & Kompleksitas Antrean.
4.  **[Bagian 4 (Soal 151 - 200)](./06-logika-dan-antrian/06-logika-dan-antrian-part-4.md)** - Kasus Gabungan & Pemecahan Masalah Informatika.

---

## 🚀 Kesimpulan untuk OSN-K
*   **Logika** digunakan untuk memfilter data dan membuat percabangan (IF-ELSE).
*   **Queue** digunakan untuk mensimulasikan proses yang adil (siapa cepat dia dapat).
*   **Stack** digunakan untuk proses yang mendalam (seperti tombol 'Back' di browser atau fitur 'Undo').

---
[< Materi Sebelumnya: Algorithm Design](./05-algorithm-design.md) | [Materi Selanjutnya: Graf Sederhana](./07-graf-sederhana.md)
[< Kembali ke Beranda Materi](../README.md)
