# Panduan Pengelolaan Konten

## Mengubah profil dan kontak

Ubah `data/profile.json`. Foto profil disimpan pada `assets/images/profile/` dan CV pada `assets/documents/`.

Kosongkan nilai seperti `email`, `linkedin`, `github`, `whatsapp`, atau `cv` bila informasinya belum tersedia. Website tidak akan menampilkan tautan palsu untuk link kosong.

## Menambah pengalaman

Tambahkan objek baru ke array `data/experience.json`:

```json
{
  "organization": "Nama instansi",
  "position": "Posisi atau kegiatan",
  "type": "Internship | Professional Experience | Organization | Volunteer",
  "period": "Januari 2026 - Sekarang",
  "description": "Deskripsi tugas yang dapat diverifikasi.",
  "image": ""
}
```

## Prestasi

Tambahkan objek ke `data/achievements.json`. Gunakan `certificates` untuk beberapa sertifikat, `images` untuk foto penghargaan, dan `gallery` untuk dokumentasi.

## Proyek

Tambahkan objek baru ke `data/projects.json` dan unggah gambar ke folder thumbnail atau screenshot. `thumbnail` dapat dikosongkan agar website menampilkan ikon. Tandai proyek yang belum selesai sebagai `placeholder` atau `In Progress`, jangan menyebutnya sebagai proyek selesai bila belum ada bukti.

## Galeri

Isi `data/gallery.json` dengan album:

```json
{
  "title": "Judul album",
  "description": "Deskripsi kegiatan",
  "date": "2026",
  "photos": [
    { "src": "assets/images/documentation/album/foto.jpg", "caption": "Caption foto" }
  ]
}
```

## Menghapus data

Hapus objek JSON yang bersangkutan, simpan file valid, lalu lakukan commit. Nama file gambar tidak perlu ditulis jika hanya ingin menghapus tampilan data.

## Optimasi gambar

Gunakan JPEG/WebP untuk foto dan SVG hanya untuk gambar sederhana. Pertahankan foto profil di sekitar 1200 px, gambar galeri 1600 px, dan thumbnail 1200 x 750 px agar tidak lambat.

## Publikasi

Buka **Settings > Pages** pada repository GitHub, pilih **GitHub Actions** sebagai Source, lalu jalankan workflow `Deploy to GitHub Pages`. Website akan tersedia pada domain GitHub Pages repository.
