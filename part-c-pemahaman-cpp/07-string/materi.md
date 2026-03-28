# 7. Manipulasi String (Pesan Tersembunyi di Balik Kalimat)
 
 Selamat! Kamu sudah sampai di Modul Tambahan Spesialis OSN-K 2025. Di sini kita akan membahas tipe data yang paling "manusiawi" tapi punya banyak jebakan biner: **`std::string`**.
 
 Di soal OSN-K terbaru, juri sering memutar-mutar kalimat atau mengecek kecocokan karakter (*Pattern Matching*). Jika kamu tidak paham indexing string, kamu akan tersesat di labirin huruf!
 
 ---
 
 ### 📝 Latihan Soal Tracing
 Sudah paham teorinya? Uji ketajaman matamu di sini:
 👉 **[Bank Soal Modul 07: String (Set 01)](./latihan/set-01.md)**
 
 ---
 
 ## 🧵 A. String: Barisan Kursi Penonton (Indexing)
 
 C++ menganggap sebuah `string` bukanlah satu kesatuan padat, melainkan **Array dari Karakter (`char`)**. 
 
 **Analogi Deretan Kursi Bioskop:**
 Jika ada string `string s = "TOKI";`, bayangkan ada 4 kursi bioskop:
 
 | Indeks | 0 | 1 | 2 | 3 |
 |---|---|---|---|---|
 | **Karakter** | 'T' | 'O' | 'K' | 'I' |
 
 > [!IMPORTANT]
 > **Aturan Mutlak:** Selalu mulai dari indeks **0**. Huruf 'T' ada di kursi 0, bukan kursi 1. 
 > Jika kamu memanggil `s[4]`, kamu sedang mencoba duduk di luar gedung bioskop! (*Out of Bounds*).
 
 ---
 
 ## 📏 B. Menghitung Panjang Barisan (`.length()` vs `.size()`)
 
 Untuk tahu berapa banyak kursi yang terisi, C++ menyediakan method `.length()` atau `.size()`. Keduanya **kembar identik** di OSN-K.
 
 ```cpp
 string s = "KOMPUTER";
 int n = s.length(); // n bernilai 8
 ```
 
 **Jebakan Batman:**
 Hati-hati dengan loop yang menggunakan `.length()`.
 ```cpp
 for (int i = 0; i < s.length(); i++) { ... } // AMAN (i sampai 7)
 for (int i = 0; i <= s.length(); i++) { ... } // BAHAYA! (i sampai 8, s[8] tak ada!)
 ```
 
 ---
 
 ## 🔄 C. Operasi Pembalikan (Tracing Mundur)
 
 Juri OSN-K sangat suka menyuruhmu membaca string dari arah belakang menggunakan rumus indeks yang terlihat rumit.
 
 **Rumus Rahasia Baca Belakang:** `s[n - 1 - i]`
 
 ```cpp
 string s = "ABC";
 int n = s.length(); // 3
 for (int i = 0; i < n; i++) {
     cout << s[n - 1 - i];
 }
 ```
 
 **Tracing Human Compiler:**
 1. `i = 0` $\rightarrow$ `s[3 - 1 - 0]` = `s[2]` $\rightarrow$ **'C'**
 2. `i = 1` $\rightarrow$ `s[3 - 1 - 1]` = `s[1]` $\rightarrow$ **'B'**
 3. `i = 2` $\rightarrow$ `s[3 - 1 - 2]` = `s[0]` $\rightarrow$ **'A'**
 *Output:* **CBA**
 
 ---
 
 ## 🧩 D. Pattern Matching Sederhana
 
 Ini adalah soal favorit baru di OSN-K 2025. Mengecek apakah dua string cocok atau mengandung pola tertentu.
 
 ```cpp
 string S = "ABCBAC";
 string T = "BAC";
 bool cocok = true;
 for (int i = 0; i < 3; i++) {
     if (S[i+3] != T[i]) cocok = false;
 }
 ```
 
 **Tracing Logika:**
 - `i = 0` $\rightarrow$ `S[3]` (B) vs `T[0]` (B) $\rightarrow$ Cocok!
 - `i = 1` $\rightarrow$ `S[4]` (A) vs `T[1]` (A) $\rightarrow$ Cocok!
 - `i = 2` $\rightarrow$ `S[5]` (C) vs `T[2]` (C) $\rightarrow$ Cocok!
 *Hasil:* **cocok = true**.
 
 > [!TIP]
 > **Tips Kertas Buram:** Jika ada soal manipulasi string, tuliskan indeks angka (0, 1, 2, ...) di atas setiap hurufnya agar matamu tidak bergeser saat melakukan tracing.
 
 ---
 
 ## 🧮 E. Rahasia ASCII: Angka di Balik Huruf
 
 **Temuan OSN-K:** Sering kali juri meminta kamu mengubah karakter angka `'5'` menjadi nilai integer `5`, atau mengubah huruf kecil menjadi besar.
 
 **Trik Pengurangan Nol (`'5' - '0'`):**
 Karena urutan kode ASCII angka itu berurutan, kamu bisa mendapatkan nilai asli sebuah karakter angka dengan menguranginya dengan karakter `'0'`.
 ```cpp
 char c = '7';
 int angka = c - '0'; // angka bernilai 7 (Integer)
 ```
 
 **Trik Huruf Besar & Kecil:**
 Jarak antara `'a'` (kecil) dan `'A'` (besar) selalu **32**.
 - `'a' - 32` = `'A'`
 - `'A' + 32` = `'a'`
 
 > [!TIP]
 > Jika kamu melihat operasi matematika pada `string` seperti `s[i] - '0'`, jangan bingung! Itu hanyalah cara C++ untuk "memeras" nilai angka murni dari sebuah teks.
 
 ---
 
 ⏩ **Lanjut ke Modul Selanjutnya:** [Dinamis Vector & Matrix 2D (Loker yang Bisa Melar)](../08-vector/materi.md)
 
 [< Kembali ke Part C](../README.md)
