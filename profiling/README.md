# Profiling

## JProfiler

Referensi : [JProfiler Help - Introduction](https://www.ej-technologies.com/resources/jprofiler/help/doc/main/introduction.html)

JProfiler adalah alat profesional untuk menganalisis apa yang terjadi di dalam JVM yang sedang berjalan. Ini adalah alat profil Java terkemuka untuk pemrofilan di JVM. Antarmuka pengguna JProfiler yang intuitif membantu Anda menyelesaikan bottleneck kinerja, menemukan kebocoran memori, dan memahami masalah threading.

Berikut adalah beberapa fitur utama dari JProfiler:
- **Kemudahan penggunaan luar biasa**: Mengkonfigurasi sesi adalah hal yang mudah, integrasi pihak ketiga membuat memulai menjadi mudah dan data profil disajikan dengan cara yang alami.
- **Profil basis data untuk JDBC, JPA dan NoSQL**: Panggilan basis data adalah alasan utama masalah kinerja dalam aplikasi bisnis. Probe JDBC dan JPA/Hibernate JProfiler serta probe NoSQL untuk MongoDB, Cassandra dan HBase menunjukkan alasan akses basis data yang lambat dan bagaimana pernyataan lambat dipanggil oleh kode Anda.
- **Profil remote tanpa konfigurasi**: Melakukan profil pada JVM yang berjalan di mesin remote tidak pernah semudah ini dengan JProfiler. Fungsionalitas terowongan SSH bawaan menghubungkan Anda ke mesin bahkan melalui beberapa lompatan dan kemudian JProfiler mengurus sisanya.
- **Dukungan bawaan untuk Docker dan Kubernetes**: Dengan JProfiler, Anda dapat melakukan profil pada JVM yang berjalan di dalam wadah Docker atau Kubernetes tanpa konfigurasi apa pun di dalam wadah.
- **Dukungan luar biasa untuk Kerangka Kerja Java Enterprise**: Dukungan khusus untuk JEE dan Spring hadir dalam sebagian besar tampilan di JProfiler.

### Instalasi
Kita dapat menginstal JProfiler dpada situs https://www.ej-technologies.com/products/jprofiler/overview.html

JProfiler juga tersedia sebagai plugin untuk Intellij Idea https://plugins.jetbrains.com/plugin/253-jprofiler

## pprof

pprof adalah *tool* untuk membuat *profiling* program Go. Ini adalah *standard library* Go dan dapat digunakan untuk menghasilkan profil rinci program Go, termasuk profil CPU, memori, dan konkurensi.

### Penggunaan

Untuk menggunakan pprof pada aplikasi golang, perlu import `net/http/pprof` dan buat handlers untuk profiling. Kalau aplikasimu adalah web server dan menggunakan HTTP server default, kita bisa tinggal import library nya dengan blank identifier, seperti di bawah ini:

```go
import _ net/http/pprof
```

Tapi kemungkinan besar tidak menggunakan HTTP server default. Kalau begitu perlu membuat handlers berikut:

```go
    r.HandleFunc("/debug/pprof/", pprof.Index)
    r.HandleFunc("/debug/pprof/heap", pprof.Index)
    r.HandleFunc("/debug/pprof/cmdline", pprof.Cmdline)
    r.HandleFunc("/debug/pprof/profile", pprof.Profile)
    r.HandleFunc("/debug/pprof/symbol", pprof.Symbol)
    r.HandleFunc("/debug/pprof/trace", pprof.Trace)
```

Untuk mengetestnya, kita buat handler yang mengambil data dari database, hit third-party API, kemudian melakukan kalkulasi yang memakan banyak CPU.
Lalu kita hit server secara terus menerus selama 5 menit sambil melakukan profiling. Untuk melakukan profiling, kita memanggil API `/debug/pprof/profile` dan menentukan berapa lama profiling berjalan pada parameter `seconds`, kemudian simpan hasilnya pada sebuah file. Berikut ini adalah command untuk melakukan profiling dengan curl:
```go
curl --output myappprofile "localhost:4560/debug/pprof/profile?seconds=300"
```
Tunggu sampai profiling selesai kemudian kita bisa analisa hasilnya.

Setelah kita dapatkan file hasil pprof, kita dapat menganalisanya menggunakan go tool pprof. Kita dapat menganalisanya dengan command line interaktif atau dengan web interface.
Untuk membukanya dalam command line interaktif:

```go
go tool pprof myappprofile
```

Kita dapat mengetik `help` untuk melihat command yang tersedia.
Salah satu command yang bisa kita gunakan adalah `top`. Ini untuk melihat fungsi yang paling banyak memakan resource.

Untuk menganalisa hasil pprof pada web interface, gunakan command berikut:

```go
go tool pprof -http localhost:3435 myappprofile
```

Parameter `localhost:3435` adalah alamat untuk mengakses web interface nya. Kita dapat mengubahnya sesuai keinginan. Sekarang coba buka alamat tersebut di web browser.

### Referensi

- [Profiling Go App](https://www.jajaldoang.com/id/post/profiling-go-app-with-pprof/)
- [Golang Profiling](https://granulate.io/blog/golang-profiling-basics-quick-tutorial/)


## Node JS Profiler (`--prof`)

Cara termudah di Node.js untuk membuat profile application adalah dengan menggunakan profiler bawaan, yang mengumpulkan semua data dari fungsi-fungsi dan mencatatnya ke dalam sebuah file. Node.js mengimplementasikan hal ini dengan memperkenalkan flag--prof, yang berkomunikasi dengan profiler V8 dan kemudian mencatat datanya.

### Penggunaan Node.js inbuilt profiler

1. **Mengaktifkan Profiler**:
   Pertama-tama, Anda perlu mengaktifkan profiler saat memulai aplikasi Node.js Anda. Anda dapat melakukannya dengan menggunakan flag `--prof` saat memulai aplikasi Anda:
   ```bash
   node --prof app.js
   ```

2. **Mengumpulkan Data Profil**:
   Setelah Anda mengaktifkan profiler, Node.js akan mengumpulkan data profil selama aplikasi Anda berjalan. Data ini akan disimpan dalam file log dengan ekstensi `.log` yang akan dibuat di direktori saat ini.

3. **Menghasilkan Laporan Profil**:
   Setelah Anda mengumpulkan data profil, Anda dapat menghasilkan laporan profil dengan menggunakan perintah `node --prof-process`. Ini akan mengambil file log profil yang telah Anda kumpulkan dan menghasilkan laporan yang dapat dibaca manusia:
   ```bash
   node --prof-process isolate-0xnnnnnnnnnnnn-v8.log > profile.txt
   ```

4. **Menganalisis Laporan Profil**:
   Buka file `profile.txt` dalam editor teks dan analisis laporan untuk menemukan area aplikasi Anda yang mungkin membutuhkan optimalisasi.

5. **Optimalisasi**:
   Gunakan informasi dari laporan profil untuk mengidentifikasi dan mengoptimalkan bagian kode yang lambat atau tidak efisien.
