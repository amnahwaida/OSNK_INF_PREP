# 03. Pengenalan Pola - Bagian 3 (Soal 101-150)

[< Bagian 2 (51-100)](03-pattern-recognition-part-2.md) | [🏠 Indeks](../03-pattern-recognition.md) | [Bagian 4 (151-200) >](03-pattern-recognition-part-4.md)

---
### Soal #101: Aturan Subgrid Sudoku
Dalam Sudoku 9x9, angka 1-9 tidak boleh berulang di baris, kolom, dan kotak 3x3 (subgrid).
Jika angka "5" sudah ada di posisi baris 1 kolom 1, di manakah angka "5" BOLEH diletakkan di baris 2?
A. Baris 2 Kolom 1
B. Baris 2 Kolom 2
C. Baris 2 Kolom 5
D. Baris 2 Kolom 3

<details>
<summary>💡 Hint</summary>
Baris 1, 2, dan 3 kolom 1, 2, dan 3 masuk dalam satu kotak 3x3 yang sama.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Baris 2 Kolom 5.**
Kolom 5 berada di subgrid yang berbeda dengan kolom 1, sehingga tidak melanggar aturan pengulangan subgrid.
</details>

### Soal #102: Pola Angka Minesweeper
Dalam game Minesweeper, kamu melihat angka "3" di sebuah kotak. Apa artinya berdasarkan pengenalan pola?
A. Ada 3 ranjau di seluruh area permainan.
B. Ada tepat 3 ranjau di 8 kotak di sekeliling angka tersebut.
C. Kamu punya 3 nyawa tersisa.
D. Kotak tersebut akan meledak dalam 3 detik.

<details>
<summary>💡 Hint</summary>
Angka adalah "sensor" pasif untuk deteksi pola ranjau di sekitarnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ada tepat 3 ranjau di sekelilingnya.**
Pola angka membantu pemain melakukan deduksi logika posisi ranjau.
</details>

### Soal #103: Pola Line Clear Tetris
Dalam Tetris, baris balok akan menghilang (cleared) jika...
A. Warnanya semua merah.
B. Baris tersebut terisi penuh secara horizontal tanpa ada lubang kosong.
C. Kamu menekan tombol Enter.
D. Balok mencapai langit-langit.

<details>
<summary>💡 Hint</summary>
Pola "Penuh" memicu aksi "Hapus".
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terisi penuh secara horizontal.**
Dekomposisi tujuan game: Menyusun pola padat untuk mengurangi tumpukan.
</details>

### Soal #104: Perilaku Ghost Pac-Man
Hantu Merah (Blinky) selalu mengejar posisi koordinat Pac-Man secara langsung. Ini adalah contoh pola...
A. Pergerakan acak.
B. Pathfinding (Pencarian jalur) yang ditujukan ke target dinamis.
C. Hantu yang sedang tersesat.
D. Pola diam di tempat.

<details>
<summary>💡 Hint</summary>
Algoritma mengenali pola posisi target untuk menentukan arah gerak.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pathfinding ke target dinamis.**
Mengenali pola gerak musuh memudahkan pemain menghindar.
</details>

### Soal #105: Pola Match-3 Candy Crush
Jika kamu menjajajarkan 4 permen dengan warna yang sama secara vertikal, apa yang terjadi?
A. Tidak terjadi apa-apa.
B. Terbentuk permen spesial (Striped Candy) yang bisa menghancurkan satu kolom.
C. Permainan langsung menang.
D. HP kamu akan bergetar selamanya.

<details>
<summary>💡 Hint</summary>
Jumlah (Count) dalam satu pola menentukan tingkat bonus.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Terbentuk permen spesial.**
Pola $> 3$ memicu fungsi algoritma yang lebih kuat (Power-up).
</details>

### Soal #106: Pola Warna Wordle
Kamu menebak kata, dan huruf "A" berwarna Kuning. Apa artinya?
A. Huruf A tidak ada di kata tersebut.
B. Huruf A ada di kata tersebut tapi di posisi yang salah.
C. Huruf A ada di kata tersebut dan posisinya sudah benar.
D. Kamu harus membayar untuk melihat jawabannya.

