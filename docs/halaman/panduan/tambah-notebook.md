---
layout: default
title: Menambah notebook
parent: Panduan
permalink: /panduan/tambah-notebook
last_modified_date: 2019-07-13
---

Halaman ini berisikan panduan menambahkan notebook anda di halaman [kumpulan notebook]({{ site.baseurl }}{% link halaman/kumpulan-notebook.md %}).

# Daftar Isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## Persiapan

- Diasumsikan bahwa Anda sudah pernah melakukan _pull request_ sebelumnya. Jika belum, baca [cara mengunggah notebook]({{ site.baseurl }}{% link halaman/panduan/mengunggah-notebook.md %}).
- Repo Anda sudah diperbarui dengan repo hidrokit-nb, jika belum, baca [memperbarui dengan pull request]({{ site.baseurl }}{% link halaman/panduan/pull-request.md %}).
- Pastikan bahwa notebook Anda sudah tersimpan dalam repo hidrokit-nb. Cek notebook Anda dengan melihat [kumpulan notebook melalui NBViewer](https://nbviewer.jupyter.org/github/taruma/hidrokit-nb/tree/master/notebook/).
- Menentukan kategori untuk notebook Anda (umum/hidrokit/demo).

---
## Menambahkan Notebook

Tentukan kategori yang sesuai dengan notebook Anda. Gunakan kategori umum jika tidak sesuai dengan kategori demo/hidrokit. Ada tiga _YAML file_ untuk masing-masing kategori. Notebook bisa lebih dari satu kategori, hanya perlu melakukan langkah pengubahan _YAML file_ sebanyak tiga kali. 

### Buka dokumen YAML kategori

- Pastikan Anda berada di repo Anda (yang selalu ditandai dengan `forked from taruma/hidrokit-nb`) dan sudah paling terbaru. Cari _file_ dengan memilih pilihan **Find File**.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_00.png" alt="find file button"><br>
</div>

- Cari _file YAML_ sesuai kategori. Untuk kategori umum, bernama `umum.yml`; Untuk kategori hidrokit, bernama `hidrokit.yml`; Untuk kategori demo, bernama `demo.yml`. Buka file dengan menekan `enter` atau memilih `docs/_data/{kategori}.yml`.<br>Catatan: Anda bisa membuka berkas tersebut pada direktori `docs/_data/`.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_baru_00.png" alt="find yaml file"><br>
</div>

- Klik gambar pensil untuk melakukan perubahan.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_baru_01.png" alt="edit yaml file"><br>
</div>

- Tambah informasi notebook Anda **di barisan paling bawah**.

### Format penulisan

- Tambahkan informasi notebook Anda dengan menggunakan format sebagai berikut:
{% raw %}
```
- title       : >-
    {{ judul singkat notebook }}
  notebook    : {{ nama berkas notebook tanpa .ipynb }}
  date        : {{ isi tanggal dengan format YYYY-MM-DD }}
  author      : {{ pengunggah }}
  version     : {{ versi notebook }}
```
{% endraw %}

- Catatan: 
  - untuk `author` isikan nama _username_ github. 
  - untuk `version`, jika notebook tidak memiliki versi, isikan dengan nilai `1.0.0`.
  - pastikan isian `notebook` sesuai dengan penamaan berkasnya.

- Contoh pengisian informasi notebook: <br> Saya ingin menambahkan notebook saya yang berjudul "Tutorial satu" dengan nama berkas "taruma_tutorial_satu.ipynb" yang telah masuk pada tanggal 13 Juli 2019.

```
- title       : >-
    Tutorial satu
  notebook    : taruma_tutorial_satu
  date        : 2019-07-13
  author      : taruma
  version     : 1.0.0
```

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_baru_02.png" alt="add new notebook info"><br>
</div>

- Jika telah selesai mengubah dokumen, lanjutkan dengan memilih **Commit changes**. Sertakan juga info commit jika diperlukan.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/tambah_baru_03.png" alt="commit changes"><br>
</div>

- Jika notebook Anda ingin disertakan pada kategori lain, ulangi langkah diatas dengan berkas YAML yang berbeda. Jika sudah selesai, lanjutkan dengan melakukan _pull request_. 

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

