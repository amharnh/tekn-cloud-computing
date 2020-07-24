# Pertemuan ke-3 Praktikum Teknologi Cloud

## Heroku Command Line Interface

Sebelum memulai menggunakan Heroku CLI, kita harus mendownloadnya terlebih dahulu di [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) dan download sesuai dengan OS yang kita miliki dan install software tersebut pada komputer kita
![11](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/11.png)


Langkah - langkah untuk penggunaan awal dari Heroku CLI tersebut yaitu :
1. Pada GUI Bash, ketikan heroku login

![12](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/12.png)

2. Nantinya kita akan diminta untuk Login akun Heroku pada tab browser yang muncul
![13](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/13.png)
![14](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/14.png)

3. Bila sudah melakukan Login, maka tampilan pada Heroku CLI akan menjadi seperti ini
![15](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/15.png)


## Deployment ke PaaS di Heroku untuk Python
### Create App
- Hal pertama yang dilakukan yaitu kita melakukan clone folder heroku python dengan menggunakan perintah berikut
![16](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/16.png)

- Sehingga hasilnya akan menampilkan seperti gambar berikut
![17](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/17.png)

### Deploy App
- Pada bagian ini kita membuat folder untuk app sebagai tempat penyimpanan app tersebut di heroku, pada gambar berikut telah terbuat app dengan nama quiet-ridge-25026
![18](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/18.png)

- kemudian push folder app dari local kita ke heroku tersebut dengan perintah git push heroku master
![19](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/19.png)

- Setelah selesai melakukan proses tersebut, kita dapat mencoba membuka app kita di heroku dengan menggunakan perintah
![20](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/20.png)
![21](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/21.png)

- Atau disini kita dapat mencoba menjalankannya pada Localhost
### Declare app dependencies
- Sebelumnya kita harus menginstall library yang dibutuhkan agar dapat dijalankan
![24](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/24.png)

- Untuk melihat daftar library yang terlihat bisa dengan menggunakan perintah berikut
![25](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/25.png)

### Run App in Localhost
- Untuk menjalankannya pada localhost, maka kita perlu menjalankan library collectstatic terlebih dahulu
![26](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/26.png)

- Kemudian untuk run localhostnya, (untuk versi windows) dapat dengan menggunakan perintah "heroku local web -f Procfile.windows"

![27](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/27.png)
- Setelah itu kita dapat mengakses localhost dari app heroku python tersebut dengan browser pada alamat [http://localhost:5000](http://localhost:5000)

### Modify App
- Pada tahap ini kita mencoba melakukan modifikasi dari app yang kita buat

- Hal pertama yang dilakukan yaitu menambahkan library 'requests' pada requirement.txt
![28](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/28.png)

- Lalu mengetikan perintah 'import requests' pada views.py
![29](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/29.png)

- Dan pada saat ditest tampilan di localhostnya dengan menggunakan perintah heroku local, maka akan menampilkan tampilan sebagai berikut

![52](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/52.png)
![30](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/30.png)

### Push app ke heroku
- Untuk cara push pada heroku hampir sama seperti pada push ke Git, yaitu add -> commit -> push (git push heroku master)
![31](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/31.png)
![32](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/32.png)

- Kemudian pada saat di test pada app web heroku (quiet-ridge-25026.herokuapp.com), maka akan menampilkan tampilan yang sama seperti pada di localhost sebelumnya

![53](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/53.png)
![33](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-03/Image/33.png)