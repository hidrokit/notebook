# Berkontribusi

## Kode etik

Proyek ini dan seluruh yang berpartisipasi harus mengikuti [**Kode Etik** yang berlaku](CODE_OF_CONDUCT.md).

## Bentuk Kontribusi

Proyek ini menerima kontribusi berupa perbaikan/penambahan dokumentasi, memperbagus/memperbaiki situs, ide, saran/kritik, membalas isu, _pull request_ atau segala bentuk yang menurut Anda dapat mengembangkan proyek ini.

Kontribusi dalam proyek ini dapat dikategorikan dalam bentuk GitHub/Dokumentasi (label: `github`/`documentation`) dan Situs (label: `site`).

### Berkontribusi GitHub/Dokumentasi

Bentuk kontribusi GitHub/Dokumentasi berupa: 
- Perbaikan/koreksi dokumentasi yang berkaitan langsung dengan penggunaan/penampilan pada GitHub seperti _issue template_, `README.md`, `CONTRIBUTING.md`, dll.
- Ide/Saran layanan _Integrations & Services_.
- Moderasi/Triase isu atau PR.
- Membantu menyelesaikan isu berlabel github/documentation yang dibuat. 

### Berkontribusi Situs

Bentuk kontribusi Situs berupa: 
- Perbaikan/Mengoreksi penulisan/kode.
- Memperbagus/mengembangkan situs.
- Membantu menyelesaikan isu berlabel site yang dibuat. 

Situs hidrokit-nb dibuat menggunakan Jekyll & GitHub Pages. Untuk instalasi pada mesin lokal baca [README pada direktori `docs/`](docs/README.md).


## Repository Tree

Berikut struktur berkas/direktori yang digunakan dalam proyek ini. Stuktur direktori diusahakan untuk sesederhana mungkin. 

```
hidrokit-nb
+---.github
+---_old      [DEPRECATED]
+---_assets
+---docs
\---notebook
```

Berikut kegunaan masing-masing direktori:
- `.github/`: Pengaturan templat isu/PR.
- `_assets/`: Direktori media. Gambar yang digunakan proyek ini disimpan di direktori ini.
- `docs/`: Situs Jekyll. Seluruh dokumen di dalam direktori ini ditujukan untuk membuat situs hidrokit-nb.
- `notebook/`: Koleksi notebook. Berisikan files `.ipynb` hasil unggahan kolaborator.

Berikut direktori yang tidak digunakan lagi:
- `_old`: Arsip. Direktori ini sudah tidak digunakan lagi, hanya sebagai penyimpanan file `.ipynb` yang terdahulu.
