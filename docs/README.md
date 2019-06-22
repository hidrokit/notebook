# README SITUS

Situs hidrokit-nb dibuat menggunakan Jekyll & GitHub Pages dengan menggunakan `remote-theme` dari Just the Docs oleh Patrick Marsceill. Disarankan untuk **membaca** manual penggunaan tema di [Just the Docs](https://pmarsceill.github.io/just-the-docs/) agar mengetahui fitur yang tersedia.

Dianjurkan untuk melakukan instalasi pada mesin lokal sebelum melakukan pull request agar memudahkan saat melakukan pengembangan/perbaikan. Baca bagian [instalasi lokal](#Instalasi-lokal) untuk lebih lanjut.

Untuk memulai kontribusi dalam situs, berikut yang harus dipersiapkan/diketahui:
- Terbiasa dengan penulisan Markdown, HTML, dan CSS.
- Pengetahuan tentang HTML dan CSS.
- Sudah memasang/instalasi Ruby, Jekyll, dan Bundler.
- Mengetahui menggunakan Jekyll (*front matter* dan *_config.yml*)
- Diasumsikan sudah memahami menggunakan Git dan Github.

## Struktur Direktori

```
hidrokit-nb/docs
|   Gemfile
|   index.md
|   README.md
|   _config.yml
|   _config_local.yml
|   
+---assets
|   +---images
|   |   +---favicon
|   |   \---panduan
|   \---js
|           
\---halaman
    |   kumpulan-notebook.md
    |   
    \---panduan
            lisensi-notebook.md
            mengunggah-notebook.md
            panduan.md
```

Keterangan:
- `Gemfile`: file Gem yang digunakan untuk instalasi Jekyll.
- `index.md`: halaman depan situs.
- `_config.yml`: konfigurasi yang digunakan saat _deployment_ di GitHub.
- `_config_local.yml`: konfigurasi yang digunakan untuk mesin lokal.
- `assets/`: _Media Directory_ | Direktori khusus penyimpanan media.
  - `images/`: berisikan media gambar yang digunakan untuk situs.
  - `js/`: berisikan file yang digunakan untuk fitur pencarian di situs.
- `halaman/`: _Page Directory_ | Direktori khusus untuk seluruh halaman dalam situs.
  - `panduan/`: Berisikan halaman panduan/bantuan/tutorial/tips.

Direktori/files bisa ditambahkan jika diperlukan.

## Instalasi lokal

Langkah ini tidak jauh berbeda dengan yang ada di halaman [Just the Docs](https://pmarsceill.github.io/just-the-docs/). Diasumsikan bahwa Ruby beserta Jekyll dan Bundler sudah terinstalasi, baca [Quickstart](https://jekyllrb.com/docs/) untuk informasi lebih lanjut.

1. Buka *command prompt/terminal*, pastikan sudah berada di direktori `hidrokit-nb/docs/`. Masukan perintah berikut untuk melakukan instalasi:
```bash
$ bundle install
```

2. Jalankan server lokal dengan menggunakan konfigurasi lokal.

```bash
$ bundle exec jekyll serve --config _config_local.yml
```

3. Buka browser dan masukkan halaman [http://localhost:4000](http://localhost:4000)

4. *(Opsional)* Memperbarui file index untuk fitur pencarian.

```bash
$ bundle exec just-the-docs rake search:init
```
