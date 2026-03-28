# 08. Teori Himpunan (Belajar Ngelompokin Gabungan Data)

> "Pernah nggak sih kamu disuruh ngumpulin data teman sekelas? Ada yang suka Bakso, ada yang suka Mi Ayam, ada yang suka KEDUANYA, dan ada yang nggak suka dua-duanya. Nah, selamat datang di dunia **Himpunan**!"

Di OSN-K Informatika, Teori Himpunan ini gampang banget tapi super penting. Kenapa? Karena logika himpunan ini dipakai setiap hari oleh programmer buat *nyari data* di *database* (kayak pas kamu lagi pakai fitur *filter* barang di Shopee atau Tokopedia).

Yuk, kita bahas pelan-pelan pakai perumpamaan sehari-hari!

---

## 📦 1. Kenalan Dulu: Apa Itu Himpunan?

**Himpunan (Set)** itu sederhananya adalah **sebuah wadah, keranjang, atau grup** yang isinya benda-benda atau angka-angka yang jelas batasannya. Isi dari wadah itu disebut **anggota**.

**Contoh Gampang:**
- Keranjang $A$ = {Budi, Siti, Anton}
- Keranjang $B$ = {1, 3, 5, 7, 9} (Isinya cuma angka ganjil di bawah 10)

### Aturan Main Keranjang (Wajib Ingat!):
1. **Nggak Boleh Ada yang Kembar:** Kalau kamu nulis {1, 2, 2, 3}, komputer bakal otomatis ngapus angka 2 yang dobel. Jadinya cuma {1, 2, 3} aja. Sebuah keranjang himpunan nggak peduli seberapa banyak kamu masukin barang yang sama, dia cuma ngitung "jenisnya" aja.
2. **Urutan Nggak Ngaruh:** Nulis {A, B, C} itu persis sama dengan {C, A, B}. Nggak ada istilah ranking satu atau dua, yang penting bareng-bareng di dalam satu keranjang.

**Istilah Keren (Biar Kayak Anak OSN):**
- **Kardinalitas** (ditulis $|A|$ atau $n(A)$): Ini cuma bahasa Matematika buat **"Ada berapa sih jumlah anggotanya?"**.
  - Contoh: Keranjang $A$ = {Budi, Siti, Anton}. Jumlah anggotanya 3 orang, berarti $|A| = 3$. Gampang kan?
- **Himpunan Semesta ($S$)**: Ini "Dunia"-nya. Misal kita lagi bahas anak basket di sekolah, berarti semestanya ya **semua murid di sekolah itu**. Nggak usah mikirin murid dari sekolah lain.
- **Himpunan Kosong ($\emptyset$)**: Sesuai namanya, keranjang nol putul. Nggak ada isinya sama sekali. Jumlah anggotanya = 0.

---

## 🎨 2. Mencampur & Memisah Keranjang (Operasi Himpunan)

Biar gampang bayanginnya, di sekolahmu ada 2 wadah ekskul:
- Wadah ekskul $A$ (Anak Basket) = {Budi, Siti, **Andi**}
- Wadah ekskul $B$ (Anak Paskibra) = {**Andi**, Cici, Dedi}

Nah, operasi himpunan itu ibarat kita ngutak-ngatik isi kedua wadah ini.

### A. Gabungan / Union (Simbolnya: $\cup$ kayak Mangkok kebuka)
Ini ibarat kepala sekolah bilang: **"Kumpulin semua anak Basket ATAU Paskibra ke lapangan!"**.
- Kuncinya: kata **ATAU** (huruf 'U' di kata ata**U** mirip simbol $\cup$).
- Tuang semua isi wadah A dan B ke lapangan. Tapi ingat aturan #1: **Yang main dua ekskul cuma dihitung SEKALI badannya**. Si Andi jangan dihitung jadi dua orang!
- $A \cup B$ = {Budi, Siti, Andi, Cici, Dedi}

### B. Irisan / Intersection (Simbolnya: $\cap$ kayak Topi/Mangkok kebalik)
Ini ibarat kepala sekolah nyari anak yang **super sibuk**. Anak yang ikut ekskul Basket **DAN** Paskibra sekaligus.
- Kuncinya: kata **DAN** (huruf 'n' di kata da**n** mirip simbol $\cap$).
- Siapa nama yang muncul di wadah A, tapi JUGA MUNCUL di wadah B? Yap, si Andi.
- $A \cap B$ = {Andi}

### C. Kurang-kurangan / Selisih (Simbolnya: $-$)
Kepala sekolah bilang: **"Saya minta anak yang HANYA ikut Basket. Tolong usir kalau ada yang ternyata ikut Paskibra juga."**
- Caranya: Ambil semua anak Basket (Wadah $A$), lalu cek satu per satu. Lho, ternyata Andi diam-diam ikut Paskibra juga. Yasudah, coret nama Andi dari daftar ini.
- $A - B$ = {Budi, Siti}
- *Hati-hati:* $A - B$ beda banget sama $B - A$. Kalau $B - A$ berarti nyari anak Paskibra murni (Hanya Paskibra) = {Cici, Dedi}. Jangan kebolak!

