---
title: "Huffman Coding"
date: 2025-06-09
categories: [algorithm]
tags: [huffmanCoding, transmisiData]
---

Huffman Coding adalah algoritma kompresi data yang mengkodekan karakter dengan panjang bit bervariasi, di mana karakter yang lebih sering muncul mendapatkan kode lebih pendek.

Langkah-langkah:

Hitung frekuensi kemunculan setiap karakter.

Buat pohon Huffman dengan menggabungkan node karakter berdasarkan frekuensi terendah.

Traversal pohon untuk memberikan kode (0 untuk kiri, 1 untuk kanan).

Gantikan karakter dalam teks dengan kode Huffman.

Untuk dekompresi, gunakan pohon Huffman untuk menerjemahkan kode kembali ke karakter.

Keunggulan dari Huffman Coding ini adalah dapat mengurangi data secara efisien, terutama untuk data dengan banyak karakter berulang.

Dengan Huffman Coding, kita dapat mengoptimalkan penyimpanan dan transmisi data.