# 05. Algorithm Design - Bagian 2 (Soal 51-100)

[< Bagian 1 (1-50)](05-algorithm-design-part-1.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 3 (101-150) >](05-algorithm-design-part-3.md)

---
### Soal #51: Algoritma "Kelipatan 5"
Tuliskan angka kelipatan 5 antara 1 sampai 21. Berapa angka terakhir yang ditulis?
A. 20
B. 21
C. 25
D. 15

<details>
<summary>💡 Hint</summary>
Bilangan kelipatan 5: 5, 10, 15, 20. Cek batas atasnya (21).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 20**
Angka 20 adalah kelipatan 5 terbesar yang masih di bawah 21.
</details>

### Soal #52: Algoritma "Parkir Mall"
1 jam pertama Rp 5.000. Setiap jam berikutnya Rp 2.000. Berapa biaya parkir 3 jam?
A. Rp 7.000
B. Rp 9.000
C. Rp 11.000
D. Rp 15.000

<details>
<summary>💡 Hint</summary>
Total = (Jam 1) + (Sisa Jam x Harga per jam).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Rp 9.000**
$5.000 + (2 \times 2.000) = 5.000 + 4.000 = 9.000$.
</details>

### Soal #53: Algoritma "Trace Variabel"
1. $A = 5$
2. $B = A + 3$
3. $A = B - 2$
Berapa nilai $A$ dan $B$ sekarang?
A. $A=5, B=8$
B. $A=6, B=8$
C. $A=8, B=8$
D. $A=6, B=5$

<details>
<summary>💡 Hint</summary>
Ikuti baris demi baris. Nilai variabel bisa berubah (Update) seiring jalannya langkah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. A=6, B=8**
$B = 5+3=8$. Lalu $A = 8-2=6$.
</details>

### Soal #54: Algoritma "Cari Nama Terpanjang"
Daftar: "Ani", "Budi", "Candra". Manakah yang dipilih algoritma pencari kata terpanjang?
A. Ani
B. Budi
C. Candra
D. Semua sama

<details>
<summary>💡 Hint</summary>
Hitung jumlah karakter (huruf) pada masing-masing kata.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Candra**
Candra memiliki 6 huruf, lebih banyak dari Ani (3) dan Budi (4).
</details>

### Soal #55: Algoritma Penukaran (3 Variabel)
$X=1, Y=2, Z=3$.
1. Pindahkan isi $X$ ke $W$ (cadangan).
2. Pindahkan isi $Y$ ke $X$.
3. Pindahkan isi $Z$ ke $Y$.
4. Pindahkan isi $W$ ke $Z$.
Berapa urutan isi $X, Y, Z$ sekarang?
A. 2, 3, 1
B. 1, 2, 3
C. 3, 2, 1
D. 2, 1, 3

<details>
<summary>💡 Hint</summary>
Isi $X$ jadi 2, isi $Y$ jadi 3, isi $Z$ jadi nilai awal $X$ (1).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. 2, 3, 1**
Ini adalah algoritma pergeseran nilai (*Shift*).
</details>

### Soal #56: Algoritma "Tiket Bioskop"
"Anak-anak (di bawah 12 thn) diskon 50%". Umur Dito 12 tahun tepat. Apakah diskon?
A. Ya, karena masih sekolah.
B. Tidak, karena syaratnya harus "di bawah" 12 (artinya 0-11 tahun).
C. Ya, karena 12 masih kecil.
D. Berkurang dikit.

<details>
<summary>💡 Hint</summary>
Perhatikan kata kunci "di bawah" (<) vs "di bawah atau sama dengan" ($\le$).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak diskon.**
Dalam logika kaku, 12 tidak lebih kecil dari 12.
</details>

### Soal #57: Algoritma Loop "Terhenti"
"Ulangi: Makan 1 suap nasi, sampai piring kosong". Jika piring sudah kosong dari awal, apa yang dilakukan?
A. Tetap makan sekali.
B. Tidak makan sama sekali (Langsung selesai).
C. Menangis.
D. Makan piringnya.

