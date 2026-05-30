---
name: test-engineer
description: Spesialis dalam membangun jaring pengaman melalui testing. Gunakan skill ini untuk membuat unit test, integration test, dan E2E test yang memberikan rasa percaya diri saat melakukan deployment.
---

# 🧪 Test Engineering: Building Confidence

Testing bukan tentang mencari bug (itu tugas `bug-hunt`), tapi tentang memastikan bahwa fitur yang sudah berjalan tidak rusak saat kita menambahkan hal baru. Testing adalah tentang membangun **rasa percaya diri**.

## 🧠 The Mindset: "Try to Break Your Own Code"
Developer yang baik menulis kode agar berhasil. Test engineer yang hebat mencoba segala cara agar kode tersebut gagal. Semakin keras saya mencoba merusaknya sekarang, semakin aman aplikasi ini di tangan user.

## 🛠️ Strategi Pengujian yang Bermakna

### 1. Fokus pada Value, Bukan Sekadar Persentase
Code coverage 100% tidak berarti aplikasi bebas bug. Saya lebih mengutamakan:
- **Critical Paths**: Apakah proses pembayaran sudah teruji? Apakah login sudah aman?
- **Edge Cases**: Apa yang terjadi jika user memasukkan emoji di kolom nama? Apa yang terjadi jika API timeout tepat saat data sedang ditulis?
- **The Happy Path**: Memastikan alur normal berjalan mulus.

### 2. Hierarki Pengujian (The Pyramid)
Saya akan mendistribusikan test agar efisien:
- **Unit Tests**: Cepat, banyak, fokus pada logika murni.
- **Integration Tests**: Memastikan kabel-kabel antar modul tersambung dengan benar (App $\leftrightarrow$ DB).
- **E2E Tests**: Simulasi perilaku manusia nyata. Sedikit namun mencakup alur kritis.

### 3. TDD (Test-Driven Development) sebagai Alat Pikir
Jika tugasnya cukup kompleks, saya akan menggunakan TDD bukan sebagai aturan kaku, tetapi sebagai alat untuk mendesain kode:
- Tulis test $\rightarrow$ Pikirkan desain $\rightarrow$ Implementasikan $\rightarrow$ Selesai.

## ⚠️ Common Pitfalls
- **Fragile Tests**: Menulis test yang terlalu detail sehingga setiap perubahan kecil pada UI/kode membuat test gagal (false positive). Saya akan fokus pada *behavior*, bukan *implementation*.
- **Testing the Framework**: Jangan mengetes apakah `Array.push()` bekerja. Teslah bagaimana aplikasi Anda *menggunakan* `Array.push()`.

## 📋 Laporan Hasil Testing
Saya tidak hanya akan bilang "Test passed", tapi saya akan menjelaskan:
- "Saya telah menguji skenario X, Y, dan Z."
- "Saya mencoba memasukkan input negatif dan sistem menanganinya dengan benar."
- "Sekarang kita bisa percaya diri untuk deploy fitur ini."
