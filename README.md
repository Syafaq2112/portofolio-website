# Portofolio — Syafaq Jiwa Raharjo

Website portofolio pribadi yang dibangun untuk **Tugas K2 — Teknologi Platform (ITB)**.
Situs statis (HTML, CSS, JavaScript) yang di-deploy otomatis menggunakan **CI/CD pipeline**.

🔗 **Live:** _(akan diisi setelah deploy ke GitHub Pages)_

## ✨ Fitur

- Desain modern, responsif (mobile & desktop)
- Mode gelap / terang dengan penyimpanan preferensi
- Animasi reveal saat scroll, progress bar, smooth scrolling
- Section: Hero, Tentang, Pendidikan, Pengalaman, Proyek, Skill, Kontak

## 🛠️ Teknologi

| Bagian       | Teknologi                          |
| ------------ | ---------------------------------- |
| Markup       | HTML5                              |
| Styling      | CSS3 (custom properties, grid)     |
| Interaktif   | JavaScript (vanilla)               |
| CI/CD        | GitHub Actions → GitHub Pages      |

## 🚀 Menjalankan secara lokal

```bash
# dari dalam folder proyek
python3 -m http.server 4321
# lalu buka http://localhost:4321
```

## ⚙️ Deployment (CI/CD)

Setiap `git push` ke branch `main` akan memicu workflow di
[`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) yang otomatis
men-deploy ulang situs ke GitHub Pages. Inilah inti dari pipeline CI/CD:
**perubahan kode → otomatis live**.

## 📁 Struktur

```
portofolio-website/
├── index.html              # Halaman utama
├── styles.css              # Seluruh styling
├── script.js               # Interaktivitas
├── README.md
└── .github/workflows/
    └── deploy.yml          # Pipeline deploy otomatis
```
