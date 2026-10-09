# Panduan Guru — 16 Proyek HTML & CSS

## Prinsip pembelajaran

- Materi bagian ini **HTML dan CSS saja**. Tidak ada JavaScript, framework, atau backend.
- Hari 1–14 masing-masing memiliki mini-proyek dan folder sendiri. Hari 15–16 adalah pengecualian: keduanya merupakan satu capstone multi-halaman yang dirancang, dibangun, dan dipresentasikan selama dua pertemuan.
- Perangkat dan aplikasi sudah disediakan kantor. Hari pertama langsung mulai coding; cek editor dan browser seperlunya saja.
- Tampilkan target dan kriteria selesai kepada siswa di awal kelas. Demonstrasikan bagian kecil, lalu minta siswa ikut mengetik dan menguji.
- Boleh membuka proyek sebelumnya sebagai referensi, tetapi mulai pekerjaan hari ini di folder baru.
- Contoh proyek yang dapat dibuka di browser tersedia di [Peta Proyek Harian](./proyek-harian/index.html). Gunakan sebagai demo hasil; untuk latihan, siswa mengetik kode di folder proyek mereka sendiri.
- Contoh capstone tiga halaman tersedia di [Proyek Akhir Klub Jelajah](./proyek-harian/proyek-akhir/index.html).

## Pola waktu standar (90 menit)

| Menit | Kegiatan |
|---|---|
| 0–10 | Tampilkan contoh, jelaskan target belajar dan kriteria selesai hari ini. |
| 10–25 | Demonstrasi konsep HTML/CSS hari ini; siswa menirukan bagian inti. |
| 25–50 | Praktik terpandu membangun kerangka dan konten proyek. |
| 50–72 | Praktik mandiri: lengkapi seluruh fitur wajib. |
| 72–83 | Uji di browser, saling memberi masukan, dan perbaiki satu hal. |
| 83–90 | Tampilkan hasil, exit ticket, lalu simpan proyek hari ini. |

Sesuaikan pembagian jika kelas perlu lebih banyak waktu mengetik. Pertahankan waktu uji dan penyimpanan; fitur bonus yang boleh dikurangi.

**Struktur folder:** satu folder per hari (`hari-01-cerita-mini`, `hari-02-jadwal-kelas`, dan seterusnya), berisi `index.html`; mulai Hari 3 buat `style.css`. Gambar/video lokal, bila dipakai, disimpan dalam subfolder `assets`. Capstone Hari 15–16 memiliki beberapa file HTML dalam satu folder dan berbagi satu stylesheet.

## Peta tag HTML dan konsep CSS

Ajarkan ketika digunakan; tidak perlu meminta siswa menghafal semua tag sekaligus.

