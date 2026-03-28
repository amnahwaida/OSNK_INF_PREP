# 8. Dinamis Vector & Matrix 2D (Loker yang Bisa Melar)
 
 Selamat datang di modul puncak! Jika Array di Modul 03 adalah deretan lemari kayu yang ukurannya kaku, maka **`std::vector`** adalah lemari ajaib yang bisa meluas secara otomatis setiap kali kamu memasukkan barang baru.
 
 Di OSN-K 2025, `vector` menjadi primadona karena juri tidak perlu menentukan ukuran array di awal. Mereka bisa terus "melempar" angka ke dalam fungsi.
 
 ---
 
 ### 📝 Latihan Soal Tracing
 Sudah paham teorinya? Uji ketajaman matamu di sini:
 👉 **[Bank Soal Modul 08: Vector (Set 01)](./latihan/set-01.md)**
 
 ---
 
 ## 🎈 A. Apa itu Vector? (Prasyarat: Paham Array Dasar)
 
 Vector adalah cara C++ mengelola daftar data yang ukurannya bisa berubah-ubah saat program jalan. Kamu butuh `#include <vector>` untuk mengaktifkannya.
 
 **Analogi Loker Karet:**
 Di loker kayu (Array), kamu pesan 5 kotak, maka selamanya 5 kotak.
 Di loker karet (Vector), kamu mulai dengan 0 kotak, lalu setiap kali kamu panggil **`push_back()`**, loker itu akan menambah 1 kotak baru di bagian paling belakang.
 
 ```cpp
 vector<int> v; // Loker kosong
 v.push_back(10); // Loker berisi [10], size = 1
 v.push_back(20); // Loker berisi [10, 20], size = 2
 ```
 
 ---
 
 ## 📏 B. Operasi Dasar Vector
 
 1. **`.push_back(nilai)`**: Menambah elemen ke ujung belakang.
 2. **`.pop_back()`**: Membuang elemen paling belakang (Loker terakhir dicabut).
 3. **`.size()`**: Menghitung berapa banyak isi loker sekarang.
 4. **`v[i]`**: Mengakses isi loker ke-i (Sama persis seperti Array, mulai dari 0).
 
 **Contoh Tracing Cepat:**
 ```cpp
 vector<int> v = {1, 2, 3};
 v.push_back(4); 
 v.pop_back(); 
 v.push_back(5);
 cout << v.size() << " " << v[3];
 ```
 **Analisis:**
 - Start: `[1, 2, 3]` (size 3)
 - `push_back(4)` $\rightarrow$ `[1, 2, 3, 4]` (size 4)
 - `pop_back()` $\rightarrow$ `[1, 2, 3]` (size 3)
 - `push_back(5)` $\rightarrow$ `[1, 2, 3, 5]` (size 4)
 - *Output:* **4 5**
 
 ---
 
 ## 🧱 C. Matrix 2D (Vector of Vectors)
 
 Ini adalah jebakan maut di soal "Rahasia Petak" OSN-K 2025. Sebuah vector yang isinya adalah vector lain.
 
 ```cpp
 vector<vector<int>> matriks;
 ```
 
 **Analogi Rak Dokumen:**
 `matriks` adalah sebuah rak besar. Setiap laci di dalam rak tersebut (indeks baris) berisi satu map plastis yang di dalamnya ada banyak kertas (indeks kolom).
 
 **Akses Data:** `matriks[baris][kolom]`
 - `matriks[0][1]` artinya Baris ke-0, Kolom ke-1.
 
 **Contoh Tracing Matriks:**
 ```cpp
 vector<vector<int>> B = {{1, 2}, {3, 4}};
 cout << B[1][0]; // Baris 1, Kolom 0
 ```
 **Analisis:**
 - Baris 0 adalah `{1, 2}`.
 - Baris 1 adalah `{3, 4}`.
 - Kolom 0 dari Baris 1 adalah **3**.
 
 ---
 
 ## ⚠️ D. Hati-hati dengan `.size()` dalam Loop
 
 Di soal OSN-K 2025 (Soal 35), ada fungsi `RAHASIA(vector<int> A)`. 
 Seringkali juri melakukan perbandingan `A[j] > A[i]` di dalam *nested loop* (loop di dalam loop) yang batasnya adalah `A.size()`.
 
 **Strategi Jitu:**
 Jika kamu melihat `vector` di soal OSN-K, segera buat kotak-kotak di kertas burammu. Beri label indeks di bawahnya (0, 1, 2, ...). Jangan menebak-nebak jumlah elemen hanya dari pandangan mata, karena `push_back` bisa terjadi di tengah jalan!
 
 ---
 
 ## 🔍 E. Teknik Pencarian Biner (Binary Search)
 
 **Temuan OSN-K 2024:** Sering ada fungsi rekursif yang membagi rentang `[kiri, kanan]` menjadi dua menggunakan `mid`. 
 
 **Analogi Merobek Buku:**
 Jika kamu mencari halaman 50 di buku setebal 100 halaman, kamu buka tengahnya (halaman 50). Kalau ketemu, selesai! Kalau kegedean, cari di sebelah kiri. Kalau kekecilan, cari di sebelah kanan.
 
 ```cpp
 bool binCheck(vector<int> A, int L, int R, int X) {
     if (L > R) return false;
     int mid = (L + R) / 2;
     if (A[mid] == X) return true;
     if (A[mid] > X) return binCheck(A, L, mid - 1, X);
     else return binCheck(A, mid + 1, R, X);
 }
 ```
 
 **Trik Kecepatan OSN-K:** 
 - Jika data jumlahnya $N=1024$, Binary Search hanya butuh **10 langkah** ($\log_2 1024$).
 - Jika waktu untuk $N=1000$ adalah 20 detik dan $N=2000$ adalah 22 detik, itu ciri khas **Logarithmic Scaling**. Waktunya cuma nambah dikit meskipun datanya dobel!
 
 ---
 
 ## 🤝 F. Logika Dua Penunjuk (Two-Pointers & Merge)
 
 **Temuan OSN-K 2022:** Menggabungkan dua baris antrean terurut menjadi satu barisan panjang.
 
 **Analogi Resleting:**
 Kamu punya dua baris resleting. Kamu bandingkan gigi terdepan dari kedua baris. Mana yang lebih kecil, dia yang masuk ke barisan baru duluan. Terus begitu sampai semua gigi terpakai.
 
 ```cpp
 while (i < 5 && j < 5) {
     if (A[i] <= B[j]) {
         C[k] = A[i]; i++;
     } else {
         C[k] = B[j]; j++;
     }
     k++;
 }
 ```
 
 > [!TIP]
 > Jika ada dua indeks (seperti `i` dan `j`) yang berjalan di dua array berbeda secara bersamaan, itu adalah **Two-Pointers**. Fokuslah pada siapa yang "kalah" (nilainya lebih kecil) karena dialah yang akan berpindah indeks.
 
 ---
 
 🏁 **Selamat!** Kamu telah menyelesaikan seluruh materi **Pemahaman Kode C++**. 
 Sekarang kamu siap menghadapi **[Paket Simulasi OSN-K](../../simulasi-osnk/README.md)** yang sesungguhnya!
 
 [< Kembali ke Part C](../README.md)
