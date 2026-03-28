# 02. Strategi Analisis Paper-Based

Dalam OSN-K, kecepatan dan keakuratan simulasi manual sangat krusial.

## Teknik Utama
1. **Penyederhanaan Masalah**: Gunakan angka atau variabel yang kecil untuk memahami mekanisme dasar.
2. **Visualisasi**: Gambar diagram, pohon keputusan, atau antrian untuk mempermudah pelacakan.
3. **Penyimpanan State**: Tuliskan nilai variabel atau status sistem di setiap langkah.

## 🧪 Contoh Kasus Sederhana
Jika ada 5 lampu (L1-L5) yang awalnya mati, dan setiap langkah ke-i kita mengubah status lampu i, i+1, ... (toggle mati ke nyala atau sebaliknya).
Berapa lampu yang menyala setelah 5 langkah?

**Strategi Paper-Based:**
Gunakan tabel 0/1 (0=mati, 1=nyala).
| Step | L1 | L2 | L3 | L4 | L5 |
|------|----|----|----|----|----|
| 0    | 0  | 0  | 0  | 0  | 0  |
| 1    | 1  | 1  | 1  | 1  | 1  |
| 2    | 1  | 0  | 0  | 0  | 0  |
| ...  |    |    |    |    |    |

---
[< Kembali ke Materi Part B](./README.md)
