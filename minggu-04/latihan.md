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






Docker adalah platform perangkat lunak yang memungkinkan Anda membuat, menguji, dan menerapkan aplikasi dengan cepat. Docker mengemas perangkat lunak ke dalam unit standar yang disebut kontainer yang memiliki semua yang diperlukan perangkat lunak agar dapat berfungsi termasuk pustaka, alat sistem, kode, dan waktu proses. Dengan menggunakan Docker, Anda dapat dengan cepat menerapkan dan menskalakan aplikasi ke lingkungan apa pun dan yakin bahwa kode Anda akan berjalan.

Disini saya menggunakan Docker Toolbox untuk menjalankan Docker pada OS Windows
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/1.png)

Setelah selesai melakukan download file Docker Toolbox tersebut, kita dapat langsung melakukan instalasi DockerToolbox tersebut
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/2.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/4.png)

Setelah selesai melakukan proses instalasi, nantinya akan terbuat 2 shortcut seperti berikut
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/5.png)

Yang akan kita gunakan yaitu Docker Quickstar Terminal, jadi nantinya kita akan menjalankan Docker pada terminal tersebut

Bila proses instalasi berjalan dengan baik maka hasil akhir saat terminal tersebut dibuka akan menampilkan tampilan seperti berikut
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/6.png)

Namun kebanyakan memiliki beberapa error seperti docker-machine default tidak terdeteksi atau tidak bisa dibuat. 
Untuk mengatasinya kita dapat dengan membuat docker-machine default tersebut secara manual dengan mengetikan perintah berikut pada Command Prompt
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/7.png)
Kemudian kita dapat menjalankan Docker Quickstar Terminal dan nantinya proses pembuatan docker-machine pada terminal akan ter-skip karena telah dibuat

Untuk mengecek versi berapa Docker yang kita gunakan dapat dengan menggunakan perintah docker --version
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/8.png)

Lalu untuk mengecek hasil instalasi Docker yaitu kita dapat mencobanya dengan menjalankan image bawaan dari docker, yaitu hello-world
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/9.png)

Selain menjalankan perintah diatas, kita dapat melihat daftar docker-machine yang tersedia dengan menggunakan perintah ls dan juga melihat daftar docker-machine yang telah aktif dengan perintah ps --all
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/10.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-07/Image/11.png)






