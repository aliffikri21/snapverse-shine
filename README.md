# 💿 SNAPVERSE 2000 — 3D Y2K Web Photobooth

> **Aesthetic 4-Cut Photobooth Studio dengan Latar 3D Interaktif & Gaya Neo-Brutalism Y2K.**  
> Proyek karya untuk *Pameran Teknologi Rekayasa Multimedia (TRM)*.

---

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

---

## 🌟 Tentang Proyek

**SNAPVERSE 2000** adalah aplikasi web photobooth bergaya retro-futuristik (Y2K Neo-Brutalis) yang dirancang khusus untuk pameran interaktif. Aplikasi ini menghadirkan pengalaman berfoto strip 4-cut ala photobox Korea dengan sentuhan visual cyber tahun 2000-an, latar 3D animasi real-time, stiker interaktif drag-and-drop, serta efek audio prosedural tanpa membutuhkan server backend.

---

## ✨ Fitur Utama

- 🌐 **Latar Belakang 3D Retro (Three.js)**: Elemen wireframe geometris floating (*torus knot, icosahedron, octahedron*) yang berputar dinamis di latar belakang.
- 📸 **Sesi 4-Cut Otomatis**:
  - Countdown timer 3 detik per foto dilengkapi efek suara *beep* dan visual flash kamera.
  - Opsi jepret manual (*Single Snap*).
- 🎨 **Filter Kamera Real-Time**:
  - `Normal` — Warna natural jernih.
  - `Cyber Y2K` — Saturasi tinggi dengan nuansa neon futuristik.
  - `90s Camcorder` — Tone hangat sepia dilengkapi overlay scanline retro.
  - `Dreamy Pink` — Nuansa pastel magenta aesthetic.
  - `B&W Pop` — Kontras monokrom tajam ala pop art / manga.
- 👑 **Aksesori Kepala Virtual (Live AR Props)**:
  - Pixel Sunglasses 🕶️
  - Cyber Crown 👑
  - Neko Ears 🐱
  - Angel Halo 🪽
- 🖼️ **Studio Kustomisasi Strip Foto**:
  - **Pilihan Tema Frame**: Hot Pink, Cyber Cyan, Acid Lime, Midnight Grid, dan Holographic Gradient.
  - **Stiker Interaktif**: Tambahkan emoji Y2K favorit lalu **geser (drag-and-drop)** langsung ke posisi yang diinginkan di atas strip foto.
  - **Custom Caption**: Personalisasi teks pesan atau nama geng pada footer strip foto.
- 🔊 **Efek Suara Prosedural (Web Audio API)**:
  - Efek hitung mundur, suara shutter mekanik kamera, dan suara pop UI yang disintesis secara real-time tanpa file audio eksternal.
- 💾 **Download Hasil HD (PNG)**: Unduh strip foto beresolusi tinggi langsung ke perangkat dengan satu klik.
- 📱 **Mode Fallback Simulator**: Jika kamera tidak diizinkan atau perangkat tidak memiliki webcam, aplikasi otomatis beralih ke mode simulasi sehingga antarmuka tetap dapat diuji.

---

## 🛠️ Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| **Struktur** | Semantic HTML5 & Canvas API |
| **Gaya & Layout** | Vanilla CSS3 (Neo-Brutalism design system, CSS Grid, Flexbox) |
| **Tipografi** | [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) & [Syne](https://fonts.google.com/specimen/Syne) via Google Fonts |
| **Grafik 3D** | [Three.js r128](https://threejs.org/) via CDN |
| **Audio** | HTML5 Web Audio API (Synthesizer Oscillators & Noise Buffer) |
| **Stream Kamera** | MediaDevices `getUserMedia` API |

---

## 🚀 Cara Menjalankan

Proyek ini dibuat **zero-dependency / standalone** (tidak membutuhkan `npm install` atau build step).

### Opsi 1: Buka Langsung di Browser
1. Clone atau download repositori ini:
   ```bash
   git clone https://github.com/USERNAME/REPO-NAME.git
   ```
2. Buka file `snapverse.html` langsung dengan klik 2x atau seret ke browser favorit Anda (Chrome, Edge, Firefox, Brave, Safari).

### Opsi 2: Menggunakan VS Code Live Server (Direkomendasikan)
1. Buka folder proyek di **Visual Studio Code**.
2. Pasang ekstensi **Live Server** (oleh Ritwick Dey).
3. Klik kanan pada file `snapverse.html` dan pilih **"Open with Live Server"**.
4. Berikan izin akses kamera pada pop-up browser untuk menikmati pengalaman penuh.

---

## 🌐 Cara Deploy ke GitHub Pages

Agar aplikasi dapat diakses secara online oleh siapa saja:

1. **Ubah nama file utama** (Opsional tapi direkomendasikan):
   - Ubah nama `snapverse.html` menjadi `index.html` agar langsung terbaca sebagai halaman utama.
   *(Atau tetap gunakan `snapverse.html` dan akses via `https://<username>.github.io/<repo-name>/snapverse.html`)*.
2. Push repositori ke GitHub:
   ```bash
   git init
   git add .
   git commit -m "feat: initial commit SNAPVERSE Y2K Photobooth"
   git branch -M main
   git remote add origin https://github.com/USERNAME/REPO-NAME.git
   git push -u origin main
   ```
3. Buka repositori Anda di GitHub.
4. Masuk ke menu **Settings** > **Pages**.
5. Pada bagian **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: pilih `main` dan folder `/ (root)`
   - Klik **Save**.
6. Tunggu beberapa detik, tautan website photobooth Anda sudah live! ✨

---

## 📁 Struktur Berkas

```text
shine-project3/
├── snapverse.html    # Kode utama aplikasi (HTML, CSS, JS, Audio, Canvas, Three.js)
└── README.md         # Dokumentasi proyek
```

---

## 🎮 Panduan Penggunaan

1. **Izinkan Akses Kamera**: Saat browser meminta izin webcam, klik **Allow / Izinkan**.
2. **Pilih Filter & Prop**: Klik tombol pada bagian *Filter Kamera* dan *Aksesori Live* sesuai gaya yang diinginkan.
3. **Mulai Foto**:
   - Klik **MULAI SESI 4 FOTO OTOMATIS** untuk pemotretan berseri (interval 3 detik).
   - Atau klik **Jepret Manual** jika ingin mengambil foto satu per satu.
4. **Hias Photostrip**:
   - Pilih tema warna bingkai di panel sebelah kanan.
   - Klik stiker emoji untuk menambahkannya ke strip, lalu **drag / geser** stiker tersebut ke posisi terbaik.
   - Ubah tulisan footer pada kolom input teks.
5. **Simpan Hasil**: Klik tombol hijau **UNDUH PHOTOSTRIP (PNG HD)** untuk menyimpan hasil foto ke perangkat Anda.

---

## 📄 Lisensi

Didistribusikan di bawah Lisensi MIT. Bebas digunakan untuk keperluan edukasi, pameran, dan pengembangan non-komersial/komersial.

---

<p align="center">
  Dibuat dengan 💖 & ⚡ untuk <strong>Pameran Teknologi Rekayasa Multimedia</strong>
</p>