<details>
<summary>💡 Hint</summary>
Pengecekan kondisi dilakukan di awal sebelum aksi (While Loop).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak makan sama sekali.**
Jika kondisi berhenti sudah terpenuhi di awal, proses tidak dijalankan.
</details>

### Soal #58: Algoritma "Matikan Komputer"
Manakah langkah terakhir yang benar sesuai standar software?
A. Cabut kabel listrik.
B. Tunggu layar benar-benar gelap barulah cabut daya.
C. Klik tombol Start -> Shutdown.
D. Pencet tombol power di CPU berulang kali.

<details>
<summary>💡 Hint</summary>
Satu langkah krusial untuk memastikan semua data sudah tersimpan aman di disk sebelum daya hilang.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tunggu layar gelap baru cabut daya.**
Shutdown software memicu proses penutupan file, langkah terakhir adalah memastikan hardware benar-benar mati.
</details>

### Soal #59: Algoritma "Cek Password"
"Input: Admin123". Password asli: "admin123". Apakah login berhasil?
A. Berhasil, karena hurufnya sama.
B. Gagal, karena 'A' besar berbeda with 'a' kecil.
C. Berhasil jika HP-nya ramah.
D. Berhasil jika usernamenya benar.

<details>
<summary>💡 Hint</summary>
Aplikasi keamanan hampir selalu membedakan casing (*Case Sensitive*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gagal.**
Ketelitian karakter sangat penting dalam algoritma otentikasi.
</details>

### Soal #60: Algoritma "Jalan di Labirin"
"Selalu pegang dinding sebelah kanan dan ikuti terus". Apakah algoritma ini menjamin kamu keluar?
A. Ya, untuk labirin tipe sederhana (tanpa pulau di tengah).
B. Tidak, hanya akan membuat pusing.
C. Ya, jika labirinnya terbuat dari kaca.
D. Tidak, kamu akan terjebak selamanya.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma klasik *Wall Follower*.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Ya (untuk mayoritas labirin standar).**
Teknik ini memastikan eksplorasi yang teratur di sepanjang sirkuit labirin.
</details>

### Soal #61: Algoritma Belanja di Kantin
Budi ingin membeli nasi (Rp 5.000) dan es teh (Rp 2.000). Dia punya uang Rp 10.000. Algoritma kembalian yang benar adalah...
A. $10.000 - 5.000 + 2.000$
B. $10.000 - (5.000 + 2.000)$
C. $(10.000 - 5.000) - 2.000$
D. Jawaban B dan C benar secara matematis.

<details>
<summary>💡 Hint</summary>
Pikirkan bagaimana uang total dikurangi oleh jumlah semua belanjaan sekaligus, atau dikurangi satu-persatu.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Jawaban B dan C benar.**
Dalam algoritma, kita bisa menjumlahkan pengeluaran dulu ($5.000+2.000=7.000$) baru dikurangi ($10.000-7.000=3.000$), atau mengurangi perlahan ($10.000-5.000=5.000$, lalu $5.000-2.000=3.000$).
</details>

### Soal #62: Algoritma "Download Game"
Kecepatan download 2 MB/detik. Ukuran game 120 MB. Berapa menit waktu yang dibutuhkan?
A. 60 menit
B. 1 menit
C. 10 menit
D. 2 menit

<details>
<summary>💡 Hint</summary>
Waktu (detik) = Total Ukuran / Kecepatan. Lalu ubah ke menit (1 menit = 60 detik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 1 menit**
$120 / 2 = 60$ detik. 60 detik = 1 menit.
</details>

### Soal #63: Algoritma "Posting Foto IG"
Manakah langkah yang merupakan bagian dari "Proses" (bukan Input/Output)?
A. Memilih foto dari galeri.
B. Menulis caption.
C. Menerapkan filter efek pada foto.
D. Foto muncul di feed teman.

<details>
<summary>💡 Hint</summary>
Proses adalah tindakan mengubah atau memodifikasi data (foto) yang sudah ada.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Menerapkan filter.**
Input adalah foto/caption, output adalah tampilan di feed. Perubahan visual oleh filter adalah proses pengolahan citra.
</details>

### Soal #64: Algoritma "Antre Fotokopi"
Ada 3 siswa: A (10 lembar), B (50 lembar), C (5 lembar). Pemilik fotokopi ingin semua cepat selesai (tunggu paling singkat). Siapa yang harus difotokopi pertama?
A. Siswa B karena paling banyak untungnya.
B. Siswa A karena di tengah.
C. Siswa C karena paling sedikit jumlahnya (SJF - Shortest Job First).
D. Sesuai urutan kedatangan saja.

<details>
<summary>💡 Hint</summary>
Untuk meminimalkan waktu tunggu rata-rata, selesaikan tugas yang paling cepat (paling sedikit lembarannya) terlebih dahulu.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Siswa C.**
Ini adalah algoritma *Shortest Job First*. Jika C dikerjakan dulu (5 lembar), maka A dan B tidak perlu menunggu lama proses 50 lembar milik B.
</details>

### Soal #65: Algoritma "Pin HP (Brute Force)"
PIN HP terdiri dari 4 angka (0000-9999). Jika kamu mencoba dari 0000, 0001, 0002... sampai ketemu, apa nama algoritma ini?
A. Binary Search
B. Random Search
C. Brute Force (Linear Search)
D. Hacking Search

<details>
<summary>💡 Hint</summary>
Mencoba semua kemungkinan satu per satu tanpa strategi khusus.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Brute Force.**
Metode ini pasti berhasil tapi membutuhkan waktu paling lama jika kuncinya ada di angka besar (misal 9998).
</details>

### Soal #66: Algoritma "Mandi Pagi"
1. Gosok gigi.
2. Pakai baju.
3. Guyur badan dengan air.
4. Pakai sabun.
Manakah langkah yang melanggar logika jika diletakkan paling akhir?
A. 1
B. 2
C. 3
D. 4

<details>
<summary>💡 Hint</summary>
Kamu tidak bisa memakai baju (2) baru kemudian menyiram badan (3), baju akan basah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 2 (Pakai baju).**
Memakai baju harus dilakukan setelah badan kering/selesai mandi.
</details>

### Soal #67: Algoritma "Belajar Ujian"
"Belajarlah 25 menit, istirahat 5 menit. Ulangi 4 kali."
Berapa total waktu yang dihabiskan untuk **belajar saja**?
A. 120 menit
B. 100 menit
C. 30 menit
D. 200 menit

<details>
<summary>💡 Hint</summary>
Hanya hitung durasi belajarnya: $25 \times 4$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 100 menit**
$25 \text{ menit} \times 4 \text{ siklus} = 100 \text{ menit}$.
</details>

### Soal #68: Algoritma "Urutan Rank Game"
Rank: Bronze, Silver, Gold, Platinum.
Bila sistem menggunakan algoritma $Rank\_Points > 1000$ untuk naik ke Silver. Budi punya 999 poin. Apa Rank Budi?
A. Silver
B. Bronze
C. Gold
D. Platinum

<details>
<summary>💡 Hint</summary>
999 belum lebih besar dari 1000.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bronze**
Kurang 1 poin saja tetap dianggap belum memenuhi syarat algoritma kenaikan tingkat.
</details>

### Soal #69: Algoritma "Cek Login Caps Lock"
Username: "SiswaSMA". Kamu mengetik "siswasma". Jika sistem bersifat *Case Sensitive*, apakah berhasil?
A. Berhasil, karena hurufnya sama.
B. Gagal, karena 'S' dan 's' berbeda.
C. Berhasil jika password benar.
D. Berhasil karena sistem memaafkan kesalahan kecil.

<details>
<summary>💡 Hint</summary>
Informatika sangat presisi. Perubahan besar-kecil dianggap data yang berbeda.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gagal.**
Case-sensitive berarti membedakan huruf besar dan kecil secara mutlak.
</details>

### Soal #70: Algoritma "E-Money"
1. Tempel kartu.
2. JIKA saldo cukup, MAKA pintu terbuka dan kurangi saldo.
3. JIKA TIDAK, MAKA bunyi "Tetot" dan pintu tetap tutup.
Apa yang disebut sebagai **Input** di sini?
A. Bunyi "Tetot".
B. Pintu terbuka.
C. Saldo berkurang.
D. Penempelan kartu dan data saldo kartu.

<details>
<summary>💡 Hint</summary>
Input adalah pemicu atau data awal yang diterima sensor.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Penempelan kartu dan saldo.**
Aktivitas fisik pengguna dan data di dalam kartu adalah sumber input bagi mesin.
</details>

### Soal #71: Algoritma "Cari Teman di Kerumunan"
Cara paling sistematis mencari teman yang memakai baju merah di lapangan upacara adalah...
A. Teriak sekencang mungkin.
B. Memindai barisan mulai dari pojok kiri depan satu-persatu ke kanan (Scanning).
C. Berlari acak ke tengah lapangan.
D. Menunggu di depan gerbang.

<details>
<summary>💡 Hint</summary>
Gunakan algoritma *Linear Search* visual yang teratur agar tidak ada area yang terlewat.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Memindai barisan secara teratur.**
Ini memastikan setiap objek (siswa) diperiksa setidaknya sekali.
</details>

### Soal #72: Algoritma "Menu GoFood"
Urutan: Masukkan alamat -> Pilih Restoran -> Pilih Makanan -> Bayar.
Kenapa alamat harus dimasukkan di awal?
A. Biar aplikasi tahu jarak dan ongkir sebelum kamu belanja.
B. Iseng saja.
C. Biar restorannya tahu kamu siapa.
D. Agar makanan tidak dingin.

<details>
<summary>💡 Hint</summary>
Alamat digunakan sebagai filter awal untuk menentukan restoran mana saja yang "Available" (tersedia) untuk menjangkaumu.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Menentukan jarak dan ongkir.**
Input lokasi adalah syarat efisiensi algoritma pengiriman.
</details>

### Soal #73: Algoritma "Sorting Tinggi" (Bubble Sort)
Ali (160), Budi (150). Instruksi: "Jika yang kiri lebih tinggi dari yang kanan, tukar posisi."
Apakah mereka bertukar posisi?
A. Tidak tetap di tempat.
B. Ya, Ali pindah ke kanan dan Budi ke kiri.
C. Bergantung perintah guru.
D. Keduanya jongkok.

<details>
<summary>💡 Hint</summary>
Bandingkan 160 (kiri) and 150 (kanan). 160 > 150 adalah Benar (Ya).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ya, mereka tukar posisi.**
Ini adalah satu langkah dasar dalam *Bubble Sort* untuk mengurutkan dari yang terkecil.
</details>

### Soal #74: Algoritma "Loop Matematika"
$N = 1$. Ulangi: $N = N \times 2$ sebanyak 4 kali. Apa hasil akhir $N$?
A. 8
B. 16
C. 4
D. 32

<details>
<summary>💡 Hint</summary>
$1 \times 2 = 2 \rightarrow 2 \times 2 = 4 \rightarrow 4 \times 2 = 8 \rightarrow 8 \times 2 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 16**
Eksponensial 2 pangkat 4 ($2^4 = 16$).
</details>

### Soal #75: Algoritma "Kapasitas Lift"
Maksimum 5 orang. Jika ada 12 orang ingin naik, berapa kali lift harus bolak-balik?
A. 2 kali
B. 3 kali
C. 2,4 kali
D. 12 kali

<details>
<summary>💡 Hint</summary>
Gunakan pembulatan ke atas (*Ceiling*): $12 / 5 = 2.4$. Karena manusia tidak bisa dibagi, maka butuh satu trip lagi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 3 kali**
Trip 1 (5 orang), Trip 2 (5 orang), Trip 3 (2 orang). Total 12 orang.
</details>

### Soal #76: Algoritma "Isi Daya HP"
1. Colok charger ke listrik.
2. Hubungkan kabel ke HP.
3. JIKA daya naik, MAKA biarkan.
4. JIKA baterai 100%, MAKA cabut.
Apa "Exit Condition" (Kondisi Keluar) dari algoritma ini?
A. Daya naik.
B. Colok listrik.
C. Baterai mencapai 100%.
D. HP meledak.

<details>
<summary>💡 Hint</summary>
Condition yang membuat pengulangan/proses berhenti secara normal.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Baterai 100%.**
Inilah tujuan akhir dan titik henti algoritma pengisian daya.
</details>

### Soal #77: Algoritma "Cari Kunci Hilang"
Ibu bilang: "Cari di laci, kalau tidak ada cari di meja, kalau tidak ada cari di tas."
Kunci ternyata ada di meja. Laci sudah diperiksa. Apakah tas perlu diperiksa?
A. Perlu, buat jaga-jaga.
B. Tidak perlu, karena algoritma berhenti saat barang ditemukan.
C. Tergantung perintah ibu lagi.
D. Tasnya saja yang dibawa.

<details>
<summary>💡 Hint</summary>
Efisiensi berarti berhenti segera setelah solusi (Output) tercapai.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak perlu diperiksa.**
Dalam algoritma pencarian, kita berhenti memeriksa objek lain jika target sudah ditemukan.
</details>

### Soal #78: Algoritma "Sorting Nilai"
80, 95, 70. Urutkan dari yang **terbesar** (Descending).
A. 70, 80, 95
B. 95, 80, 70
C. 80, 70, 95
D. 95, 70, 80

<details>
<summary>💡 Hint</summary>
Urutan dari angka yang paling tinggi nilainya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 95, 80, 70**
Standard sorting descending untuk menentukan juara atau peringkat.
</details>

### Soal #79: Algoritma "Google Translate"
1. Terima input teks bahasa Inggris.
2. Cari padanan kata di database bahasa Indonesia.
3. Susun berdasarkan aturan tata bahasa (Grammar).
4. Tampilkan hasil.
Manakah yang merupakan tahapan **Abstraksi** di dalam algoritma ini?
A. Menampilkan hasil di layar.
B. Mengabaikan jenis font atau warna teks input dan hanya fokus pada makna katanya.
C. Mencari kata di database.
D. Mengetik teks di keyboard.

<details>
<summary>💡 Hint</summary>
Ingat, abstraksi adalah membuang detail yang tidak penting bagi proses inti.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengabaikan font/warna.**
Bagi penerjemah, warna teks tidak penting, yang penting adalah makna katanya.
</details>

### Soal #80: Algoritma "Alarm Snooze"
"Bunyi alarm setiap 5 menit jika tombol snooze ditekan."
Alarm mulai jam 06:00. Kamu tekan snooze 3 kali. Jam berapa akhirnya kamu benar-benar bangun (asumsi setelah snooze ketiga langsung bangun)?
A. 06:05
B. 06:10
C. 06:15
D. 06:30

<details>
<summary>💡 Hint</summary>
Satu kali snooze = 5 menit. $3 \times 5 = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 06:15**
$06:00 + (3 \times 5 \text{ menit}) = 06:15$.
</details>
### Soal #81: Algoritma "Pesan Driver"
Sistem mencari driver yang jaraknya kurang dari 2 km dari pemesan.
Driver A: 1.5 km. Driver B: 2.1 km. Driver C: 0.5 km.
Siapa yang masuk dalam radar sistem?
A. A saja
B. C saja
C. A dan C
D. Semuanya

<details>
<summary>💡 Hint</summary>
Filter kondisi: $Jarak < 2$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. A dan C.**
1.5 dan 0.5 lebih kecil dari 2, sedangkan 2.1 lebih besar.
</details>

### Soal #82: Algoritma "Password Wifi"
Password: 'internetgratis'. Temanmu mengetik 'internet gratis' (pake spasi). Kenapa gagal?
A. Karena spasi dianggap karakater kosong yang tetap dihitung oleh sistem.
B. Karena internet tidak pernah gratis.
C. Karena sinyal lemah.
D. Karena hurufnya kekecilan.

<details>
<summary>💡 Hint</summary>
Dalam string komputer, spasi memiliki kode biner sendiri (ASCII 32).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Spasi dihitung sebagai karakter.**
Kecuali algoritma diprogram untuk mengabaikan spasi (*trim*), maka input harus persis sama.
</details>

### Soal #83: Algoritma "Playlist Shuffle"
Bagaimana algoritma memutar lagu secara acak?
A. Selalu putar lagu favorit saja.
B. Memberikan angka acak (Random Number) pada setiap lagu dan memutarnya sesuai nomor tersebut.
C. Memutar lagu berdasarkan abjad tapi terbalik.
D. Menunggu perintah suara.

<details>
<summary>💡 Hint</summary>
Gunakan fungsi *Randomize* untuk menentukan urutan indek lagu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menggunakan angka acak.**
Ini menjamin variasi putar yang berbeda setiap kali mode Shuffle diaktifkan.
</details>

### Soal #84: Algoritma "Traffic Light" (Definiteness)
Lampu kuning berarti "Hati-hati". Kenapa instruksi ini dianggap kurang presisi bagi mobil otonom?
A. Karena warna kuning itu bagus.
B. Karena kata "Hati-hati" bermakna ganda (ambigu). Harusnya "Pelankan kecepatan hingga 20km/jam".
C. Karena mobil tidak bisa melihat warna.
D. Karena mobil otonom tidak punya hati.

<details>
<summary>💡 Hint</summary>
Algoritma butuh instruksi kuantitatif (angka/aksi pasti), bukan kualitatif (perasaan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Bermakna ganda (Ambigu).**
Syarat *Definiteness* mengharuskan instruksi tidak menimbulkan banyak tafsir.
</details>

### Soal #85: Algoritma "Nabung Keinginan"
Beli sepatu Rp 300.000. Tabungan tiap hari Rp 10.000. Berapa hari sampai uang terkumpul?
A. 10 hari
B. 20 hari
C. 30 hari
D. 300 hari

<details>
<summary>💡 Hint</summary>
$Target / Harian = Jumlah Hari$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 30 hari.**
$300.000 / 10.000 = 30$.
</details>

### Soal #86: Algoritma "Mode Malam HP"
1. JIKA jam > 22:00, MAKA aktifkan filter cahaya kuning.
2. JIKA jam jam < 06:00, MAKA tetap aktifkan.
3. JIKA TIDAK, matikan.
Jam menunjukkan **23:30**. Apa warna layar?
A. Biru tajam
B. Putih terang
C. Kekuningan (Warm)
D. Hitam total

<details>
<summary>💡 Hint</summary>
Kondisi nomor 1 terpenuhi karena 23:30 lebih besar dari 22:00.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kekuningan (Warm).**
Logika "Night Shift" atau "Blue Light Filter" otomatis.
</details>

### Soal #87: Algoritma "Cari Teman Sebangku"
Kamu lupa teman sebangkumu siapa. Kamu mengecek daftar absen. Dimana biasanya teman sebangkumu berada di daftar?
A. Di urutan paling atas.
B. Di nomor yang berdekatan dengan nomor absenmu (misal tepat di atas atau di bawahmu).
C. Di paling bawah.
D. Tidak ada di absen.

<details>
<summary>💡 Hint</summary>
Sistem pembagian bangku sekolah seringkali menggunakan urutan absen (Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dekat dengan nomor absenmu.**
Pemanfaatan pola (Pattern Recognition) membantu mempercepat algoritma pencarian.
</details>

### Soal #88: Algoritma "Game RPG - Level Up"
"Setiap naik level, HP (Health Point) bertambah 10% dari HP sebelumnya."
HP Level 1: 100. Berapa HP Level 3?
A. 120
B. 110
C. 121
D. 130

<details>
<summary>💡 Hint</summary>
Lvl 2: $100 + (10\% \times 100) = 110$. Lvl 3: $110 + (10\% \times 110) = ...$
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 121**
Penambahan bersifat bunga majemuk ($100 \rightarrow 110 \rightarrow 121$).
</details>

### Soal #89: Algoritma "Cek Keranjang Shopee"
Ada 5 barang di keranjang. Kamu ingin checkout semuanya. Langkah mana yang dilakukan berulang (Looping)?
A. Klik tombol "Checkout".
B. Memasukkan alamat pengiriman.
C. Menghitung (Harga barang x Jumlah) untuk setiap item satu-persatu.
D. Mengklik metode pembayaran.

<details>
<summary>💡 Hint</summary>
Looping terjadi pada proses yang harus dilakukan pada setiap individu di dalam kumpulan (Koleksi barang).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Menghitung harga per item.**
Sistem akan mengulang kalkulasi untuk item 1, lalu item 2, dan seterusnya.
</details>

### Soal #90: Algoritma "Lupa Password"
1. Masukkan email.
2. Klik "Kirim kode".
3. Cek kode di email.
4. Masukkan kode ke website.
5. Masukkan password baru 2 kali.
Kenapa disuruh masukkan password baru **2 kali**?
A. Biar website makin aman.
B. Sebagai mekanisme validasi (Input 1 harus sama dengan Input 2) untuk menghindari typo.
C. Iseng saja.
D. Biar kamu hafal.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma *Double Check* untuk meyakinkan data input sudah benar sebelum disimpan permanen.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mekanisme validasi typo.**
Kesalahan pengetikan satu huruf saja bisa membuat user tidak bisa login lagi nanti, maka dilakukan pengecekan kembar.
</details>

### Soal #91: Algoritma "Sortir Beras"
Kamu punya 1 kg beras campur krikil kecil. Algoritma paling pas adalah...
A. Mengambil satu per satu butir beras sampai krikil tersisa (Lambat).
B. Menggunakan ayakan/saringan yang lubangnya pas buat beras tapi menahan krikil (Abstraksi Fisik).
C. Mencuci beras sampai krikil hilang.
D. Memakan semuanya.

<details>
<summary>💡 Hint</summary>
Gunakan filter yang memanfaatkan perbedaan fisis (ukuran) antara beras dan krikil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menggunakan ayakan.**
Penggunaan alat (filter) jauh lebih efektif daripada pengecekan manual satu-persatu.
</details>

### Soal #92: Algoritma "Smart CCTV"
"JIKA wajah terdeteksi bukan anggota keluarga, MAKA kirim notifikasi bahaya."
Berapa output yang mungkin dari algoritma ini (binary)?
A. Banyak sekali.
B. Dua (Ya/Tidak atau Bahaya/Aman).
C. Tidak ada.
D. Wajah orang asing.

<details>
<summary>💡 Hint</summary>
Kondisi Boolean (If-Else) selalu menghasilkan salah satu dari dua pilihan aksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Dua (Bahaya/Aman).**
Logika digital dasar berbasis pada dua kondisi nilai.
</details>

### Soal #93: Algoritma "Trace Jalur Tikus"
X=5, Y=10.
1. X = X + Y
2. Y = X - Y
3. X = X - Y
Apa nilai X dan Y sekarang?
A. X=5, Y=10
B. X=10, Y=5
C. X=15, Y=15
D. X=0, Y=0

<details>
<summary>💡 Hint</summary>
Langkah 1: $X=15$. Langkah 2: $Y=15-10=5$. Langkah 3: $X=15-5=10$.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. X=10, Y=5**
Ini adalah algoritma klasik untuk **menukar isi dua variabel** tanpa variabel bantuan.
</details>

### Soal #94: Algoritma "Cuci Tangan Robot"
Sebuah instruksi: "Bilas tangan selama 20 detik."
Robot melakukan: Menaruh tangan di bawah kran tanpa membuka kran, diam 20 detik, selesai.
Salahnya di mana?
A. Waktunya kelamaan.
B. Instruksi kurang detail (Definiteness) - tidak ada perintah "Nyalakan kran".
C. Robotnya malas.
D. Kran airnya rusak.

<details>
<summary>💡 Hint</summary>
Komputer tidak punya akal sehat. Jika tidak diperintah "Buka air", ia tidak akan membukanya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Kurang detail.**
Algoritma harus menyertakan semua langkah prasyarat sebelum aksi utama dilakukan.
</details>

### Soal #95: Algoritma "Password Wifi Kafe"
"Beli kopi, di struk ada kode, masukkan kode".
Kenapa kode di struk selalu berubah setiap hari?
A. Biar keren.
B. Agar orang di luar kafe tidak bisa pakai wifi selamanya (Keamanan & Finiteness Akses).
C. Tintanya masih banyak.
D. Kasirnya gabut.

<details>
<summary>💡 Hint</summary>
Pembatasan akses (Authorization) seringkali menggunakan algoritma waktu terbatas (*Time-based access*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Keamanan & Pembatasan Akses.**
Membatasi masa berlaku password adalah bagian dari desain keamanan algoritma jaringan.
</details>

### Soal #96: Algoritma "Sorting Pakaian"
Kamu ingin mengurutkan baju dari yang paling sering dipakai ke yang paling jarang. Ini disebut sorting berdasarkan...
A. Nama merk.
B. Warna.
C. Frekuensi (Popularity Sort).
D. Harga.

<details>
<summary>�� Hint</summary>
Pilih kriteria yang mencerminkan "jumlah penggunaan".
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Frekuensi.**
Algoritma ini sering dipakai YouTube untuk menampilkan "Most Viewed" videos.
</details>

### Soal #97: Algoritma "Naik Ojek Online"
1. Buka aplikasi.
2. Cari tujuan.
3. Pesan.
4. Tunggu driver.
5. Perjalanan.
6. Beri bintang.
Langkah 6 merupakan...
A. Input bagi driver.
B. Feedback bagi algoritma sistem untuk menilai performa driver.
C. Iseng saja.
D. Kewajiban moral.

<details>
<summary>💡 Hint</summary>
Data dari user di akhir proses digunakan sistem untuk meningkatkan kualitas layanan berikutnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Feedback system.**
Data rating masuk ke algoritma reputasi driver dalam database pusat.
</details>

### Soal #98: Algoritma "Matematika Gampang"
"Tambahkan 1 ke angka X, ulangi sampai X mencapai 10". Jika mulai dari X = 11, apa yang terjadi?
A. Berhenti di 10.
B. Error, atau berputar selamanya (Infinite Loop) jika pengecekannya hanya "X == 10".
C. Kembali ke 0.
D. Angka 11 hilang.

<details>
<summary>💡 Hint</summary>
Jika kamu di angka 11 dan terus menambah, kamu tidak akan pernah bertemu angka 10.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Infinite Loop (atau berputar selamanya).**
Penting bagi algoritma memiliki syarat berhenti yang logis untuk setiap kemungkinan input.
</details>

### Soal #99: Algoritma "Cek Lulus Ujian"
Syarat: Nilai Matematika > 70 **DAN** Nilai Bahasa > 70.
Budi: Mat=90, Bahasa=65. Apakah Budi lulus?
A. Lulus, kan rata-ratanya tinggi.
B. Tidak Lulus, karena syarat DAN mewajibkan keduanya benar.
C. Lulus, bahasa bisa menyusul.
D. Tergantung kebijakan sekolah.

<details>
<summary>💡 Hint</summary>
Logika AND dalam algoritma: Benar + Salah = Salah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tidak Lulus.**
Karena salah satu syarat (Bahasa) tidak terpenuhi, maka hasil akhirnya False (Tidak).
</details>

### Soal #100: Algoritma "Kalkulator Sederhana"
Input: Angka1, Angka2, Operator (+).
Proses: Hasil = Angka1 + Angka2.
Apa yang terjadi jika Angka2 diisi huruf "A"?
A. Hasilnya jadi "Angka1A".
B. Terjadi error tipe data (Type Mismatch) karena huruf tidak bisa dijumlahkan secara matematis.
C. Kalkulator meledak.
D. Huruf A jadi angka 0.

<details>
<summary>💡 Hint</summary>
Algoritma butuh input dengan tipe data yang sesuai (*Integer/Float* vs *String*).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Error tipe data.**
Sistem perlu memastikan input valid sebelum menjalankan proses aritmatika.
</details>

---
[< Bagian 1 (1-50)](05-algorithm-design-part-1.md) | [🏠 Indeks](05-algorithm-design.md) | [Bagian 3 (101-150) >](05-algorithm-design-part-3.md)