| Materi | Kapan dipelajari |
|---|---|
| `<!doctype html>`, `html lang`, `head`, `body`, `meta charset`, `title` | Hari 1–2 |
| `meta name="description"`, `meta name="viewport"` | SEO dasar Hari 2; responsive Hari 13 |
| `h1`–`h6`, `p`, `strong`, `em`, `br`, `hr`, komentar HTML | Hari 1–2 |
| `a`, `href`, `id`, tautan eksternal, fragmen `#bagian`, tautan antarfile relatif (`kegiatan.html`, `pages/tentang.html`, `../index.html`) | Dasar dan dua file HTML Hari 2; navigasi bergaya Hari 7–8; capstone Hari 15–16 |
| `ul`, `ol`, `li` | HTML dasar Hari 1; praktik dan CSS Hari 5–6 |
| `table`, `caption`, `thead`, `tbody`, `tr`, `th`, `td`, `scope` | Hari 2 |
| `link rel="stylesheet"`, selector elemen/class, cascade dasar | Hari 3–4 |
| `form`, `label`, `input`, `select`, `option`, `textarea`, `button`, `fieldset`, `legend`, `required` | Hari 8 |
| `img`, `alt`, `figure`, `figcaption`; `video`, `source`, `controls` (opsional) | Hari 9–10 |
| `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `div`, `span` | Hari 11 |
| Box model, `display`, Flexbox atau Grid, `gap`, alignment | Hari 4, 11–12 |
| Pseudo-class `:hover`, `:focus-visible`, media query, viewport | Hari 7–8, 13–14 |

### SEO dasar dalam cakupan HTML

Jelaskan SEO sebatas struktur dan metadata HTML; SEO bukan jaminan halaman mendapat peringkat tertentu.

- **`<title>`** memberi nama dokumen pada tab browser, bookmark, dan sering menjadi calon judul hasil pencarian. Jika kosong/tidak ada, halaman tetap berfungsi, tetapi tab/bookmark kurang informatif dan mesin pencari dapat memilih teks lain sebagai judul.
- **`<meta name="description" content="...">`** memberi ringkasan yang dapat dipakai sebagai cuplikan hasil pencarian. Mesin pencari bisa memilih teks lain. Description bukan pengganti isi halaman.
- Heading harus mengikuti struktur informasi (`h1`, lalu subbagian), bukan dipilih hanya karena ukuran tampilannya.
- Teks tautan perlu menjelaskan tujuannya. `alt` mendeskripsikan gambar informatif; jangan mengisinya dengan kata kunci.
- `lang="id"` menyatakan bahasa utama halaman. Komentar HTML untuk catatan kode, bukan konten atau teknik SEO; komentar tidak tampil sebagai halaman dan sumber kode dapat dilihat orang.

## Rencana pertemuan

### Hari 1 — Basic Equipment: Cerita Mini HTML

**Yang dipelajari:** langsung menulis dokumen HTML di perangkat yang sudah disiapkan, tag dasar, menyimpan, memuat ulang, dan membaca hasil browser.  
**Tag:** `doctype`, `html`, `head`, `title`, `body`, `h1`, `h2`, `p`, `strong`, `em`, `ul`, `ol`, `li`.  
**Proyek:** halaman cerita mini atau cerita tentang kegiatan yang disukai.  
**Sampai sini:** halaman dibuka di browser, memiliki judul, dua bagian, paragraf, satu penekanan, dan daftar yang sesuai isi.

| Menit | Arahan guru |
|---|---|
| 0–5 | Pastikan editor/browser siap. Sampaikan proyek dan target; langsung mulai, tanpa instalasi atau pengenalan alat panjang. |
| 5–15 | Tampilkan contoh cerita. Demonstrasikan satu perubahan teks, simpan, lalu muat ulang browser. |
| 15–30 | Ketik kerangka dokumen dan jelaskan `head`/`body` serta title tab. Siswa mengikuti. |
| 30–48 | Siswa menulis `h1`, dua `h2`, dan paragraf cerita. Ingatkan tag pembuka dan penutup. |
| 48–62 | Tambahkan `strong`/`em` untuk penekanan serta `ul` atau `ol` dengan tiga `li`. |
| 62–74 | Siswa memperkaya cerita dan mengubah isi agar menjadi karya masing-masing. |
| 74–83 | Tukar hasil: cek tag penutup, struktur, dan tampilan browser; perbaiki satu kesalahan. |
| 83–90 | Beberapa siswa berbagi. Exit ticket: fungsi `title`, `body`, dan perbedaan `ul` dengan `ol`. |

**Cek selesai:** file tersimpan dan tampil; satu `h1`, dua `h2`, minimal tiga paragraf, satu daftar 3 item, dan satu perubahan berhasil terlihat di browser.  
**Bantuan:** bagikan kerangka HTML yang sebagian tag pembukanya sudah tersedia.  
**Tantangan:** tambahkan komentar HTML singkat dan tunjukkan bahwa komentar bukan bagian yang terlihat di halaman.

### Hari 2 — Intro to HTML: Jadwal Kelas Multi-Halaman

**Yang dipelajari:** metadata dokumen, struktur heading, tautan eksternal dan tautan ke file HTML lain, serta tabel data. Pengenalan SEO dasar lewat `title` dan description.  
**Tag:** `meta`, `title`, `h1`–`h3`, `p`, `a`, `ul`, `table`, `caption`, `thead`, `tbody`, `tr`, `th`, `td`.  
**Proyek:** situs informasi kelas dua halaman: `index.html` berisi jadwal; `tentang.html` berisi informasi kelas. Kedua halaman punya tautan untuk berpindah dan kembali.  
**Sampai sini:** siswa membuat dua file HTML di folder yang sama, menghubungkannya dengan path relatif sederhana (`href="tentang.html"`), dan membangun tabel data. Tidak ada CSS yang diwajibkan.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tunjukkan halaman informasi yang sama dengan title kosong dan title jelas; bandingkan nama tab dan konteks halaman. |
| 10–25 | Demonstrasikan `meta charset`, `title`, `meta description`, heading dan paragraf. Jelaskan bahwa metadata berada di `head`, bukan di badan konten. |
| 25–38 | Siswa membuat `index.html` dengan struktur lengkap, title, heading, dan pengantar info kelas. |
| 38–48 | Ajarkan `<a href="...">`, lalu tunjukkan bahwa `href="tentang.html"` membuka file HTML lain di folder yang sama; path ditulis relatif terhadap file saat ini. |
| 48–58 | Siswa membuat file `tentang.html` di folder yang sama dan menambahkan tautan kembali ke `index.html`. Pastikan ejaan nama file sama persis. |
| 58–72 | Demonstrasikan tabel data: `caption`, baris header `th`, `tr` dan `td`. Tegaskan tabel untuk data, bukan layout. |
| 72–80 | Siswa menambahkan jadwal minimal 3 kolom dan 4 baris data ke `index.html`. |
| 80–85 | Uji kedua arah navigasi, title tab pada kedua halaman, dan tabel. |
| 85–90 | Exit ticket: bedakan `href="#jadwal"` dengan `href="tentang.html"`; kapan menggunakan `th` bukan `td`? |

**Cek selesai:** ada dua halaman HTML dengan title masing-masing, tautan antarhalaman dua arah yang bekerja, dan tabel bercaption/header dengan 4 baris data pada halaman jadwal.  
**Catatan guru:** title yang bagus membantu konteks tetapi tidak menjamin posisi pencarian. Description bisa dipakai sebagai cuplikan atau diganti mesin pencari.

### Hari 3 — Intro to CSS: Poster Acara Berwarna

**Yang dipelajari:** menghubungkan CSS ke HTML, sintaks rule, selector elemen, warna dan tipografi.  
**HTML:** `<link rel="stylesheet" href="style.css">`, heading, paragraf.  
**CSS:** selector, property/value, `color`, `background-color`, `font-family`, `font-size`, `text-align`.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan poster HTML polos dan poster bergaya; bedakan konten dengan presentasi. |
| 10–25 | Buat `style.css`; demonstrasikan link stylesheet, selector, kurung kurawal, property dan value. |
| 25–45 | Siswa membuat poster acara baru dengan judul, tanggal, deskripsi dan pengumuman. |
| 45–65 | Atur warna latar/teks, font, ukuran judul, dan alignment. Uji perubahan satu properti setiap kali. |
| 65–75 | Siswa memilih palet warna yang kontras dan menerapkannya konsisten. |
| 75–84 | Uji: ubah sementara nama file CSS untuk melihat efeknya, pulihkan, lalu cek tampilan. |
| 84–90 | Exit ticket: identifikasi selector, property, dan value dalam satu rule. |

**Cek selesai:** HTML tetap berisi konten, CSS terhubung, poster punya hierarki visual dan teks terbaca.

### Hari 4 — Intro to CSS: Kartu Profil dengan Box Model

**Yang dipelajari:** class, box model, ukuran, margin, padding, border, radius dan selector class.  
**Proyek:** kartu profil satu halaman dengan tema visual pilihan.  
**CSS:** `.class`, `width`, `max-width`, `margin`, `padding`, `border`, `border-radius`, `box-sizing`.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan kartu sempit dan kartu yang terlalu rapat; minta siswa menunjuk area ruang dalam/luar. |
| 10–25 | Demonstrasikan class di HTML, selector titik di CSS, lalu gambarkan content–padding–border–margin. |
| 25–45 | Siswa menulis kartu profil baru: nama, deskripsi, dan tiga fakta diri. |
| 45–65 | Beri lebar maksimum, margin tengah, padding, border, radius dan latar kartu. |
| 65–75 | Ubah padding lalu margin secara terpisah; siswa memprediksi dampaknya. |
| 75–84 | Pasangan cek keterbacaan, ruang dan konsistensi class. |
| 84–90 | Exit ticket: jelaskan margin vs padding pada kartu. |

**Cek selesai:** kartu terpusat, konten memiliki ruang, batas kartu terlihat, dan lebar tidak berlebihan.

### Hari 5 — List (HTML × CSS): Menu Kantin

**Yang dipelajari:** `ul`, `ol`, `li`, daftar bersarang, serta memilih struktur berdasarkan makna.  
**Proyek:** menu kantin dengan kategori makanan/minuman dan langkah pemesanan.

| Menit | Arahan guru |
|---|---|
| 0–10 | Bandingkan menu dengan urutan cara memesan; tentukan mana yang perlu urutan. |
| 10–25 | Demonstrasikan `ul`, `ol`, `li`, dan struktur nesting. |
| 25–45 | Siswa membuat menu dengan dua kategori dan minimal empat item per kategori. |
| 45–62 | Tambahkan daftar berurutan untuk tiga langkah pemesanan; gunakan heading dan paragraf singkat. |
| 62–74 | Tambahkan file CSS baru, atur warna dasar, font, dan jarak halaman. |
| 74–84 | Saling cek: urutan daftar benar dan nesting valid; matikan CSS sementara untuk cek makna. |
| 84–90 | Exit ticket: kapan memakai `ol`, kapan memakai `ul`? |

**Cek selesai:** dua daftar kategori dan satu daftar langkah; tiap item memakai `li`; CSS terbaca dan sederhana.

### Hari 6 — List (HTML × CSS): Checklist Persiapan Acara

**Yang dipelajari:** mengelompokkan dan menata daftar dengan class, selector turunan, spacing, marker dan hover CSS.  
**Proyek:** checklist persiapan acara dengan kelompok sebelum/saat/setelah acara.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan checklist yang terlalu panjang; siswa usulkan cara mengelompokkan. |
| 10–25 | Demonstrasikan daftar bersarang, class, selector seperti `.checklist li`, `padding`, `margin`, `list-style` dan hover. |
| 25–45 | Siswa membuat tiga kelompok checklist, masing-masing minimal tiga item. |
| 45–65 | Gaya heading, jarak item, marker, dan latar kelompok tanpa mengubah makna HTML. |
| 65–75 | Tantangan inti: buat salah satu kelompok tampak berbeda dengan class tambahan. |
| 75–84 | Uji hover, nesting dan keterbacaan; berikan masukan ke pasangan. |
| 84–90 | Exit ticket: kenapa struktur daftar dibuat di HTML, bukan dengan mengetik tanda bullet sendiri? |

**Cek selesai:** tiga kelompok, masing-masing tiga item; gaya konsisten; HTML tetap bermakna tanpa CSS.

### Hari 7 — Button Style (HTML × CSS): Menu Navigasi

**Yang dipelajari:** tautan sebagai navigasi ke bagian halaman dan ke file HTML lain; menata `<a>` seperti tombol memakai CSS.  
**Tag:** `a`, `href`, `id`, `nav`, `ul`, `li`.  
**CSS:** inline/flex, padding, background, border, radius, hover dan focus.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tunjukkan tautan biasa dan menu navigasi; tanyakan apa yang terjadi saat diklik. |
| 10–25 | Ulas `href="tentang.html"` untuk pindah file dan ajarkan `href="#bagian"` untuk menuju id dalam file yang sama; keduanya adalah tautan. |
| 25–45 | Siswa membuat situs panduan hobi kecil dengan `index.html` dan `tips.html`; tambahkan nav yang berpindah di antara dua file serta tautan internal ke bagian tips. |
| 45–65 | Gaya tautan sebagai tombol/menu: padding, warna, radius dan jarak; pastikan pola nav konsisten di dua halaman. |
| 65–75 | Tambahkan `:hover` dan `:focus-visible`; pastikan keyboard Tab menunjukkan posisi fokus. |
| 75–84 | Uji semua tujuan tautan, label, hover dan fokus. |
| 84–90 | Exit ticket: apa yang dilakukan `href="#alat"` dan elemen mana memerlukan `id="alat"`? |

**Cek selesai:** navigasi antarfile dan tautan ke bagian yang tepat bekerja; menu punya label jelas dan keadaan hover/focus terlihat.  
**Catatan cakupan:** tombol di pertemuan ini adalah tautan `<a>` yang ditata seperti tombol; tidak membuat aksi yang memerlukan JavaScript.

### Hari 8 — Button Style (HTML × CSS): Formulir Pendaftaran Acara

**Yang dipelajari:** formulir HTML dasar, label dan input yang terhubung, pilihan, area teks, tombol submit, serta gaya form dan state tombol dengan CSS.  
**Tag/atribut:** `form`, `label`, `input type="text"`, `input type="email"`, `select`, `option`, `textarea`, `button type="submit"`, `fieldset`, `legend`, `name`, `required`.  
**Proyek:** formulir pendaftaran acara sekolah yang mengumpulkan nama, email latihan, pilihan sesi, dan alasan ikut.  
**Catatan penting:** form HTML mengumpulkan nilai kontrol, tetapi HTML/CSS saja tidak menyimpan atau mengirimnya ke database. Contoh memakai halaman konfirmasi statis dan data latihan saja; jangan masukkan data pribadi asli. Field bernama dapat muncul di URL ketika memakai metode GET.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan formulir pendaftaran; minta siswa mencocokkan label pertanyaan dengan tempat mengetik atau memilih. |
| 10–25 | Demonstrasikan `form`, `label for` yang cocok dengan `input id`, `name`, `type`, `required`, `select/option`, `textarea`, serta `button type="submit"`. Tunjukkan `fieldset/legend` sebagai pengelompokan opsional. |
| 25–45 | Siswa membuat form dengan nama, email latihan, pilihan sesi, dan alasan ikut. Setiap kontrol memiliki label yang terlihat dan `name` berbeda. |
| 45–62 | Tambahkan validasi browser sederhana (`required`, `type="email"`); uji kirim kosong agar pesan validasi muncul. |
| 62–74 | Tautkan form ke halaman konfirmasi statis; uji hanya dengan data contoh. Jelaskan bahwa ini tidak menyimpan data dan nilai GET dapat terlihat di URL. |
| 74–84 | Gaya label, input, select, textarea dan tombol; uji fokus keyboard, jarak, dan tampilan ponsel. |
| 84–90 | Exit ticket: apa fungsi `label`, `required`, dan apa yang belum bisa dilakukan form HTML/CSS tanpa backend? |

**Cek selesai:** form memiliki minimal tiga jenis kontrol dengan label terkait, validasi dasar berjalan, tombol submit ada, dan siswa dapat menjelaskan bahwa hasilnya tidak tersimpan di server.
**Bantuan:** mulai dengan field nama dan email saja; tambahkan pilihan sesi jika sudah selesai.
**Tantangan:** kelompokkan field dengan `fieldset/legend` atau tambahkan checkbox persetujuan opsional.

### Hari 9 — Media (HTML × CSS): Kartu Rekomendasi

**Yang dipelajari:** gambar lokal, path, `alt`, `figure`, `figcaption`, ukuran dan border CSS.  
**Proyek:** dua kartu rekomendasi buku, film, permainan, atau tempat.

| Menit | Arahan guru |
|---|---|
| 0–10 | Bandingkan gambar informatif dengan dekoratif; tanyakan teks apa yang dibutuhkan bila gambar gagal muncul. |
| 10–25 | Demonstrasikan `<img src alt>`, path relatif, `figure/figcaption`, lebar fleksibel dan `height: auto`. |
| 25–45 | Siswa membuat dua kartu rekomendasi, masing-masing gambar, judul, caption dan deskripsi. |
| 45–65 | Tambahkan `alt` yang menjelaskan gambar informatif; gaya ukuran gambar, border dan radius. |
| 65–75 | Periksa sumber gambar yang boleh digunakan dan pastikan path lokal benar. |
| 75–84 | Uji muat ulang dan minta teman membaca deskripsi alternatif dari kode. |
| 84–90 | Exit ticket: apa beda fungsi `alt` dan `figcaption`? |

**Cek selesai:** dua media termuat, tidak terdistorsi, punya alt dan caption yang sesuai.

### Hari 10 — Media (HTML × CSS): Galeri Foto/Video

**Yang dipelajari:** galeri media, caption, ukuran seragam, object-fit; pengenalan `<video controls>` bila aset lokal tersedia.  
**Proyek:** galeri bertema (hewan, alam, olahraga atau karya seni) dengan tiga item.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan galeri dengan ukuran gambar berbeda; diskusikan konsistensi tanpa memotong informasi penting. |
| 10–25 | Demonstrasikan pengulangan `figure`, `img`, `figcaption`, serta `object-fit: cover` dan kapan crop kurang sesuai. |
| 25–45 | Siswa membuat tiga item media dengan teks keterangan dan alt. |
| 45–65 | Tata galeri dengan Flexbox atau Grid sederhana, gap dan ukuran gambar konsisten. |
| 65–75 | Opsional bila guru menyediakan video lokal: tambahkan `<video controls>` dan `<source>`; jika tidak, teruskan memperbaiki galeri gambar. |
| 75–84 | Uji path, caption, alt, ukuran, dan perilaku saat jendela dipersempit. |
| 84–90 | Exit ticket: kapan `object-fit: cover` dapat menghilangkan bagian penting dari gambar? |

**Cek selesai:** galeri punya tiga media dengan teks yang sesuai dan susunan CSS konsisten. Video hanya bonus HTML, tanpa script.

### Hari 11 — Layout (HTML × CSS): Halaman Profil Klub

**Yang dipelajari:** landmark semantik dan susunan halaman; box model pada section.  
**Tag:** `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `div`, `span`.  
**Proyek:** profil klub dengan navigasi, deskripsi, artikel kegiatan, info samping dan footer.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan sketsa halaman dan minta siswa memberi nama bagian. |
| 10–25 | Jelaskan peran elemen semantik; bandingkan `section/article` dengan `div` dan `span`. |
| 25–45 | Siswa membuat struktur semantik proyek baru tanpa fokus dekorasi. |
| 45–65 | Tambahkan CSS dasar untuk lebar, margin/padding, batas bagian dan warna. |
| 65–75 | Tambahkan nav dengan anchor ke bagian yang memiliki id. |
| 75–84 | Audit: satu main, heading terstruktur, nav bekerja, footer terpisah. |
| 84–90 | Exit ticket: kapan `article` lebih sesuai daripada `div`? |