### D. Komplemen / "Selain" (Simbolnya: $A^c$)
Ucapkan kata ajaib: **"SAYA CARI SE--LA--IN..."**
- $A^c$ artinya: Coba kumpulin semua anak satu sekolah (Ingat si Himpunan Semesta $S$?), tapi tolong usir anak yang ikut Basket. Sisa anak yang nggak ikut ekskul basket itulah si komplemen.

---

## 📊 3. Gambar Adalah Penyelamat (Diagram Venn)

Materi ini biasanya disajikan dalam soal cerita OSN-K yang panjang lebar. **KUNCI RAHASIA MENJAWABNYA CUMA SATU: GAMBAR LINGKARANNYA (Diagram Venn)!** Jangan pernah coba bayangin dan ngitung diawang-awang.

- Kotak besar melambangkan seluruh sekolah (Semesta).
- Lingkaran A untuk keranjang Basket, Lingkaran B untuk keranjang Paskibra.

```
       KOTAK SEMESTA (S) = Semua Siswa di Sekolah
 _________________________________________
|                                         |
|  (BASKET - A)            (PASKIBRA - B) |
|    ________                ________     |
|   /        \              /        \    |
|  /          \            /          \   |
| |   Budi     \   ANDI   /    Cici    |  |
| |   Siti      |--------|     Dedi    |  |
| |            / (Irisan) \            |  |
|  \          /            \          /   |
|   \________/              \________/    |
|                                         |
|          Eka, Fajar (Anak Rumahan/Luar) |
|_________________________________________|
```

**Cara Gampang Bacanya (Analisis Wilayah):**
- Balon Kiri KOPONG, yang nggak numpuk (isinya Budi, Siti) = Daerah anak yang **HANYA Ikut Basket**.
- Balon Kanan KOPONG (isinya Cici, Dedi) = Daerah anak yang **HANYA Ikut Paskibra**.
- Jembatan Tengah yang numpuk (isinya Andi) = Daerah anak yang **Ikut DUA-DUANYA (Irisan)**.
- Padang Rumput Area Luar (isinya Eka, Fajar) = Daerah anak yang **NGGAK IKUT APA-APA**.

---

## 🧮 4. Rumus Anti-Dobel (Prinsip Inklusi-Eksklusi)

Ini dia materi himpunan yang **pasti keluar** di OSN! Fungsinya untuk ngitung jumlah orang yang digabungkan, biar nggak ada hitungan yang dobel.

### Kasus 2 Lingkaran (Level Gampang)

Anggaplah wali kelas mendata hobi 40 siswanya:
- Suka makan Bakso (Keranjang $A$) = 25 orang
- Suka makan Mi Ayam (Keranjang $B$) = 20 orang
- Maruk suka Keduanya ($A \cap B$, si daerah tengah) = 10 orang

**Soal #1:** Berapa jumlah anak yang suka Bakso **ATAU** Mi Ayam? (Tolong kumpulin semua yang doyan bakso/mi/keduanya!).

*Pikiran polos:* "Kan gampang, Pak. Tinggal tambahin aja 25 + 20 = 45 orang."
**STOP! Logika ini SALAH BESAR!** 🚫

Coba pikir pakai logika. Kalau kamu cuma nambah 25 + 20, **si 10 orang yang maruk tadi bakal kehitung DUA KALI**. Waktu ngedata bakso mereka angkat tangan, pas ngedata mi ayam mereka angkat tangan lagi!

Solusinya? **Karena kehitung 2 kali, kita harus ngurangi kelebihan hitungannya 1 kali.** (Makanya disebut Inklusi-Eksklusi, alias masukin-keluarin).

> **Rumus Ajaib 2 Lingkaran:**
> **Total Gabungan = Total A + Total B - Irisan Keduanya**
> $|A \cup B| = 25 + 20 - 10$
> **$= 35$ orang.** ✓ (Ini jawaban benarnya!)

**Soal #2:** Nah, kalau gitu dari 40 siswa di kelas, berapa anak aneh yang nggak suka keduanya?
*Solusi:* Ya tinggal kamu kurangi aja total anak sekelas dengan anak-anak yang suka mi/bakso tadi.
Sisa = 40 anak total - 35 anak = **5 anak**. 
Lima anak inilah yang nongkrong di "Padang Rumput Area Luar" dari Diagram Venn.

---

### Kasus 3 Lingkaran (Level Mandor OSN)

