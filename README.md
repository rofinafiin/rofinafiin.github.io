# Dokumentasi Git

Apa itu Git? Git merupakan salah satu version vontrol sistem yang paling banyak digunakan di seluruh dunia. Untuk menginstall git kita dapat mendownloadnya langsung dari website resmi [git](https://git-scm.com/download/win)

Berikut ini merupakan dokumentasi yang saya buat untuk mengupload project ke Github melalui VCS Git

## Konfigurasi username dan email Github

Untuk Username:
`git config --global user.name "username"`

Untuk Email:
`git config --global user.email "contoh@gmail.com"`

- Konfigurasi dilakukan untuk mengatur akun yang akan digunakan dalam Version Control System Git agar dapat melakukan push menuju repository di akun Github anda.

## Melakukan push menuju repository

`git init`

- Perintah git init digunakan untuk membuat reposistory di file lokal yang anda pilih


`git status`

- Perintah git status digunakan untuk mengetahui status dari repository lokal yang anda buat


`git add .`

- Setelah melakukan pengecekan menggunakan status untuk menambahkan file baru di repository yang dipilih anda dapat menggunakan **git add .** (menambahkan semua file yang ada di dalamnya) atau **git add <file>** (untuk menambahkan file yang belum ada di repository ) 
- Kemudian setelah itu cek kembali status dari repository yang dituju.


`git commit -m "penjelasan`

- Commit biasa digunakan untuk menyimpan perubahan yang dilakukan, setelah melakukan commit langkah selanjutnya adalah melakukan push menuju repository yang dituju dengan menggunakan perintah:

`git push origin master` (master/main merupakan tipe branch yang digunakan dalam repository yang dibuat)


## Pull requests
- Pull request biasa digunakan untuk menggabungkan kode (Biasanya digunakan dalam suatu repository yang terdapat lebih dari 1 contributor atau juga untuk mengupdate perubahan yang terjadi pada file dalam repository)

Sebelum mengedit lakukan pull dan fetch terlebih dahulu
`git pull origin master`
`git fetch`
`git push origin master`

- Kemudian lakukan edit pada file yang ada pada repo, jika file belum terdownload atau belum clone, anda dapat melakukan clone dengan cara

`git clone <url>`


- Setelah melakukan edit lakukan kembali perintah push, dengan mengikuti langkah-langkah yang telah ditulis sebelumnya.

- Nah, untuk melakukan pull request anda tinggal menekan **new pull request** pada repository di github, kemudian atur branch yang akan di compare perbedaannya.

- Jika semuanya sudah terupdate maka output yang akan dikeluarkan pada git akan muncul `everything already up-to-date`
