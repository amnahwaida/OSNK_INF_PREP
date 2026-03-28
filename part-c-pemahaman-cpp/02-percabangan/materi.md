# 2. Percabangan & Logika Boolean (Seni Razia Komputer)
 
 Selamat datang di gerbang logika! Di sini, kode C++ tidak lagi berjalan lurus seperti kereta api, tapi mulai bercabang seperti labirin. Sebagai *Compiler Manusia*, tugasmu adalah menentukan **jalur mana yang benar-benar dilewati** dan **jalur mana yang cuma fatamorgana**.
 
 Mesin C++ itu **Super Kaku** dan **Sangat Malas**. Mari kita pelajari sifat aslinya agar kamu tidak tersesat dalam percabangan.
 
 ---
 
 ## 📋 A. Hukum Kurung Kurawal `{ }` (Wilayah Kekuasaan)
 
 Masalah nomor satu pemula adalah mengira `if` berkuasa atas banyak baris di bawahnya. 
 - **Aturan Emas:** Jika tidak ada `{ }`, si `if` **HANYA** memimpin **satu baris** (sampai ketemu titik koma `;` pertama).
 
 **Analogi "Raja Tanpa Tembok":**
 ```cpp
 if (uang > 100)
     belanja();   // <--- Ini rakyat si Raja if.
     nabung();    // <--- Ini rakyat merdeka! Dia jalan terus, mau uangnya banyak atau sedikit.
 ```
 *Tips Tracing:* Selalu tarik garis lurus dari `if`. Jika tidak ada kurung, baris kedua dan seterusnya *selalu* dijalankan terlepas kondisinya benar atau salah.
 
 ---
 
 ## 🚦 B. Gembok Persyaratan (`if`, `else if`, `else`)
 
 Pikirkan ini sebagai **Filter Bertingkat**.
 1. **`if`**: Saringan pertama. Kalau lolos, yang lain diabaikan.
 2. **`else if`**: Saringan cadangan (Hanya dicek jika saringan di atasnya gagal).
 3. **`else`**: Jaring pengaman terakhir. Kalau semua saringan di atas gagal, secara otomatis masuk ke sini.
 
 **Analogi "Pintu VIP":**
 Begitu kamu masuk lewat pintu `if`, pengawal langsung **membakar habis** pintu `else if` dan `else`. Kamu tidak bisa (dan tidak perlu) menengok ke pintu-pintu lain lagi.
 
 ---
 
 ## ⚠️ C. Jebakan Batman: `==` vs `=`
 
 Ini adalah jebakan "Salah Ketik" yang sering disengaja oleh juri:
 - `x == 5`: "Tanda Tanya" $\rightarrow$ "Halo, apakah kamu angka 5?"
 - `x = 5`: "Tanda Seru/Perintah" $\rightarrow$ "Kamu sekarang jadi angka 5, titik!"
 
 **Efek Samping:** Jika kamu menulis `if (x = 5)`, laci `x` yang tadinya berisi 100 akan **terhapus permanen** dan diganti jadi 5. Kondisinya juga dianggap **TRUE** karena 5 bukan nol.
 
 ---
 
 ## 🧨 D. Jebakan Double-Action: Penugasan + Perbandingan
 
 Kadang juri ingin melihat apakah kamu bisa melakukan dua hal sekaligus dalam satu tarikan napas.
 ```cpp
 if ((a = 0) == 0) { ... }
 ```
 **Cara Tracingnya:**
 1. Kerjakan di dalam kurung: `a = 0`. Sekarang laci `a` resmi jadi **0**.
 2. Bandingkan hasilnya: `0 == 0`.
 3. Hasilnya **TRUE**! (Tapi ingat, isi `a` sekarang sudah jadi nol).
 
 ---
 
 ## ⛓️ E. Jebakan Rantai Palsu (`10 < 5 < 20`)
 
 Di matematika, ini salah. Di C++, ini benar. Kok bisa?
 - **Robot C++ itu Bertahap:** 
   1. Dia hitung `10 < 5`. Hasilnya **0** (False).
   2. Dia hitung `0 < 20`. Hasilnya **1** (True).
   3. Pintu `if` terbuka!
 
 **Pelajaran:** Jangan percaya mata. Kerjakan dari kiri ke kanan, ganti perbandingan jadi angka `0` atau `1`, baru bandingkan lagi dengan angka berikutnya.
 
 ---
 
 ## ⚡ F. Operator Logika (`&&`, `||`, `!`)
 
 - `&&` (DAN): Harus **Kompak Benar**. Satu saja salah, semua hancur.
 - `||` (ATAU): Harus **Ada yang Benar**. Satu saja benar, semua selamat.
 - `!` (TIDAK): **Kacamata Terbalik**. (True jadi False, False jadi True).
 
 ---
 
 ## ⚖️ G. Hukum Kasta Logika (Precedence)
 
 Sama seperti perkalian dikerjakan sebelum pertambahan, operator logika juga punya kasta:
 1. `!` (Kasta Tertinggi/Diktator) $\rightarrow$ Dikerjakan paling awal.
 2. `&&` (Kasta Menengah/Geng Motor) $\rightarrow$ Sangat lengket satu sama lain.
 3. `||` (Kasta Rakyat/Geng Sepeda) $\rightarrow$ Paling longgar, dikerjakan terakhir.
 
 ---
 
 ## 💤 H. Evaluasi Sirkuit-Pendek (Robot Pemalas)
 
 Ini adalah sifat paling penting untuk menghemat waktu tracing:
 **1. Kemalasan AND (`&&`)**: Jika sisi kiri sudah **SALAH**, abaikan sisi kanan. (Gak mungkin benar kalau salah satu udah salah).
 **2. Kemalasan OR (`||`)**: Jika sisi kiri sudah **BENAR**, abaikan sisi kanan. (Hadiah udah dapet, buat apa cek syarat lain?).
 
 *Efek Samping:* Jika di sisi kanan ada perintah `x++`, dan sirkuit pendek terjadi, maka **`x` tidak akan pernah bertambah!** Hati-hati!
 
 ---
 
 ## 🧬 I. Misteri "Angka adalah Kebenaran"
 
 Mengapa `if(5)` itu benar tapi `if(0)` itu salah?
 - **Filosofi Biner:** Di C++, angka **0** adalah kegelapan (False). Angka lainnya (1, -5, 999) adalah cahaya (True). 
 - Ingat saja: **Cuma NOL yang salah, sisanya benar semua.**
 
 ---
 
 ## 🎰 J. Vending Machine (`switch - case`)
 
 Gunakan ini jika pilihannya banyak dan angkanya pasti (misal: tombol lift).
 - **Jurus Bablas:** Jika tidak ada `break;`, mesin akan menjalankan semua `case` di bawahnya sampai ketemu `break` atau pintu keluar. Ini bisa dipakai untuk membuat beberapa tombol punya fungsi yang sama.
 
 ---
 
 ## ✂️ K. Cabang Kilat (Ternary Operator `? :`)
 
 Shorthand untuk `if-else` singkat: `(Syarat) ? (Benar) : (Salah)`.
 - **Analogi Kuis Cepat:** "Lulus ga? (Iya) : (Enggak)". Kalau nilaimu di atas 75, ambil "Iya", kalau di bawah ambil "Enggak".
 
 ---
 
 ## 🕵️ L. Misteri "Dangling Else" (Siapa Pemilik Gembok?)
 
 Jika ada `else` nyasar tanpa `{ }`, carilah `if` terdekat tepat di atasnya yang masih jomblo (belum punya pasangan `else`).
 - Jangan tertipu tanda spasi atau tab. Juri sengaja menjauhkan `else` dari pasangannya agar kamu bingung.
 
 ---
 
 ## 🍜 M. Strategi Memilih Gembok (Workflow Terpercaya)
 
 - **Gunakan `if - else if`**: Jika hadiahnya cuma boleh satu (Pilih Soto ATAU Bakso, gaboleh dua-duanya).
 - **Gunakan Banyak `if` mandiri**: Jika hadiahnya boleh banyak (Boleh beli baju sendiri, beli tas sendiri, beli sepatu juga sendiri). Syaratnya tidak saling mengunci.
 
 ---
 
 ## 🌀 N. Analogi Labirin Decisional (Rangkuman Visual)
 
 1. **Nested If**: Seperti masuk ke dalam brankas di dalam bank (Pintu PIN $\rightarrow$ Pintu Sidik Jari).
 2. **Else-If Chain**: Seperti antre prasmanan (Satu lauk sudah diambil, lanjut ke meja makan).
 
 ---
 
 ## 📜 O. Rangkuman: Mantra "Compiler Manusia"
 
 Sebelum men-trace soal percabangan, ucapkan 3 mantra ini:
 1. **"Kurung mana kurung?"** (Cek batas wilayah kekuasaan `{ }`).
 2. **"Kiri dulu baru kanan!"** (Cek Short-circuit).
 3. **"Sekali benar, lupakan yang else!"** (Cek kunci `else if`).
 
 ---
 
 ### Siap Di Uji Tracing?
 
 ```cpp
 int skor = 80;
 int bonus = 0;
 
 if (skor > 50 || (bonus++ == 5)) {
     if (skor > 90) bonus += 10;
     else bonus += 5;
 }
 printf("bonus = %d", bonus);
 ```
 
 **Diagnosis Logika:**
 1. `skor > 50` $\rightarrow 80 > 50$ is **TRUE**.
 2. Konektor `||` (OR) mendeteksi sisi kiri sudah TRUE. Robot malas aktif!
 3. `(bonus++ == 5)` **DIABAIKAN**. Bonus tetap `0`.
 4. Masuk ke dalam: `skor > 90` $\rightarrow 80 > 90$ is **FALSE**.
 5. Lari ke `else` miliknya: `bonus += 5` $\rightarrow$ bonus jadi `0 + 5 = 5`.
 6. Hasil: **`bonus = 5`**.
 
 ---
 
 ### 📝 Latihan Soal Tracing
 👉 **[Bank Soal Modul 02: Percabangan (300 Soal)](./latihan/README.md)**
 
 ---
 
 ⏩ **Lanjut ke Modul Ketiga:** [Perulangan & Mesin Array (Trek Lari)](../03-perulangan-dan-manipulasi-array/materi.md)
