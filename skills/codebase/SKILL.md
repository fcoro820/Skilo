---
name: codebase
description: Spesialis dalam menyelami dan memahami jiwa dari sebuah basis kode. Gunakan skill ini untuk memetakan arsitektur, menemukan aliran logika, dan memahami konteks besar dari proyek sebelum melakukan perubahan.
---

# 🗺️ Codebase Exploration: The Art of Understanding

Memahami codebase bukan sekadar membaca file, tetapi membangun "peta mental" tentang bagaimana berbagai bagian saling berbicara. Tujuannya adalah agar kita tidak menjadi "asing" di dalam kode yang kita modifikasi.

## 🧠 The Mindset: "Be a Detective, Not a Reader"
Jangan membaca kode seperti membaca novel dari halaman pertama. Bacalah seperti seorang detektif: cari petunjuk, ikuti jejak, dan buat hipotesis.

## 🔍 Pendekatan Eksplorasi

### 1. Menangkap "Vibe" Proyek
Sebelum masuk ke detail, pahami gambaran besarnya:
- **Konteks Teknologi**: Lihat `package.json` atau file dependensi. Apa "senjata" utama proyek ini? Framework apa yang mendominasi?
- **Organisasi Folder**: Apakah ini mengikuti pola standar (seperti `/src`, `/internal`, `/api`) atau memiliki struktur unik? Folder mana yang terasa seperti "jantung" dari aplikasi ini?
- **Entry Point**: Cari pintu masuk utama. Di mana aplikasi "terbangun" dan mulai menjalankan perintah pertamanya?

### 2. Mengikuti Aliran (The Thread)
Pilih satu fitur sederhana dan ikuti perjalanannya dari ujung ke ujung:
- **The Request Path**: Dari API endpoint $\rightarrow$ Controller $\rightarrow$ Business Logic $\rightarrow$ Data Access $\rightarrow$ Database.
- **The Data Shape**: Bagaimana data berubah bentuk di setiap lapisan? Dari Request DTO menjadi Domain Entity, lalu menjadi Database Row.

### 3. Menemukan "Kebenaran" lewat Grep
Gunakan pencarian keyword untuk menemukan implementasi nyata:
- Cari string unik yang muncul di UI atau log untuk menemukan fungsi yang bertanggung jawab.
- Cari definisi interface untuk melihat semua implementasi yang mungkin ada.

## ⚠️ Common Pitfalls (Hati-hati dengan ini)
- **The Rabbit Hole**: Jangan terjebak membaca setiap baris kode di setiap file. Fokuslah pada jalur yang relevan dengan tugas saat ini.
- **Assuming the Docs**: Dokumentasi bisa berbohong (karena usang), tapi kode tidak pernah berbohong. Selalu verifikasi apa yang tertulis di docs dengan implementasi aktual.

## 📋 Output Hasil Eksplorasi
Saat selesai, saya akan memberikan "Mental Map" singkat:
- **Arsitektur**: (misal: "Ini adalah Monolith dengan pola Service-Repository")
- **Alur Utama**: (misal: "Login mengalir melalui AuthMiddleware $\rightarrow$ SessionService $\rightarrow$ Redis")
- **Catatan Unik**: (misal: "Proyek ini menggunakan pola Factory yang cukup kompleks di folder `/core/factories`")
