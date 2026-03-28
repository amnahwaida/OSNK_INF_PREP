# 05. Algorithm Design - Bagian 5 (Soal 201-250)

[< Bagian 4 (151-200)](05-algorithm-design-part-4.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 6 (251-300) >](05-algorithm-design-part-6.md)

---
### Soal #201: Algoritma "Checklist Pagi"
1. Bangun tidur.
2. JIKA mandi >= 10 menit, MAKA sarapan di jalan.
3. JIKA mandi < 10 menit, MAKA sarapan di meja.
Andi mandi 10 menit tepat. Dimana dia sarapan?
A. Di meja.
B. Di jalan.
C. Tidak jadi sarapan.
D. Di kamar mandi.

<details>
<summary>💡 Hint</summary>
Syarat sarapan di jalan adalah mandi >= 10. Angka 10 termasuk ke dalam syarat tersebut.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Di jalan.**
Logika inklusif (dengan tanda sama dengan) memasukkan nilai batas ke kategori atas.
</details>

### Soal #202: Algoritma "Sorting Nama" (Quick Sort Concept)
Kamu memilih satu nama (Pivot) "Budi". Lalu semua nama yang abjadnya sebelum 'B' dipindah ke kiri, dan setelah 'B' ke kanan.
Ini adalah langkah dasar dari algoritma...
A. Bubble Sort
B. Quick Sort
C. Selection Sort
D. Shuffle