**Cek selesai:** konten punya struktur semantik yang masuk akal dan bagian halaman terpisah rapi.

### Hari 12 — Layout (HTML × CSS): Katalog dengan Grid/Flex

**Yang dipelajari:** layout multi-kolom dengan CSS Grid atau Flexbox, container/item, `gap`, alignment dan wrapping.  
**Proyek:** katalog empat kartu produk atau hobi.

| Menit | Arahan guru |
|---|---|
| 0–10 | Bandingkan daftar satu kolom dan katalog kartu di layar lebar. |
| 10–25 | Demonstrasikan satu metode utama (Grid atau Flexbox) dan jelaskan container, item dan gap. Jangan mengajarkan dua layout sekaligus jika kelas masih pemula. |
| 25–45 | Siswa membuat empat `article` dengan judul dan deskripsi. |
| 45–65 | Atur kolom, jarak, alignment, lebar konten dan tampilan kartu. |
| 65–75 | Uji lebar jendela; rapikan saat kartu mulai terlalu sempit. |
| 75–84 | Pasangan memeriksa struktur dan konsistensi kartu. |
| 84–90 | Exit ticket: properti apa yang menjadikan container sebuah grid/flex? |

**Cek selesai:** empat item tertata dengan gap konsisten; tata letak dibuat dengan CSS, bukan tabel HTML.

