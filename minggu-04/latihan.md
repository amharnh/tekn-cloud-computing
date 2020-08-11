# Pertemuan ke-4 Praktikum Teknologi Cloud

## Instalasi Openstack pada Ubuntu 18.04.3

Sebelum memulai praktikum kali ini, kita harus menyiapkan OS yang akan digunakan yaitu Ubuntu 18.04.3 dengan ketentuan spesifikasi sebagai berikut.

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/1.png)

Maka dari ini pada proses instalasi Ubuntu pada Virtualbox Manager kita sesuaikan dengan spesifikasi yang diminta
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/2.png)

- Update Ubuntu

Karena kita masih baru saja menggunakan OS Ubuntu tersebut maka semua software yang ada telah lama tidak ter-update maka dari itu kita memerlukan proses update untuk software - softwarenya
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/4.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/5.png)

Setelah proses Update telah selesai, kita harus melakukan reboot terlebih dahulu agar software yang telah diupdate dapat berjalan dengan baik

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/6.png)


- Tambah User Stack

Pada praktikum kali ini kita menggunakan user baru dengan nama "stack" pada Ubuntu
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/7.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/8.png)

- Install Git dan download devstack

untuk proses install git dan download devstack disini kita akan melakukannya pada user stack
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/9.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/10.png)

- Membuat konfigurasi file devstack

Bagian ini merupakan bagian paling penting dikarenakan setiap pengaturan pada masing - masing pengguna akan berbeda. Yang membedakan yaitu ada pada host IP
Untuk mengecek berapa host IP yang dimiliki oleh kita yaitu dengan menggunakan perintah ifconfig

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/11.png)

host IP tersebut nantinya akan digunakan di dalam pengaturan file local.conf

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/12.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/13.png)

- Install Openstack

Untuk melakukan instalasi Openstack dapat dengan menggunakan perintah ./stack.sh , namun proses ini membutuhkan waktu lumayan lama tergantung koneksi internet yang dimiliki
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/14.png)

Bila proses telah selesai maka hasil akhirnya akan menampilkan tampilan berikut
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-04/Image/15.png)