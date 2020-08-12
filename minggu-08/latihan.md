# Pertemuan ke-8 Praktikum Teknologi Cloud

## Docker Compose

Pada praktikum ke 8 ini kita masih sama menggunakan terminal dari Docker toolbox yang telah kita install pada praktikum sebelumnya
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/1.png)

Namun pada praktikum kali ini kita akan mencoba mengenal tentang Docker Compose
Docker-compose disini adalah sebuah alat dari docker yang digunakan untuk mendefinisikan dan menjalankan aplikasi multi kontainer. Dengan docker-compose kita bisa menjalankan kontainer 1 dengan yang lainya dengan 1 perintah . Docker-compose juga menggunakan yaml file untuk menyimpan konfigurasi dari service yang dibuat.

Dalam praktikum ini kita akan membuat folder baru sebagai tempat untuk melakukan praktikum bernama composetest
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/2.png)

- Membuat file setup 
### app.py
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/3.png)

### requirements.txt
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/4.png)

- Membuat Dockerfile

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/5.png)

- Membuat docker-compose.yml untuk konfigurasi service
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/6.png)

- Menjalankan compose-up

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/7.png)

Dihasil akhir nantinya kita akan mengakses localhost:5000 di browser dan akan menampilkan hasil sebagai berikut

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-08/Image/8.png)
