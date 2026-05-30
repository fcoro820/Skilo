# 🌟 Skilo: AI Engineering Partner Framework

**Skilo** adalah sebuah framework konfigurasi dan instruksi untuk mentransformasi AI Coding Agent menjadi seorang **Engineering Partner**. 

Berbeda dengan AI asisten biasa yang hanya mengeksekusi perintah, Skilo dirancang untuk membawa filosofi engineering yang mendalam: memastikan setiap baris kode tidak hanya "jalan", tetapi juga elegan, stabil, aman, dan mudah dipelihara.

## 🚀 Filosofi Utama

Skilo beroperasi berdasarkan **The Engineering Partner Manifesto** yang menekankan pada:
- **Kualitas di atas Kecepatan**: Memastikan fondasi yang kuat sebelum membangun fitur.
- **Proaktif & Transparan**: Memberikan saran optimasi dan peringatan risiko keamanan tanpa diminta.
- **Berbasis Bukti**: Selalu membaca kode dan menjalankan tes sebelum menyarankan perubahan.
- **Siklus Adaptasi**: Terus belajar dari feedback pengguna dan mencatatnya dalam `MEMORY.md`.

## 🧠 Sistem Keahlian (Skills)

Skilo memiliki berbagai "mode" atau skill spesialis yang dapat diaktifkan secara otomatis tergantung pada konteks tugas:

| Skill | Peran | Deskripsi |
| :--- | :--- | :--- |
| `codebase` | The Explorer | Memetakan arsitektur dan memahami aliran logika sistem. |
| `workflow` | The Strategist | Merancang strategi eksekusi dan memecah kompleksitas tugas. |
| `bug-hunt` | The Detective | Mendiagnosis dan membasmi bug dengan pendekatan sistematis. |
| `fixer` | The Craftsman | Refactoring dan optimasi kode agar lebih elegan dan efisien. |
| `test-engineer`| The Guardian | Membangun jaring pengaman melalui unit, integration, dan E2E tests. |
| `security-audit`| The Paranoid | Mencari celah kerentanan dan mengaudit manajemen secret. |
| `code-reviewer` | The Mentor | Menjadi quality gate terakhir untuk memastikan standar tertinggi. |
| `docs` | The Translator | Mengubah kompleksitas teknis menjadi dokumentasi yang jelas. |
| `devops` | The Bridge | Menangani otomatisasi, infrastruktur, dan deployment. |

## 📂 Struktur Proyek

- `/skills`: Berisi instruksi mendalam untuk setiap spesialisasi (SKILL.md).
- `/templates`: Template standar untuk ADR, Bug Report, Changelog, dan README.
- `AGENTS.md`: Manifesto dan filosofi kerja.
- `MEMORY.md`: Log adaptasi dan pembelajaran agent.
- `toolbelt.md`: Daftar tool CLI yang digunakan untuk eksekusi teknis.

## 🛠️ Cara Kerja

Skilo menggunakan teknik **Skill Chaining**. Sebagai contoh, saat diminta menambahkan fitur baru, Skilo akan:
1. **Explorer** (`codebase`) $\rightarrow$ Memahami konteks.
2. **Strategist** (`workflow`) $\rightarrow$ Merencanakan langkah.
3. **Guardian** (`test-engineer`) $\rightarrow$ Menulis test.
4. **Craftsman** (`fixer`) $\rightarrow$ Mengimplementasikan kode.
5. **Mentor** (`code-reviewer`) $\rightarrow$ Mereview hasil.
6. **Translator** (`docs`) $\rightarrow$ Mendokumentasikan perubahan.

---
*Skilo bukan sekadar agent; ia adalah partner Anda dalam menciptakan software yang luar biasa.*
