# Cambridge IELTS Web App (Meridian)

Web app interaktif untuk latihan soal Cambridge IELTS Academic (Buku 19 & 20) secara mandiri atau bersama teman.

## Fitur Utama

- **Audio Listening Terintegrasi**: 16 track audio Cambridge 19 (Test 1 - 4, Part 1 - 4) langsung terhubung dan siap diputar di browser tanpa perlu import file mp3 manual.
- **Split-Screen Reading & PDF Viewer**: Tampilan soal reading di sebelah kiri (langsung menampilkan PDF buku Cambridge) dan lembar jawaban di sebelah kanan (seperti tes asli IELTS Computer-Delivered).
- **Auto Jump Halaman PDF**: Tombol cepat untuk langsung melompat ke halaman Passage 1, Passage 2, atau Passage 3 sesuai tes yang dipilih.
- **Auto Grading**: Penilaian otomatis dengan kunci jawaban resmi untuk Cambridge 19 dan Cambridge 20 lengkap beserta konversi band score IELTS.
- **Modul Latihan Tambahan**: Vocabulary flashcards, grammar quiz, latihan writing & speaking.

## Struktur File

```text
cambridge-ielts-web/
├── index.html                   # Halaman web utama
├── audio/
│   └── c19/                     # File MP3 listening Cambridge 19
├── pdf/
│   ├── cambridge_ielts_19_academic.pdf
│   └── cambridge_ielts_20_academic_students_book.pdf
├── .gitignore
└── README.md
```

## Cara Menjalankan & Hosting

Web app ini 100% frontend statis (HTML, CSS, dan vanilla JavaScript murni di browser). **Tidak memerlukan backend server (tidak butuh Node.js / Python / database)**.

### 1. Di Hosting Biasa / cPanel / Shared Hosting
Tinggal upload seluruh isi folder ini ke `public_html` atau direktori web server.

### 2. Di GitHub Pages
1. Push folder ini ke repository GitHub.
2. Buka repository di GitHub -> **Settings** -> **Pages**.
3. Pilih source branch: `main` dan folder `/(root)` -> Klik **Save**.
4. Website akan langsung online di URL GitHub Pages kamu.

### 3. Di Lokal (Offline)
Bisa langsung double-click file `index.html` di browser (Chrome / Edge / Firefox) atau gunakan live server:
```bash
python -m http.server 8000
```
Lalu buka `http://localhost:8000`.
