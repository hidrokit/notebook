---
layout: default
title: Pull Request
parent: Panduan
permalink: /panduan/pull-request
---

Terima kasih telah melakukan _pull request_ sebelumnya. 🙏 Halaman ini ditujukan bagi Anda yang ingin mengunggah notebook lagi atau melakukan perubahan pada repo hidrokit. 

Jika Anda ingin mengunggah notebook lagi setelah melakukan _Pull Request_ pertama Anda, kemungkinan akan menemukan konflik pada _repo_ Anda dikarenakan _repo_ hidrokit-nb akan terus berkembang dan diperbarui seiringnya waktu, sehingga _repo_ Anda bisa tertinggal (*behind*) dari _repo_ hidrokit-nb. Untuk mengatasi konflik ini ada berbagai cara untuk mengunggah notebook lagi.

Kami merekomendasikan menggunakan cara [Perbarui _repo_ Anda](#perbarui-repo-anda). Jika Anda menghadapi kesulitan atau tiba-tiba pesan _error_, Anda bisa memilih melakukan [*Delete Forked Repository*](#delete-forked-repository) jika tidak mau ambil pusing. 😁

DAFTAR ISI
{: .no_toc .text-delta}

1. TOC
{:toc}

---

<div align="center" markdown="1">
## _Delete Forked Repository_
</div>

Ini merupakan solusi paling cepat yaitu menghapus _repo_ Anda dan melakukan langkah *Pull Request* sebagaimana pengalaman pertama Anda. Langkah ini tidak memerlukan pengalaman dalam menggunakan Git/GitHub, jadi ini merupakan solusi paling sederhana bagi kebanyakan orang. 

### _Delete Repository_
- Klik "Settings" pada halaman _repo_ Anda. 
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_00.png" alt="open settings"><br>
</div>

- _Scroll down_ ke bagian paling bawah halaman. Pada "Danger Zone", klik **Delete this repository**
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_01.png" alt="delete this repository"><br>
</div>

- Ketik nama _repo_ Anda yaitu `hidrokit-nb`. Dan lanjutkan dengan klik **I understand the consequences, delete this repository**
<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/delete_fork_02.png" alt="delete confirmation"><br>
</div>

Catatan: Menghapus _repo_ Anda tidak menghilangkan hasil kontribusi Anda sebelumnya di _repo_ hidrokit-nb. 

---
<div align="center" markdown="1">
## Perbarui _repo_ Anda
</div>

Jika *repo* Anda tidak disentuh/diubah semenjak _pull request_ pertama Anda. Langkah ini setidaknya lebih praktis dan konsisten untuk melakukan pengunggahan rutin. Dan dengan mengikuti langkah ini, setidaknya Anda mengetahui konsep Git dan integrasinya dengan GitHub. Cara ini tidak membutuhkan Anda memasang Git di komputer Anda. 🙌.

- Buka _repo_ Anda yang beralamat `https://github.com/<username>/hidrokit-nb`.
- Anda bisa melihat status _repo_ Anda. Dari gambar terlihat bahwa _repo_ tertinggal `25 commits` yang bisa diartikan tertinggal 25 langkah dari _repo utama_ yaitu hidrokit-nb.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_00.png" alt="info repo"><br>
</div>

- Langkah berikutnya adalah memperbarui _repo_ Anda dengan melakukan _pull request_. Akan tetapi, Anda ingin mengarahkan target yang diperbarui adalah _repo_ Anda. Klik **Pull request** atau **New pull request** untuk memulai.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_01.png" alt="pull request"><br>
</div>

- Anda ingin memastikan bahwa kotak merah mengarah ke _repo_ Anda (`<username anda>/hidrokit-nb`) seperti yang ada pada gambar. Klik **compare across forks** untuk menampilkan pilihan selain _repo_ Anda. Pastikan bahwa Anda memperbarui _repo_ Anda dari _repo_ hidrokit-nb (`taruma/hidrokit-nb`). Lanjutkan dengan membuat _pull request_ dengan mengklik **Create pull request**. 

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_02.png" alt="comparing repo"><br>
</div>

- Isi pesan _pull request_ sesuka Anda (Ini _repo_ Anda juga 😁), akan tetapi lebih baik jika selalu membiasakan memberi/mencatat pesan setiap aktivitas anda. Jika sudah mengisinya, lanjut dengan memilih **Create pull request**.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_03.png" alt="pull request message"><br>
</div>

- Anda akan melihat rangkaian sejarah _commits_ dari _repo_ Anda yang tertinggal (*outdated*) dengan _repo_ hidrokit-nb yang terbaru.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_04.png" alt="commit history"><br>
</div>

- Lanjutkan dengan melakukan **Merge pull request**.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_05.png" alt="merge pull request"><br>
</div>

- Anda akan diminta mengisi pesan. Gunakan pesan yang sudah dipilih (atau tidak 😏) dan lanjutkan dengan memilih **Confirm merge**.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_06.png" alt="merge pull request"><br>
</div>

- Anda akan melihat pesan bahwa proses _pull request_ berhasil.

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_07.png" alt="merged success"><br>
</div>

- Jika anda melihat halaman _repo_ Anda, Anda akan melihat bahwa _repo_ Anda 1 *commit* dari _repo_ hidrokit-nb. Yang artinya, _repo_ Anda sudah paling baru. 

<div align="center">
    <img src="{{ site.baseurl }}/assets/images/panduan/update_repo_08.png" alt="your repo status"><br>
</div>

<div align="center" markdown="1">
🎉🎊 Selamat! Anda telah berhasil memperbarui _Pull Request_ pertama Anda. 🎊🎉
{: .fs-5 .fw-700}

Dan menambah wawasan mengenai Git dan Github.
{: .fs-1}
</div>

Dari sini Anda bisa melakukan proses pengunggahan notebook seperti di halaman mengunggah notebook, dengan melewati tahap _fork_.

---
## Rebase/Merged Repository

Langkah ini terjadi jika _repo_ Anda memiliki perubahan yang kemungkinan konflik dengan _repo_ hidrokit-nb. Konflik tersebut harus diatasi/dievaluasi secara manual. Anda setidaknya harus melakukan operasi rebase untuk menyetarakan `HEAD` dari _repo_ hidrokit-nb dengan _repo_ Anda. 

Untuk langkah ini, Anda harus memiliki pengetahuan dan pengoperasian Git sehingga langkah ini tidak dianjurkan jika Anda hanya menggunakan _repo_ Anda untuk mengunggah notebook. 

Bagi _software developer_ atau yang memiliki wawasan Git, dapat mengembangkan bagian ini. 🙏