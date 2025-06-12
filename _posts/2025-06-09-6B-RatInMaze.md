---
title: "🐭Rat In Maze"
date: 2025-06-09
categories: [problem, algorithm]
tags: [problem, algorithm]
---

Rat in Maze Algorithm adalah salah satu contoh klasik dalam pemrograman rekursif dan pencarian jalur (pathfinding). Algoritma ini menggunakan metode backtracking untuk mencari semua kemungkinan jalur dari titik awal ke titik tujuan.
🔍 Konsep Utama

Algoritma ini mencoba semua kemungkinan jalur dan kembali ke langkah sebelumnya jika jalur tersebut buntu. Tujuannya adalah mencari semua solusi atau salah satu jalur yang memungkinkan tikus mencapai tujuan.

### 🎮 Representasi Visual
- 🟢 = Jalan (dapat dilewati)
- 🔴 = Dinding (tidak dapat dilewati)
- 🐭 = Posisi tikus
- 🎯 = Tujuan

### Masalah Umum yang Diselesaikan
- 🗺️ Pencarian Jalur: Bagaimana mencari jalan keluar dari labirin yang kompleks?
- 🧠 Pengambilan Keputusan: Bagaimana program bisa "berpikir" saat harus memilih banyak jalur?

### 🌍 Manfaat di Dunia Nyata
- AplikasiNavigasiGPS untuk mencari rute tercepat
- Robotika: Robot menemukan jalan dalam lingkungan
- Game Development: AI karakter mencari jalur optimal
- Puzzle Solving: Menyelesaikan Sudoku dan teka-teki logika

### ⚙️ Cara Kerja Algoritma
📝 Langkah-langkah Algoritma

- 🚀 Mulai dari posisi awal (0,0)
- ✅ Validasi posisi:

Posisi dalam batas maze
Posisi adalah jalan (bernilai 1)
Posisi belum dikunjungi


- 📍 Tandai posisi sebagai bagian dari solusi
🎯 Cek tujuan: Jika mencapai tujuan, simpan jalur
🔄 Eksplorasi rekursif ke semua arah yang valid
↩️ Backtrack: Hapus tanda jika tidak ada jalur valid

- 🎯 Urutan Prioritas Pergerakan
1. Down (Bawah) ↓
2. Right (Kanan) →
3. Up (Atas) ↑
4. Left (Kiri) ←