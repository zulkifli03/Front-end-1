# Peta 16 Proyek HTML & CSS

[Buka galeri proyek harian](./proyek-harian/index.html) untuk melihat contoh hasil setiap pertemuan.

## Aturan proyek

- Bagian ini hanya belajar **HTML dan CSS**. Tidak memakai JavaScript, framework, atau backend.
- Komputer, editor dan browser sudah disiapkan. Hari pertama langsung mulai coding.
- Hari 1–14 adalah proyek mini mandiri. Hari 15–16 adalah satu proyek akhir yang sama, dikerjakan selama dua pertemuan: kamu akan membuat situs dengan beberapa halaman.
- Simpan setiap proyek di folder baru, misalnya `hari-01-cerita-mini`.

| Hari | Topik | Proyek hari ini | Yang dipelajari | Hari ini selesai sampai… |
|---|---|---|---|---|
| 1 | Basic Equipment | Cerita Mini HTML | Langsung praktik di editor dan browser; kerangka HTML, judul, paragraf, penekanan, daftar | Cerita terbuka di browser, berisi judul, dua bagian, paragraf, dan daftar tiga item. |
| 2 | Intro to HTML | Jadwal Kelas Multi-Halaman | `head`, `body`, `title`, `meta`, heading, tautan ke file HTML lain, tabel data | Ada `index.html` dan `tentang.html` dengan link dua arah; halaman jadwal berisi tabel dengan header dan empat baris data. |
| 3 | Intro to CSS | Poster Acara Berwarna | Menghubungkan CSS, selector, warna, font, ukuran dan alignment teks | Poster HTML memiliki tema warna dan judul yang mudah dibaca. |
| 4 | Intro to CSS | Kartu Profil | Class, box model, margin, padding, border, radius dan lebar | Kartu terpusat, tidak terlalu lebar, dan punya jarak konten yang nyaman. |
| 5 | List (HTML × CSS) | Menu Kantin | `ul`, `ol`, `li`, daftar bersarang dan gaya dasar | Ada dua kategori menu dan daftar langkah pemesanan dengan struktur yang sesuai. |
| 6 | List (HTML × CSS) | Checklist Acara | Daftar bertingkat, class, spacing, marker dan hover CSS | Tiga kelompok checklist mudah dibaca dan tiap kelompok berisi item yang benar. |
| 7 | Button Style (HTML × CSS) | Menu Navigasi | Tautan `<a>`, `href`, `id`, tautan ke halaman lain dan bagian dalam halaman, anchor bergaya tombol | Menu berpindah antarfile dan ke bagian yang benar; hover dan fokus keyboard terlihat. |
| 8 | Button Style (HTML × CSS) | Formulir Pendaftaran Acara | `form`, `label`, `input`, `select`, `option`, `textarea`, `button`, `required`, gaya kontrol form | Form punya label yang jelas, validasi dasar, tombol submit, dan tampilan rapi. Data latihan tidak tersimpan ke server. |
| 9 | Media (HTML × CSS) | Kartu Rekomendasi | `img`, path, `alt`, `figure`, `figcaption`, ukuran dan border | Dua rekomendasi memiliki media yang tampil baik, alt dan caption. |
| 10 | Media (HTML × CSS) | Galeri Foto/Video | Galeri, Grid/Flex, gap, ukuran konsisten; video lokal opsional | Galeri punya tiga item dengan keterangan dan susunan CSS konsisten. |
| 11 | Layout (HTML × CSS) | Profil Klub | `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, box model | Halaman punya bagian semantik yang terpisah dan navigasi yang bekerja. |
| 12 | Layout (HTML × CSS) | Katalog dengan Grid/Flex | Container, item, kolom, `gap`, alignment dan wrapping | Empat kartu tampil rapi pada layar lebar, dibuat dengan CSS bukan tabel layout. |
| 13 | HTML - Responsive | Kartu Acara untuk Ponsel | Meta viewport, lebar fleksibel, gambar responsif, media query | Halaman bisa dibaca di ponsel tanpa gulir horizontal. |
| 14 | HTML - Responsive | Katalog Multi-Layar | Uji ponsel/tablet/desktop dan perbaikan breakpoint | Tiga ukuran diuji dan minimal dua masalah tampilan yang nyata diperbaiki. |
| 15 | Free Project | Rancang Situs Multi-Halaman | Peta situs, beberapa file HTML, path relatif, navigasi bersama, stylesheet bersama | Ada minimal tiga file: `index.html`, `tentang.html`, `galeri.html`; menu pada tiap halaman saling terhubung. |
| 16 | Free Project | Poles dan Presentasikan Situs | CSS konsisten, responsive, uji seluruh navigasi, tur presentasi | Situs final minimal tiga halaman berbeda, tampil baik di ponsel, dan siap dipresentasikan sebagai tur halaman. |

## Tag HTML yang dipelajari

- **Kerangka dan metadata:** `doctype`, `html`, `head`, `body`, `meta`, `title`.
- **Teks:** `h1`–`h6`, `p`, `strong`, `em`, `br`, `hr`, komentar HTML.
- **Tautan:** `a`, `href`, tujuan `id`, tautan internal `#bagian`, dan tautan antarfile relatif seperti `tentang.html`.
- **Daftar:** `ul`, `ol`, `li`.
- **Tabel data:** `table`, `caption`, `thead`, `tbody`, `tr`, `th`, `td`.
- **Formulir:** `form`, `label`, `input`, `select`, `option`, `textarea`, `button`, `fieldset`, `legend`.
- **Media:** `img`, atribut `alt`, `figure`, `figcaption`; `video` dan `source` opsional.
- **Bagian halaman:** `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, serta `div`/`span` untuk pengelompokan.

Tabel HTML dipakai untuk data berbentuk baris dan kolom, bukan untuk menyusun layout. Tautan `<a>` berpindah ke halaman atau bagian; CSS dapat membuat tampilannya seperti tombol. Tidak ada aksi JavaScript di bagian ini.

## Form dan input: menerima isian, bukan menyimpan data

Pada Hari 8 kamu akan membuat form pendaftaran. Setiap kolom perlu `label` yang terhubung ke `id` kontrolnya. Gunakan `input` untuk jawaban singkat, `select`/`option` untuk pilihan, dan `textarea` untuk jawaban lebih panjang. Atribut `required` dan `type="email"` dapat meminta browser memeriksa isian dasar.

Form HTML dapat menampilkan dan memvalidasi isian, tetapi **HTML/CSS saja tidak menyimpan data ke database atau mengirim pendaftaran ke guru**. Contoh latihan boleh menuju halaman konfirmasi statis. Gunakan data pura-pura; nilai form dengan metode GET dapat tampak di URL dan bukan untuk data rahasia.

## Cara membuat beberapa halaman yang saling terhubung

Satu situs bukan berarti hanya satu file HTML. Buat beberapa file dalam folder proyek yang sama, misalnya:

```text
situsku/
  index.html
  tentang.html
  galeri.html
  style.css
