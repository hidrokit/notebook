---
layout: default
title: Kumpulan Notebook
nav_order: 2
permalink: /kumpulan-notebook
last_modified_date: 2022-03-26
---
<div align="center" markdown="1">
# Kumpulan Notebook
{: .no_toc}
</div>

<div align="justify" markdown="1">
> "Jupyter notebook merupakan halaman web yang mampu membuat dan membagikan dokumen yang memiliki _live code_, persamaan, visualisasi, atau teks narasi. Penggunaannya berupa _data cleaning and transformation_, simulasi numerik, pemodelan statistik, visualisasi data, _machine learning_, dll." - Project Jupyter, [jupyter.org](https://jupyter.org)
{: .fs-5}
</div>

<div align="justify" markdown="1">
Notebook di hidrokit-nb dibagi menjadi dua bagian yaitu bagian hidrokit yang terdiri dari laporan implementasi, manual subpaket hidrokit.contrib, dan manual paket hidrokit. Yang kedua adalah bagian umum yang berisikan notebook untuk penggunaan python dan arsip.

Kami mengajak Anda untuk membuat isu atau melakukan _pull request_ sendiri untuk mendaftarkan notebook Anda di halaman ini.
</div>

---

## Daftar isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## Legenda
{: .no_toc .text-delta}

- <i class="fas fa-calendar-day"></i> _Tanggal_{: .text-delta}
- <i class="fas fa-code-branch"></i> _Versi_{: .text-delta}
- <i class="fas fa-book-open"></i> _Buka melalui NBViewer_{: .text-delta}
- <i class="fab fa-github"></i> _Lihat di GitHub_{: .text-delta}
- _@author (username github)_{: .text-delta}
- <i class="fas fa-download"></i> _Download (jika tersedia di repo)_{: .text-delta}

{% assign col_imp = site.data.hidrokit | where: "category", "implementasi" | sort: "date" | reverse %}
{% assign col_contrib = site.data.hidrokit | where: "category", "contrib" | sort: "title" %}
{% assign col_main = site.data.hidrokit | where: "category", "main" | sort: "title" %}
{% assign col_archive = site.data.general | where: "category", "arsip" | sort: "title" %}
{% assign col_general = site.data.general | where: "category", "general" | sort: "date" | reverse %}

---

<div align="center" markdown="1">
## Laporan Implementasi
{: .label .label-blue .fs-6 .mt-0}
Laporan Implementasi (LI) merupakan buku (jupyter notebook) yang memeragakan penggunaan python dan/atau machine learning pada topik sumberdaya air. Buku ini juga sebagai demonstrasi penggunaan paket hidrokit, yaitu proyek open-source paket python untuk analisis hidrologi.
</div>

{% include daftar_notebook.md source=col_imp %}

---

<div align="center" markdown="1">
## Manual Subpaket hidrokit.contrib
{: .label .label-green .fs-6 .mt-0}
Kumpulan _notebook_ manual untuk penggunaan fungsi pada subpaket `hidrokit.contrib`.
</div>

{% include daftar_notebook.md source=col_contrib %}

---

<div align="center" markdown="1">
## Manual hidrokit
{: .label .label-green .fs-6 .mt-0}
Kumpulan _notebook_ manual untuk penggunaan fungsi dan modul yang tersedia di `hidrokit` (main). 

Pengembangan pada fungsi utama pada hidrokit dialihkan ke pengembangan pada subpaket .contrib sejak versi 0.3.x
{: .text-delta .fs-2}
</div>

{% include daftar_notebook.md source=col_main %}

---

<div align="center" markdown="1">
## Umum
{: .label .label-yellow .fs-6 .mt-0}
Kumpulan _notebook_ umum yang memeragakan penggunaan python. 
</div>

{% include daftar_notebook.md source=col_general %}

---

<div align="center" markdown="1">
## Arsip
{: .label .label-red .text-delta .fs-6 .mt-0}
Arsip notebook yang sudah kadaluarsa (outdated). 

</div>

{% include daftar_notebook.md source=col_archive %}

<!-- Link -->
[taruma]: https://github.com/taruma