<details>
<summary>💡 Hint</summary>
Membagi data berdasarkan satu titik acuan disebut pemisahan (*Partitioning*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Quick Sort.**
Salah satu algoritma pengurutan tercepat yang paling populer digunakan.
</details>

### Soal #203: Algoritma "Router - Hop Count"
Packet data menyeberang antar router. Setiap kali pindah router, status 'Hop' berkurang 1. Jika 'Hop' mencapai 0 tetapi belum sampai tujuan, paket tersebut akan dibuang. Tujuannya?
A. Biar paketnya istirahat.
B. Mencegah paket berputar selamanya di jaringan (Infinite Loop protection).
C. Biar internet makin lambat.
D. Biar router tidak kepanasan.

<details>
<summary>💡 Hint</summary>
Istilahnya adalah TTL (*Time to Live*). Gunanya untuk memberhentikan data yang tersesat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah infinite loop.**
Mekanisme penghentian paksa untuk menjaga kebersihan trafik jaringan.
</details>

### Soal #204: Algoritma "Cek Tahun Kabisat" (Urutan Benar)
1. JIKA habis dibagi 400, MAKA Kabisat.
2. JIKA TIDAK, namun habis dibagi 100, MAKA Bukan Kabisat.
3. JIKA TIDAK, namun habis dibagi 4, MAKA Kabisat.
Apa status tahun **1900**?
A. Kabisat.
B. Bukan Kabisat.
C. Tergantung bulan Februari.
D. Error algoritma.

<details>
<summary>💡 Hint</summary>
1900 tidak habis dibagi 400 (Lanjut ke langkah 2). 1900 habis dibagi 100 (Selesai).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bukan Kabisat.**
Aturan pengecualian tahun abad yang tidak habis dibagi 400.
</details>

### Soal #205: Algoritma "Kapasitas Server"
"Satu server kuat melayani 100 orang". Saat ini orang ke-101 masuk. Apa respon sistem cerdas?
A. Menendang orang pertama keluar.
B. Mengalihkan (Redirect) orang ke-101 ke server cadangan.
C. Server langsung terbakar.
D. Meminta semua orang pulang.

<details>
<summary>💡 Hint</summary>
Ini disebut strategi *Load Balancing* (Penyeimbang Beban).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengalihkan ke server lain.**
Algoritma pembagian beban kerja agar sistem tidak tumbang (*Crash*).
</details>

### Soal #206: Algoritma "Antivirus - Heuristic"
Antivirus tidak kenal virus baru ini, tapi virus ini melakukan tindakan "Hapus Semua File Sistem". Antivirus langsung memblokirnya.
Ini adalah algoritma pendeteksian berdasarkan...
A. Nama virus.
B. Perilaku (Behavior Algorithm).
C. Ukuran file.
D. Tanggal download.

<details>
<summary>💡 Hint</summary>
Mengenali bahaya dari ciri-ciri tindakan tak lazim, bukan dari identitas tertulis.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Perilaku.**
Algoritma cerdas yang bisa mendeteksi ancaman baru yang belum terdaftar di database.
</details>

### Soal #207: Algoritma "Ganti Rugi"
Pesan belanja: Rp 100rb. Barang rusak. Toko mengembalikan (Refund) 120% dari harga. Berapa uang yang diterima?
A. Rp 100.000
B. Rp 120.000
C. Rp 20.000
D. Rp 1.200.000

<details>
<summary>💡 Hint</summary>
00.000 \times 1.2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 120.000.**
Perhitungan sanksi atau insentif dalam algoritma kompensasi.
</details>

### Soal #208: Algoritma "Smart Home - Lampu"
1. JIKA hari sudah gelap (dari sensor cahaya).
2. DAN JIKA ada orang di ruangan (dari sensor infra merah).
3. MAKA nyalakan lampu.
Jika hari sudah gelap tapi ruangan kosong, apa yang terjadi?
A. Lampu menyala.
B. Lampu mati.
C. Sensor rusak.
D. Lampu kedap-kedip.

<details>
<summary>💡 Hint</summary>
Gerbang logika AND: Salah satu False membuat seluruh hasil False.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Lampu mati.**
Algoritma penghematan energi otomatis yang efektif.
</details>

### Soal #209: Algoritma "Pencarian Paling Cepat" (Google Index)
Kenapa Google bisa menampilkan 1 miliar hasil pencarian hanya dalam 0,5 detik?
A. Karena Google memakai komputer super.
B. Karena Google sudah memproses & mengurutkan (Index) seluruh web sebelum kamu bertanya.
C. Karena Google menebak-nebak saja.
D. Karena internet sangat cepat.

<details>
<summary>💡 Hint</summary>
Google tidak mencari satu-persatu di internet saat kamu ketik; mereka sudah punya "Daftar Isi" raksasa yang siap dibaca.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengindeksan (Indexing).**
Teknik optimasi pencarian tingkat tinggi untuk menangani data skala besar.
</details>

### Soal #210: Algoritma "Membuat Pola Barisan"
Ditetapkan barisan: 1, 3, 6, 10, ... Apa angka selanjutnya?
A. 13
B. 15
C. 14
D. 20

<details>
<summary>💡 Hint</summary>
+2=3$. +3=6$. +4=10$. Berarti 0+\dots? = \dots?$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 15**
Pola bilangan segitiga. Algoritma harus mampu mendeteksi kenaikan pola yang dinamis ($+2, +3, +4, +5$).
</details>
### Soal #211: Algoritma "Insertion Sort" (Analogi Main Kartu)
Kamu memegang kartu 5, 2, 8. Kamu ambil 2, sisipkan di sebelum 5. Lalu ambil 8, biarkan di tempat.
Proses menyisipkan data ke posisi yang benar satu-persatu ini disebut...
A. Insertion Sort.
B. Bubble Sort.
C. Selection Sort.
D. Quick Sort.

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana kamu merapikan kartu di tanganmu secara natural.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Insertion Sort.**
Algoritma ini sangat efisien untuk data yang jumlahnya sedikit atau sudah hampir terurut.
</details>

### Soal #212: Algoritma "Penghapusan Akun"
"Jika akun dihapus, MAKA hapus semua postingan akun tersebut dari database."
Apa yang terjadi jika algoritma ini lupa dijalankan (Bug)?
A. Akun tetap ada.
B. Postingan menjadi "Yatim Piatu" (Orphaned Data) yang tetap ada meski pemilik akun sudah tidak ada.
C. Database meledak.
D. User jadi senang.

<details>
<summary>💡 Hint</summary>
Data yang tidak memiliki referensi pemilik disebut data sampah yang membebani memori.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Postingan tetap ada.**
Inilah pentingnya algoritma penghapusan yang menyeluruh (*Cascading Delete*).
</details>

### Soal #213: Algoritma "Smart Chatbot"
User: "Halo". Bot: "Halo juga!".
User: "Jam berapa?". Bot: "Jam 12:00".
User: "xyz123". Bot: "Maaf, saya tidak mengerti".
Instruksi terakhir (xyz123) menunjukkan algoritma...
A. Error sistem.
B. Default Response (Respon Standar) untuk input yang tidak ada di database.
C. Bot sedang lelah.
D. Bot minta dipuji.

<details>
<summary>💡 Hint</summary>
Setiap algoritma harus memiliki penanganan untuk input yang tidak terduga (*Unrecognized input*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Default Response.**
Menjaga interaksi tetap elegan meskipun sistem tidak punya jawaban spesifik.
</details>

### Soal #214: Algoritma "Diskon Bertingkat"
"Diskon 10%, jika pakai kartu member diskon lagi 5% dari harga setelah diskon pertama."
Harga: Rp 100.000. Berapa harga akhirnya?
A. Rp 85.000
B. Rp 85.500
C. Rp 90.000
D. Rp 15.000

<details>
<summary>💡 Hint</summary>
Langkah 1: 00.000 - 10.000 = 90.000$. Langkah 2: 0.000 - (5\% \times 90.000) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 85.500.**
Perhitungan diskon majemuk yang sering digunakan dalam modul kasir.
</details>

### Soal #215: Algoritma "Cek Password" (Brute Force Protection)
"Setelah 3 kali salah, berikan jeda 1 menit sebelum bisa mencoba lagi."
Apa fungsi algoritma jeda ini?
A. Biar user istirahat.
B. Menghambat algoritma "Brute Force" (penebak otomatis) agar tidak bisa mencoba jutaan kali dalam sekejap.
C. Biar server dingin.
D. Biar user ingat passwordnya.

<details>
<summary>💡 Hint</summary>
Mempersulit peretas dengan membatasi kecepatan percobaan (*Rate Limiting*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menghambat Brute Force.**
Keamanan algoritma login seringkali menggunakan faktor waktu sebagai pelindung tambahan.
</details>

### Soal #216: Algoritma "Shortest Task First" (Optimasi)
Tugas A (2 jam), Tugas B (1 jam), Tugas C (3 jam).
Agar total waktu antrean (tunggu) semua orang minimal, urutan mana yang benar?
A. C - A - B
B. B - A - C
C. A - B - C
D. Sembarang

<details>
<summary>💡 Hint</summary>
Selesaikan yang paling cepat dulu agar orang lain tidak menunggu lama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. B - A - C.**
B (1 jam) + A (2 jam) + C (3 jam). Inilah algoritma penjadwalan CPU paling dasar.
</details>

### Soal #217: Algoritma "Search" (Wildcard)
Kamu mencari file dengan mengetik "Tugas*". Apa yang ditemukan sistem?
A. Hanya file bernama "Tugas".
B. Semua file yang diawali kata "Tugas" (misal: "TugasMTK", "TugasIPA").
C. File bergambar bintang.
D. Tidak ada hasil.

<details>
<summary>💡 Hint</summary>
Tanda bintang (*) berarti "Boleh apa saja setelah ini".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Diawali kata "Tugas".**
Pencarian fleksibel (*Wildcard Search*) menggunakan simbol untuk mewakili karakter acak.
</details>

### Soal #218: Algoritma "Kompresi Gambar" (Lossy)
Kenapa foto WhatsApp kualitasnya lebih rendah dari foto di Galeri?
A. WhatsApp sengaja merusak.
B. Algoritma kompresi WhatsApp membuang detail warna yang kurang terlihat mata manusia agar ukuran file kecil (Hemat Kuota).
C. HP kamu rusak.
D. Jaringan lemah.

<details>
<summary>💡 Hint</summary>
Abstraksi data gambar dengan membuang piksel yang dianggap tidak signifikan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kompresi data.**
Inilah *Lossy Compression*, algoritma yang menukar kualitas dengan efisiensi pengiriman.
</details>

### Soal #219: Algoritma "Urutan Rank Kelas" (Tie-Breaker)
Ali dan Budi punya nilai rata-rata sama (90). Ali absen 0 hari, Budi absen 2 hari.
Sistem: "Jika rata-rata sama, pilih yang absennya lebih sedikit".
Siapa juara 1?
A. Ali
B. Budi
C. Keduanya juara 1.
D. Tidak ada juara.

<details>
<summary>💡 Hint</summary>
Kriteria kedua (Absensi) digunakan sebagai pemutus seri (*Tie-Breaker*).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ali.**
Algoritma sorting tingkat lanjut seringkali memiliki beberapa kriteria berurutan.
</details>

### Soal #220: Algoritma "Loop Matematika" (Increment)
 = 0$. Ulangi:  = N + 2$. Ulangi sampai  > 10$.
Apa angka terakhir yang disimpan di 0
A. 10
B. 12
C. 11
D. 2

<details>
<summary>💡 Hint</summary>
0, 2, 4, 6, 8, 10 ... apakah 10 sudah > 10? Belum. Lanjut sekali lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 12.**
Loop berhenti segera setelah kondisi 2 > 10$ terpenuhi.
</details>

### Soal #221: Algoritma "Keliling Persegi" (Input Check)
Rumus:  \times 4$. Input: himBHs5$. Apa output yang benar bagi program yang aman?
A. -20
B. 20
C. Tampilkan pesan: "Input harus positif!".
D. 0

<details>
<summary>💡 Hint</summary>
Panjang benda tidak mungkin bernilai negatif.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Pesan Error.**
Pengecekan validitas input (*Sanitization*) mencegah algoritma menghasilkan data yang mustahil.
</details>

### Soal #222: Algoritma "Searching" (Index)
Daftar: [Apel, Jeruk, Mangga]. Di komputer, "Apel" berada di index nomor...
A. 1
B. 0
C. A
D. 3

<details>
<summary>💡 Hint</summary>
Mayoritas bahasa pemrograman modern memulai urutan (Array Index) dari angka 0.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0**
Urutan data komputer: 0, 1, 2, dst. Penting bagi pemahaman dasar CT.
</details>

### Soal #223: Algoritma "Block Teman"
"Jika Budi diblokir oleh Anda, maka Budi tidak bisa melihat postingan Anda."
Jika Budi membuat akun baru (palsu), apakah dia bisa melihat postingan Anda?
A. Tidak bisa, sistem pintar.
B. Bisa, karena identitas digitalnya (User ID) sudah berbeda di mata algoritma.
C. Tergantung settingan HP.
D. Postingan Anda hilang.

<details>
<summary>💡 Hint</summary>
Blokir biasanya berbasis pada Identitas Akun, bukan Identitas Fisik orangnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bisa.**
Kelemahan algoritma blokir sederhana yang tidak mengenali perangkat atau alamat IP.
</details>

### Soal #224: Algoritma "Pesan Makan" (Delivery Time)
Waktu kirim = (Jarak x 2 menit) + Waktu Masak (10 menit).
Jarak: 5 km. Berapa lama totalnya?
A. 10 menit
B. 20 menit
C. 25 menit
D. 30 menit

<details>
<summary>💡 Hint</summary>
 + 10 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 20 menit.**
Data input jarak diolah oleh rumus estimasi waktu (ETA algorithm).
</details>

### Soal #225: Algoritma "Sortir Berdasarkan Tanggal"
File A (1 Januari), File B (30 Desember tahun lalu), File C (1 Februari).
Urutan dari yang **Terbaru** (Newest to Oldest):
A. C - A - B
B. A - B - C
C. B - A - C
D. C - B - A

<details>
<summary>💡 Hint</summary>
Urutkan dari bulan yang paling jauh angkanya di kalender tahun ini.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. C (Februari) - A (Januari) - B (Desember lalu).**
Inilah logika pengurutan kronologis terbalik (Reverse Chronological).
</details>

### Soal #226: Algoritma "Kalkulator Pajak"
"Pajak 10% jika penghasilan > Rp 4jt. Jika tidak, pajak 0%."
Penghasilan Budi: Rp 4.000.000 tepat. Berapa pajaknya?
A. Rp 400.000
B. Rp 0
C. Rp 40.000
D. Serikhlasnya.

<details>
<summary>💡 Hint</summary>
Syaratnya adalah "lebih besar dari". Angka 4jt tidak lebih besar dari 4jt.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 0.**
Logika "Strictly Greater Than" (>) mengecualikan nilai batas itu sendiri.
</details>

### Soal #227: Algoritma "Game - Damage Calculation"
"Damage = Serangan - Pertahanan Musuh".
Serangan kamu: 50. Pertahanan Musuh: 70. Apa Damage-nya?
A. -20
B. 0 (Minimal damage biasanya tidak boleh negatif).
C. 50
D. Musuhnya kalah.

<details>
<summary>💡 Hint</summary>
Algoritma game biasanya menambahkan pengecekan: "Jika hasil < 0, maka set jadi 0".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 0**
Logika pencegahan nilai negatif dalam simulasi sistem realitas fisik.
</details>

### Soal #228: Algoritma "Sorting Gelembung" (Bubble Sort Ascending)
Daftar: [5, 4, 3]. Setelah satu putaran (Round 1) penuh, angka mana yang pasti di posisi paling benar?
A. Angka 5 di paling belakang.
B. Angka 3 di paling depan.
C. Semua sudah rapi.
D. Angka 4 di tengah.

<details>
<summary>💡 Hint</summary>
Bubble sort mendorong angka terbesar ke ujung kanan "seperti gelembung".
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Angka 5 di paling belakang.**
Setiap satu putaran, satu angka terbesar akan "mengapung" sampai ke posisi akhir yang seharusnya.
</details>

### Soal #229: Algoritma "Antivirus - Scan" (Partial Scan)
Kenapa scan folder tertentu lebih cepat daripada scan seluruh komputer?
A. Karena antivirus malas.
B. Karena jumlah data (Input Size) yang diproses lebih sedikit, sehingga langkah pengulangan pencarian lebih singkat.
C. Folder itu isinya virus semua.
D. Komputernya takut.

<details>
<summary>💡 Hint</summary>
Efisien waktu berbanding lurus dengan jumlah data yang harus diperiksa (*Linear Time Complexity*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Input Size lebih sedikit.**
Contoh nyata bagaimana abstraksi area pencarian menghemat waktu eksekusi.
</details>

### Soal #230: Algoritma "Mencari Nama" (Binary Search Trick)
Kamu mencari nama "Zulkifli" di buku telepon. Haruskah kamu mulai dari tengah?
A. Ya, selalu mulai dari tengah itu paling aman (Teori Binary Search).
B. Tidak, secara cerdas kita bisa langsung buka bagian belakang (Interpolation Search).
C. Mulai dari depan saja.
D. Tanya orang.

<details>
<summary>💡 Hint</summary>
Manusia sering menggunakan data "Kira-kira letaknya dimana" untuk memotong langkah lebih banyak lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Langsung ke belakang.**
Inilah optimasi algoritma pencarian jika kita tahu distribusi datanya (Z pasti di belakang).
</details>

### Soal #231: Algoritma "Cek Koneksi" (Ping)
Waktu ping: 500 ms. Artinya...
A. Internet super cepat.
B. Sinyal dikirim dan dibalas dalam waktu 0,5 detik (Cukup lambat untuk game online).
C. Provider kamu bangkrut.
D. Download film selesai dalam 0,5 detik.

<details>
<summary>💡 Hint</summary>
Ping mengukur waktu pulang-pergi paket data dalam milidetik (1000 ms = 1 detik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Waktu kirim-balas 0,5 detik.**
Parameter efisiensi latensi dalam algoritma jaringan.
</details>

### Soal #232: Algoritma "Matematika Bunga"
"Bunga 1% per bulan dari sisa uang". Uang: Rp 1.000.000. Setelah 1 bulan, berapa uangnya?
A. Rp 1.001.000
B. Rp 1.010.000
C. Rp 1.100.000
D. Rp 2.000.000

<details>
<summary>💡 Hint</summary>
\% \text{ dari } 1 \text{ juta} = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 1.010.000.**
\% \times 1.000.000 = 10.000$. Penambahan saldo otomatis oleh sistem perbankan.
</details>

### Soal #233: Algoritma "Lupa Password" (Security)
"Masukkan kode yang dikirim ke HP Anda". Ini merupakan pertahanan terhadap...
A. Orang yang tidak punya HP.
B. Orang yang tahu password Anda tapi tidak memegang HP Anda (Two-Factor Authentication).
C. Provider sinyal.
D. Iklan.

<details>
<summary>💡 Hint</summary>
Menambah lapisan keamanan di luar sekadar "apa yang dihafal" (Password).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Two-Factor Authentication (2FA).**
Algoritma keamanan yang menggabungkan dua kunci berbeda untuk akses akun.
</details>

### Soal #234: Algoritma "Sorting Warna"
Daftar: Merah, Putih, Biru. Urutkan berdasarkan "Urutan Warna Pelangi" (Me-Ji-Ku-Hi-Bi-Ni-U).
A. Merah - Biru - Putih
B. Merah - Putih - Biru
C. Putih - Merah - Biru
D. Biru - Merah - Putih

<details>
<summary>💡 Hint</summary>
Putih tidak ada di pelangi, biasanya ditaruh paling akhir (Default). Merah (Me) paling depan, Biru (Bi) setelahnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Merah - Biru - Putih.**
Pengurutan data berdasarkan standar referensi tertentu (Custom Sort).
</details>

### Soal #235: Algoritma "Auto-Brightness"
"Jika cahaya lingkungan terang, naikkan kecerahan layar agar terbaca".
Siapa yang memberikan **Input** terang/gelap pada algoritma ini?
A. Mata user.
B. Sensor cahaya (Ambient Light Sensor) di dekat kamera depan.
C. Aplikasi penghemat baterai.
D. Google.

<details>
<summary>💡 Hint</summary>
Hardware pendeteksi rangsang cahaya di perangkat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor cahaya.**
Penerjemahan kondisi fisis menjadi data digital untuk diproses algoritma.
</details>

### Soal #236: Algoritma "Mode Gelap" (Dark Mode)
Kenapa sistem mengganti background putih jadi hitam?
A. Agar tulisan tidak terbaca.
B. Menghemat daya baterai (pada layar OLED) dan mengurangi kelelahan mata.
C. Biar HP-nya terlihat mahal.
D. Biar user cepat tidur.

<details>
<summary>💡 Hint</summary>
Pada layar tertentu, piksel warna hitam berarti lampu piksel tersebut mati (0 daya).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hemat daya & nyaman di mata.**
Optimasi antarmuka berdasarkan efisiensi energi hardware.
</details>

### Soal #237: Algoritma "Search" (Autocomplete)
Baru ketik "A-L-G-O", sistem sudah menyarankan "ALGORITMA". Ini bekerja dengan mencari...
A. Kata yang paling banyak dicari orang lain yang diawali huruf tersebut.
B. Kata yang paling kamu suka.
C. Nama temanmu.
D. Kata yang paling pendek.

<details>
<summary>💡 Hint</summary>
Memanfaatkan database frekuensi pencarian populer.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Kata populer.**
Contoh nyata dari algoritma prediksi berbasis data besar (*Big Data*).
</details>

### Soal #238: Algoritma "Filter Chat" (Bukan Kata Kasar)
"Jika pesan mengandung 'MENANG', ganti jadi 'JUARA'".
Pesan: "SAYA MENANG LOMBA". Apa hasilnya?
A. SAYA JUARA LOMBA.
B. SAYA MENANG LOMBA.
C. SAYA *** LOMBA.
D. PESAN DIHAPUS.

<details>
<summary>💡 Hint</summary>
Algoritma cari dan ganti (*Replace*) mengganti per-kata secara spesifik.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. SAYA JUARA LOMBA.**
Fungsi dasar manipulasi teks dalam sistem otomasi pesan.
</details>

### Soal #239: Algoritma "Matematika Jarak"
Kamu jalan 10 langkah ke Depan, lalu 4 langkah ke Belakang. Dimana posisi akhirmu dari titik awal?
A. 14 langkah di depan.
B. 6 langkah di depan.
C. 10 langkah di belakang.
D. 4 langkah di depan.

<details>
<summary>💡 Hint</summary>
0 - 4 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 6 langkah di depan.**
Logika posisi relatif dalam sistem koordinat sederhana.
</details>

### Soal #240: Algoritma "Antrean GoFood - Status"
1. Pesanan Diterima.
2. Driver Menuju Resto.
3. Driver Memesan.
4. Driver Mengantar.
5. Selesai.
Kenapa status ini penting?
A. Biar user tidak bosan.
B. Menunjukkan transparansi proses (Feedback) agar user tahu algoritma berjalan di tahap mana.
C. Biar drivernya bangga.
D. Biar makanannya makin enak.

<details>
<summary>💡 Hint</summary>
Setiap sistem harus memberikan informasi status saat menjalankan proses yang memakan waktu lama.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Transparansi proses.**
Bagian dari "Sistem Informasi" untuk menjaga kepercayaan pengguna.
### Soal #241: Algoritma "Family Tree" (Tree Structure)
Dalam silsilah keluarga, Ayah berada di posisi atas, Anak di bawah. Struktur data ini disebut...
A. Linear List.
B. Tree (Pohon).
C. Grid.
D. Loop.

<details>
<summary>💡 Hint</summary>
Memiliki satu akar (Root) yang bercabang ke bawah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tree.**
Struktur hirarkis yang digunakan komputer untuk mengelola folder dan file.
</details>

### Soal #242: Algoritma "Sorting Usia"
Guru ingin membagi kelas jadi kelompok beranggotakan 2 orang dengan selisih usia paling sedikit. Algoritma apa yang harus guru lakukan pertama kali?
A. Memasangkan secara acak.
B. Mengurutkan (Sorting) seluruh siswa berdasarkan tanggal lahir.
C. Menghitung jumlah siswa.
D. Bertanya siapa yang mau berkelompok.

<details>
<summary>💡 Hint</summary>
Dengan data yang sudah terurut, dua orang yang paling mirip usianya pasti duduk berdekatan di daftar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sorting tanggal lahir.**
Penyelesaian masalah optimasi menggunakan data terurut.
</details>

### Soal #243: Algoritma "Chat - Read Receipt"
"Jika pesan sudah dibuka oleh penerima, ubah status 'Terkirim' menjadi 'Dibaca'".
Ini adalah contoh mekanisme...
A. Input user.
B. Event Trigger (Pemicu berdasarkan aksi tertentu).
C. Error aplikasi.
D. Penghapusan data.

<details>
<summary>💡 Hint</summary>
Perubahan status terjadi otomatis segera setelah "Event" (pesan dibuka) terdeteksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Event Trigger.**
Bagian dinamis dari desain algoritma aplikasi komunikasi.
</details>

### Soal #244: Algoritma "RAM vs Storage"
Data di RAM (Memori) akan hilang jika listrik mati, sedangkan di Storage (Harddisk) tidak.
Manakah algoritma yang **Paling Berisiko** jika tidak ada fitur Auto-save?
A. Algoritma pengetikan di layar (data disimpan di RAM).
B. Algoritma pemindahan file ke flashdisk.
C. Algoritma pencarian Google.
D. Algoritma ganti wallpaper.

<details>
<summary>💡 Hint</summary>
Data yang sedang diketik biasanya hanya mengambang di memori sementara.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Hasil mengetik.**
Pentingnya memindahkan data dari yang mudah menguap (*Volatile*) ke yang permanen.
</details>

### Soal #245: Algoritma "Nilai KKM"
"Lulus jika (Nilai >= 75) **DAN** (Kehadiran >= 80%)".
Status: Nilai 100, Kehadiran 70%. Hasil?
A. Lulus
B. Tidak Lulus
C. Lulus Bersyarat
D. Tanya Wakasek

<details>
<summary>💡 Hint</summary>
Logika AND menuntut ketaatan pada **semua** aturan tanpa terkecuali.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lulus.**
Meskipun nilai sempurna, syarat kehadiran tidak terpenuhi (False).
</details>

### Soal #246: Algoritma "Kalkulator Sederhana" (Round)
Hasil asli: 7.9. Kamu ingin output dibulatkan ke bawah (*Floor*). Hasilnya?
A. 8
B. 7
C. 7.5
D. 0

<details>
<summary>💡 Hint</summary>
Pembulatan ke bawah mengabaikan desimal berapapun besarnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 7.**
Operasi pembulatan sering digunakan untuk indeks array atau pembagian jumlah barang.
</details>

### Soal #247: Algoritma "Cari Nama Unik"
Daftar: [Ani, Budi, Ani, Cici]. Algoritma penghapusan duplikat akan menghasilkan...
A. [Ani, Budi, Cici]
B. [Ani, Budi, Ani, Cici]
C. [Budi, Cici]
D. [Ani]

<details>
<summary>💡 Hint</summary>
Data yang sama hanya boleh muncul satu kali saja di hasil akhir.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. [Ani, Budi, Cici].**
Aplikasi pembersihan data (*De-duplication*) untuk efisiensi penyimpanan.
</details>

### Soal #248: Algoritma "Multi-Tasking" (OS)
Komputer seolah-olah menjalankan 10 aplikasi barengan. Rahasianya?
A. Prosesornya ada 1000.
B. Algoritma "Time Slicing" (Membagi waktu super cepat antar aplikasi sehingga mata manusia tidak menyadari gantiannya).
C. Aplikasinya saling bantu.
D. Ghaib.

<details>
<summary>💡 Hint</summary>
Prinsip penjadwalan CPU dalam Sistem Operasi modern.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pembagian waktu (Time Slicing).**
Kecepatan eksekusi ribuan kali per detik membuat ilusi keserentakan.
</details>

### Soal #249: Algoritma "Password Wifi" (Encryption Key)
Kenapa router minta password panjang?
A. Biar kabel tidak panas.
B. Semakin panjang password, semakin banyak kemungkinan kombinasi yang harus dicoba (Key Space Expansion).
C. Biar tidak ada yang pake.
D. Biar router tidak bosan.

<details>
<summary>💡 Hint</summary>
Algoritma Brute Force akan butuh waktu bertahun-tahun untuk menebak password yang sangat panjang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memperbanyak kombinasi.**
Prinsip dasar ketahanan kriptografi terhadap serangan tebakan.
</details>

### Soal #250: Algoritma "Sorting Ranking" (Informatika Konteks)
Kamu ingin mengurutkan 1000 pemenang lomba coding. Algoritma mana yang paling pas untuk menangani data besar tersebut secara cepat?
A. Bubble Sort.
B. Merge Sort atau Quick Sort.
C. Menunjuk manual satu per satu.
D. Tidak usah diurutkan.

<details>
<summary>💡 Hint</summary>
Gunakan konsep "Divide and Conquer" untuk kecepatan tinggi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Merge Sort / Quick Sort.**
Efisien secara algoritma (O(n log n)) jauh melampaui algoritma sederhana (O(n²)).
</details>


---
[< Bagian 4 (151-200)](05-algorithm-design-part-4.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 6 (251-300) >](05-algorithm-design-part-6.md)
