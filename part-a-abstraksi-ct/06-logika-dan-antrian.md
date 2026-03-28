# 06. Logika Dasar dan Antrian (Logic & Queue)

> "Komputer tidak pernah bingung, ia hanya mengikuti logika yang kamu berikan. Jika hasilnya salah, periksa logikanya, bukan komputernya."

Selamat! Kamu sudah mempelajari 4 pilar utama Computational Thinking. Sekarang, kita akan masuk ke dua konsep teknis yang sangat sering muncul di soal OSN-K Informatika: **Logika Boolean** dan **Struktur Data Antrian (Queue)**.

---

## 🧠 Bagian 1: Logika Boolean (Gerbang Logika)

Dalam dunia komputer, segala sesuatu hanya bernilai **TRUE** (Benar/1) atau **FALSE** (Salah/0). Logika ini digunakan untuk mengambil keputusan.

### 1. Operator Logika Dasar

Ada 3 operator utama yang wajib kamu hafal:

| Operator | Simbol | Penjelasan Sederhana |
| :--- | :--- | :--- |
| **AND** | `DAN` | Bernilai BENAR hanya jika **SEMUA** syarat terpenuhi. |
| **OR** | `ATAU` | Bernilai BENAR jika **SALAH SATU** saja syarat terpenuhi. |
| **NOT** | `TIDAK` | Membalikkan nilai (Benar jadi Salah, Salah jadi Benar). |

### 2. Analogi Kehidupan Nyata

*   **AND**: Kamu boleh jajan JIKA (Punya Uang **DAN** Ada Penjual). Jika salah satu tidak ada, kamu tidak jajan.
*   **OR**: Kamu bisa pergi ke sekolah JIKA (Naik Bus **ATAU** Naik Motor). Jika punya salah satu, kamu bisa berangkat.
*   **NOT**: Status "Lapar" adalah **TIDAK** " Kenyang".

### 3. Tabel Kebenaran (Truth Table)

| A | B | A AND B | A OR B | NOT A |
| :--- | :--- | :--- | :--- | :--- |
| Benar | Benar | **Benar** | **Benar** | Salah |
| Benar | Salah | Salah | **Benar** | Salah |
| Salah | Benar | Salah | **Benar** | **Benar** |
| Salah | Salah | Salah | Salah | **Benar** |

---

## 🚶 Bagian 2: Antrian (Queue)

**Queue** (Antrian) adalah cara mengatur data atau benda dengan aturan **FIFO (First In, First Out)**.

### 1. Prinsip FIFO
Artinya: **"Siapa yang pertama datang, dia yang pertama keluar/dilayani."**

### 2. Contoh dalam Keseharian:
*   **Antrian Kasir**: Orang yang pertama berdiri di depan kasir akan dilayani lebih dulu.
*   **Printer**: Dokumen yang kamu klik "Print" pertama kali akan dicetak lebih dulu.
*   **Antrian Tol**: Mobil yang masuk gerbang tol duluan akan keluar duluan.

### 3. Operasi pada Antrian:
*   **Enqueue**: Menambah orang/data ke baris belakang.
*   **Dequeue**: Mengambil orang/data dari baris paling depan (selesai dilayani).

---

## 📚 Bagian 3: Tumpukan (Stack) - Sahabat Antrian

Seringkali di soal OSN-K, Antrian (Queue) dibandingkan dengan **Stack** (Tumpukan).

*   **Prinsip Stack**: **LIFO (Last In, First Out)**.
*   **Artinya**: "Siapa yang terakhir datang, dia yang pertama keluar."
*   **Analogi**: Tumpukan piring. Piring yang kamu taruh paling atas (terakhir) adalah yang akan kamu ambil duluan.

---

## ❓ Latihan Soal Logika & Antrian

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

### Soal #06: Operasi Campuran
Hasil dari (BENAR **AND** SALAH) **OR** (NOT SALAH) adalah...
A. Benar
B. Salah
C. Kosong
D. Error

