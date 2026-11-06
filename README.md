# Meridian IELTS — Cambridge 19 & 20 Practice Suite

A complete, self-contained single-page web application for practicing authentic Cambridge IELTS Academic tests (Books 19 & 20). Built with zero build steps, modern HTML5/CSS/JavaScript, offline capability, and ready to host directly on **GitHub Pages**, **Vercel**, or **Netlify**.

---

## 🌟 Key Features

### 1. 🎧 Built-in Audio (No Manual Import Needed)
- All 16 official Listening audio tracks for **Cambridge 19** (Test 1 to 4, Parts 1 to 4) are pre-connected to the web app.
- Audio plays directly within the embedded player with speed controls (0.75x, 1x, 1.25x, 1.5x), ±10s seeking, and examination mode.
- Users no longer need to manually pick or import MP3 files from their local storage.
- Custom audio import into IndexedDB is still supported if users have extra audio files or Cambridge 20 tracks.

### 2. 📖 Integrated PDF Reader & Side-by-Side Split View
- **Authentic Computer-Delivered IELTS Experience**: On desktop/tablet, the screen automatically splits into:
  - **Left Panel (56%)**: Embedded Cambridge IELTS Book PDF displaying the reading passage or questions booklet.
  - **Right Panel (44%)**: Digital Answer Sheet with inputs, multiple-choice buttons, True/False/Not Given controls, and countdown timer.
- **Passage Jump Buttons**: Click `Passage 1`, `Passage 2`, or `Passage 3` to jump directly to the exact page of the passage in the PDF:
  - *Cambridge 19 Academic*: T1 (p.18, 22, 27), T2 (p.41, 45, 50), T3 (p.63, 68, 73), T4 (p.86, 90, 94).
  - *Cambridge 20 Academic*: T1 (p.11, 16, 21), T2 (p.47, 52, 57), T3 (p.86, 91, 96), T4 (p.122, 126, 131).
- **Pop-out Window (`↗ Pop-out`)**: For students with dual monitors or larger displays, open the PDF in a dedicated window or browser tab with 1 click.
- **Listening Booklet View**: Optional button to display the PDF questions booklet during Listening tests (essential for map labeling, diagrams, and tables!).
- **Mobile Responsive Tab Bar**: On mobile screens, effortlessly toggle between `📖 Cambridge PDF` and `✍️ Answer Sheet` with live question progress indicator.

### 3. 🎯 Full Built-in Auto-Grading (C19 & C20)
- **100% Official Answer Keys Transcribed**:
  - **Cambridge 19 Academic**: Tests 1, 2, 3, 4 (Listening & Reading: all 40/40 questions).
  - **Cambridge 20 Academic**: Tests 1, 2, 3, 4 (Listening & Reading: all 40/40 questions).
- **Instant IELTS Band Calculation**: Computes raw scores and converts to IELTS Band Scores (1.0 - 9.0).
- Detailed answer analysis showing correct answers, your answers, spelling/capitalization tolerance, and alternative acceptable answers.

### 4. 🧠 Additional Practice Modules
- **Spaced Repetition Vocabulary**: Built-in flashcard deck with IELTS topic words.
- **Grammar Lessons**: Interactive quizzes with instant explanations.
- **Writing Practice Hub**: Task 1 & Task 2 prompts with band descriptors and sample structures.
- **Speaking Hub**: Part 1, 2, and 3 simulation prompts.

---

## 📂 Repository Structure

```text
cambridge-ielts-web/
├── index.html                   # Main single-page web app
├── audio/
│   └── c19/                     # 16 pre-connected MP3 files
│       ├── T1 P1.mp3 ... T1 P4.mp3
│       ├── T2 P1.mp3 ... T2 P4.mp3
│       ├── T3 P1.mp3 ... T3 P4.mp3
│       └── T4 P1.mp3 ... T4 P4.mp3
├── pdf/
│   ├── cambridge_ielts_19_academic.pdf               # 27.8 MB
│   └── cambridge_ielts_20_academic_students_book.pdf # 3.5 MB
├── .gitignore
└── README.md
```

> **Note on file sizes**: All files in this repository are strictly under 30 MB each, comfortably below GitHub's 100 MB single-file push limit.

---

## 🚀 How to Host (Cara Hosting)

### Opsi 1: GitHub Pages (Paling Mudah & Gratis)
1. Buat repository baru di GitHub akun kamu/temanmu (misal: `cambridge-ielts-web`).
2. Push repository ini ke GitHub:
   ```bash
   git remote add origin https://github.com/<username>/cambridge-ielts-web.git
   git branch -M main
   git push -u origin main
   ```
3. Di halaman repository GitHub:
   - Buka tab **Settings** -> pilih menu **Pages** di sidebar kiri.
   - Di bagian **Build and deployment > Branch**: pilih `main` dan folder `/(root)`.
   - Klik **Save**.
4. Dalam 1-2 menit, web app akan aktif di:
   `https://<username>.github.io/cambridge-ielts-web/`

### Opsi 2: Vercel (Super Cepat dengan Global CDN)
1. Buka [vercel.com](https://vercel.com) dan login dengan akun GitHub.
2. Klik **Add New Project** -> **Import Git Repository**.
3. Pilih repository `cambridge-ielts-web`.
4. Framework Preset biarkan **Other**, klik **Deploy**.
5. Web langsung online dengan custom subdomain gratis `*.vercel.app` + HTTPS aktif.

### Opsi 3: Netlify
1. Buka [netlify.com](https://netlify.com) -> **Add new site** -> **Import an existing project**.
2. Hubungkan ke repository GitHub -> Deploy site.

### Opsi 4: Jalankan Lokal (Offline / Testing)
- Cukup buka file `index.html` langsung di browser Chrome/Edge, atau
- Gunakan simple HTTP server:
  ```bash
  # Python 3:
  python -m http.server 8080
  # Atau Node.js:
  npx serve
  ```
  Lalu buka `http://localhost:8080`.

---

## 🛠️ Credits & Attribution
- Test materials: Cambridge IELTS Authentic Practice Tests.
- UI Design: Meridian Aesthetic (Midnight ink & brass theme).
