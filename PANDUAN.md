# Panduan Deploy Portofolio GitHub

Paket ini berisi dua bagian:

- `profile-readme/README.md` → tampilan profil GitHub kamu
- `site/` → situs portofolio (GitHub Pages)

Ganti dulu semua placeholder: `USERNAME`, `EMAIL_KAMU@example.com`, `LINKEDIN_KAMU`.
Cari dengan Ctrl+F di kedua file (`README.md` dan `site/index.html`).

## A. Profil README (tampil di halaman profil)

1. Di GitHub, buat repo baru bernama **sama persis dengan username kamu** (contoh: `fathah/fathah`), set **Public**, centang *Add a README*.
2. Buka `README.md` di repo itu, timpa isinya dengan isi `profile-readme/README.md`, lalu commit.
3. Buka `github.com/USERNAME`, README akan tampil di profil.

## B. Situs portofolio (GitHub Pages)

1. Buat repo baru bernama **USERNAME.github.io** (Public).
2. Upload isi folder `site/` (`index.html` dan `style.css`) ke root repo, lalu commit.
3. Buka **Settings → Pages**, pada *Build and deployment* pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu Save.
4. Tunggu 1–2 menit, situs aktif di `https://USERNAME.github.io`.

## C. Lewat terminal (opsional)

```bash
cd site
git init
git add .
git commit -m "Portofolio pertama"
git branch -M main
git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
git push -u origin main
```

## D. Tips

- Pin 3–6 repo terbaik di profil (tombol *Customize your pins*).
- Pastikan repo Fire Guard, KampusMart, dan Tekkom Retail punya README dengan screenshot. Ubah link repo di `index.html` jika nama repo kamu berbeda.
- Tambahkan foto atau screenshot proyek ke folder `site/img/` dan pasang di kartu proyek.
