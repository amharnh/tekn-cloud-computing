Langkah 1 Periksa konfigurasi aplikasi
Mari kita verifikasi bahwa aplikasi yang kita terapkan di skenario sebelumnya sedang berjalan. Kita akan menggunakan perintah kubectl get dan mencari Pod yang ada:
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/1.png)

Jika tidak ada pod yang berjalan maka itu berarti lingkungan interaktif masih memuat ulang keadaan sebelumnya. Harap tunggu beberapa detik dan daftarkan kembali Pod tersebut. Anda dapat melanjutkan setelah Anda melihat Pod yang sedang berjalan.

Selanjutnya, untuk melihat kontainer apa yang ada di dalam Pod itu dan gambar apa yang digunakan untuk membangun kontainer tersebut, kita menjalankan perintah deskripsi pod:
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/2.png)


Di sini kita melihat detail tentang container Pod: alamat IP, port yang digunakan, dan daftar peristiwa yang terkait dengan daur hidup Pod.

Keluaran dari perintah gambarkan sangat luas dan mencakup beberapa konsep yang belum kami jelaskan, tapi jangan khawatir, mereka akan menjadi familiar pada akhir bootcamp ini.

Catatan: perintah menjelaskan dapat digunakan untuk mendapatkan informasi mendetail tentang sebagian besar primitif kubernetes: node, pods, deployments. Keluaran mendeskripsikan dirancang agar dapat dibaca manusia, bukan untuk dijadikan skrip.

Langkah 2 Tunjukkan aplikasi di terminal
Ingatlah bahwa Pod berjalan di jaringan pribadi yang terisolasi - jadi kita perlu akses proxy ke Pod tersebut sehingga kita dapat men-debug dan berinteraksi dengannya. Untuk melakukan ini, kita akan menggunakan perintah kubectl proxy untuk menjalankan proxy di jendela terminal kedua. Klik pada perintah di bawah ini untuk secara otomatis membuka terminal baru dan menjalankan proxy: 
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/3.png)

echo -e "\ n \ n \ n \ e [92mMulai Proxy. Setelah memulai, tidak akan menghasilkan respons. Silakan klik Tab Terminal pertama \ n"; kubectl proxy

Sekarang lagi, kita akan mendapatkan nama Pod dan mengkueri Pod itu langsung melalui proxy. Untuk mendapatkan nama Pod dan menyimpannya dalam variabel lingkungan POD_NAME:
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/4.png)

ekspor POD_NAME = $ (kubectl get pods -o go-template --template '{{range .items}} {{. metadata.name}} {{"\ n"}} {{end}}') echo Nama Pod: $ POD_NAME

Untuk melihat keluaran dari aplikasi kita, jalankan permintaan curl. ![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/5.png)

Url adalah rute ke API dari Pod.

Langkah 3 Lihat log kontainer
Apa pun yang biasanya dikirimkan aplikasi ke STDOUT menjadi log untuk container di dalam Pod. Kita bisa mengambil log ini menggunakan perintah kubectl logs: 
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/6.png)

Catatan: Kami tidak perlu menentukan nama container, karena kami hanya memiliki satu container di dalam pod.

Langkah 4 Menjalankan perintah di wadah
Kita dapat menjalankan perintah secara langsung di container setelah Pod aktif dan berjalan. Untuk ini, kami menggunakan perintah exec dan menggunakan nama Pod sebagai parameter. Mari daftar variabel lingkungan: 
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/7.png)

Sekali lagi, perlu disebutkan bahwa nama container itu sendiri dapat dihilangkan karena kita hanya memiliki satu container di dalam Pod.

Selanjutnya mari kita mulai sesi bash di wadah Pod: 
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/8.png)

Kami sekarang memiliki konsol terbuka di wadah tempat kami menjalankan aplikasi NodeJS kami. Kode sumber aplikasi ada di file server.js:
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/9.png)

Anda dapat memeriksa apakah aplikasi tersebut aktif dengan menjalankan perintah curl: 
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/10.png)

Catatan: di sini kami menggunakan localhost karena kami menjalankan perintah di dalam NodeJS Pod. Jika Anda tidak dapat terhubung ke localhost: 8080, periksa untuk memastikan Anda telah menjalankan perintah kubectl exec dan menjalankan perintah dari dalam Pod

Untuk menutup keluar jenis koneksi kontainer Anda.
![~](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-14/Image/11.png)