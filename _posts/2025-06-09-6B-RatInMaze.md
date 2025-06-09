---
title: "Rat In Maze"
date: 2025-06-09
categories: [problem, algorithm]
tags: [problem, algorithm]
---

Algoritma Rat in a Maze adalah metode klasik dalam pemrograman rekursif dan pencarian jalur yang menggunakan teknik backtracking untuk menemukan jalan keluar dari labirin. Tujuannya adalah mencari jalur dari titik awal (0,0) ke tujuan dalam labirin yang berisi jalan (1) dan dinding (0).

Langkah-langkah:

Mulai dari posisi awal dan periksa apakah posisi tersebut valid dan belum dikunjungi.

Tandai posisi sebagai bagian dari solusi dan coba bergerak ke arah yang mungkin (kanan atau bawah).

Jika tidak ada jalur yang valid, mundur (backtrack) ke posisi sebelumnya.

Manfaat:
Digunakan dalam aplikasi dunia nyata seperti GPS dan robotika dan melatih logika rekursif dan pengambilan keputusan.