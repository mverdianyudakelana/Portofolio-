# Portfolio — M. Verdian Yuda Kelana

Website portofolio statis yang responsif, ringan, dan kompatibel dengan GitHub Pages.

## Menjalankan secara lokal

```bash
python3 -m http.server 4173
```

Buka `http://localhost:4173`.

## Struktur penting

- `index.html` — struktur halaman utama.
- `css/styles.css` — seluruh styling dan responsive layout.
- `js/app.js` — pengambilan JSON, render konten, modal, tema, dan navigasi.
- `data/` — profil, pengalaman, prestasi, kemampuan, minat, proyek, dan galeri.
- `assets/images/` — foto profil, sertifikat, dokumentasi, dan aset proyek.
- `assets/documents/` — CV dan dokumen pendukung.
- `DOCUMENTATION.md` — panduan menambah, mengubah, dan menghapus konten.

## Deployment GitHub Pages

1. Pastikan branch utama bernama `main`.
2. Buka **Settings → Pages** pada repository GitHub.
3. Pada **Source**, pilih **GitHub Actions**.
4. Push perubahan ke branch `main`.
5. Workflow `.github/workflows/deploy.yml` akan memublikasikan website secara otomatis.

Untuk repository bernama `username.github.io`, website tersedia langsung di domain tersebut. Untuk repository lain, URL biasanya `https://username.github.io/nama-repository/`.

## Kontak dan asset

Informasi kontak, CV, foto profil, sertifikat, galeri, dan proyek masih perlu diisi oleh pemilik. File placeholder tidak boleh dianggap sebagai bukti prestasi atau pengalaman fiktif.
