---
layout: default
title: Mengunggah Notebook
parent: Panduan
# nav_order: 1
permalink: /panduan/mengunggah-notebook
---

Halaman ini merupakan panduan dalam mengunggah notebook ke repo hidrokit-nb. Tidak diperlukan pengetahuan Git/Github untuk mengunggah notebook melalui GitHub.

# Daftar Isi
{: .no_toc .text-delta }

1. TOC
{:toc}

---
## Persiapan

1. Notebook yang dimaksud adalah _file_ berekstensi `.ipynb`.
1. Menamai _file_ dengan format `pemilik-judul.ipynb` atau `pemilik-judul-v0.ipynb` jika memiliki nomor versi (isi spasi dengan `-`). Gunakan nama _username_ GitHub untuk konsistensi.
1. Pastikan notebook sudah tertera lisensinya (baca: [Lisensi Notebook]({{ site.baseurl }}{% link halaman/panduan/lisensi-notebook.md %})).
1. Memiliki akun GitHub (jika belum, [daftar disini](https://github.com/join)).
1. Dilakukan melalui komputer (_desktop_).

---
## Unggah Notebook ke hidrokit-nb

Jika ini bukan pengalaman pertama dalam mengunggah notebook / _pull request_ di _repo_ hidrokit-nb, baca [Pull Request]({{ site.baseurl}}{% link halaman/panduan/pull-request.md %}).

### *Fork hidrokit-nb*
- Masuk akun [GitHub](https://github.com/login).
- Buka tautan [https://github.com/taruma/hidrokit-nb/](https://github.com/taruma/hidrokit-nb/).
- Klik ___Fork___ pada tepi kanan atas.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_00.png" alt="Fork Button"><br>
</div>

- Akan muncul proses _forking_.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_01.png" alt="Forking"><br>
</div>

- Tunggu proses _fork_ selesai.

### _Upload Files_
- Setelah proses _fork_ selesai. Klik `notebook` pada daftar _folder_.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_02.png" alt="clicking notebook directory"><br>
</div>

- Klik __Upload files__. Pastikan bahwa Anda berada di direktori `hidrokit-nb/notebook/`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_03.png" alt="click upload files"><br>
</div>

- Akan terbuka halaman untuk mengunggah _file_. Anda bisa mengupload dengan cara ___drag files___ atau mengklik pilihan __choose your files__. Pastikan berada di direktori `hidrokit-nb/notebook`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_04.png" alt="drag or upload files"><br>
</div>

- Pastikan bahwa notebook anda terunggah.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_05.png" alt="make sure file is uploaded"><br>
</div>

- Isi deskripsi _commit_ seperti pada gambar. Pastikan pilihan sudah seperti di gambar. Klik **Commit Changes**. 
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_06.png" alt="add commit message"><br>
</div>

- Hasil unggah dapat dilihat dengan membuka direktori `notebook`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_07.png" alt="double check file is uploaded"><br>
</div>

### _Pull Request_

Jika notebook yang ingin diunggah sudah tersimpan pada _repo_ Anda. Saatnya menggabungkan hasil unggahan/perubahan yang Anda lakukan dengan _repo_ hidrokit-nb. 

- Dari halaman _forked repository_ yang telah Anda buat klik **New pull request**. Alamat _forked repository_ Anda berupa `https://github.com/<username>/hidrokit-nb`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_08.png" alt="new pull request"><br>
</div>

- Akan muncul tampilan "Comparing changes". Klik **compare accross forks** untuk membandingkan _repo_ Anda dengan _repo_ hidrokit-nb. Pastikan _repo_ hidrokit di posisi kiri dan _repo_ Anda di posisi kanan (perhatikan tanda panah ⬅ yang berarti menggabungkan kanan ke kiri). Bandingkan cabang **master**. Klik **Create Pull Request** untuk ke langkah berikutnya.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_09.png" alt="comparing changes"><br>
</div>
Jika mendapatkan pesan "Can't automatically merge". Abaikan dan lanjut dengan klik **Create Pull Request**.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_10.png" alt="if something is not right"><br>
</div>

- Isi _Pull Request_ dengan informasi notebook Anda. Untuk judul isi sejelas dan sesingkat mungkin. Centang pilihan "Allow edit from maintainers" untuk memberikan akses pengelola mengubah PR. Klik **Create Pull Request**.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_11.png" alt="pull request message"><br>
</div>

- Dari sini, pengelola akan memeriksa PR Anda. Jika terdapat konflik, pengelola akan memberi tahu langkah selanjutnya (hal ini seharusnya tidak terjadi jika ini merupakan PR pertama Anda). Jika tidak memiliki konflik, PR anda akan digabungkan ke _repo_ hidrokit-nb dan notebook Anda akan muncul di direktori _repo_ hidrokit-nb

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_12.png" alt="you are done"><br>
</div>

<div align="center" markdown="1">
🎉🎊 Selamat! Anda telah membuat _Pull Request_ pertama Anda. 🎊🎉
{: .fs-5 .fw-700}

Kami menanti kontribusi Anda berikutnya. 👍👍 
{: .fs-5 .fw-300}
</div>

---
## Bacaan lebih lanjut
- [Forking Project](https://guides.github.com/activities/forking/)
- [Pull Requests](https://help.github.com/en/articles/about-pull-requests)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
