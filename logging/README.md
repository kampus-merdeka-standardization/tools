# Logging Manager

## Splunk
### Pendahuluan Splunk

Splunk adalah platform terkemuka yang memungkinkan organisasi untuk mencari, memantau, menganalisis, dan memvisualisasikan data mesin yang dihasilkan oleh aplikasi, server, dan perangkat keras jaringan dalam waktu nyata. Alat ini membantu dalam pengindeksan data besar, pencarian dan pemulihan data, dan juga dalam pembuatan laporan dan dasbor. Fitur utama Splunk mencakup kemampuan untuk mencari, menganalisis, dan memvisualisasikan data dalam waktu nyata serta pengumpulan dan pengindeksan data dari berbagai sumber.

Splunk memiliki peran penting dalam membangun ketahanan digital di perusahaan. Tujuan utamanya adalah menciptakan dunia digital yang lebih aman dan tahan banting dengan membantu tim keamanan, IT, dan DevOps menjaga organisasi mereka beroperasi dengan aman. Produk Splunk terkenal antara lain Splunk Enterprise yang memungkinkan pencarian, analisis, dan visualisasi semua data, serta Splunk Cloud Platform yang menawarkan fungsionalitas serupa dalam model SaaS (Software as a Service). Splunk juga memiliki produk Universal Forwarder yang populer untuk memindahkan data ke Splunk Enterprise dan Splunk Cloud Platform. Selain itu, Splunk menawarkan solusi SIEM (Security Information and Event Management), SOAR (Security Orchestration, Automation, and Response), dan solusi observabilitas.

Nama "Splunk" sendiri berasal dari hobi "spelunking", yang merupakan eksplorasi gua dan tambang. Dalam konteks ini, Splunk membantu dalam eksplorasi "gua informasi" dan "penambangan data", menghilangkan hambatan data untuk mengungkap makna dan langkah-langkah yang dapat diambil oleh organisasi. Dengan Splunk, organisasi dapat memantau, mencari, mengindeks, dan mengkorelasikan data besar dari berbagai sumber, serta dengan mudah mencari data besar dan mengatur peringatan, laporan, dan visualisasi yang relevan. Ini juga mendukung upaya berbagai area, mulai dari keamanan siber hingga kepatuhan, manajemen data hingga pemantauan IT dan observabilitas, serta manajemen IT dan bisnis secara keseluruhan.

Dalam hal ini, Splunk bukan hanya menawarkan kemampuan-kemampuan ini, tetapi juga membuka peluang bagi organisasi untuk melakukan banyak hal dengan kemampuan tersebut, yang pada akhirnya hanya dibatasi oleh kreativitas pengguna.