<details>
<summary>💡 Hint</summary>
Hijau = Benar semua. Kuning = Ada tapi salah tempat. Abu-abu = Tidak ada.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Ada tapi di posisi salah.**
Wordle menggunakan pola umpan balik visual untuk mengeliminasi kemungkinan kata.
</details>

### Soal #107: Gabungan Angka 2048
Dalam game 2048, jika kotak angka 8 bertabrakan dengan kotak angka 8, mereka akan menjadi...
A. 88
B. 0
C. 16
D. 2048

<details>
<summary>💡 Hint</summary>
Operasi matematikanya adalah Penjumlahan ($X + X$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 16.**
Pola pengulangan kelipatan dua ($2^n$) adalah inti dari game ini.
</details>

### Soal #108: Pola Pertumbuhan Snake
Dalam game Snake, setiap ular memakan "apel", tubuhnya bertambah panjang. Apa risiko dari pola pertumbuhan ini?
A. Ular makin cepat lari.
B. Snake makin sulit bermanuver karena ekornya bisa tertabrak kepalanya sendiri.
C. Snake akan berubah warna menjadi pelangi.
D. Apelnya akan habis.

<details>
<summary>💡 Hint</summary>
Dekomposisi: Ruang gerak tetap, panjang objek bertambah.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Makin sulit bermanuver.**
Pola peningkatan kesulitan seiring kemajuan pemain.
</details>

### Soal #109: Langkah Kuda Catur (Knight)
Kuda berada di kotak Putih. Setelah melompat satu kali (pola L), ia pasti akan mendarat di kotak berwarna...
A. Putih
B. Hitam
C. Hijau
D. Transparan

<details>
<summary>💡 Hint</summary>
Pola L: 2 langkah lurus + 1 langkah samping. Cobalah di papan catur.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Hitam.**
Secara matematis, pola gerak Kuda selalu mengubah warna pijakan dari warna saat ini.
</details>

### Soal #110: Kombinasi Kartu Poker
Mana yang memiliki pola lebih kuat/tinggi nilainya?
A. Three of a Kind (3 angka sama)
B. Full House (3 angka sama + 2 angka sama lain)
C. One Pair (2 angka sama)
D. High Card (Angka tertinggi acak)

<details>
<summary>💡 Hint</summary>
Makin kompleks polanya (makin sulit didapat), makin tinggi nilainya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Full House.**
Pola ini merupakan gabungan dari pola yang lebih sederhana, sehingga lebih sulit muncul secara statistik.
</details>

### Soal #111: Gunting Batu Kertas
Jika polanya adalah: Gunting mengalahkan Kertas, Kertas mengalahkan Batu. Maka Batu mengalahkan...
A. Semua
B. Gunting
C. Batu lagi
D. Tidak ada

<details>
<summary>💡 Hint</summary>
Ini adalah pola sirkular (lingkaran kekuatan).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Gunting.**
Pola relasi melingkar yang seimbang.
</details>

### Soal #112: Kondisi Menang Tic-Tac-Toe
Dalam papan 3x3, kamu menang jika membentuk pola 3 simbol yang sama secara...
A. Horizontal saja
B. Vertikal saja
C. Horizontal, Vertikal, atau Diagonal
D. Berjejer di pojok-pojok saja

<details>
<summary>💡 Hint</summary>
Ada 8 kemungkinan pola garis lurus untuk menang.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Horizontal, Vertikal, atau Diagonal.**
Pengenalan pola garis lurus adalah mekanisme utama deteksi kemenangan.
</details>

### Soal #113: Rule Tangan Kiri di Labirin
Jika kamu masuk ke labirin dan selalu meletakkan tangan kirimu di dinding tanpa pernah mengangkatnya, apa polanya?
A. Kamu akan pusing.
B. Kamu dijamin akan menemukan jalan keluar (meskipun butuh waktu lama).
C. Kamu akan tersesat selamanya.
D. Tanganmu akan kotor.

<details>
<summary>💡 Hint</summary>
Ini adalah algoritma Wall-follower untuk navigasi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Akan menemukan jalan keluar.**
Pola penelusuran batas ini efektif untuk labirin yang terhubung secara topologi satu blok.
</details>

### Soal #114: Tower of Hanoi
Aturan: Piringan besar tidak boleh di atas piringan kecil.
Jika ada Piringan 1 (Kecil), 2 (Sedang), dan 3 (Besar). Di manakah posisi Piringan 2 yang BENAR?
A. Di bawah Piringan 3
B. Di atas Piringan 1
C. Di antara Piringan 3 (bawah) dan Piringan 1 (atas)
D. Di mana saja sesuka hati

<details>
<summary>💡 Hint</summary>
Ikuti pola urutan: Besar -> Kecil (dari bawah ke atas).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Di antara 3 (bawah) dan 1 (atas).**
Pola tumpukan mengecil ke atas adalah aturan tetap game ini.
</details>

### Soal #115: Pusat Rubik's Cube
Setelah diputar-putar sejauh apapun, kotak di bagian paling tengah setiap sisi Rubik tidak akan pernah berpindah tempat relatif terhadap pusat lainnya. Mengapa?
A. Karena dilem.
B. Karena secara mekanis pusat adalah poros tetap yang menentukan pola warna sisi tersebut.
C. Karena pusat adalah kotak gaib.
D. Pusat sebenarnya bergerak tapi kita tidak sadar.

<details>
<summary>💡 Hint</summary>
Warna sisi Rubik ditentukan oleh warna kotak pusatnya.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pusat adalah poros tetap.**
Strategi penyelesaian Rubik dimulai dengan mengenali pusat sebagai pola acuan.
</details>

### Soal #116: Pola Lipat Kertas (Origami)
Jika kamu melipat kertas menjadi dua, lalu menggunting bentuk segitiga di lipatannya, saat dibuka akan muncul dua segitiga yang...
A. Berjauhan
B. Berhimpitan membentuk pola cermin (Simetris)
C. Berubah menjadi kotak
D. Menghilang

<details>
<summary>💡 Hint</summary>
Lipatan bertindak sebagai sumbu simetri.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berhimpitan pola cermin.**
Pengenalan pola simetri sangat penting dalam geometri dan desain.
</details>

### Soal #117: Pola Merajut (Knitting)
Pola rajutan tertulis: K1, P1, K1, P1. (K=Knit, P=Purl).
Setelah P1 terakhir, apa langkah selanjutnya?
A. K2
B. P1
C. K1
D. Berhenti

<details>
<summary>💡 Hint</summary>
Lihat pola pengulangannya ($A-B-A-B-...$).
</details>

<details>
<summary>✅ Jawaban</summary>
**C. K1.**
Rajutan adalah pengulangan pola simpul yang sangat konsisten.
</details>

### Soal #118: Pola Tenun (Weaving)
Benang Lusi (tegak) dan Pakan (mendatar) disilangkan: Atas, Bawah, Atas, Bawah.
Apa fungsi dari pola selang-seling ini?
A. Agar kain terlihat berwarna-warni.
B. Agar benang saling mengunci dan membentuk lembaran kain yang kuat.
C. Biar prosesnya lama.
D. Agar kainnya bolong-bolong.

<details>
<summary>💡 Hint</summary>
Interlocking (Saling mengunci) adalah tujuan dari pola struktur kain.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Benang saling mengunci.**
Kekuatan kain berasal dari pengulangan pola fisik yang teratur.
</details>

### Soal #119: Pola Ubin (Tessellation)
Bentuk manakah yang bisa menutupi seluruh lantai tanpa ada celah sedikitpun?
A. Lingkaran
B. Segi Lima (Pentagon) Beraturan
C. Kotak (Persegi) atau Segi Enam (Hexagon)
D. Bintang

<details>
<summary>💡 Hint</summary>
Tessellation adalah pola pengulangan bentuk yang pas dipasangkan tanpa sisa ruang.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Kotak atau Segi Enam.**
Pola ini ditemukan di ubin rumah dan juga sarang lebah.
</details>

### Soal #120: Geometri Syamil (Islamic Art)
Sering kita temukan pola bintang 8 atau 12 yang sangat rumit di masjid. Pola ini dibangun dari...
A. Gambar tangan bebas tanpa penggaris.
B. Pengulangan bentuk dasar lingkaran dan kotak yang saling tumpang tindih secara simetris.
C. Stiker yang dibeli di pasar.
D. Foto pemandangan alam.

<details>
<summary>💡 Hint</summary>
Keindahan matematika berasal dari keteraturan pola dasar.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pengulangan bentuk dasar secara simetris.**
Ini adalah dekomposisi seni menjadi rumus geometri.
</details>

### Soal #121: Deret Fibonacci di Alam
Pola jumlah kelopak bunga seringkali: 3, 5, 8, 13, 21.
Apa angka selanjutnya dalam pola ini?
A. 25
B. 34
C. 40
D. 50

<details>
<summary>💡 Hint</summary>
Angka berikutnya adalah jumlah dari dua angka sebelumnya.
$8+13=21$, $13+21=...$
</details>

<details>
<summary>✅ Jawaban</summary>
**B. 34.**
Pola Fibonacci ditemukan secara luas di alam, dari kelopak bunga hingga susunan biji bunga matahari.
</details>

### Soal #122: Golden Ratio (Rasio Emas)
Banyak seniman menggunakan rasio 1.618 untuk membuat karya yang terlihat proporsional dan mata manusia menganggapnya "Indah". Ini adalah contoh...
A. Kebetulan semata.
B. Pola estetika berbasis matematika.
C. Aturan paksa dari pemerintah.
D. Keajaiban dunia.

<details>
<summary>💡 Hint</summary>
Otak manusia mengenali pola proporsi tertentu sebagai kenyamanan visual.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola estetika berbasis matematika.**
Banyak logo perusahaan terkenal (seperti Apple atau Google) menggunakan pola rasio ini.
</details>

### Soal #123: Segitiga Sierpinski
Sebuah segitiga besar dibagi 4, bagian tengahnya dibuang. Lalu segitiga sisa dibagi lagi dengan pola yang sama terus menerus sampai tak terhingga. Bentuk ini disebut...
A. Lingkaran
B. Kotak Ajaib
C. Fraktal
D. Garis Lurus

<details>
<summary>💡 Hint</summary>
Fraktal adalah pola yang mirip dengan dirinya sendiri meskipun diperbesar/diperkecil.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. Fraktal.**
Fraktal adalah dekomposisi geometri yang berulang secara rekursif (berulang ke diri sendiri).
</details>

### Soal #124: Keserupaan Diri (Self-similarity)
Kamu melihat kembang kol (Brokoli Roma). Jika kamu memotong satu bagian kecil, bentuknya terlihat persis seperti kembang kol yang besar. Pola ini disebut...
A. Fotokopi alam.
B. Self-similarity (Keserupaan diri).
C. Kerusakan pertumbuhan.
D. Penipuan mata.

<details>
<summary>💡 Hint</summary>
Bagian kecil mencerminkan pola keseluruhan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Self-similarity.**
Pola fraktal di alam membantu tumbuhan tumbuh efisien dengan instruksi genetik yang sederhana tapi diulang.
</details>

### Soal #125: Kristal Salju (Snowflake)
Semua kristal salju memiliki pola dasar simetri berapa arah?
A. 4 (Kotak)
B. 5 (Bintang)
C. 6 (Hexagonal)
D. 8 (Octagonal)

<details>
<summary>💡 Hint</summary>
Molekul air ($H_2O$) membeku membentuk kristal es dengan sudut $60^\circ$ atau $120^\circ$.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 6 (Hexagonal).**
Pola molekuler menentukan bentuk visual makroskopisnya.
</details>

### Soal #126: Pola Sarang Lebah
Lebah madu membuat ruangan berbentuk Hexagon (segi enam), bukan lingkaran atau kotak. Apa alasannya secara fungsional?
A. Agar terlihat modern.
B. Bentuk hexagon memungkinkan ruangan paling luas dengan penggunaan lilin (bahan bangunan) paling sedikit dan tanpa celah.
C. Karena lebah hanya bisa berhitung sampai angka 6.
D. Karena ratu lebah suka bentuk segi enam.

<details>
<summary>💡 Hint</summary>
Efisiensi penggunaan lahan dan material.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Paling luas dengan material paling sedikit.**
Ini adalah pola optimasi geometri di alam.
</details>

### Soal #127: Bentuk Gelembung Sabun
Satu gelembung sabun selalu berbentuk bola. Ini terjadi karena pola tegangan permukaan yang...
A. Ingin meledak.
B. Menarik ke arah pusat untuk menciptakan luas permukaan paling minimal.
C. Mengikuti arah tiupan angin.
D. Suka pada bentuk bulat.

<details>
<summary>💡 Hint</summary>
Alam selalu mencari pola energi terendah atau bentuk paling stabil.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan luas permukaan paling minimal.**
Matematika di balik gelembung sabun digunakan ilmuwan untuk mempelajari pola struktur minimal.
</details>

### Soal #128: Pola Lingkaran Pohon
Lingkaran tahun pohon: Terang (Musim Hujan/Tumbuh Cepat), Gelap (Musim Kemarau/Tumbuh Lambat).
Jika dalam potongan kayu ada 20 garis gelap, berapa umur pohon tersebut?
A. 5 tahun
B. 10 tahun
C. 20 tahun
D. 40 tahun

<details>
<summary>💡 Hint</summary>
Satu pasang (Terang+Gelap) biasanya mewakili siklus satu tahun.
</details>

<details>
<summary>✅ Jawaban</summary>
**C. 20 tahun.**
Membaca pola lingkaran pohon (Dendrokronologi) membantu ilmuwan mengetahui sejarah iklim masa lalu.
</details>

### Soal #129: Jejak Semut
Semut berjalan beriringan mengikuti satu jalur yang sama. Pengenalan pola apa yang mereka gunakan?
A. Mereka menghafal setiap batu di jalan.
B. Mereka mengikuti jejak bahan kimia (Feromon) yang ditinggalkan semut sebelumnya.
C. Mereka saling berpegangan tangan.
D. Semut paling depan membawa bendera penunjuk arah.

<details>
<summary>💡 Hint</summary>
Ini adalah pola komunikasi berbasis jejak kimiawi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengikuti jejak feromon.**
Algoritma semut (Ant Colony Optimization) digunakan dalam ilmu komputer untuk mencari rute terpendek.
</details>

### Soal #130: Tarian Lebah (Waggle Dance)
Lebah yang menemukan bunga akan menari di depan lebah lain. Kecepatan getaran dan sudut tarian adalah pola untuk memberitahu...
A. Bahwa ia sedang senang.
B. Jarak dan arah lokasi sumber makanan terhadap posisi matahari.
C. Bahwa ada predator mendekat.
D. Nama bunga yang ditemukan.

<details>
<summary>💡 Hint</summary>
Tarian adalah dekomposisi data peta menjadi pola gerak tubuh.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Jarak dan arah lokasi makanan.**
Bahasa pola hewan seringkali sangat akurat dan saintifik.
</details>

### Soal #131: Geometri Jaring Laba-laba
Jaring laba-laba memiliki pola radial (seperti jari-jari roda) dan spiral (melingkar). Fungsi pola spiral perekat adalah untuk...
A. Menghias jaring agar cantik.
B. Menangkap dan menahan serangga agar tidak bisa lepas.
C. Tempat laba-laba tidur siang.
D. Sebagai tangga darurat.

<details>
<summary>💡 Hint</summary>
Setiap bagian jaring punya peran (dekomposisi fungsi). Radial untuk struktur, Spiral untuk perangkap.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menangkap dan menahan serangga.**
Laba-laba adalah insinyur pola alami yang sangat hebat.
</details>

### Soal #132: Perubahan Warna Bunglon
Bunglon berubah warna bukan untuk menyamar saja, tapi juga sebagai pola ekspresi...
A. Lapar atau Haus.
B. Mood (Emosi) dan pengaturan suhu tubuh.
C. Ingin menari.
D. Penuaan usia.

<details>
<summary>💡 Hint</summary>
Warna adalah output visual dari kondisi internal (pola emosi/fisik).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mood dan Suhu.**
Pola warna kulit bunglon adalah indikator status biologisnya.
</details>

### Soal #133: Kunang-kunang yang Kompak
Di beberapa tempat, ribuan kunang-kunang bisa berkedip secara bersamaan (Synchronized). Apa polanya?
A. Ada pemimpin yang memberi aba-aba.
B. Setiap individu menyesuaikan ritme kedipnya sedikit demi sedikit dengan tetangga di sebelahnya sampai frekuensinya sama.
C. Mereka menggunakan jam tangan yang sama.
D. Efek pantulan cermin saja.

<details>
<summary>💡 Hint</summary>
Ini adalah contoh "Emergence" - pola besar yang muncul dari aturan sederhana di setiap individu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan ritme dengan tetangga.**
Pola siklus kedip saling mempengaruhi hingga terjadi harmonisasi masal.
</details>

### Soal #134: Gerombolan Ikan (Schooling)
Ikan berenang bersama dalam pola rapat yang selalu berubah bentuk. Mengapa predator sulit menangkapnya?
A. Karena ikan-ikannya berteriak.
B. Pola gerakan ribuan ikan membuat predator bingung menentukan target tunggal (Efek sensorik overload).
C. Karena airnya menjadi keruh.
D. Karena ikan menjadi sangat besar.

<details>
<summary>💡 Hint</summary>
Banyaknya pola gerak yang pecah membingungkan algoritma visual predator.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Predator bingung menentukan target.**
Pola pertahanan kolektif sangat efektif di dunia hewan.
</details>

### Soal #135: Gerumbul Hewan (Herd)
Saat ada singa, kawanan zebra lari bersamaan. Jika satu zebra belok kiri, yang lain ikut belok kiri. Apa aturannya?
A. Zebra mematuhi rambu lalu lintas.
B. Aturan sederhana: Tetap dekat dengan teman disebelahmu dan jangan menabrak.
C. Mereka sudah janjian di WhatsApp.
D. Zebra paling depan adalah jenderal perang.

<details>
<summary>💡 Hint</summary>
Pola kolektif muncul dari interaksi lokal antar individu (Flocking Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Tetap dekat dan jangan menabrak.**
Tiga aturan (Separation, Alignment, Cohesion) menciptakan pola "Herd" yang kompleks.
</details>

### Soal #136: Gelombang Macet (Phantom Traffic Jam)
Terkadang jalanan macet total, tapi saat sudah jalan, tidak ada kecelakaan atau perbaikan jalan. Mengapa?
A. Ada hantu yang menghalangi jalan.
B. Karena satu mobil ngerem mendadak, menyebabkan pola reaksi berantai pengereman yang merambat ke belakang lebih lambat.
C. Jalanannya sedang lelah.
D. Polisi sengaja menutup jalan diam-diam.

<details>
<summary>💡 Hint</summary>
Ini adalah pola gelombang kejut (Shockwave) dalam aliran partikel.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Reaksi berantai pengereman.**
Pola ini bisa dijelaskan dengan matematika dinamika fluida.
</details>

### Soal #137: Peta MRT/LRT (Topologis)
Garis rute di peta MRT seringkali lurus sempurna atau sudut $45^\circ$, meskipun jalan aslinya berkelok-kelok. Mengapa?
A. Agar hemat tinta print.
B. Karena bagi penumpang, pola koneksi antar stasiun lebih penting daripada lokasi geografis yang akurat.
C. Pembuat petanya malas menggambar tikungan.
D. Supaya keretanya terlihat cepat.

<details>
<summary>💡 Hint</summary>
Penyederhanaan informasi (Abstraksi) dilakukan untuk menonjolkan pola relasi/konektivitas.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Pola koneksi lebih penting.**
Pola ini mempermudah pengguna merencanakan perjalanan tanpa bingung oleh detail jalan raya di atasnya.
</details>

### Soal #138: Persimpangan Bundaran (Roundabout)
Di bundaran, kendaraan yang sudah di dalam lingkaran punya prioritas jalan. Apa tujuannya?
A. Biar mobilnya terus berputar.
B. Menciptakan pola aliran yang kontinu tanpa perlu lampu merah (menghindari kemacetan statis).
C. Biar sopirnya pusing.
D. Sebagai tempat pajangan patung di tengah.

<details>
<summary>💡 Hint</summary>
Dekomposisi tujuan: Menjaga arus tetap mengalir (Flow).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menciptakan pola aliran kontinu.**
Bundaran lebih efisien daripada lampu merah untuk volume kendaraan sedang.
</details>

### Soal #139: Sambungan Jembatan
Di jembatan beton panjang, ada celah bergerigi di setiap beberapa puluh meter. Apa polanya?
A. Celah itu adalah kesalahan konstruksi.
B. Pola celah ekspansi agar jembatan bisa memuai saat panas dan menyusut saat dingin tanpa retak.
C. Agar ban mobil berbunyi "dug-dug".
D. Tempat membuang sampah.

<details>
<summary>💡 Hint</summary>
Pola fisik menyesuaikan dengan perilaku material terhadap perubahan suhu (Pattern of Expansion).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Celah ekspansi untuk pemuaian.**
Insinyur mengenali pola fisika zat padat untuk keamanan infrastruktur.
</details>

### Soal #140: Spillway Waduk
Waduk memiliki saluran pelimpah (spillway). Jika ketinggian air melebihi pola batas tertentu, air akan tumpah otomatis. Apa fungsinya?
A. Biar airnya terlihat seperti air terjun.
B. Mencegah air meluap melewati puncak bendungan yang bisa merusak struktur.
C. Membuang ikan yang terlalu banyak.
D. Memberi air pada sawah di bawah secara gratis.

<details>
<summary>💡 Hint</summary>
Threshold (Ambang batas) adalah mekanisme kontrol berbasis pola data (ketinggian).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencegah kerusakan struktur.**
Sistem pengamanan waduk bekerja berdasarkan pola level air yang terdeteksi.
</details>

### Soal #141: Pitch Kincir Angin
Sudut kemiringan bilah kincir angin berubah mengikuti kecepatan angin. Mengapa?
A. Agar kincirnya terlihat menari.
B. Menyesuaikan pola aliran udara agar energi yang ditangkap tetap maksimal tapi tidak merusak turbin (Pitch Control).
C. Karena bilahnya lembek tertiup angin.
D. Biar burung-burung takut mendekat.

<details>
<summary>💡 Hint</summary>
Optimalisasi variabel Input (angin) menjadi Output (listrik) melalui penyesuaian pola fisik.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Menyesuaikan pola aliran udara.**
Teknologi ini menggunakan sensor pola kecepatan angin untuk optimasi daya.
</details>

### Soal #142: Panel Surya Pelacak (Sun Tracking)
Panel surya yang bisa bergerak mengikuti arah matahari sepanjang hari menghasilkan listrik lebih banyak. Pola geraknya adalah...
A. Bergerak acak mencari sinar paling terang.
B. Mengikuti pola busur matahari dari Timur ke Barat berdasarkan waktu.
C. Diam saja tapi lensanya yang berputar.
D. Berputar cepat seperti baling-baling.

<details>
<summary>💡 Hint</summary>
Matahari memiliki pola harian yang sangat terprediksi.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengikuti pola busur matahari.**
Mengenali pola gerak semu matahari memungkinkan efisiensi energi yang tinggi.
</details>

### Soal #143: Termostat Cerdas
AC inverter baru menurunkan daya listriknya saat suhu ruangan sudah mendekati target. Apa polanya?
A. Pola pendinginan bertahap (Feedback Loop).
B. AC akan mati mendadak lalu nyala lagi.
C. AC meniupkan es batu.
D. Suhu ruangan akan terus turun sampai menjadi beku.

<details>
<summary>💡 Hint</summary>
Algoritma menyesuaikan Output berdasarkan selisih antara Status Saat Ini dan Target.
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Pola pendinginan bertahap.**
Sistem hemat energi mengenali pola suhu untuk mengatur beban kerja kompresor.
</details>

### Soal #144: Siklus Defrost Kulkas
Tersedia pemanas kecil di kulkas yang nyala setiap 8 jam selama 15 menit. Mengapa?
A. Biar makanan di dalam hangat sebentar.
B. Mencairkan pola penumpukan bunga es di evaporator agar sirkulasi udara tetap lancar.
C. Untuk menguji daya tahan lampu kulkas.
D. Biar tagihan listriknya mahal.

<details>
<summary>💡 Hint</summary>
Pola perawatan berkala secara otomatis (Maintenance Pattern).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mencairkan penumpukan bunga es.**
Tanpa pola siklus ini, kulkas lama-lama tidak akan dingin karena tertutup es.
</details>

### Soal #145: Fase Mesin Cuci
Urutan: Timbang Baju -> Isi Air -> Cuci -> Bilas -> Peras.
Jika kamu melihat mesin cuci sedang berputar sangat kencang dan mengeluarkan banyak suara getaran, ia sedang berada di fase...
A. Isi Air
B. Cuci
C. Bilas
D. Peras (Spin)

<details>
<summary>💡 Hint</summary>
Putaran kencang (High Speed) diperlukan untuk membuang air dari serat kain dengan gaya sentrifugal.
</details>

<details>
<summary>✅ Jawaban</summary>
**D. Peras (Spin).**
Mengenali pola aktivitas mesin membantu kita memantau proses kerja alat rumah tangga.
</details>

### Soal #146: Power Level Microwave
Microwave "Low Power" sebenarnya tidak mengecilkan kekuatan gelombang mikronya, tapi menyalakannya secara bergantian (Contoh: 5 detik nyala, 10 detik mati). Apa sebutan pola ini?
A. Pola Rusak.
B. Duty Cycle (Siklus Kerja).
C. Pola Hemat Baterai.
D. Pola Berkedip.

<details>
<summary>💡 Hint</summary>
Rata-rata energi yang dihasilkan dalam satu periode waktu (Dekomposisi waktu).
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Duty Cycle.**
Pola INTERVENSI waktu digunakan untuk mengontrol intensitas energi.
</details>

### Soal #147: Pengereman Regeneratif Mobil Listrik
Saat mobil listrik mengerem, motor berubah menjadi generator dan mengisi baterai. Apa polanya?
A. Mengubah pola energi kinetik (gerak) menjadi energi listrik.
B. Mobil akan meledak jika sering dibalas ngerem.
C. Remnya menggunakan magnet kulkas.
D. Ban mobil akan berputar terbalik.

<details>
<summary>💡 Hint</summary>
Konversi energi secara efisien dengan mengenali pola penggunaan (saat melambat).
</details>

<details>
<summary>✅ Jawaban</summary>
**A. Mengubah pola energi kinetik jadi listrik.**
Dekomposisi pengereman tidak hanya untuk berhenti, tapi juga untuk recovery energi.
</details>

### Soal #148: Logika Lift
Jika kamu di lantai 5 memanggil lift ke bawah, dan lift sedang di lantai 8 sedang turun melewati lantai 6. Apa yang dilakukan lift?
A. Terus ke lantai 1 lalu naik lagi ke lantai 5.
B. Berhenti di lantai 5 untuk menjemputmu karena searah dengan tujuannya.
C. Melewati Anda begitu saja karena dia sombong.
D. Menunggu di lantai 8 sampai kamu memanggil lagi.

<details>
<summary>💡 Hint</summary>
Algoritma lift dirancang untuk rute paling efisien sesuai pola permintaan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Berhenti di lantai 5.**
Pola "Pick up on the way" meminimalkan waktu tunggu dan konsumsi energi.
</details>

### Soal #149: Sensor Eskalator
Eskalator di mall yang sepi bergerak sangat lambat atau berhenti, lalu melaju normal saat ada orang mendekat. Sensor apa yang bekerja?
A. Sensor Berat
B. Sensor Gerak atau Inframerah
C. Sensor Suara langkah kaki
D. Sensor Kehadiran Mall

<details>
<summary>💡 Hint</summary>
Mengenali pola kehadiran manusia di area pintu masuk eskalator.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Sensor Gerak/Inframerah.**
Dekomposisi operasional: Jika tidak ada input (orang), kurangi output (kecepatan) untuk hemat energi.
</details>

### Soal #150: Pintu Otomatis Supermarket
Mengapa pintu otomatis tidak terbuka saat ada kucing lewat tetapi terbuka saat manusia lewat?
A. Pintunya takut pada kucing.
B. Sensor disetel untuk mengenali pola objek dengan ketinggian dan ukuran tertentu (Thresholding).
C. Kucing jalannya terlalu pelan.
D. Karena kucing tidak bawa uang belanja.

<details>
<summary>💡 Hint</summary>
Filter pola digunakan untuk menghindari "false alarm" atau pembukaan pintu yang tidak perlu.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengenali pola ukuran objek.**
Sistem sensor modern melakukan pemilahan pola untuk efisiensi dan keamanan.
</details>

<details>
<summary>✅ Jawaban</summary>
**B. Mengenali pola ukuran objek.**
Sistem sensor modern melakukan pemilahan pola untuk efisiensi dan keamanan.
</details>

