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

Jika ini bukan pengalaman pertama dalam mengunggah notebook. Baca [Pull Request ke-dua](#pull-request-ke-dua).

### *Fork hidrokit-nb*
- Masuk akun [GitHub](https://github.com/login).
- Buka tautan [https://github.com/taruma/hidrokit-nb/](https://github.com/taruma/hidrokit-nb/).
- Klik ___Fork___ pada tepi kanan atas.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_00.png"><br>
</div>

- Akan muncul proses _forking_.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_01.png"><br>
</div>

- Tunggu proses _fork_ selesai.

### _Upload Files_
- Setelah proses _fork_ selesai. Klik `notebook` pada daftar _folder_.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_02.png"><br>
</div>

- Klik __Upload files__. Pastikan bahwa Anda berada di direktori `hidrokit-nb/notebook/`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_03.png"><br>
</div>

- Akan terbuka halaman untuk mengunggah _file_. Anda bisa mengupload dengan cara ___drag files___ atau mengklik pilihan __choose your files__. Pastikan berada di direktori `hidrokit-nb/notebook`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_04.png"><br>
</div>

- Pastikan bahwa notebook anda terunggah.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_05.png"><br>
</div>

- Isi deskripsi _commit_ seperti pada gambar. Pastikan pilihan sudah seperti di gambar. Klik **Commit Changes**. 
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_06.png"><br>
</div>

- Hasil unggah dapat dilihat dengan membuka direktori `notebook`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_07.png"><br>
</div>

### _Pull Request_

Jika notebook yang ingin diunggah sudah tersimpan pada _repo_ Anda. Saatnya menggabungkan hasil unggahan/perubahan yang Anda lakukan dengan _repo_ hidrokit-nb. 

- Dari halaman _forked repository_ yang telah Anda buat klik **New pull request**. Alamat _forked repository_ Anda berupa `https://github.com/<username>/hidrokit-nb`.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_08.png"><br>
</div>

- Akan muncul tampilan "Comparing changes". Klik **compare accross forks** untuk membandingkan _repo_ Anda dengan _repo_ hidrokit-nb. Pastikan _repo_ hidrokit di posisi kiri dan _repo_ Anda di posisi kanan (perhatikan tanda panah ⬅ yang berarti menggabungkan kanan ke kiri). Bandingkan cabang **master**. Klik **Create Pull Request** untuk ke langkah berikutnya.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_09.png"><br>
</div>
Jika mendapatkan pesan "Can't automatically merge". Abaikan dan lanjut dengan klik **Create Pull Request**.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_10.png"><br>
</div>

- Isi _Pull Request_ dengan informasi notebook Anda. Untuk judul isi sejelas dan sesingkat mungkin. Centang pilihan "Allow edit from maintainers" untuk memberikan akses pengelola mengubah PR. Klik **Create Pull Request**.
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_11.png"><br>
</div>

- Selamat! 🎉🎉 untuk membuat _Pull Request_ pertama Anda. Dari sini, pengelola akan memeriksa PR Anda. Jika terdapat konflik, pengelola akan memberi tahu langkah selanjutnya. Jika semuanya bisa langsung digabungkan terimakasih untuk berkontribusi di proyek ini. Kami menanti kontribusi Anda kedepan. 😊
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/unggah_notebook_12.png"><br>
</div>

---
## *Pull Request* ke-dua

Jika Anda ingin mengunggah notebook lagi setelah melakukan _Pull Request_ pertama Anda, kemungkinan akan menemukan konflik pada _repo_ Anda dikarenakan _repo_ hidrokit-nb akan terus berkembang dan diperbarui seiringnya waktu, sehingga _repo_ Anda bisa tertinggal _update_ dari _repo_ hidrokit-nb. Untuk mengatasi konflik ini ada berbagai cara untuk mengunggah notebook lagi.

### _Delete Forked Repository_

Ini merupakan solusi paling cepat yaitu menghapus _repo_ Anda dan melakukan langkah *Pull Request* sebagaimana pengalaman pertama Anda. Langkah ini tidak memerlukan pengalaman dalam menggunakan Git/GitHub, jadi ini merupakan solusi paling sederhana bagi kebanyakan orang. 

#### _Delete Repository_
{: .no-toc}
- Klik "Settings" pada halaman _repo_ Anda. 
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_00.png"><br>
</div>

- _Scroll down_ ke bagian paling bawah halaman. Pada "Danger Zone", klik **Delete this repository**
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_01.png"><br>
</div>

- Ketik nama _repo_ Anda yaitu `hidrokit-nb`. Dan lanjutkan dengan klik **I understand the consequences, delete this repository**
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_02.png"><br>
</div>

Catatan: Menghapus _repo_ Anda tidak menghilangkan hasil kontribusi Anda sebelumnya di _repo_ hidrokit-nb. 

### _Rebase/Merged Repository_

Ini memerlukan pengetahun/pengalaman Git. Jika Anda bukan _developer_, kami sarankan untuk menggunakan langkah diatas. Jika Anda _developer_, Anda bisa membantu mengembangkan bagian ini. 

---
## Bacaan lebih lanjut
- [Forking Project](https://guides.github.com/activities/forking/)
- [Pull Requests](https://help.github.com/en/articles/about-pull-requests)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