Referensi:
- [Splunk Documentation](https://docs.splunk.com/Documentation).
- [What Is Splunk & What Does It Do? An Introduction To Splunk | Splunk](https://www.splunk.com/en_us/data-insider/what-is-splunk.html).


### Cara Kerja Splunk

Splunk adalah sebuah platform yang memungkinkan pengumpulan, pencarian, pemantauan, dan analisis data dari berbagai sumber. Berikut adalah bagaimana Splunk bekerja:

1. **Pengumpulan Data**:
   - Splunk memiliki kemampuan untuk mengumpulkan data dari berbagai sumber seperti log server, data jaringan, data real-time, atau data dari aplikasi dan basis data lainnya.
   - Data ini dapat diambil dari file statis atau aliran data real-time.
   - Splunk juga memanfaatkan Universal Forwarder, sebuah mekanisme populer untuk mendapatkan data ke dalam Splunk Enterprise dan Splunk Cloud Platform.

2. **Indeksasi**:
   - Setelah data dikumpulkan, Splunk mengindeks data tersebut untuk memudahkan pencarian dan analisis【197†source】.
   - Indeksasi membantu dalam mengorganisir data dalam format yang efisien sehingga pencarian dan pengambilan data menjadi cepat dan mudah.

3. **Pencarian dan Analisis**:
   - Splunk menyediakan antarmuka pencarian yang kuat yang memungkinkan pengguna untuk mencari, menganalisis, dan memvisualisasikan data yang telah diindeks.
   - Pengguna dapat mencari data besar dan mengatur peringatan, laporan, dan visualisasi yang relevan.
   - Splunk Enterprise memungkinkan pengguna untuk mencari, menganalisis, dan memvisualisasikan semua data, memberikan wawasan yang dapat diambil tindakan.
   
4. **Visualisasi dan Laporan**:
   - Pengguna dapat membuat dashboard dan laporan berdasarkan hasil analisis untuk memvisualisasikan data dan wawasan yang diperoleh.

5. **Monitoring dan Pemantauan**:
   - Splunk juga digunakan untuk memonitor dan mengidentifikasi tren atau masalah dalam data secara real-time atau historis.

6. **Ekstensibilitas**:
   - Splunk menawarkan berbagai perangkat lunak, aplikasi, dan API, memberikan banyak fleksibilitas untuk organisasi dalam mematangkan ketahanan digital mereka.
   - Selain itu, Splunk mendukung berbagai solusi dari cybersecurity hingga kepatuhan, pipa data hingga pemantauan IT dan observabilitas, serta manajemen IT dan bisnis secara keseluruhan.

Splunk, pada dasarnya, berfungsi sebagai sarana untuk menjelajahi "gua informasi" dan "menambang" data, membantu organisasi mengungkap makna dan langkah-langkah tindakan dari data mereka.

Referensi:
- [How Splunk Works](https://www.tutorialspoint.com/splunk/index.htm) (Tutorialspoint)
- [Splunk Architecture and Components](https://mindmajix.com/splunk-architecture-and-components) (Mindmajix)
- [What Is Splunk & What Does It Do?](https://www.splunk.com/en_us/blog/tips-and-tricks/what-is-splunk-and-what-does-it-do-an-introduction-to-splunk.html) (Splunk Official Website)


### Kelebihan dan Kekurangan Splunk

#### Kelebihan:
1. **Pengolahan Data dalam Skala Besar:** Splunk mampu mengonsumsi dan memproses volume data jaringan, server, keamanan siber, dan event aplikasi yang besar, menampilkan data tersebut untuk analisis yang mudah.
2. **Pemantauan Real-Time:** Splunk memungkinkan pemantauan data dalam real-time, yang sangat penting untuk mendeteksi masalah secepat mungkin dan merespons insiden keamanan【215†edtech】.
3. **Analisis Data:** Splunk menawarkan kemampuan analisis data yang kuat, termasuk pencarian, pelaporan, dan visualisasi data, untuk membantu organisasi mendapatkan wawasan dari data mereka.
4. **Alat Manajemen Keamanan dan Insiden (SIEM):** Splunk juga berfungsi sebagai alat Manajemen Insiden dan Keamanan (SIEM) penuh, dengan kemampuan untuk memantau lalu lintas jaringan dan memberi peringatan kepada administrator berdasarkan ambang batas dan pengaturan yang disesuaikan.
5. **Ekstensibilitas:** Splunk memiliki ekstensibilitas tinggi dengan adanya add-ons dan aplikasi yang dapat membantu meningkatkan fungsionalitasnya.

#### Kekurangan:
1. **Biaya:** Biaya merupakan kekurangan yang signifikan, terutama bagi bisnis kecil. Harga dimulai dari $2000 per tahun untuk 1GB per hari, sehingga dapat di luar jangkauan untuk organisasi kecil dan menengah.
2. **Kecepatan dan Kompleksitas:** Beberapa pengembang mengeluh tentang kecepatan yang lebih lambat dan kompleksitas yang merupakan dua kekurangan lainnya dari Splunk.
3. **Kurva Belajar:** Untuk menggunakan Splunk, organisasi harus melatih orang yang akan menggunakan solusi ini, yang berarti setiap karyawan baru harus dilatih jika mereka tidak memiliki pengalaman sebelumnya.

Referensi:
- Mezmo. (n.d.). Splunk Alternatives for Fast, Affordable Log Management. Retrieved from [mezmo.com](https://www.mezmo.com/blog/splunk-alternatives/)
- Edtech. (n.d.). Splunk Tutorial: What is Splunk. Retrieved from [edtech.com](https://www.edtech.co.in/training/splunk/splunk-tutorial.php)
- SoftwareTestingHelp. (2021, April 14). Splunk Tutorial For Beginners: Explore Machine Data With Splunk. Retrieved from [softwaretestinghelp.com](https://www.softwaretestinghelp.com/splunk-tutorial-1/)


### Cara Install Splunk

Berikut adalah langkah-langkah umum untuk menginstal Splunk:

1. **Unduh Splunk**:
   - Kunjungi situs web resmi Splunk di [splunk.com](https://www.splunk.com/).
   - Pilih versi Splunk yang ingin Anda instal, seperti Splunk Enterprise, dan unduh paket instalasi untuk sistem operasi Anda (Windows, Linux, atau MacOS).

2. **Install Splunk**:
   - Buka paket instalasi yang telah Anda unduh.
   - Ikuti petunjuk pada wizard instalasi untuk menyelesaikan proses instalasi. Pada sistem operasi Windows, proses ini mungkin termasuk menjalankan file eksekusi yang telah Anda unduh, sementara pada Linux, Anda mungkin perlu menjalankan beberapa perintah di terminal.

3. **Konfigurasi Splunk**:
   - Setelah instalasi selesai, buka Splunk Web dengan menavigasi ke `https://localhost:8000` di browser web Anda.
   - Login menggunakan kredensial default (`admin` sebagai username dan `changeme` sebagai password) atau kredensial yang telah Anda tentukan selama proses instalasi.
   - Ikuti petunjuk di Splunk Web untuk menyelesaikan konfigurasi awal dan mengubah password default.

4. **Tambahkan Data ke Splunk**:
   - Di Splunk Web, pilih "Add Data" dari menu utama.
   - Ikuti petunjuk untuk menambahkan sumber data ke Splunk, seperti log file atau data streaming.

5. **Mulai Menggunakan Splunk**:
   - Setelah Anda menambahkan data ke Splunk, Anda dapat mulai mencari, menganalisis, dan memvisualisasikan data Anda menggunakan antarmuka Splunk Web.

6. **Pembaruan dan Pemeliharaan**:
   - Untuk memastikan Splunk berjalan dengan benar, pastikan untuk memeriksa pembaruan secara berkala dan mengikuti praktik terbaik pemeliharaan seperti yang dijelaskan dalam dokumentasi resmi Splunk.

Instruksi lebih lanjut dan spesifik dapat ditemukan di [Dokumentasi Resmi Splunk](https://docs.splunk.com/Documentation) dan [tutorial instalasi lainnya](https://www.guru99.com/download-install-splunk.html).

## Kibana

Kibana adalah alat visualisasi dan eksplorasi data open-source yang digunakan untuk analisis log dan time-series, pemantauan aplikasi, dan kasus penggunaan intelijen operasional. Kibana menawarkan fitur yang kuat dan mudah digunakan seperti histogram, grafik garis, diagram lingkaran, dan dukungan geospasial built-in dan menyediakan integrasi ketat dengan Elasticsearch, analitik populer dan mesin pencari, yang membuat Kibana menjadi pilihan default untuk memvisualisasikan data yang disimpan dalam Elasticsearch.

### Kelebihan

- Dashboard 
- Integrasi dengan Elastic Search
- Search, Filters, dan Charts

### Kekurangan

- Search queries sedikit lebih kompleks
- Dashboard dan laporan sedikit rumit

### Referensi

- [Kibana](https://www.pointstar.co.id/kibana/)
- [Pros Con Kibana](https://www.trustradius.com/products/kibana/reviews?qs=pros-and-cons#product-details)

## Grafana

Grafana adalah analitik sumber terbuka multi-platform dan aplikasi web visualisasi interaktif. Ini menyediakan bagan, grafik, dan peringatan untuk web saat terhubung ke sumber data yang didukung.

Grafana merupakan aplikasi open-source untuk memonitor dan menganalisa metrics. Kita menggunakan Grafana untuk memvisualisasikan metrics menjadi grafik-grafik yang menarik untuk dilihat dan mudah dimengerti. Grafana memiliki banyak fitur yang powerful untuk memonitor dan menganalisa. Grafana juga memiliki fitur alerting yang sangat berguna. Feature ini telah banyak digunakan oleh ribuan perusahaan.

Salah satu cara termudah untuk mengeksplore grafa pada komputer lokal adalah dengan menginstal grafana dengan docker, pastikan kamu telah menginstal docker pada komputer yang kamu gunakan.

Gunakan ini untuk menjalankan Grafana dengan docker. Kalau ingin menggunakan metode lain, bisa lihat di https://grafana.com/get.
```go
docker run -d -p 3000:3000 grafana/grafana
```

Buka http://localhost:3000/ untuk masuk ke dashboard Grafana. Login dengan username default admin dan password admin. Setelah login, jangan lupa untuk ganti password. Kemudian kamu akan melihat halaman ini:

![Grafana](https://cms.halovina.com/wp-content/uploads/2021/05/grafana-dashboard.jpg)

### Kelebihan

- Open-source
- Dashboard dibuat di sisi client
- Pengaturannya sederhana, tidak memerlukan server HTTP
- Plugin Grafana merender data secara real-time

### Kekurangan

- Tidak support log analysis
- Customization fungsi lebih sedikit
- Organisasi dasbornya terbatas dan dokumentasinya tidak sesuai standar

### Referensi

- [Mengenal Grafana Aplikasi Web](https://halovina.com/mengenal-grafana-aplikasi-web-visualisasi-interaktif/)
- [Gravana vs Kibana](https://www.geeksforgeeks.org/grafana-vs-kibana/)