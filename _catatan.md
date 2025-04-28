npm init -y
npm install live-server --save-dev
save di script package: "dev": "live-server"
npm run dev

Struktur:
```<!DOCTYPE html>
<title>
<head>
    --meta data--
```
## Basic metadata:
- Mengatur judul halaman
- Memberikan deskripsi singkat
- Dukungan responsif dasar halaman
- Informasi encoding

```
- <title>Judul Halaman</title>
- <meta name="description"
content = "deskripsikan halaman di sini">
- <meta name="viewport">
content = "width=device-width, initial-scale=1.0"
- <meta charset="UTF-8>
```

## Basic formatting:
```
- <p>Sekumpulan text</p>
- <b><u><i><mark><br>etc
```

## Multipage and hyperlinking
- Base document file (index.html)
- Halaman bisa di dalam sebuah folder
- Metadata dan Body berlaku hanya pada halamannya sendiri, tidak bisa di-turunkan
- Bisa membuat referensi ke halaman lain yang berbeda

```
<a href="nama-file.html">Text Hyperlink</a>
<a href="nama-file.html" target ="_blank">Ketika di-klik membuka tab browser baru</a>

