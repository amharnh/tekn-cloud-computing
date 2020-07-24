# Pertemuan ke-2 Praktikum Teknologi Cloud

---

## Perbedaan dari IaaS, PaaS, dan SaaS

### IaaS (Infrastructure as a Service)
adalah sebuah layanan yang disediakan oleh perusahaan, grup, komunitas, ataupun pemerintah yang memungkinkan pengguna untuk mendapatkan kendali penuh terhadap infrastruktur yang digunakan, jaringan komputer dasar, jaringan pengiriman konten, routing, penyimpatan data komoditas, dan hosting sistem operasi tervisualisasi.

### PaaS (Platform as a Service)
adalah sebuah layanan yang disediakan oleh perusahaan, grup, komunitas, ataupun pemerintah yang menyediakan layanan berupa framework / platform yang digunakan untuk pengembangan perangkat lunak.

### SaaS (Software as a Service)
adalah sebuah layanan yang disediakan oleh perusahaan, grup, komoditas, ataupun pemerintah yang memungkinkan pengguna untuk dapat tetap menggunakan suatu software dan dengan device apapun melalui koneksi internet.

---

## Arsitektur Platform SaaS

![Arsitektur SaaS](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-02/Image/saas-arsitektur.png)

Dengan menggunakan model tersebut, arsitektur pada SaaS ini memungkinkan layanan untuk dapat digunakan oleh banyak pengguna dan dari berbagai jenis device seperti pada gambar diatas (App Server, Mobiles, Networks, PC, Codes, dan Database), dikarenakan aplikasi ini diinstall pada banyak mesin untuk mendukung skalabilitas.

Alasan menggunakan Arsitektur SaaS

- Dari Pendapat Konsumen

Produk SaaS ini merupakan salah satu cara termudah untuk menggunakan layanan atau produk digital dimana pengguna hanya cukup mengaksesnya melalui web, membayar layanan tersebut, dan lalu menggunakannya.

- Dari Pendapat Perusahaan

Produk SaaS ini membantu mereka dalam mengiklankan produk perusahaan mereka ke pasar dunia dan juga memungkinkan mereka untuk mempertahankan kontrol keseluruhan atas produk tersebut, selain itu juga membantu dalam mengurangi jangka waktu bagi produk untuk mencapai pasar, mengurangi biaya perawatan produk, memudahkan pembaruan produk, dan lain - lain.


---

## Tahapan membangun aplikasi SaaS berbasis Cloud

![Membangun SaaS](https://github.com/amharnh/tekn-cloud-computing/blob/master/minggu-02/Image/membangun-saas.png)

Bisnis SaaS saat ini merupakan sebuah industri yang tumbuh dengan sangat cepat yang menarik banyak orang dan perusahaan. Organisasi-organisasi yang tertarik tersebut semakin banyak mengembangkan aplikasinya masing - masing di cloud. Sebelum memulai mengembangkan aplikasi pada Cloud, perlu kita mengerti tentang pen-skala-an di cloud karena memiliki beberapa manfaat dan risiko yang nantinya akan kita hadapi.

- Membangun Cloud

Saat membangun aplikasi SaaS, ada kemungkinan besar bahwa kita membangunnya di Cloud, hal ini dikarenakan Cloud memiliki banyak keunggulan seperti memudahkan dalam skalabilitas yang berbeda dengan saat kita menggunakan server lokal.

- Bagaimana cara kita memulainya ?

Bahasa pemrograman mana yang harus kita pakai, basis data apa yang akan kita gunakan, perangkat lunak apa yang harus kita pilih? Ada banyak pertanyaan yang pasti akan terpikirkan pada saat kita pertama kali baru memulainya. Karenanya disini kita akan mencoba fokus pada 3 hal-hal tersebut yang merupakan bagian terpenting untuk membangun aplikasi pada Cloud.

- Bahasa Pemrograman

Membangun aplikasi pada cloud berarti kita membangun suatu produk dengan bahasa pemrograman modern. Selain membutuhkan kemampuan dan keterampilan pribadi, pilihan bahasa pemrograman dipengaruhi oleh kemungkinan masing-masing bahasa. Ada berbagai bahasa pemrograman modern di luar sana sehingga sulit untuk memilih yang tepat. Sehingga disini kita hanya perlu melihat yang paling menonjol dan mencoba bermain-main dengan bahasa pemrograman tersebut dan lakukan eksperimen sebanyak mungkin.
Saat ini, Python merupakan salah satu bahasa pemrograman modern yang paling banyak digunakan oleh programmer. Python adalah bahasa pemrograman yang banyak digunakan, dan dirancang untuk menekankan pada keterbacaan kode. Python dapat melakukan banyak hal. Apa pun aplikasi web yang ingin kita bangun, kemungkinan ada kerangka kerjanya di Python dan juga tingkat fleksibilitas python untuk mengatasi berbagai kasus dalam penggunaannya

- Basis Data

Selain memilih penggunaan bahasa pemrograman, kita juga harus pintar dalam memilih pemasangan basis data yang akan digunakan. Disini kami merekomendasikan penggunaan document-oriented database. Jenis database ini sangat berbeda dengan konsep tradisional database relasional.
Alasan untuk menggunakan document-oriented database yaitu dikarenakan database jenis ini mendapatkan informasi tipenya dari data itu sendiri. Dengan demikian setiap instansi data dapat berbeda dari yang lain yang memungkinkan lebih banyak fleksibilitas, terutama ketika berhadapan dengan perubahan dan sering mengurangi ukuran basis data.
Singkatnya, konsep document-oriented database menawarkan pengalaman yang lebih banyak dengan teknik pemrograman modern.

- Perangkat Lunak

Disini kami merekomendasikan menggunakan MongoDB sebagai aplikasi untuk database aplikasi
Alasan memilih menggunakannya dikarenakan MongoDB merupakan document-oriented database yang memberikan kinerja tinggi, ketersediaan tinggi, dan skalabilitas mudah. Selain kinerja, Skalabilitas adalah faktor terpenting bagi kita sebagai pengembang aplikasi SaaS.
Banyak pengembang SaaS bertujuan untuk meningkatkan skala bisnis mereka. Selain mengubah skala produk dari perspektif bisnis, kita tidak boleh melupakan masalah teknis. Menskalakan teknologi dengan MongoDB cukup mudah. Dengan menggunakan automatic sharding, Kita dapat mendistribusikan data di berbagai mesin.
Sharding adalah metode untuk menyimpan data di beberapa mesin dan MongoDB menggunakan sharding untuk mendukung penyebaran dengan dataset besar.


