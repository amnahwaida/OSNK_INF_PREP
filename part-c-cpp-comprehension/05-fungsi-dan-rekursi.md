# 05. Fungsi dan Rekursi

Rekursi adalah teknik di mana sebuah fungsi memanggil dirinya sendiri. Dalam OSN-K, soal rekursi sering muncul untuk menguji kemampuan *tracing stack*.

## Komponen Penting Rekursi
1. **Base Case**: Kondisi di mana rekursi berhenti.
2. **Recursive Step**: Bagian di mana fungsi memanggil dirinya dengan argumen yang lebih sederhana.

## 🧪 Contoh Dry Run Rekursi

```cpp
int f(int n) {
    if (n == 0) return 0;
    return n + f(n - 1);
}
```

Jika dipanggil `f(3)`:
1. `f(3)` mengembalikan `3 + f(2)`
2. `f(2)` mengembalikan `2 + f(1)`
3. `f(1)` mengembalikan `1 + f(0)`
4. `f(0)` mengembalikan `0` (Base Case)

**Unwinding**:
`f(1) = 1 + 0 = 1`
`f(2) = 2 + 1 = 3`
`f(3) = 3 + 3 = 6`

---
## ❓ Latihan Singkat
Apa hasil dari `misterius(4)`?
```cpp
int misterius(int n) {
    if (n <= 1) return 1;
    return n * misterius(n - 1);
}
```

<details>
<summary>✅ Jawaban</summary>
**24** (Ini adalah fungsi faktorial: 4 * 3 * 2 * 1 = 24).
</details>

---
[< Kembali ke Materi Part C](./README.md)
