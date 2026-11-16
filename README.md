# Fullscreen Video Gallery (Auto-Detect GitHub Folder)

## Struktur Folder
```
├── index.html
└── vid/
    └── (masukkan semua file video Anda di sini, nama file bebas)
```

## Cara Pakai di GitHub Pages (100% Otomatis)
1. Ekstrak file ZIP ini.
2. Masukkan semua file video Anda (`.mp4`, `.webm`, `.mov`, dll.) ke dalam folder `vid/` — **tidak perlu mengganti nama file**.
3. Upload file `index.html` beserta folder `vid/` ke repositori GitHub Anda (pastikan visibilitas repositori adalah **Public**).
4. Buka tab **Settings > Pages** di repositori GitHub Anda, pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
5. Buka link GitHub Pages Anda (`https://username.github.io/nama-repo/`). Skrip akan otomatis mendeteksi username, nama repositori, dan seluruh isi video di dalam folder `vid/`.

## Catatan
- Maksimal ukuran per file video di GitHub standar adalah **100 MB** (disarankan < 50 MB agar loading cepat).
- Menggunakan `sessionStorage` cache agar pengunjung tidak terkena batas *rate-limit* GitHub API saat me-refresh halaman.
