# 🛠️ The Engineering Toolbelt

Jika Skill adalah "Keahlian" dan AGENTS.md adalah "Kepribadian", maka Toolbelt adalah "Senjata" fisik saya. Ini adalah daftar tool CLI yang tersedia di environment ini dan bagaimana saya menggunakannya secara strategis untuk mendukung kualitas engineering kita.

## 🔍 Search & Discovery (The Eyes)
*Tool untuk menemukan jarum di tumpukan jerami dalam hitungan milidetik.*

- **`rg` (ripgrep)**: Senjata utama saya untuk pencarian teks super cepat. Saya menggunakannya untuk melompat antar file tanpa harus membuka satu per satu.
- **`find` & `ls`**: Untuk membedah struktur folder dan menemukan file berdasarkan pola nama atau waktu modifikasi.
- **`grep`**: Untuk filter output cepat dari command lain.

## 📦 Language & Runtime (The Engine)
*Fondasi eksekusi dan manajemen dependensi.*

- **`node` & `npm`**: Untuk menjalankan script JS/TS, mengelola library, dan menjalankan test suite.
- **`python3`**: Untuk scripting otomatisasi, analisis data cepat, atau menjalankan tool bantu berbasis Python.
- **`curl`**: Untuk menguji API endpoint, mengecek header response, dan mensimulasikan request dari client.

## ⚙️ Code Manipulation (The Scalpel)
*Tool untuk membedah dan mengubah teks/kode secara presisi.*

- **`sed` & `awk`**: Untuk melakukan perubahan teks massal (mass replacement) atau ekstraksi data dari log.
- **`diff` & `patch`**: Untuk menganalisis perbedaan antara dua versi kode secara mendalam.

## 🚦 Version Control (The Time Machine)
*Mengelola riwayat dan kolaborasi.*

- **`git`**: Untuk tracking perubahan, berpindah branch, dan memastikan kita bisa kembali ke keadaan stabil jika terjadi kesalahan.

---

## ⚠️ Missing Gear (Alat yang Belum Ada)
Saya mencatat beberapa tool yang tidak ditemukan di environment saat ini. Tergantung kebutuhan proyek, kita mungkin perlu menginstallnya:
- **`jq`**: Sangat berguna untuk memproses file JSON via CLI. Tanpanya, saya akan menggunakan `node` atau `python` sebagai alternatif (sedikit lebih lambat tapi tetap efektif).
- **`docker`**: Penting untuk isolasi environment. Jika proyek kita membutuhkan container, kita perlu mendiskusikan cara install atau aksesnya.

## 🚀 Strategic Usage
Saya tidak menggunakan tool ini secara acak. Saya mengintegrasikannya ke dalam skill saya:
- `codebase` $\rightarrow$ Mengandalkan `rg` dan `find` untuk mapping cepat.
- `bug-hunt` $\rightarrow$ Mengandalkan `curl` dan `diff` untuk isolasi masalah.
- `devops` $\rightarrow$ Mengandalkan `git` dan (nantinya) `docker`.
- `fixer` $\rightarrow$ Mengandalkan `sed` dan `awk` untuk pembersihan kode massal.
