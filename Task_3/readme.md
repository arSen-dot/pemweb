# Dokumentasi Web Pendaftaran

Halaman web sederhana dua halaman: formulir pendaftaran dan detail pendaftar.

## Struktur File

- `pendaftaran.html` — halaman formulir pendaftaran
- `detail.html` — halaman detail informasi pendaftar (data dummy)
- `styles.css` — seluruh desain kedua halaman

## Halaman 1: Formulir Pendaftaran

Form menggunakan `method="get"` dengan `action="detail.html"`.

| Field | Tipe | name |
|---|---|---|
| Nama Lengkap | text | `nama` |
| NIM | text | `nim` |
| Email | email | `email` |
| Jenis Kelamin | radio | `jk` |
| Program Studi | select | `prodi` |
| Kelas | text | `kelas` |

## Desain Query String

Data dilempar dari halaman pendaftaran ke halaman detail lewat query string (hanya didesain, tidak ditangkap):

```
detail.html?nama=...&nim=...&email=...&jk=...&prodi=...&kelas=...
```

Contoh:

```
detail.html?nama=Reksa+Ariel+Saputra&nim=124140119&email=reksa@student.itera.ac.id&jk=Laki-laki&prodi=Teknik+Informatika&kelas=RB
```

## Halaman 2: Detail Pendaftar

Menampilkan data dummy: data pribadi, informasi akademik, dan tabel keterangan. Tombol "Kembali ke Form" mengarah ke `pendaftaran.html`.

## CSS

`styles.css` memakai 38 selector (syarat minimal 3), mencakup desain layout, box, tabel, dan form. Tidak ada inline style.
