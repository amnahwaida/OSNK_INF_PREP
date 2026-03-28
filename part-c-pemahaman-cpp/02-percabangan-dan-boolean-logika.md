# 2. Percabangan & Logika Boolean (Seni Razia Komputer)

Sekarang saatnya kamu menjadi Pak Dengklek sebagai Polisi Gerbang Tol (atau Guru BP).
Kode di OSN-K penuh dengan blok pengawal keamanan yang disebut **Percabangan (`if`, `else if`, `else`)** yang dirakit menggunakan gembok kode **Logika Boolean (`&&` AND, `||` OR)**.

Mesin C++ itu **Super Kaku** dan **Super Egois Pemalas**. Mari kita bongkar anatomi kedua sikap buruk mesin ini supaya kamu tidak terjebak men-Trace cabang yang salah.

---

## 🚦 A. Gembok Persyaratan (Kaku dan Buta Masa Lalu)

Percabangan `if` menuntut pelacakan variabel di lembar buram-mu harus **100% presisi**.

```cpp
int nyawa = 5;

if (nyawa > 5) {
    printf("Bos Nyala");
} else if (nyawa == 5) {
    printf("Siaga Satu");
} else {
    printf("Game Over");
}
```

**Analisis Compiler Manusia-mu:**
- Baris `if (nyawa > 5)`: Apakah $5$ lebih besar dari $5$? **SALAH (FALSE)**! ($5$ itu sama besar, bukan lebih besar). Karena itu, blok ini otomatis mental.
- Baris `else if (nyawa == 5)`: Apakah $5$ sama presisi eksak seidentik-identiknya dengan $5$?  **BENAR (TRUE)**. Cetak `Siaga Satu`.

### ⚠️ Jebakan Batman #3: Ketipu Tanda Sama Dengan Ganda (`==` vs `=`)
Hati-hati, OSN Informatika hobinya memakan *kewarasan* matamu:
- `x == 5`: Ini TANDA TANYA *"Apakah X itu 5?"*
- `x = 5`: Ini TANDA PERINTAH MUTLAK *"Ganti isi kotak X sekarang jadi bernilai 5, bodo amat tadinya isi apa!"*
Jadi kalau ketemu jebakan bodoh di percabangan:
```cpp
int x = 10;
if (x = 5) { // <--- JEBAKAN JAHAT INI VALID DI C++!
   // x benar-benar diobrak abrik jadi 5, dan kondisinya dianggap TRUE!
}
```
*(Tapi santai, standard etika silabus OSN-K Indonesia jarang mengeluarkan trik jahat receh syntax C++ level begini, rata-rata soal pure berfokus di algoritmanya).*

---

## 💤 B. Evaluasi Sirkuit-Pendek (Kemalasan Paripurna Mesin C++)

Nah ini dia **Senjata Utama Level Dewa** di kodingan panjang OSN-K. Seringkali percabangan menggunakan konektor ganda:
- `&&` (DAN / AND): DUA-DUANYA WAJIB BENAR!
- `||` (ATAU / OR): CUKUP SALAH SATU AJA BENAR, BERES!

Apa rahasianya? Mesin C++ itu sifatnya egois memikirkan jalan pintas (**Short-Circuit Evaluation**).

### 1. Kemalasan AND (`&&`) -> *Razia BP Rambut & Kaos Kaki*
Bayangkan peraturan BP Sekolah: 
> *"Kamu akan diusir pulang `JIKA (Rambut Gondrong && Kaos Kaki Bebas)`."*

Sistem kerja Guru BP (C++): Beliau narik murid satu-satu. Cek kepalanya. Eh ternyata rambut sang murid **Pendek / Cukur Rapi (FALSE untuk gondrong)**. 
Apakah Guru BP sudi menengok melihat sepatu/kaos kaki murid itu? **NGGAK PENTING!** Tentu aja NGGAK! Toh, rambutnya aja udah nggak gondrong, syarat `&& (DAN DUA-DUANYA)` udah pasti ambyar gagal total. Guru BP langsung tendang murid itu untuk masuk kelas tanpa melirik kaos kaki!

**Hukum Sirkuit-Pendek AND:**
Dalam `A && B`, **JIKA KONDISI `A` SUDAH FALSE (SALAH)**, C++ **BUTA DAN MENOLAK MEMBACA KONDISI `B`!** Murni ter-skip diabaikan!

### 2. Kemalasan OR (`||`) -> *Event Undian Mobil*
Bayangkan syarat dapat Mobil di Mall: 
> *"Kamu berhak menang `JIKA (Kupon Nomor 1 Tembus || Kupon Nomor 2 Tembus)`."*

Sistem C++: Menggosok Kupon Nomor 1. Eh, isinya **JACKPOT!! (TRUE)**.
Apakah sistem masih capek-capek menggosok melihat isi Kupon Nomor 2? **TIDAK PERLU!** Karena syarat `||` (ATAU), asal ada SATU saja yang nyantol lunas, seluruh gerbang tol langsung terbuka lebar kegirangan!

**Hukum Sirkuit-Pendek OR:**
Dalam `A || B`, **JIKA KONDISI `A` SUDAH TRUE (BENAR)**, C++ **BUTA DAN MENOLAK MEMBACA KONDISI `B`!** Pintu sukses langsung jebol saat iterasi pertama.

---

### Siap Di Uji Tracing?

Menguji tingkat kewaspadaan matamu sebagai *Compiler*:
```cpp
int uang = 100;
int dompet = 0;

if (uang > 500 && (dompet++ > 0)) {
    printf("Miliarder\n");
} else {
    printf("Dompet = %d", dompet);
}
```
*(Catatan: `dompet++` berfungsi menambah nyawa `dompet` sebesar 1 sesai evaluasi).*

**Diagnosis Logika Papan Tulis Juri C++:**
1. Mesin masuk ke `if (uang > 500)`. Apakah `100` lebih besar dari `500`? **BENAR-BENAR SALAH (FALSE)**!
2. Di sebelah teks ada konektor `&&`. 
3. *Short-Circuit Mode ON!* Karena sayap Kiri sudah **FALSE**, seluruh kalimat di kanan dipotong / dibuang sama mesin. C++ **MENOLAK** menjalankan `(dompet++ > 0)`.
4. Akibat hukum pemalasan ini, baris manipulasi mutasi `dompet++` sama sekali TIDAK PERNAH DIJALANKAN SEJARAH BUMI! Variable `dompet` tetap perawan tak tersentuh di angka `0`.
5. Mesin melompat ke `else`.
6. Teks mencetak mutlak `Dompet = 0`.

Apabila kamu dengan lugu mencetak "Dompet = 1" di jawaban Silangmu, kamu baru saja termakan ilusi dan kehilangan poin krusial OSN-K milikmu. Berhati-hatilah dengan egoisme mesin C++!

⏩ **Lanjut ke Modul Ketiga:** [Perulangan & Mesin Array (Trek Lari & Playlist Spotify)](./03-perulangan-dan-manipulasi-array.md)