### Hari 13 — HTML - Responsive: Kartu Acara untuk Ponsel

**Yang dipelajari:** meta viewport, ukuran fleksibel, gambar tidak meluber dan satu media query.  
**Proyek:** kartu acara yang terbaca pada ponsel dan desktop.  
**CSS:** `%`, `max-width`, `width: 100%`, media query.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan halaman desktop di viewport kecil; minta siswa mencatat masalah. |
| 10–25 | Periksa meta viewport; demonstrasikan container/gambar fleksibel dan satu breakpoint. |
| 25–45 | Siswa membuat halaman acara baru dengan judul, detail, gambar dan anchor informasi. |
| 45–65 | Terapkan lebar maksimum di layar lebar dan padding lebih kecil di layar sempit. |
| 65–75 | Pastikan tidak ada elemen tetap yang memaksa overflow. |
| 75–84 | Uji viewport ponsel dan perbaiki satu masalah nyata. |
| 84–90 | Exit ticket: apa yang berubah hanya pada layar sempit melalui media query? |

**Cek selesai:** halaman terbaca di ponsel tanpa scroll horizontal; media tetap di dalam container.

### Hari 14 — HTML - Responsive: Katalog Multi-Layar

**Yang dipelajari:** menguji dan memperbaiki layout ponsel, tablet dan desktop; breakpoint mengikuti kebutuhan konten.  
**Proyek:** katalog baru empat item dengan susunan yang berubah sesuai ruang.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tampilkan checklist dan ukuran uji contoh: ponsel 375 px, tablet 768 px, desktop 1280 px. |
| 10–25 | Demonstrasikan cari masalah → ubah satu rule → uji ulang; tunjukkan perubahan jumlah kolom. |
| 25–45 | Siswa buat katalog baru empat item memakai HTML semantik dan CSS Grid/Flex. |
| 45–65 | Susun tampilan desktop dan media query untuk layar sempit; pilih breakpoint saat konten memerlukannya. |
| 65–75 | Uji tiga lebar dan catat masalah aktual. |
| 75–84 | Perbaiki minimal dua masalah dan minta pasangan menjalankan checklist. |
| 84–90 | Exit ticket: tulis satu masalah, rule CSS yang diubah, dan hasil uji sesudahnya. |

