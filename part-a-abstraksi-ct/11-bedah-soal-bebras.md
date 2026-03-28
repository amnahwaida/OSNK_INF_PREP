# 11. Bedah Soal: Eksekusi Tipe Bebras (Soal Cerita Bergambar)

> *"Lho Kak, di silabus OSN-K Informatika Part A itu katanya tes 'Cerita Bergambar' ala Bebras. Kok daritadi kita malah pusing belajar Teori Graf, Kombinatorika, sama Himpunan sih? Nggak nyambung dong?"*

**Eits, kata siapa nggak nyambung?** 🛑

Di level SD atau SMP, kalian mungkin bisa ngerjain soal Bebras murni pakai *feeling* atau *trial-and-error*. Tapi di level OSN-K SMA, soalnya sengaja didesain untuk **membuat kepala kalian meledak kalau masih pakai cara nebak-nebak manual!**

Semua modul Teori Logika Matematika yang baru saja kita pelajari (Modul 1 s.d. 10) adalah **SENJATA RAHASIA TAK KASAT MATA** yang dipakai oleh anak-anak peraih medali untuk menghempaskan soal Bebras dalam 1 menit.

Mari kita bongkar bagaimana teori-teori "membosankan" tadi berubah jadi pedang sakti saat diadukan dengan soal Bebras.

---

## 🐹 1. Soal Labirin Pak Dengklek (Wujud Asli: Teori Graf)

**Visual Soal Bebras:**
Biasanya disajikan gambar labirin ruwet atau jalan tikus dari desa A ke desa B. Disertakan jebakan, jalan buntu, atau jembatan putus. Pertanyaannya: *"Berapa langkah tercepat?"* atau *"Apakah mungkin selamat sampai tujuan?"*

**Kesalahan Pemula:**
Si Anak Polos akan mulai mencoret-coret kertas, menarik garis belok-belok pakai pensil. Kalau labirinnya ukuran 10x10 sih gampang. Gimana kalau labirin ukuran 100x100 kotak? Waktu 2.5 jam habis cuma buat narik garis!

**Solusi Hacker OSN-K (Pakai Ilmu Modul 7: Graf Sederhana):**
Anak olimpiade tahu bahwa **Labirin adalah sebentuk GRAF bertipe Grid (Kotak-Kotak)**.
1. Setiap kotak ubin di lantai adalah **Titi/Node/Vertex**.
2. Garis antar kotak (kalau nggak terhalang tembok) adalah **Sisi/Edge**.
3. Dari sini, mereka nggak akan nebak garis manual. Mereka akan pakai insting algoritma `BFS (Breadth-First Search)` di pikiran mereka: menyemprot air / tinta ke segala arah secara bersamaan level-demi-level untuk nyari jalan terpendek tak terbantahkan.
4. Atau, kalau pertanyaannya "Bisakah kita mengunjungi semua desa tanpa melewati jalan yang sama 2 kali?" $\rightarrow$ Mereka langsung pakai rumus **Euler Path** (cek derajat ganjil-genap tiap desa)!

*(Tuh kan, soal gambar desa-desa aslinya mah soal Graf!)*

---

## 🔠 2. Soal Mesin Sandi Huruf Pak Dengklek (Wujud Asli: Kombinatorika / PHP)

**Visual Soal Bebras:**
"Pak Dengklek punya alat yang bisa mengubah huruf menjadi simbol. `B E B E K` berubah jadi `[Segitiga] [Kotak] [Segitiga] [Kotak] [Bintang]`. Kalau Pak Dengklek memasukkan kata `K E R A`, bentuk apa yang mungkin keluar?" (Ini soal asli silabus Puspresnas Lho!).

**Kesalahan Pemula:**
Menebak-nebak oh segitiga itu artinya huruf apa ya? Terus kok Bintang artinya huruf apa. Fokusnya ada pada *menghafal bentuk per bentuk*.

**Solusi Hacker OSN-K (Pakai Ilmu Modul 3: Pattern Recognition & Kombinatorika):**
Pola! Cukup lihat strukturnya.
- Kata `BEBEK` punya susunan karakter: (Anggap aja Karakter ke-1,2,3,4,5).
- Karakter 1 KEMBAR dengan Karakter 3 (Yaitu Huruf B).
- Karakter 2 KEMBAR dengan Karakter 4 (Yaitu Huruf E).
- Berarti output mesin pastilah simbol berformat: `X - Y - X - Y - Z`. Coba cek opsi pilihan ganda yang punya kembaran di indeks yang sama!
- Lalu pertanyaan "Ada berapa banyak kemungkinan simbol palsu yang bisa diketik oleh monyet *Pigeonhole*?" $\rightarrow$ Langsung pakai jurus Modul 9: *Pigeonhole Principle*.

---

## 👗 3. Soal Campur Gabung Kombinasi Pak Pakaian (Wujud Asli: Himpunan)

**Visual Soal Bebras:**
"Di desa Bebek, 30 bebek memakai Topi Merah, 20 memakai Syal Kuning, dan 15 Bebek suka pakai Kacamata Hitam. Bebek yang suka pakai Topi Merah DAN Syal Kuning tapi BENCI kacamata hitam ada..."

**Kesalahan Pemula:**
Menggambar bebek satu-satu di kertas buram, atau nebak-nebak angka ditambahkan kurangi seenak hati. Ujung-ujungnya minus.

**Solusi Hacker OSN-K (Pakai Ilmu Modul 8: Teori Himpunan):**
Gak usah pusingin bebeknya! Langsung ambil penggaris dan gambar **Diagnosis 3 Lingkaran Diagram Venn**.
- Lingkaran A = Topi
- Lingkaran B = Syal
- Lingkaran C = Kacamata
Mulailah mengisi dari **udel paling dalam (irisan ketiganya)**, lalu sikat keluar dengan rumus nyanyi *Maju-Mundur-Maju* (Inklusi-Eksklusi). Bebek nggak penting, yang penting adalah operasi `Selisih (A - C)` di himpunannya!

---

## 🎯 Inti Pelajaran Part A

Jadi, jangan tertipu kalau nanti di soal OSN-K kamu disodorkan soal Cerita yang ada gambar lucunya. **Tanya pada dirimu sendiri: *"Ini bajunya doang yang Bebras, aslinya ini lagi disuruh ngitung Graf, Kombinasi, atau Himpunan sih?"***.

Begitu kamu tahu "oh ini aslinya soal Kombinatorika (Slot Kosong)", maka dalam 30 detik kamu pasti bisa mencoret opsi jebakan dan mendapatkan jawaban pastinya.

Selamat! Kamu sudah menyelesaikan seluruh amunisi teori **Part A (Abstraksi Berpikir Komputasional)**. Di tahap ini, insting membaca pola dan pemodelan matematis-mu sudah setajam silet.

Ambil nafas panjang, sedia secangkir kopi, dan... 

**Mari kita bersiap memasuki wilayah medan perang sesungguhnya:** 
**⏩ [Bagian B: Pemecahan Masalah Komputasional (Studi Kasus Koding)](../../part-b-pemecahan-masalah/README.md)** *(Akan menjadi folder berikutnya!)*

---
[< Materi Sebelumnya: Model Matematis & Deret Pola Bilangan](./10-deret-dan-pola-bilangan.md)
[< Kembali ke Beranda Materi](../README.md)
