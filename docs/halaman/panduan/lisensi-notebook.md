---
layout: default
title: Lisensi Notebook
parent: Panduan
# nav_order: 1
permalink: /panduan/lisensi-notebook
---

<div class="code-example" markdown="1">
**Halaman ini hanya menyertakan informasi terkait lisensi. Untuk legalitas, harap hubungi pengacara atau lembaga hukum yang terkait.**
</div>

# Daftar isi
{: .no_toc .text-delta }

1. TOC
{:toc}

## Informasi Lisensi

Seluruh notebook diharapkan menyertakan informasi lisensi. Hal ini diperlukan untuk memastikan aturan penggunaan kode/data yang diberikan oleh notebook. Lisensi sangat penting untuk keberlangsungan proyek _open-source_. 

Perlu diingat, dengan mengunggahnya notebook ke repo ini berarti perlu diadari bahwa _source code_ notebook tersedia **publik**. Akan tetapi, pemilik tetap memiliki hak milik akan notebooknya dan lisensi produknya. **Jika tidak memiliki informasi lisensi, maka notebook tersebut termasuk dalam kategori [No License](https://choosealicense.com/no-permission/)**. Pada umumnya, ini berarti **orang lain tidak memiliki ijin untuk menggunakan, menyalin, mendistribusikan, mengubah notebook**. Dan hal tersebut bertentangan dengan tujuan utama mengunggah notebook ke dalam repo ini. Sehingga sangat disarankan untuk menyertakan informasi lisensi pada notebook. Perlu diingat bahwa _open source_ bukan selalu berarti gratis ataupun bebas. 

Bacaan lebih lanjut:
- [The Legal Side of Open Source](https://opensource.guide/legal/)

## Apa lisensi yang harus digunakan?

Untuk menentukan lisensi notebook, bisa mengunjungi [Choose a License](https://choosealicense.com/) untuk memahami lisensi apa yang tepat. Perlu dicatat bahwa notebook bisa terdiri dari **kode dan data**. Lisensi kode dan data terpisah satu sama lain. 

Kami menyarankan untuk menggunakan lisensi ini dalam notebook:
- Untuk kode disarankan [berlisensi MIT](https://choosealicense.com/licenses/mit/).
- Untuk data disarankan [berlisensi CC-BY-4.0](https://choosealicense.com/licenses/cc-by-4.0/).

Kedua lisensi tersebut memastikan bahwa produk (kode/data) dapat dikembangkan lebih lanjut tanpa mengabaikan kontribusi pemilik produk.

## Menulis lisensi pada notebook

Setelah menentukan lisensi, pemilik bisa menambahkan informasi lisensi dalam satu baris _markdown_ dalam notebook (diawal/diakhir).

<div class="code-example" markdown="1">
Source code in this notebook is licensed under a [MIT License](https://opensource.org/licenses/MIT). Data in this notebook is licensed under a [Creative Common Attribution 4.0 International](https://choosealicense.com/licenses/cc-by-4.0/). 
</div>
```markdown
Source code in this notebook is licensed under a [MIT License](https://opensource.org/licenses/MIT). Data in this notebook is licensed under a [Creative Common Attribution 4.0 International](https://choosealicense.com/licenses/cc-by-4.0/). 
```