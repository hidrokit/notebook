---
layout: default
title: Menambah notebook
parent: Panduan
permalink: /panduan/tambah-notebook
---

<div align="justify" markdown="1">
**Halaman ini kadaluarsa _outdated_. Penambahan daftar notebook lebih mudah dengan hanya mengubah _file YAML_ pada direktori _data. **
{: .label .label-red .fs-1}
</div>

Halaman ini berisikan panduan menambahkan notebook anda di halaman [kumpulan notebook]({{ site.baseurl }}{% link halaman/kumpulan-notebook.md %}).

# Daftar Isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## Persiapan

- Diasumsikan bahwa Anda sudah pernah melakukan _pull request_ sebelumnya. Jika belum, baca [cara mengunggah notebook]({{ site.baseurl }}{% link halaman/panduan/mengunggah-notebook.md %}).
- Repo Anda sudah diperbarui dengan repo hidrokit-nb, jika belum baca [memperbarui dengan pull request]({{ site.baseurl }}{% link halaman/panduan/pull-request.md %}).
- Pastikan bahwa notebook Anda sudah tersimpan dalam repo hidrokit-nb. Cek notebook Anda dengan melihat [kumpulan notebook melalui NBViewer](https://nbviewer.jupyter.org/github/taruma/hidrokit-nb/tree/master/notebook/).
- Menentukan kategori untuk notebook (umum/hidrokit/demo).

---
## Menambahkan Notebook

### Buka dokumen `kumpulan-notebook.md`

- Pastikan Anda berada di repo Anda (yang selalu ditandai dengan `forked from taruma/hidrokit-nb`). Cari _file_ dengan memilih pilihan **Find File**.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_00.png" alt="find file button"><br>
</div>

- Cari _file_ bernama `kumpulan-notebook.md`. Kemudian buka `docs/halaman/kumpulan-notebook.md`.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_01.png" alt="search file"><br>
</div>

- Klik gambar pensil untuk melakukan perubahan.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_02.png" alt="pencil button"><br>
</div>
Catatan: tampilan di github tidak begitu bagus meski dokumen _markdown_, ini dikarenakan banyaknya penggunaan Block Inline Attribute List (IAL)

- Cari bagian kategori yang ingin ditambahkan. Tips: lihat baris yang dikomentari `<!-- ---------NOTEBOOK KATEGORI UMUM --------- -->`. 

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_03.png" alt="find your category"><br>
</div>

### Format penulisan

- Tambahkan notebook Anda dengan menggunakan format sebagai berikut:

```
1. `YYYY-MM-DD` [`NBViewer`](link-notebook-anda) Judul Notebook oleh Pemilik/Penulis.
```
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_06.png" alt="write your line"><br>
</div>

Tips: Anda tidak perlu menyesuaikan penomoran daftar (2./3./4.), cukup tulis `1. ...`, situs akan mengatur sendiri dan mengisi penomoran yang tepat.

### Salin _link_/tautan/pranala notebook Anda

- Tautan yang diminta adalah tautan yang berasal dari *NBViewer*.
- Buka [halaman kumpulan notebook melalui NBViewer](https://nbviewer.jupyter.org/github/taruma/hidrokit-nb/tree/master/notebook/), buka notebook anda dengan mengkliknya.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_04.png" alt="browse nbviewer"><br>
</div>

- Salin tautan dari kotak alamat _browser_ Anda.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_05.png" alt="notebook link"><br>
</div>

- Kembali ke halaman github, ganti `link-notebook-anda` dengan tautan yang sudah disalin sebelumnya.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_07.png" alt="change with your link"><br>
</div>

- Jika telah selesai mengubah dokumen `kumpulan-notebook.md`, lanjutkan dengan memilih **Commit changes**. Sertakan juga info commit jika diperlukan.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_08.png" alt="commit"><br>
</div>

### Melakukan _pull request_

- Buka halaman _repo_ Anda, dan lakukan _pull request_. Langkah melakukan pull request sama dengan langkah pada dihalaman [mengunggah notebook]({{ site.baseurl }}{% link halaman/panduan/mengunggah-notebook.md %}).

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_09.png" alt="pull request"><br>
</div>

<div align="center" markdown="1">
🎉🎊 Selamat! Anda telah membuat _Pull Request_!! 🎊🎉
{: .fs-5 .fw-700}

Kami menanti kontribusi Anda berikutnya. 👍👍 
{: .fs-5 .fw-300}
</div>