**Cek selesai:** tiga ukuran diuji, minimal dua masalah yang nyata diperbaiki, tidak ada overflow.

### Hari 15 — Free Project: Rancang dan Bangun Situs Multi-Halaman

**Yang dipelajari:** merancang situs beberapa halaman, memakai navigasi antarfile HTML relatif, dan membagi isi ke halaman yang berbeda.  
**Proyek akhir:** situs pilihan siswa untuk dipresentasikan kepada keluarga. Pilih satu topik yang dapat memiliki beberapa bagian, misalnya klub, hobi, hewan, tempat wisata, resep, atau acara. Hari 15–16 adalah satu proyek yang sama.  
**Target hari ini:** rencana situs dan sekurang-kurangnya tiga file HTML dengan kerangka/konten awal: `index.html`, `tentang.html`, `galeri.html`. Ketiganya berada dalam satu folder proyek.

| Menit | Arahan guru |
|---|---|
| 0–10 | Tunjukkan contoh [Proyek Akhir Klub Jelajah](./proyek-harian/proyek-akhir/index.html); klik Beranda, Kegiatan, dan Galeri agar siswa melihat bahwa setiap menu membuka halaman berbeda. |
| 10–20 | Siswa memilih topik dan membuat peta situs: nama tiap halaman, isi yang ditempatkan di sana, dan nav yang sama pada semua halaman. |
| 20–30 | Demonstrasikan folder dengan `index.html`, `tentang.html`, `galeri.html`, `style.css`, serta `assets`. Jelaskan browser membuka `index.html` sebagai halaman awal. |
| 30–40 | Buat nav lintas halaman dengan `<a href="tentang.html">Tentang</a>`. Tunjukkan bahwa path relatif dihitung dari file HTML saat ini; file di subfolder memerlukan path seperti `pages/tentang.html`, sedangkan menuju folder induk memakai `../index.html`. |
| 40–60 | Siswa membuat kerangka ketiga file, masing-masing dengan `title` dan `h1` yang berbeda, lalu menyalin nav dengan tautan yang benar ke semua halaman. |
| 60–74 | Isi `index.html` (pengenalan), `tentang.html` (cerita/detail), dan `galeri.html` (minimal tiga item gambar/karya dengan teks alternatif). Buat satu stylesheet bersama dan hubungkan dari ketiga file. |
| 74–84 | Uji setiap item menu dari setiap halaman. Cek ejaan nama file, title, dan apakah semua halaman bisa kembali ke Beranda. |
| 84–90 | Checkpoint guru: setidaknya tiga HTML bisa dibuka dan saling terhubung. Exit ticket: siswa jelaskan kenapa `href="tentang.html"` dapat menemukan file itu. |

