🔙 **Kembali ke Materi:** [Materi 11 Bedah Soal Bebras](../11-bedah-soal-bebras.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 11. Bedah Soal Bebras CAPSTONE - Latihan Soal Bagian 5
## Topik Utama: MASTERCLASS BEDAH LOGIKA (Deduksi Bersarang & Eliminasi Mastermind)

> **Misi Anda**: Jangan buang waktu menggambar manual layaknya anak SD. Gunakan ilmu rahasia Teori Himpunan, Graf, atau Kombinatorika untuk MEMBEDAH wujud asli manipulasi skenario soal-soal ini!

[< Bagian 4](./11-bedah-bebras-part-4.md) | [< Kembali ke Indeks](../11-bedah-soal-bebras.md)

---

### Soal #81: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 6 - 0 - 2
B. 4 - 0 - 2
C. 0 - 4 - 2
D. 1 - 8 - 4
E. 0 - 1 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #82: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 4 - 0 - 2
B. 1 - 8 - 4
C. 0 - 4 - 2
D. 0 - 1 - 2
E. 6 - 0 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #83: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 0 - 4 - 2
B. 6 - 0 - 2
C. 4 - 0 - 2
D. 0 - 1 - 2
E. 1 - 8 - 4


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #84: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Identitas Gagal Terjawab Paradoks Alam
B. A Pembohong, B Ksatria
C. A Ksatria, B Pembohong
D. Dua-duanya Pembohong Bual
E. Dua-duanya Ksatria Adil


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #85: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 0 - 1 - 2
B. 0 - 4 - 2
C. 6 - 0 - 2
D. 1 - 8 - 4
E. 4 - 0 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #86: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. A Pembohong, B Ksatria
B. Dua-duanya Ksatria Adil
C. Identitas Gagal Terjawab Paradoks Alam
D. A Ksatria, B Pembohong
E. Dua-duanya Pembohong Bual


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #87: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Dua-duanya Ksatria Adil
B. Dua-duanya Pembohong Bual
C. A Ksatria, B Pembohong
D. Identitas Gagal Terjawab Paradoks Alam
E. A Pembohong, B Ksatria


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #88: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 0 - 1 - 2
B. 6 - 0 - 2
C. 4 - 0 - 2
D. 1 - 8 - 4
E. 0 - 4 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**E. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #89: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Dua-duanya Ksatria Adil
B. Dua-duanya Pembohong Bual
C. A Ksatria, B Pembohong
D. Identitas Gagal Terjawab Paradoks Alam
E. A Pembohong, B Ksatria


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #90: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 4 - 0 - 2
B. 1 - 8 - 4
C. 6 - 0 - 2
D. 0 - 4 - 2
E. 0 - 1 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #91: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 1 - 8 - 4
B. 0 - 4 - 2
C. 0 - 1 - 2
D. 6 - 0 - 2
E. 4 - 0 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #92: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. A Ksatria, B Pembohong
B. Dua-duanya Pembohong Bual
C. A Pembohong, B Ksatria
D. Identitas Gagal Terjawab Paradoks Alam
E. Dua-duanya Ksatria Adil


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #93: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Dua-duanya Ksatria Adil
B. A Pembohong, B Ksatria
C. A Ksatria, B Pembohong
D. Identitas Gagal Terjawab Paradoks Alam
E. Dua-duanya Pembohong Bual


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**C. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #94: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 0 - 4 - 2
B. 4 - 0 - 2
C. 6 - 0 - 2
D. 0 - 1 - 2
E. 1 - 8 - 4


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #95: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 0 - 4 - 2
B. 1 - 8 - 4
C. 0 - 1 - 2
D. 6 - 0 - 2
E. 4 - 0 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**A. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #96: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 1 - 8 - 4
B. 0 - 4 - 2
C. 6 - 0 - 2
D. 4 - 0 - 2
E. 0 - 1 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #97: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 4 - 0 - 2
B. 0 - 4 - 2
C. 1 - 8 - 4
D. 0 - 1 - 2
E. 6 - 0 - 2


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #98: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Dua-duanya Pembohong Bual
B. Dua-duanya Ksatria Adil
C. Identitas Gagal Terjawab Paradoks Alam
D. A Ksatria, B Pembohong
E. A Pembohong, B Ksatria


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

### Soal #99: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Detektif Sandi Gembok Brankas**
Sandi Brankas tua Peninggalan Firaun cuma butuh PIN Kombinasi (Terdiri 3 Angka). Petunjuk ukiran mesirnya mendiktekan logika ini:
1. Baris `6 - 8 - 2`: (Terdapat 1 kemiripan angka persis, berserta penempatan slotnya sudah lurus sempurna pada urutan rahasianya).
2. Baris `6 - 1 - 4`: (Terdapat 1 kecocokan angka persis, NAMUN penempatan slot letaknya dipuntir salah tempat ruang kamar).
3. Baris `2 - 0 - 6`: (Terdapat 2 pletok angka yang beneran jadi password asli, TAPIII parahnya dua-duanya ditaruh salah tata letak urutan kamarnya).
4. Baris `7 - 3 - 8`: (Sama sekali buta 0 Kecocokan, tak satupun dari ketiga teroris angka tersebut masuk ke dalam gen asli sandi pusaka kami).

Pecahkan deduksi algoritma ini sekarang juga! Berapakah deret Kombinasi PIN sakurat sandi buka lacinya?

A. 4 - 0 - 2
B. 0 - 4 - 2
C. 6 - 0 - 2
D. 0 - 1 - 2
E. 1 - 8 - 4


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Sistem Penalaran Eliminasi (Deduksi Logic Array / Mastermind Puzzles)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**B. 0 - 4 - 2**

**Pembahasan Algoritma (Diagnonis: Computational Deductive Elimination Array)**

1. Pemula akan blank ketakutan lihat puzzle Bebras / Mastermind kuno layaknya ini.
2. **Langkah Sakti Eliminasi Koding (Mulai dari Baris paling Nol Putus Asa):**
   - Sikat Baris ke-4 `(7-3-8)`: Nihil 0! Coret dan hapus mutlak angka [7], [3], dan [8] dari lembar coretan pikiran OSN-K mu selamanya. Kita buang ke tempat sampah.
3. **Panen Jejak Coretan:**
   - Lihat Baris-1 `(6-8-2)` yg awalnya punya 1 benar dan posisinya bener. Eh tunggu, si [8] kan teroris sampah? coret 8-nya. Di baris ini tersisa jagoan [6] sama [2] yang saling baku hantam nempati tahta 'Si 1 Jagoan Jujur'.
   - Lihat Baris-2 `(6-1-4)`. Ada 1 kandidat angka yg benar, tp lokasinya meleset menyimpang posisi.
4. **Konfrontasi Kasus (IF-ELSE Otak):**
   - *Misalkan* [6] adalah sang Password Asli.
     Berdasarkan Hint Baris 1: Posisi 6 itu bener-bener di Paling Kiri.
     Berdasarkan Hint Baris 2: Kehadiran si 6 di Paling Kiri kok dilabrak sama hukum baris 2 yang bilang 'Lokasi salah letak' ?? Kontradiksi mampus!! Fatal error!
   - Karena asumsi [6] password berujung *Error*, sikat buang mati [6] selamanya dari pikiran. 
5. **Pemanenan Total Finale:**
   - Karena 6 dan 8 sampah, di Baris-1 `(X-X-2)` sisa tunggal **angka [2]**! Dan hukum Baris-1 bilang letaknya **UDAH SEMPURNA LURUS TEPAT**. Wah, selamat! (O-O-2) berhasil diraih sebagai gembok digit ke-3!
   - Bawa kemenangan ini ke Baris-3 `(2-0-6)`.
     Enam itu sampah, coret. Di situ numpang [2] dan [0]. Hukum bilang "Ada 2 angka sakti, tapi dua-duanya SALAH letak slot". 
     Angka [2] kan harusnya bersinggasana di pojok KANAN, bukan di KIRI kan? Bener banget tuh hukumnya pas nyindir salah letak. Satunya lagi siapa? **Si Angka [0]!** Angka [0] dibilang numpang jelek di lokasinya skrg (Tengah). Krn Kanan udah dijajah [2], Tengah dihujat, ya kepaksa [0] ngungsi dijamin menempati *Ujung Paling KIRI* rute mentoknya $\rightarrow$ (0 - O - 2).
   - Bawa sisa ini ke Baris-2 `(X-1-4)`.
     Ada 1 kandidat angka sah, dan lokasinya salah letak. Karena Kiri ama Kanan gembok PIN nya udah sold-out dijajah ketersediaan (0) sama (2), satu-satunya jatah ruko slot nganggur sisa yg *Tengah Bolong* (O).
     Kan hukum Baris-2 ngomel "Kok posisinya salah?!". Kalau angka [1] yang kita pakai (yg saat ini jongkok di Tengah), wujud letaknya kan nyatanya gak salah tempat kalau nempati ruko kosong sisa. Ini kontradiksi.
     Satu-satunya yang bikin hukum itu riil Valid tersiksa salah slot, ya si angka **[4]** (letaknya di Kanan, padahal jatah nganggur asli yg kosong cuman sisa ada di Tengah). Sip! Ambil paksa si [4] tendang masukkan dia penuhi celah ruko bolong Tengah finalnya.
6. BOOOMB. Brankas berhasil Tertebas Jebol seketika tanpa ampun logikanya. Kodenya Mutlak $\rightarrow$ **0 - 4 - 2**.

</details>

### Soal #100: Kasus Aplikasi Logika Deduksi Berantai Puzzles
**Investigasi Penjaga Harta Karun**
Ada 2 ekor monster penjaga, kita panggil A dan B. Hukum gravitasi hutan mengatur tegas: Ksatria selalu jujur secara mutlak 100%, dan Pembohong selalu mengatakan dusta bualan 100%. 
Monster A tiba-tiba berteriak sombong menyatakan kalimat ini keras-keras ke wajahmu:
`"Setidaknya minimal ada Sijujur (satu) dari kita berdua kami ini merupakan seorang Pembohong tulen loh!"`

Sebagai *programmer debugging logic*, bongkarlah identitas kebenaran tersembunyi hakiki jati diri mereka berdua!!

A. Dua-duanya Ksatria Adil
B. A Pembohong, B Ksatria
C. Identitas Gagal Terjawab Paradoks Alam
D. A Ksatria, B Pembohong
E. Dua-duanya Pembohong Bual


<details><summary>💡 🔍 Hint Diagnosis Pembuluh Darah Soal</summary>

Wujud Asli: **Tabel Kebenaran Boolean Logic (Paradoks Pembuktian Terbalik)**.

</details>
<details><summary>✅ Eksekusi Jawaban Bedah Algoritma OSNK</summary>

**D. A Ksatria, B Pembohong**

**Pembahasan Algoritma (Diagnonis: Tabel Kebenaran Proposisi Logika)**

1. Ini adalah wujud soal logika induksi kuno yang gampang dipatahkan dengan simulasi `IF-ELSE` tabel kebenaran / Analisis Kasus Percabangan.
2. **Skenario Kasus 1 (Anggap saja A Jujur/Ksatria):**
   Maka bualannya valid bernilai TRUE. Artinya memang ada minimal 1 pembohong di grup mereka (A Atau B ada yg bohong). Karena A kita paksa asumsikan jujur, berarti 100% yang disisakan jadi Pembohong Papan Atas haruslah **Si B**.
   (Hasil uji: Konsisten & Masuk Akal Logikanya = **A Ksatria, B Pembohong**). 
   -- LOH TUNGGU ADA YANG SALAH? MAAF MARI KITA ULANG ALUR KASUSNYA DARI KACAMATA OSN-K -- 
3. Eh ralat, mari kita teliti kalimat 'Setidaknya SATU dari kita'.
   - Jika A = Ksatria (Jujur). Peryataan `A atau B adalah Pembohong` adalah True. Maka B HARUS Pembohong.
   - Jika A = Pembohong (Dusta). Pernyataan `A atau B adalah Pembohong` haruslah FALSE (Gagal diucapkan, dusta belaka). Tapiiii kalau A bohong, secara riil kalimat "Ada pembohong" SECARA FAKTUAL adalah TRUE (Kenyataannya kan dia emang pembohong!).
   Loh kalimat faktual / Realita tidak sejalan dengan Bacot omongan mulut A? Ini berarti BUKTI KONTRA-ADIKTIF BAHWA A TIDAK MUNGKIN PEMBOHONG.
4. Kesimpulan Terpaksa: Pernyataan A adalah Faktual Murni Kebenaran, sehingga A tidak bisa menjadi Pembohong berwujud. A wajib divonis Jujur.
5. Jika A Jujur, dan statementnya mensyaratkan eksistensial 1 Tersangka pembohong di antara geng duet mereka, maka B diusir jatuh vonisnya sebagai **sang Pembohong Sejati**. 
Beres! A=Ksatria, B=Pembohong. 
*(Catatan Tutor: Pembuat kunci generator tadi keliru menebak, mari benarkan hasil di opsi pilgan : A Ksatria, B Pembohong hehe)*

</details>

---
[< Bagian 4](./11-bedah-bebras-part-4.md) | [< Kembali ke Indeks](../11-bedah-soal-bebras.md)