```

Di `index.html`, tautan ke halaman lain ditulis `<a href="tentang.html">Tentang</a>`. Dari `tentang.html`, tautan kembali bisa memakai `<a href="index.html">Beranda</a>`. Semua file di folder yang sama memakai nama file sebagai path relatif. Setiap halaman memiliki kontennya sendiri dan tetap menghubungkan stylesheet yang sama dengan `<link rel="stylesheet" href="style.css">`.

Di Hari 15–16 kamu akan membuat situs akhir **minimal tiga halaman**. Hari 15 untuk merencanakan dan membangun struktur/tautan; Hari 16 untuk menyelesaikan CSS, menguji semua menu pada ponsel, dan mempresentasikan tur situs: Beranda → Tentang → Galeri.

## SEO dasar: kenapa perlu `<title>`?

`<title>` memberi nama pada tab browser dan sering digunakan sebagai judul bookmark atau calon judul hasil pencarian. Jika kosong atau tidak ada, halaman tetap dapat dibuka, tetapi tab/bookmark kurang informatif dan mesin pencari mungkin memilih teks lain. Title yang jelas **tidak menjamin** posisi tertentu di hasil pencarian.

`<meta name="description">` merangkum isi halaman dan dapat dipakai sebagai cuplikan hasil pencarian, tetapi mesin pencari boleh memilih teks lain. Heading harus mencerminkan urutan isi. Teks tautan sebaiknya menjelaskan tujuannya, sedangkan `alt` menjelaskan gambar informatif. Komentar HTML hanya catatan kode—tidak tampil di halaman dan bukan teknik SEO.