**Cek selesai hari 15:** ada peta situs; tiga dokumen HTML berbeda; nav dengan tautan antarhalaman pada setiap dokumen; tiap halaman punya title/h1 sendiri; shared stylesheet sudah terhubung; galeri berisi minimal tiga item.  
**Bantuan:** mulai dengan hanya dua halaman (`index.html` dan `tentang.html`), pastikan tautannya benar, lalu duplikasi pola untuk `galeri.html`.  
**Tantangan:** tempatkan halaman di subfolder `pages` lalu sesuaikan path relatif, atau tambahkan `jadwal.html` sebagai halaman keempat.

### Hari 16 — Free Project: Poles, Uji, dan Presentasikan Situs

**Yang dipelajari:** menyelesaikan desain konsisten di beberapa halaman, responsif, uji navigasi, dan menjelaskan keputusan HTML/CSS.  
**Proyek:** lanjutkan situs multi-halaman yang sama dari Hari 15—bukan kembali membuat satu halaman tunggal.  
**Batas minimum:** tiga halaman HTML yang saling terhubung, stylesheet yang konsisten, isi berbeda dan bermakna di tiap halaman, gambar/alt pada galeri, layout ponsel, dan presentasi tur situs.

| Menit | Arahan guru |
|---|---|
| 0–10 | Siswa membuka folder proyek dan checklist checkpoint Hari 15; pilih tiga prioritas penyelesaian. |
| 10–20 | Demonstrasikan satu stylesheet yang dipakai bersama dengan `<link rel="stylesheet" href="style.css">`; jelaskan lokasi CSS relatif terhadap setiap file HTML. |
| 20–45 | Siswa memperbaiki visual seluruh halaman: warna, font, spacing, kartu/media, state hover/focus, dan konsistensi header/nav/footer. |
| 45–60 | Buat layout responsif dengan media query; uji satu halaman ponsel, lalu pastikan stylesheet bersama memperbaiki halaman lainnya juga. |
| 60–70 | Uji semua link dari setiap halaman, termasuk tautan kembali Beranda, galeri, tautan fragmen dan gambar. Periksa title unik dan alt media. |
| 70–78 | Latihan presentasi sebagai tur: Beranda → Tentang → Galeri; siswa menjelaskan tujuan tiap halaman dan menunjukkan perpindahan lewat menu. |
| 78–86 | Presentasi kepada kelas/keluarga, 2–3 menit per siswa atau kelompok. Bila kelas besar, presentasi bergiliran di kelompok kecil. |
| 86–90 | Refleksi dan simpan/backup seluruh folder situs, bukan hanya satu file HTML. |

**Cek selesai final:** situs berisi minimal tiga halaman berbeda; nav berfungsi dua arah dan konsisten; CSS bersama termuat; konten/media dapat dibaca di desktop dan ponsel; siswa bisa mendemonstrasikan tur halaman tanpa bantuan guru.

**Checklist orang tua/audiens:** apakah mudah kembali ke Beranda? Apakah jelas menu apa yang membuka halaman lain? Apakah tiap halaman memiliki isi sendiri? Apakah teks dan gambar nyaman dilihat di ponsel?

## Rubrik ringkas

Beri skor 0–2 untuk setiap kriteria: **0** belum ada/tidak bekerja, **1** sebagian atau perlu bantuan, **2** lengkap dan siswa dapat menjelaskan.

1. Tag dan konsep HTML sesuai target hari.
2. Struktur konten/nesting mudah dipahami.
3. CSS diterapkan konsisten dan teks/media tetap terbaca.
4. Proyek dibuka, diuji, dan satu keputusan/perbaikan dapat dijelaskan siswa.
5. Untuk capstone Hari 15–16: tiga atau lebih halaman punya konten berbeda dan tautan antarhalaman yang berfungsi.

Nilai hasil belajar, bukan jumlah kode atau seberapa cepat siswa mengetik.
