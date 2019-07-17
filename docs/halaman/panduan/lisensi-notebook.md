---
layout: default
title: Lisensi Notebook
parent: Panduan
# nav_order: 1
permalink: /panduan/lisensi-notebook
---

<div align="justify" markdown="1">
**Halaman ini hanya menyertakan informasi terkait lisensi. Untuk legalitas, harap hubungi pengacara atau lembaga hukum yang terkait.**
{: .label .label-yellow .fs-1}
</div>

# Daftar isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## Informasi Lisensi

Seluruh notebook diharapkan menyertakan informasi lisensi. Hal ini diperlukan untuk memastikan aturan penggunaan kode/data yang disediakan oleh notebook. 

Perlu diingat, dengan mengunggahnya notebook ke repo hidrokit-nb berarti perlu disadari bahwa _source code_ notebook Anda tersedia **publik** dan bisa tersalin melalui [_forking_]. Akan tetapi, pemilik tetap memiliki hak milik akan notebooknya dan lisensi produknya. **Jika tidak memiliki informasi lisensi, maka notebook tersebut termasuk dalam kategori [No License](https://choosealicense.com/no-permission/)**. Pada umumnya, ini berarti **orang lain tidak memiliki ijin untuk menggunakan, menyalin, mendistribusikan, mengubah notebook**. Dan hal tersebut bertentangan dengan tujuan utama mengunggah notebook ke dalam repo hidrokit-nb. Sehingga sangat disarankan untuk **selalu** menyertakan informasi lisensi pada notebook. 

---
## Memilih lisensi

Untuk menentukan lisensi notebook, bisa kunjungi [Choose a License](https://choosealicense.com/) untuk memahami lisensi apa yang tepat. Perlu dicatat bahwa notebook bisa terdiri dari **kode dan data**. Lisensi kode dan data terpisah satu sama lain. 

Kami menyarankan untuk menggunakan lisensi ini dalam notebook:
- Untuk kode disarankan [berlisensi MIT](https://choosealicense.com/licenses/mit/).
- Untuk data disarankan [berlisensi CC-BY-4.0](https://choosealicense.com/licenses/cc-by-4.0/).

Kedua lisensi tersebut memastikan bahwa produk (kode/data) dapat dikembangkan lebih lanjut tanpa mengabaikan kontribusi pemilik produk.

---
## Menulis lisensi pada notebook

Setelah menentukan lisensi, pemilik bisa menambahkan informasi lisensi dalam satu baris _markdown_ dalam notebook (diawal/diakhir).

<div class="code-example" markdown="1">
Source code in this notebook is licensed under a [MIT License](https://choosealicense.com/licenses/mit/). Data in this notebook is licensed under a [Creative Common Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). 
</div>
```markdown
Source code in this notebook is licensed under a [MIT License](https://choosealicense.com/licenses/mit/). Data in this notebook is licensed under a [Creative Common Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). 
```

<!-- LINK -->
[_forking_]: https://help.github.com/en/articles/fork-a-repo
