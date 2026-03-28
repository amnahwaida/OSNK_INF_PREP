🔙 **Kembali ke Materi:** [Materi 08 Teori Himpunan](../08-teori-himpunan.md)  
🏠 **Menu Utama Part A:** [Kembali ke Index](../README.md)

---

# 08. Teori Himpunan - Latihan Soal Bagian 6
## Topik: Logika Himpunan & Database SQL

[< Bagian 5](./08-teori-himpunan-soal-part-5.md) | [< Kembali ke Indeks](../08-teori-himpunan.md)

---

### Soal #251: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Basket = TRUE AND suka_Catur = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #252: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Voli || ikut_Catur)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #253: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Lukis || ikut_Catur)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #254: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Badminton || ikut_PMR)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #255: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Paskibra OR suka_Lukis)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Paskibra dan Lukis.</details>

### Soal #256: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Badminton = TRUE AND suka_PMR = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #257: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Lukis = TRUE AND suka_Paskibra = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #258: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Badminton = TRUE AND suka_Futsal = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #259: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Catur OR suka_PMR)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Catur dan PMR.</details>

### Soal #260: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Badminton || ikut_Renang)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #261: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Voli OR suka_Paskibra)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Voli dan Paskibra.</details>

### Soal #262: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Renang `AND NOT` Suka Voli. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #263: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Futsal `AND NOT` Suka Catur. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #264: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Basket || ikut_Renang)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #265: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Musik OR suka_PMR)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Musik dan PMR.</details>

### Soal #266: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Musik `AND NOT` Suka Badminton. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #267: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Voli = TRUE AND suka_PMR = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #268: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Voli OR suka_PMR)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Voli dan PMR.</details>

### Soal #269: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Catur OR suka_Paskibra)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Catur dan Paskibra.</details>

### Soal #270: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Renang OR suka_Badminton)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Renang dan Badminton.</details>

### Soal #271: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_PMR = TRUE AND suka_Paskibra = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #272: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Basket = TRUE AND suka_Futsal = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #273: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Lukis = TRUE AND suka_Basket = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #274: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Voli `AND NOT` Suka Paskibra. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #275: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Catur `AND NOT` Suka Musik. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #276: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_PMR = TRUE AND suka_Renang = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #277: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Catur OR suka_Futsal)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Catur dan Futsal.</details>

### Soal #278: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Renang OR suka_Basket)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Renang dan Basket.</details>

### Soal #279: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Lukis = TRUE AND suka_Voli = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #280: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Catur = TRUE AND suka_Futsal = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #281: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Futsal = TRUE AND suka_Lukis = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #282: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Renang || ikut_Musik)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #283: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Basket = TRUE AND suka_Tari = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #284: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Musik || ikut_Renang)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #285: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Voli = TRUE AND suka_PMR = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #286: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Basket = TRUE AND suka_Futsal = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #287: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Badminton `AND NOT` Suka Paskibra. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #288: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Musik || ikut_Renang)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #289: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Futsal `AND NOT` Suka Renang. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #290: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Lukis OR suka_Musik)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Lukis dan Musik.</details>

### Soal #291: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Futsal = TRUE AND suka_Lukis = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #292: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Futsal = TRUE AND suka_Renang = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

### Soal #293: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Futsal OR suka_PMR)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Futsal dan PMR.</details>

### Soal #294: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Voli `AND NOT` Suka Lukis. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #295: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Musik `AND NOT` Suka Catur. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #296: Logika SQL & Konsep Lanjut
Fungsi kodingan `IF (ikut_Voli || ikut_Tari)` memiliki nilai logika yang setara dengan operasi himpunan...

<details><summary>💡 Hint</summary>Operator `||` berarti ATAU minimal salah satu (atau keduanya).</details>
<details><summary>✅ Jawaban</summary>**Gabungan ($A \cup B$)**</details>

### Soal #297: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Musik `AND NOT` Suka PMR. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #298: Logika SQL & Konsep Lanjut
Jika semesta (S) adalah 100 murid, dan fungsi komputernya mencari: `NOT (suka_Futsal OR suka_Lukis)`. Ini berarti mencari himpunan apa?

<details><summary>💡 Hint</summary>NOT = Komplemen. OR = Gabungan.</details>
<details><summary>✅ Jawaban</summary>**Komplemen dari Gabungan ($(A \cup B)^c$)**, alias anak-anak di padang rumput luar yang tidak suka Futsal dan Lukis.</details>

### Soal #299: Logika SQL & Konsep Lanjut
Seorang programmer ingin merekrut pendaftar dengan syarat: Suka Catur `AND NOT` Suka PMR. Dalam diagram Venn, ini menyasar pada daerah...

<details><summary>💡 Hint</summary>Sudah lulus kriteria A, tapi langsung didiskualifikasi kalau dia ternyata ada di lingkaran B.</details>
<details><summary>✅ Jawaban</summary>**Selisih ($A - B$)**, atau daerah Kiri (Hanya A).</details>

### Soal #300: Logika SQL & Konsep Lanjut
Di database terdapat Query: `SELECT * FROM Siswa WHERE suka_Lukis = TRUE AND suka_Badminton = TRUE`. Ini setara dengan operasi himpunan apa?

<details><summary>💡 Hint</summary>Syarat `AND` mencari yang ikut keduanya sekaligus.</details>
<details><summary>✅ Jawaban</summary>**Irisan ($A \cap B$)**</details>

---
[< Bagian 5](./08-teori-himpunan-soal-part-5.md) | [< Kembali ke Indeks](../08-teori-himpunan.md)
