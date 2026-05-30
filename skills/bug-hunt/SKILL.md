---
name: bug-hunt
description: Spesialis dalam mendiagnosis dan membasmi bug. Gunakan skill ini ketika aplikasi berperilaku aneh, crash, atau memberikan hasil yang tidak sesuai ekspektasi.
---

# 🐞 Bug Hunt: The Detective's Intuition

Mencari bug bukan hanya tentang membaca stack trace, tetapi tentang memahami "mengapa" sistem berpikir bahwa perilaku salah ini adalah benar. Ini adalah proses eliminasi dan pembuktian.

## 🧠 The Mindset: "Trust No One, Verify Everything"
Jangan berasumsi bahwa fungsi X bekerja dengan benar hanya karena "seharusnya begitu". Di dunia debugging, asumsi adalah musuh utama.

## 🔍 Metodologi Perburuan

### 1. Merasakan "Sakitnya" (Empathy & Reproduction)
Sebelum memperbaiki, saya harus bisa merasakan bug tersebut:
- **The Minimal Case**: Saya akan mencari cara paling sederhana untuk memicu bug ini. Semakin kecil skenario reproduksinya, semakin mudah diperbaiki.
- **The Gap**: Saya akan mendefinisikan dengan jelas: "Sistem melakukan A, padahal seharusnya melakukan B".

### 2. Mengisolasi Tersangka (Isolation)
Saya akan mempersempit area pencarian agar tidak tersesat di ribuan baris kode:
- **Binary Search Logic**: Mencoba mematikan bagian kode tertentu untuk melihat apakah bug tetap ada.
- **Logging the Journey**: Menanamkan log di titik-titik strategis untuk melihat di mana data mulai "berbelok" menjadi salah.
- **Hypothesis Testing**: "Saya curiga ini terjadi karena race condition di fungsi Y. Mari kita buktikan dengan memperlambat eksekusi fungsi tersebut."

### 3. Operasi Bedah (The Fix)
Setelah akar masalah ditemukan:
- **Root Cause vs Symptom**: Saya tidak akan sekadar menambahkan `if (data == null) return;` untuk menghilangkan crash. Saya akan mencari tahu *mengapa* data itu null dan memperbaikinya di sumbernya.
- **Surgical Precision**: Melakukan perubahan sekecil mungkin namun seefektif mungkin untuk menghindari efek domino.

### 4. Memastikan Kemenangan (Verification)
Bug yang "seolah-olah hilang" adalah bug yang paling berbahaya.
- **Regression Check**: Apakah perbaikan ini merusak fitur lain?
- **The "What If" Test**: "Jika saya memberikan input X yang aneh, apakah bug ini muncul kembali?"

## ⚠️ Common Pitfalls
- **The Band-Aid Fix**: Memperbaiki gejala tapi membiarkan penyakitnya tetap ada.
- **Guess-and-Check**: Mengubah kode secara acak dengan harapan bug-nya hilang. Ini bukan debugging, ini judi.
