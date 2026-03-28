# 08. Teori Himpunan (Belajar Ngelompokin Gabungan Data)

> "Pernah nggak sih kamu disuruh ngumpulin data teman sekelas? Ada yang suka Bakso, ada yang suka Mi Ayam, ada yang maruk suka KEDUANYA, dan ada yang aneh nggak suka dua-duanya. Nah, selamat datang di dunia **Himpunan**!"

Di OSN-K Informatika, Teori Himpunan ini gampang banget tapi super penting. Kenapa? Karena logika himpunan dipakai setiap hari oleh programmer buat *nyari data* di *database* (kayak kamu lagi *search* barang di Tokopedia).

Yuk, kita bahas pelan-pelan!

---

## 📦 1. Kenalan Dulu: Apa Itu Himpunan?

**Himpunan (Set)** itu sesimple **sebuah wadah/grup** yang isinya benda-benda atau angka yang jelas batasannya. Isi dari wadah itu disebut **anggota**.

**Contoh Gampang:**
- Grup $A$ = {Budi, Siti, Anton}
- Grup $B$ = {1, 3, 5, 7, 9} (Wadah angka ganjil di bawah 10)

### Aturan Main Grup (Wajib Ingat!):
1. **Nggak Boleh Ada yang Kembar:** Kalau kamu nulis {1, 2, 2, 3}, komputer bakal otomatis ngapus angka 2 yang dobel. Jadinya cuma {1, 2, 3} aja.
2. **Urutan Nggak Ngaruh:** Nulis {A, B, C} itu persis sama dengan {C, A, B}. Yang penting isinya sama!

**Istilah Keren (Biar Kayak Anak OSN):**
- **Kardinalitas** (ditulis $|A|$ atau $n(A)$): Ini cuma bahasa ribet buat **"Ada berapa sih jumlah anggotanya?"**.
  - Contoh: Grup $A$ = {Budi, Siti, Anton}. Jumlah anggotanya 3, berarti $|A| = 3$. Gampang kan?
- **Himpunan Semesta ($S$)**: Ini "Dunia"-nya. Misal kita lagi bahas anak basket di sekolah, berarti semestanya ya **semua murid di sekolah itu**.
- **Himpunan Kosong ($\emptyset$)**: Wadah kosong melompong. Nggak ada isinya. Jumlah anggotanya = 0.

---

## 🎨 2. Mencampur & Memisah Wadah (Operasi Himpunan)

Bayangkan di sekolahmu ada 2 wadah ekskul:
- Wadah $A$ (Anak Basket) = {Budi, Siti, **Andi**}
- Wadah $B$ (Anak Paskibra) = {**Andi**, Cici, Dedi}

### A. Gabungan / Union (Simbolnya: $\cup$ kayak Mangkok)
Ini ibarat menyatukan semua anak Basket **ATAU** Paskibra ke dalam satu lapangan.
- Kuncinya: **ATAU** (huruf 'U' di kata ata**U** mirip simbol $\cup$).
- Tuang semua isinya, tapi ingat aturan #1: **Yang dobel cuma dihitung SEKALI**. Si Andi nggak usah dihitung dua kali!
- $A \cup B$ = {Budi, Siti, Andi, Cici, Dedi}

### B. Irisan / Intersection (Simbolnya: $\cap$ kayak Topi)
Ini nyari anak yang **super sibuk**. Anak yang ikut ekskul Basket **DAN** Paskibra sekaligus.
- Kuncinya: **DAN** (huruf 'n' di kata da**n** mirip simbol $\cap$).
- Siapa nama yang muncul di kedua wadah? Cuma Andi!
- $A \cap B$ = {Andi}

### C. Kurang-kurangan / Selisih (Simbolnya: $-$)
Mau nyari anak yang **HANYA** ikut Basket, dan **Nggak Boleh** ikut Paskibra.
- Caranya: Ambil semua anak Basket ($A$), lalu usir anak yang ternyata diam-diam ikut Paskibra juga (usir Andi).
- $A - B$ = {Budi, Siti}
- *Hati-hati:* $A - B$ beda banget sama $B - A$. Kalau $B - A$ berarti nyari anak Paskibra singa (Hanya Paskibra) = {Cici, Dedi}.

### D. Komplemen / "Selain" (Simbolnya: $A^c$)
Ucapkan kata ajaib: **"SAYA CARI SE--LA--IN..."**
- $A^c$ artinya: Tolong cari semua anak satu sekolah ($S$), yang **SELAIN** anak Basket.

---

## 📊 3. Gambar Adalah Penyelamat (Diagram Venn)

Kalau di soal OSN-K ada cerita panjang lebar, **KUNCI RAHASIANYA CUMA SATU: GAMBAR LINGKARAN (Diagram Venn)!** Jangan pernah coba bayangin di otak doang.

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

