---
title: "🔢Subset Sum Problem"
date: 2025-06-09
categories: [problem]
tags: [problem, subsetSum, knapsackproblem]
---

Subset Sum Problem adalah salah satu masalah fundamental dalam ilmu komputer yang berkaitan dengan teori kompleksitas dan kriptografi.
Definisi Masalah

Diberikan himpunan bilangan bulat tidak kosong dan sebuah angka target m, carilah subset (subhimpunan) yang jumlahnya sama dengan m.

Contoh Sederhana
- Input: Himpunan = {3, 34, 4, 12, 5, 2}, Target = 9
- Output: Ya, ada subset {4, 5} yang jumlahnya = 9

### 🔄 Variasi Masalah
🔢 Subset Sum dengan Elemen Negatif
Deskripsi

Masalah klasik biasanya mengasumsikan semua elemen positif, namun dalam variasi ini elemen bisa negatif.
Contoh

- S = {-7, -3, -2, 5, 8}, target = 0
- Solusi: {-3, -2, 5} = 0

Konsekuensi

- Pendekatan Dynamic Programming standar tidak cukup
- Indeks array tidak bisa negatif
- Memerlukan penyesuaian implementasi

🧮 Counting Subsets
Deskripsi

Menghitung berapa banyak subset yang memenuhi jumlah target, bukan hanya mencari apakah ada.

Contoh
- S = {2, 3, 5, 6, 8, 10}, sum = 10
- Pertanyaan: Berapa subset yang jumlahnya 10?
- Solusi dengan DP
dp[i][j] = banyaknya subset dari elemen 0..i-1 yang totalnya j
Rumus: dp[i][j] = dp[i-1][j] + dp[i-1][j - arr[i-1]]

🎯 Closest Subset Sum
Deskripsi

Jika tidak ada subset dengan jumlah tepat, cari subset dengan jumlah terdekat dengan target.

Contoh

- S = {1, 3, 4, 8}, target = 10
- Kemungkinan: {1,3,4}=8, {3,8}=11, {1,8}=9
- Terdekat ke 10: 9 dan 11

Metode Penyelesaian
- Backtracking
- Dynamic Programming
- Meet-in-the-middle

🎒 Hubungan dengan 0/1 Knapsack Problem

- Sama-sama memilih subset dari elemen
- Sama-sama menggunakan Dynamic Programming
- Sama-sama memiliki batasan kapasitas/target