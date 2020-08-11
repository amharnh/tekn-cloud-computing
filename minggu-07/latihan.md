# Pertemuan ke-7 Praktikum Teknologi Cloud

## Teknologi Virtualisasi dan Container - Docker

Sebelum memulai menggunakan Docker, kita harus mengenal terlebih dahulu tentang apa itu docker.

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