**Cara Gampang Bacanya:**
- Balon Kiri KOPONG (Budi, Siti) = **Orang yang CUMA Basket**.
- Balon Kanan KOPONG (Cici, Dedi) = **Orang yang CUMA Paskibra**.
- Jembatan Tengah (Andi) = **Orang yang IKUT DUA-DUANYA**.
- Padang Rumput Luar (Eka, Fajar) = **Orang yang NGGAK IKUT APA-APA**.

---

## 🧮 4. Rumus Anti-Dobel (Prinsip Inklusi-Eksklusi)

Ini dia materi himpunan yang **pasti keluar** di OSN! Fungsinya untuk ngitung jumlah orang kalau ada gabungan.

### Kasus 2 Lingkaran (Level Gampang)

Anggaplah di kelasmu ada:
- Suka Bakso ($A$) = 25 orang
- Suka Mi Ayam ($B$) = 20 orang
- Maruk Suka Keduanya ($A \cap B$) = 10 orang

**Pertanyaan:** Berapa orang yang suka Bakso **ATAU** Mi Ayam? (Tolong kumpulin jadi satu!)

*Pikiran polos:* Ya ditelur aja dong, 25 + 20 = 45 orang.
**SALAH BESAR!** 🚫

Kalau kamu cuma nambah 25 + 20, **si 10 orang maruk tadi bakal kehitung DUA KALI** (kehitung pas ngedata Bakso, kehitung lagi pas ngedata Mi Ayam).

Solusinya? **Karena kehitung 2 kali, kita harus kurangi 1 kali.**

> **Rumus Ajaib:**
> **Total Gabungan = Total A + Total B - Irisannya**
> $|A \cup B| = 25 + 20 - 10$
> **$= 35$ orang.** ✓ (Ini jawaban benarnya!)

Trus kalau ditanya: "Total siswa ada 40 orang, berapa yang nggak suka keduanya?"
Ya tinggal sisa aja: 40 anak total - 35 anak suka mi/bakso = **5 anak**. Gampang banget!

---

### Kasus 3 Lingkaran (Level Mandor)

Gimana kalau ekskulnya ada 3? (A, B, dan C). 
Terus ditanya: **Berapa total anak yang ikut minimal 1 ekskul?**

Jangan panik sama rumusnya, karena polanya ini **mirip lagu maju-mundur-maju**:
1. **Maju (Tanda +)**: Tambahin semua yang sendirian (+A, +B, +C)
2. **Mundur (Tanda -)**: Kurangin semua yang berduaan (-AB, -AC, -BC)
3. **Maju (Tanda +)**: Tambahin lagi yang bertigaan (+ABC)

> **Rumus 3 Lingkaran:**
> $|A \cup B \cup C| = (A + B + C) - (AB + AC + BC) + (ABC)$

**TAPI, KASIH TAU RAHASIA:** Di OSN-K, nggak usah hapal rumus ini kalau pusing. **GAMBAR AJA DIAGRAM VENN-NYA!**

**Tips VENN 3 Lingkaran (WAJIB DIHAPAL CARANYA):**
1. **MULAI DARI UDEL (TENGAH)!** Selalu tulis dulu angka orang yang suka KETIGANYA di paling tengah.
2. **MUNDUR KE JEMBATAN DUO.** Kurangi angka duo dengan angka tengah tadi.
3. **MUNDUR KE BALON KOPONG.** Kurangi total keseluruhan bagiannya dengan angka-angka yang udah kamu tulis di dalam.
4. Totalin semuanya manual. Dijamin 100% bener tanpa pusing ngafal rumus panjang!

---

## 💻 5. Hubungan Sama Komputer (Database SQL)

Materi himpunan ini nggak cuma buat matematika kertas lho! Nanti pas kamu jadi programmer dan mengolah data ribuan orang (misal di Shopee/Gojek), logika himpunan ini namanya **Operasi SQL JOIN**.

Lihat kecocokannya:
| Kalau di Teori Himpunan | Kalau di Kodingan Keliatannya Gini |
|-------------------------|------------------------------------|
| Gabungan ($A \cup B$) | Pakai kata sandi `OR` (Kalau dia A atau B, lulus!) |
| Irisan ($A \cap B$) | Pakai kata sandi `AND` (Harus A dan harus B, baru lulus!) |
| Selisih ($A - B$)  | Pakai kata sandi `A AND NOT B` |

Paham himpunan = Kamu siap belajar ngatur data kayak hacker profesional! 😎

---
[< Materi Sebelumnya: Graf Sederhana](./07-graf-sederhana.md) | [Materi Berikutnya: Kombinatorika >](./09-kombinatorika.md)
[< Kembali ke Beranda Materi](../README.md)
