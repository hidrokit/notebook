---
layout: default
title: Kumpulan Notebook
nav_order: 2
permalink: /kumpulan-notebook
---
<div align="center" markdown="1">
# Kumpulan Notebook
{: .no_toc}
</div>

<div align="justify" markdown="1">
> "Jupyter notebook merupakan halaman web yang mampu membuat dan membagikan dokumen yang memiliki _live code_, persamaan, visualisasi, atau teks narasi. Penggunaannya berupa _data cleaning and transformation_, simulasi numerik, pemodelan statistik, visualisasi data, _machine learning_, dll." - Project Jupyter, [jupyter.org](https://jupyter.org)
{: .fs-5}
</div>

<div align="center" markdown="1">
[Lihat Kumpulan Notebook via NBViewer](https://nbviewer.jupyter.org/github/taruma/hidrokit-nb/tree/master/notebook/){: .btn .btn-blue .fs-4 .mb-4 .mb-md-0 .mr-2 }
</div>

<div align="justify" markdown="1">
Notebook di hidrokit-nb dibagi menjadi tiga kategori yaitu umum, hidrokit, dan demo. Pembagian kategori ini hanya berlaku untuk pengkategorian melalui halaman ini (jika melihat langsung dari _repo_ atau _NBViewer_ seluruh notebook disimpan dalam satu _folder_). Halaman ini diperbarui manual sehingga notebook yang telah diterima _pull request_-nya bisa saja tidak tampil di halaman ini. 

Kami mengajak Anda untuk membuat isu untuk mendaftarkan notebook Anda atau melakukan _pull request_ sendiri untuk mendaftarkan notebook Anda di halaman ini.
</div>


---

## Daftar isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
<div align="center" markdown="1">
## Umum <!-- ---------NOTEBOOK KATEGORI UMUM --------- -->
{: .label .label-blue .fs-6 .mt-0}
Kumpulan _notebook_ yang mendemonstrasikan kegunaan python dalam bidang hidrologi (data)
</div>

{% include daftar_notebook.md source=site.data.umum %}

---
<div align="center" markdown="1">
## Hidrokit <!-- ---------NOTEBOOK KATEGORI HIDROKIT --------- -->
{: .label .label-green .fs-6 .mt-0}
Kumpulan _notebook_ yang berkaitan dengan kegunaan `hidrokit`
</div>

{% include daftar_notebook.md source=site.data.hidrokit %}

---
<div align="center" markdown="1">
## Demo <!-- ---------NOTEBOOK KATEGORI DEMO --------- -->
{: .label .label-yellow .fs-6 .mt-0}
Kumpulan _notebook_ yang menerapkan python/hidrokit dalam kasus nyata/lapangan.
</div>

{% include daftar_notebook.md source=site.data.demo %}

---
<div align="center" markdown="1">
## Arsip
{: .label .label-red .fs-6 .mt-0}
Kumpulan _notebook_ yang sudah tidak digunakan/tidak layak pakai
</div>

{% include daftar_arsip.md %}

<!-- Link -->
[taruma]: https://github.com/taruma