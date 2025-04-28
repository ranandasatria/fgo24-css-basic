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
```

## Tags Syntax
1. Paired: biasanya digunakan untuk memuat konten di antara bukaan dan tutupan
    contoh: <b>...</b>
2. Self-close/Void: biasanya berdiri sendiri karena tidak memerlukan konten tambahan lain
    contoh: <br>

## Attributes
- Setiap element tags memiliki attribute yang berbeda sesuai dengan peruntukkannya
- Ada yang memiliki attribute serupa karena memang tujuan dibubuhkannya juga sama atau hampir mirip

```
<p align="justify">
<igm src="/path/to/img.jpg" alt="alt text">
Lorem ipsum dolor sit amet
</p>
```

Attribute yang ada pada tiap tag html:
- class, id: untuk memberikan identitas, target selector css/js pada html
- style: untuk mengatur bagaimana konten pada tag tersebut ditampilkan secara inline

Attribute yang ada pada beberapa tag html saja:
- src: biasanya merujuk pada suatu resource url, bisa digunakan untuk tag img, script
- etc ...

## Basic Layouting
- Pengaturan tata letak yang dibagi berdasarkan jenis konten yang ingin ditampilkan
- Untuk membuat blok perjenis konten, bisa dipisahkan dengan div
- Diperbolehkan ada div di dalam div
- Secara umum, div tidak diperbolehkan ada di dalam tag formatting

## Images
- Untuk menampilkan gambar pada dokumen html, dapat menggunakan tag img
- Ada 2 attribute wajib pada tag, yakni src dan alt
- src: untuk memberikan acuan terhadap file gambar yang ingin ditampilkan
- alt: untuk memberikan teks alternatif jikafile gambar tidak dapat dimuat

## Table Structure
- Menggunakan tag table yang di dalamnya terdiri dari **thead**, **tbody**, dan **tfoot**
- tfoot opsional
- thead bagian judul dari setiap kolom tabel
- Di dalam sebagian tabel, terdiri dari tr untuk baris, td untuk kolom
- terkusus untuk thead, kolom dapat menggunakan th
- span untuk ngemerge kolom atau row

## Form Structure
- Formulir yang diisi user
- Untuk menginput data yang akan diproses/disimpan oleh server
- Form terdiri dari tag form, lalu di dalamnya ada input dan juga button
- Variasi input lain -> selection option

## Obsolote Tags and Attributes
- Banyak tags dan attributes yang sudah obsolete atau tidak digunakan lagi di HTML5
- Untuk memformat text disarankan dengan CSS
- Untuk animasi juga, seperti tag marquee, karena sudah tidak digunakan lagi

Tag:
- font
- marquee
- etc

Attribute:
- align
- border
- bgcolor
- etc

## Semantic Tag HTML
- HTML5 memiliki standar baku dalam pembuatan layout 
- Adanya semantic tag agar developer bisa deteksi bagian halaman web dari sintaks saja
- Disarannkan untuk mengganti div secara garis besar
- <header>, <nav>, <section>, <article>, <aside>, <footer>