Gimana kalau ekskulnya malah ada 3? (Ekskul Musik, Tari, dan Lukis). 
Terus ditanya: **Berapa total anak yang ikut minimal 1 dari ketiga ekskul itu?**

Jangan panik! Meskipun rumusnya kelihatan panjang, polanya ini **mirip lagu maju-mundur-maju yang gampang diingat**:
1. **Maju (Tanda +)**: Tambahin dulu total anak di masing-masing ekskul sendirian ($+A, +B, +C$)
2. **Mundur (Tanda -)**: Karena pasti ada yang tumpang tindih waktu kamu nambahin barusan, mari kurangi dengan irisan per 2 serangkainya ($-AB, -AC, -BC$)
3. **Maju (Tanda +)**: Lho, waktu kamu kurangin 2 serangkai tadi, saking semangatnya, anak yang ikut KETIGANYA malah ikut kebuang abis. Jadi kita harus kembalikan mereka satu kali ($+ABC$)

> **Rumus Resmi 3 Lingkaran:**
> $|A \cup B \cup C| = (A + B + C) - (AB + AC + BC) + (ABC)$

**TAPI, KASIH TAU RAHASIA:** Waktu ngerjain soal OSN-K Matematika/Informatika, **JANGAN MENGANDALKAN RUMUS INI!** Ini rawan banget salah hitung buat pemula. Mending **KEMBALI MENGGAMBAR DIAGRAM VENN-NYA (Bikin 3 lingkaran yang saling nabrak)!**

**Step-by-step Trik VENN 3 Lingkaran (WAJIB DIIKUTI CARA INI):**
Bayangkan soal cerita panjang lebar kasih data macem-macem.
1. **MULAI DARI UDEL (KOTAK TENGAH PALING DALAM)!** Jangan pernah nulis dari luar. Selalu cari tau dulu berapa anak yang SUKA KETIGA-TIGANYA. Tulis angkanya di pusaran paling dalam. (Misal ada 5 anak).
2. **MUNDUR KE JEMBATAN DUO.** Cek data anak yang cuma suka 2 ekskul (Misal: pecinta Musik & Tari ada 15). Ingat, 5 orang udel tadi udah termasuk di 15 ini. Jadi yang murni cuma Music & Tari = $15 - 5 = 10$. Tulis angkanya. Lakukan untuk duo-duo yang lain.
3. **MUNDUR KE BALON KOPONG.** Sekarang cek data utama (Total anak Musik 50). Dari angka 50 ini, kurangi dengan angka-angka di dalam perut lingkaran musik yang sudah kamu tulis dari langkah 1 dan 2. Sisanya adalah angka anak yang "SAYA CUMA MAU MUSIK TITIK!".
4. Setelah SEMUA KOLOM di diagram Venn terisi angka, kamu tinggal **TAMBAHKAN MANUAL PAKAI KALKULATOR OTAKMU**. Dijamin 100% jawabanmu nyeni dan bener tanpa harus hafal rumus!

---

## 💻 5. Apa Hubungannya Sama Programming & Komputer?

Materi himpunan ini nggak cuma diciptakan buat ngerjain soal ujian di atas kertas lho! Nanti pas kamu udah mulai ngoding dan bikin aplikasi yang ngolah data jutaan manusia (kayak admin database Gojek atau sekolahan), logika himpunan ini bakal jadi nyawa utamamu pakai bahasa **SQL (Structured Query Language)**.

Namanya di *database* bukan lagi Himpunan, tapi **Operasi JOIN**. Lihat terjemahannya:

| Di Matematika Kelas | Di Dunia Programmer Namanya | Contoh Kasus Sehari-hari |
|---------------------|-----------------------------|--------------------------|
| Gabungan ($A \cup B$) | Pakai syarat **`OR`** (Atau) | "Sistem, tolong tampilin daftar siswa yang Alamatnya Jakarta `OR` Bandung." (Pasti ditampilin gabungannya!) |
| Irisan ($A \cap B$) | Pakai syarat **`AND`** (Dan) / `INNER JOIN` | "Sistem, tolong tampilin cowok yang Tampan `AND` Tajir." (Cuma yang memenuhi DUA kriteria sekaligus yang lolos!) |
| Selisih ($A - B$)  | Pakai syarat **`A AND NOT B`** / `LEFT JOIN` | "Sistem, tolong tampilkan data siswa kelas 10, tapi yang status SPP-nya `NOT` Lunas." (Anak kelas 10 yang lunas langsung diusir dari daftar). |

Intinya: Menguasai himpunan berarti kamu sudah siap *berpikir* persis layaknya mesin pencari Google saat memfilter data miliaran halaman! 😎

---
[< Materi Sebelumnya: Graf Sederhana](./07-graf-sederhana.md) | [Materi Berikutnya: Kombinatorika >](./09-kombinatorika.md)
[< Kembali ke Beranda Materi](../README.md)
