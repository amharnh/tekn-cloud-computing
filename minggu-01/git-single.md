## Pada pertemuan pertama ini kita belajar tentang instalasi Git pada komputer dan juga dilakukan konfigurasi Git tersebut, setelah itu kita belajar tentang cara memanipulasi repository yang akan kita gunakan pada Git

### Untuk langkah - langkah instalasinya yaitu sebagai berikut:

1. Pastikan anda sudah memiliki file git yang siap untuk di install. Bila belum memiliki file tersebut, bisa dengan mendownload [disini](https://git-scm.com/downloads)

![1](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/1.png)

2. Lakukan langkah - langkah seperti pada gambar di bawah :
![2](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/2.png)
![3](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/3.png)
![4](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/4.png)
![5](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/5.png)
![6](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/6.png)
![7](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/7.png)
![8](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/8.png)
![9](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/9.png)
![10](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/10.png)
![11](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/11.png)

3. Setelah proses instalasi selesai, kita bisa mengeceknya melalui :
![12](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/12.png)
![13](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/13.png)

atau dengan mengetikan perintah "git version" di command prompt
![14](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/instalasi/14.png)


### Setelah proses instalasi Git telah selesai, hal yang selanjutnya kita lakukan yaitu melakukan konfigurasi Git tersebut dengan menggunakan Git Bash, dan dengan cara sebagai berikut : 

1. Ketikan perintah git config --global user.name "----" dan git config --global user.emal ---- (tanda ---- diisi dengan username dan email anda yang terdaftar di GitHub)

2. Setelah proses pengetikan perintah tersebut selesai, kita bisa mengeceknya dengan melihat konfigurasi yang ada dengan perintah git config --list

![konfigurasi](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/konfigurasi/2.png)


### Kemudian hal yang dilakukan selanjutnya yaitu tentang cara memanipulasi file .md atau file markdown 

Sebelumnya kita perlu membuat Repository terlebih dahulu di akun GitHub kita dengan cara

![create Repo](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/1.png)

Bila proses pembuatan Repo berhasil, maka akan menampilkan

![Repo done](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/2.png)

selanjutnya kita melakukan manipulasi file markdown dari komputer local

1. Pertama kita lakukan proses clone isi dari repository kita yang ada di GitHub dengan mengetikan perintah

![Clone](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/3.png)

setelah proses clone selesai, maka folder dari repo github kita akan tersimpan pada lokasi berikut

![Repo Lokal](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/4.png)

2. lalu selanjutnya kita bisa membuat file .md atau markdown dengan menggunakan perintah vim, dan untuk melihat isi dari file tersebut bisa dengan menggunakan perintah cat

![Vim Cat](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/5.png)

3. Selanjutnya kita gunakan perintah git add untuk menambahkan file yang kita modifikasi ke antrian yang nantinya akan kita commit

![Add](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/6.png)

4. Pada langkah ini, kita menggunakan perintah git commit yang digunakan untuk menyimpan perubahan pada file yang telah di add sebelumnya dengan disertakan log aktivitas

![Commit](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/7.png)

5. Setelah proses add dan commit telah dilakukan, hal selanjutnya yang dilakukan yaitu kita melakukan proses push file dan folder pada repo lokal tersebut ke repo github dengan menggunakan perintah git push

![Push](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/10.png)

6. Setelah proses push telah selesai, kalian bisa mengeceknya pada repo github milik kalian masing - masing

![Hasil](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/11.png)

![Hasil](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-01/repository/12.png)