<details>
<summary>💡 Hint</summary>
Kerjakan dalam kurung dulu, lalu NOT, baru OR.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Benar.**
1. (Benar AND Salah) = **Salah**
2. (NOT Salah) = **Benar**
3. Salah OR Benar = **Benar**
</details>

### Soal #07: Antrian Printer Sekolah
Printer sedang mencetak: Tugas_MTK, Tugas_Indo.
Kemudian Guru memasukkan Tugas_IPA. Saat Tugas_MTK sedang dicetak, Listrik mati dan Printer mereset antrian (semua yang belum dicetak hilang).
Apa yang harus dimasukkan kembali ke antrian agar urutannya tetap benar?
A. Tugas_MTK saja
B. Tugas_Indo dan Tugas_IPA
C. Tugas_IPA saja
D. Semua tugas (MTK, Indo, IPA)

<details>
<summary>💡 Hint</summary>
Tugas_MTK adalah yang pertama (sedang diproses), sisanya masih menunggu di Queue.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tugas_Indo dan Tugas_IPA.**
Tugas_MTK dianggap sudah "keluar" dari antrian karena sedang diproses. Yang hilang saat reset adalah data yang masih mengantri.
</details>

### Soal #08: Stack "Undo" di Notepad
Kamu mengetik: "Halo", lalu "Dunia". Tombol "Undo" (Ctrl+Z) bekerja dengan prinsip Stack.
Jika kamu menekan HP "Undo" satu kali, kata apa yang hilang?
A. Halo
B. Dunia
C. Semuanya
D. Tidak ada yang hilang

<details>
<summary>💡 Hint</summary>
Aksi terakhir adalah yang pertama dibatalkan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dunia.**
Ketik "Halo" (masuk stack), ketik "Dunia" (masuk stack paling atas). Undo mengambil data paling atas (LIFO).
</details>

### Soal #09: Logika XOR (Exclusive OR)
XOR bernilai BENAR jika **HANYA SALAH SATU** dari A atau B yang benar (tidak boleh keduanya benar).
Jika A = Benar dan B = Benar, maka A XOR B adalah...
A. Benar
B. Salah
C. Mungkin
D. Selalu Benar

<details>
<summary>💡 Hint</summary>
XOR benci kesamaan. Jika sama-sama Benar atau sama-masing Salah, hasilnya SALAH.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Salah.**
Karena keduanya Benar, maka syarat "hanya salah satu" tidak terpenuhi.
</details>

### Soal #10: Antrian Masuk Kelas
Siswa masuk kelas: Andi, Budi, Citra, Doni.
Ibu Guru memanggil 2 orang pertama untuk maju ke depan. Lalu masuk Siswa baru bernama Eka.
Siapakah orang ke-2 di dalam antrian sekarang?
A. Citra
B. Doni
C. Eka
D. Budi

<details>
<summary>💡 Hint</summary>
Queue: (A, B, C, D). Dequeue 2x. Enqueue(E).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Doni.**
1. Awal: (Andi, Budi, Citra, Doni)
2. Panggil 2: Andi dan Budi keluar. Sisa: (Citra, Doni)
3. Eka masuk: (Citra, Doni, Eka)
Orang ke-1 adalah Citra, orang ke-2 adalah Doni.
</details>

---

## 🚀 Kesimpulan untuk OSN-K
*   **Logika** digunakan untuk memfilter data dan membuat percabangan (IF-ELSE).
*   **Queue** digunakan untuk mensimulasikan proses yang adil (siapa cepat dia dapat).
*   **Stack** digunakan untuk proses yang mendalam (seperti tombol 'Back' di browser atau fitur 'Undo').

---
[< Materi Sebelumnya: Algorithm Design](./05-algorithm-design.md) | [Materi Selanjutnya: Graf Sederhana](./07-graf-sederhana.md)
[< Kembali ke Beranda Materi](../README.md)
