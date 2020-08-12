# Pertemuan ke-12 Praktikum Teknologi Cloud

## Docker Orchestration

Pada praktikum kali ini kita akan belajar tentang Docker Orchestration. Disini masih menggunakan fitur Play With Docker yang akan digunakan sebagai pengganti OS Linux untuk menjalankan Docker

### Section 1 - Apa itu Orchestration
Docker / Container Orchestration ini sebenarnya adalah mengurus daur hidup dari container-container yang ada, yang ada dalam environment yang dinamik. Contoh orchestrator yang dikenal kalangan masyarakat luas, salah satunya adalah kubernetes, atau docker swarm.

![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/0.png)

Cara kerja Docker orchestrator ini yaitu pod IP address bertugas untuk menyimpan container-container yang dipakai oleh host tersebut, lalu di kontainer tersebut, interaksi antar kontainer dalam docker orchestration dijalankan via service third party, sehingga service tersebut dapat meregulasi usage image file dalam kontainer.


### Section 2 - Melakukan konfigurasi mode Swarm
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/1.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/2.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/4.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/5.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec2/6.png)

### Section 3 - Menerapkan aplikasi di beberapa host
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec3/1.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec3/2.png)

### Section 4 - Skala Aplikasi
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec4/1.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec4/2.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec4/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec4/4.png)

### Section 5 - Kuras node dan penjadwalan ulang Container
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/1.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/2.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/4.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/5.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/Sec5/6.png)

### Penyelesain
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/SecCU/1.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/SecCU/2.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/SecCU/3.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/SecCU/4.png)
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-12/Image/SecCU/5.png)