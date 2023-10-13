# Repo

## GitHub
GitHub adalah platform populer untuk pengembangan perangkat lunak yang memungkinkan pengguna untuk menyimpan kode pada penyimpanan berbasis cloud, melacak setiap perubahan yang ada pada kode, dan berkolaborasi dalam proyek. GitHub memungkinkan pengguna untuk mengunggah file dan membuat repository sendiri atau bergabung dengan repository proyek open source. Repository ini seperti sebuah folder pada komputer, namun memerlukan izin akses dari pemiliknya untuk dapat membuka, mengedit, atau menghapus setiap file yang ada pada dalamnya. GitHub juga berguna untuk menambah relasi atau jaringan, berkolaborasi, dan mempromosikan pekerjaan para pengembang. GitHub telah memperoleh jutaan pengguna dan menjadi platform go-to untuk proyek perangkat lunak yang kolaboratif sejak berdiri pada tahun 2008.

## Gitlab
### Pengertian GitLab

GitLab adalah solusi hosting Git populer dan open source yang diimplementasikan oleh lebih dari 50.000 organisasi. Selama beberapa tahun terakhir, GitLab telah berkembang dengan dukungan komunitas yang kuat, mampu menangani ribuan pengguna pada server tunggal dan beberapa server dalam kluster aktif. GitLab juga didefinisikan sebagai repositori kode open source dan platform pengembangan perangkat lunak kolaboratif untuk proyek DevOps dan DevSecOps besar. GitLab menawarkan lokasi untuk penyimpanan kode online dan kemampuan untuk pelacakan masalah dan integrasi Continuous Integration/Continuous Deployment (CI/CD).

### Kegunaan GitLab

GitLab membantu tim pengembangan dan pengembang dalam menangani seluruh siklus hidup aplikasi mereka secara menyeluruh. Ini memungkinkan penyebaran aplikasi ke berbagai jenis lingkungan, melindungi proses build dan sumber kode aplikasi dari ancaman keamanan. Beberapa fitur utama dari GitLab mencakup pipa CI/CD yang kuat, registry bawaan yang dapat diimplementasikan secara instan tanpa konfigurasi, integrasi sempurna dengan Kubernetes, dan kemampuan untuk mengimpor proyek besar serta mengekspor kode lain dalam proyek.

### Kelebihan dan Kekurangan GitLab

- **Kelebihan**:
  - Mudah diatur.
  - Antarmuka pengguna dan alat yang ramah pengguna.
  - Memungkinkan sejumlah tak terbatas repositori pribadi gratis.
  - Dapat mengintegrasikan banyak API dan layanan pihak ketiga.
  - Uptime yang sangat dapat diandalkan.
- **Kekurangan**:
  - Antarmuka pengguna dapat sedikit rumit untuk ditinjau.
  - Alat ini memiliki beberapa bug yang dapat membuatnya sedikit ceroboh.

### Cara Menggunakan GitLab

1. **Inisialisasi Repositori**:
   - Saat repositori diinisialisasi, folder tertentu dibuat dengan beberapa direktori dan konfigurasi.
2. **Membuat File Notepad**:
   - Buat file notepad untuk repositori dengan menggunakan perintah `touch input.txt` dan `notepad input.txt`.
3. **Menyimpan dan Menutup Notepad**:
   - Ketik apa saja di dalam notepad, lalu simpan dan tutup.
4. **Mengecek Status File**:
   - Gunakan perintah `git status` untuk memeriksa status file.
5. **Menambahkan File ke Area Staging**:
   - Gunakan perintah `git add.` untuk menambahkan file ke area staging.
6. **Commit File**:
   - Gunakan perintah `git commit -m "input"` untuk commit file.
7. **Mengecek Status File (lagi)**:
   - Gunakan perintah `git status` untuk memeriksa status file lagi.
8. **Mendorong Notepad ke Repositori GitLab**:
   - Pergi ke GitLab Anda dan salin perintah `git remote origin`, lalu kembali ke Git Bash dan tempel perintah tersebut.
   - Gunakan perintah `git remote -v`, diikuti oleh `git push -u origin master` untuk mendorong file ke repositori remote.
   - Sekarang periksa GitLab Anda untuk melihat apakah ada penambahan pada proyek baru yang awalnya Anda buat.



## Bitbucket

Bitbucket Cloud adalah hosting kode dan alat kolaborasi berbasis Git, yang dibuat untuk tim. Integrasi Jira dan Trello Bitbucket yang terbaik di kelasnya dirancang untuk menyatukan seluruh tim perangkat lunak untuk menjalankan sebuah proyek. Kami menyediakan satu tempat bagi tim Anda untuk berkolaborasi dalam kode dari konsep hingga Cloud, membangun kode berkualitas melalui pengujian otomatis, dan menerapkan kode dengan percaya diri.

##### Why Bitbucket ?
###### Features 
1. [CI/CD](https://bitbucket.org/product/features/pipelines)

   - Bitbucket Pipelines: Alat CI/CD yang terintegrasi dengan Bitbucket Cloud, yang memungkinkan tim untuk membangun, menguji, dan menyebarkan kode mereka di Bitbucket12.

   - Keunggulan Bitbucket Pipelines: Tidak perlu mengatur server, menyinkronkan repositori, atau mengonfigurasi manajemen pengguna. Cukup gunakan template berbasis bahasa untuk membuat konfigurasi CI/CD dalam dua langkah.
   - Fitur Bitbucket Pipelines: Dukungan untuk berbagai bahasa dan platform, konfigurasi sebagai kode dengan file bitbucket-pipelines.yml, penyesuaian dengan struktur cabang, integrasi dengan Jira dan Confluence, dan penggunaan Bitbucket Pipes untuk membuat alur kerja otomatis yang kuat.

   - Model harga Bitbucket Pipelines: Berdasarkan penggunaan, dengan konkurensi tak terbatas. Memberikan visibilitas yang tak tertandingi ke status build dan deployment di dalam Bitbucket dan Jira.

2. [Cloud Security](https://bitbucket.org/product/cloud-security)

   - **Keamanan data di Atlassian Cloud**: data aman di Atlassian Cloud, yang mencakup pengaturan keamanan seperti IP yang ditentukan sebelumnya, autentikasi dua faktor, dan kunci keamanan FIDO U2F.

   - **Koneksi SAML SSO**: dapat menambahkan Atlassian Access untuk menghubungkan produk cloud Anda dengan penyedia SAML SSO Anda.

   - **Enkripsi data**: menjamin bahwa repositori Anda dienkripsi saat diam (AES-256) dan saat transit (TLS 1.2+), sehingga kode Anda selalu aman.

   - **Standar kepercayaan**: komitmen Atlassian untuk memberikan tingkat tertinggi keamanan, keandalan, privasi, dan kepatuhan dalam produk-produknya. Halaman ini juga mengarahkan Anda ke Atlassian Trust Center, yang merupakan sumber informasi tentang semua kebutuhan keamanan Anda.

   - **Perlindungan GDPR**: Atlassian sepenuhnya berinvestasi dalam kesuksesan pelanggan dan perlindungan data. Menyediakan _Data Processing Addendum_ (DPA) yang telah ditandatangani sebelumnya, untuk membantu Anda memenuhi persyaratan transfer lanjutan di bawah GDPR.

   - **Program Bug Bounty**: Atlassian telah bermitra dengan Bugcrowd untuk memberi imbalan atas penelitian kerentanan yang unik. Anda dapat mengirimkan laporan melalui program Bug Bounty jika Anda menemukan kerentanan.

3. [DevSecOps](https://www.atlassian.com/software/bitbucket/features/devsecops)

   - **Keamanan pengembangan**: Membuat keamanan menjadi bagian dari siklus pengembangan Anda dengan menggunakan integrasi Snyk untuk Bitbucket Cloud.

   - **Pemindaian kode**: Memindai kode Anda saat di-push ke pull request, sehingga Anda dapat memperbaiki masalah secepatnya dan sepanjang proses review kode Anda.

   - **Laporan keamanan**: melihat laporan, anotasi, dan metrik keamanan di pull request Anda dengan menggunakan fitur code insights.

   - **Dasbor keamanan**: Mendapatkan visibilitas tentang keamanan repositori Anda dengan menggunakan dasbor khusus. Lihat insight keamanan dan jumlah total kerentanan di repositori ini, yang dikelompokkan berdasarkan skor risiko rendah, sedang, dan tinggi.

   - **Konfigurasi sederhana**: Memindai dependensi untuk kerentanan secara otomatis dengan menambahkan beberapa baris konfigurasi ke bitbucket-pipelines.yml Anda.

4. [Code Review](https://bitbucket.org/product/features/code-review)

   - **_Interface_ berbasis kode**: Sebuah antarmuka yang memungkinkan Anda menemukan bug lebih cepat, berkolaborasi dengan mudah, dan menggabungkan kode dengan percaya diri.

   - **Fitur-fitur baru**: Sebuah tampilan samping-samping yang diperbarui dengan fitur komentar kontekstual dan manajemen tugas membuat peninjauan diff besar lebih intuitif.

   - **Integrasi hasil tes dan pemindaian keamanan**: Hasil tes dan pemindaian keamanan diintegrasikan dalam tampilan permintaan tarik Anda, sehingga Anda mendapat peringatan tentang bug potensial sebelum Anda mengirimkan kode.

   - **Kondisi penggabungan**: Daftar kondisi untuk ditinjau oleh reviewer sebelum menyetujui, sehingga permintaan tarik secara konsisten diverifikasi sebelum digabungkan.

   - **Tampilan satu halaman**: Tidak ada tab dan tidak ada pergantian konteks. Semua yang perlu Anda ketahui ditampilkan di sebelah kanan kode di sidebar kanan.

   - **Rencana premium**: Rencana premium memungkinkan Anda menegakkan pemeriksaan penggabungan, yaitu, sampai kondisi penggabungan terpenuhi, PR tidak akan digabungkan.

   - **Konversi umpan balik menjadi tugas**: Ubah umpan balik Anda menjadi tugas yang dapat ditindaklanjuti dengan menangkap item tindak lanjut di daftar to-do.

   - **Navigasi pohon file**: Memiliki banyak perubahan di beberapa file? Navigasi pohon file Bitbucket Cloud memudahkan Anda menemukan apa yang Anda cari.

   - **Code Insights**: Code Insights, didukung oleh vendor DevOps terbaik, menampilkan hasil tes, pemindaian keamanan, dan lainnya langsung di tampilan permintaan tarik Anda1. Memperbaiki bug sebelum Anda mengirimkan kode berarti menghemat waktu untuk rapat insiden. Pelajari lebih lanjut

   - **Komentar dan diff dalam konteks kode**: Persempit lingkaran umpan balik antara pengirim dan peninjau dengan melihat komentar dan diff langsung dalam konteks kode. Kemudian, tetapkan tugas atau buat masalah Jira langsung dari dalam permintaan tarik Anda.

##### Integration
1. [Jira Integration](https://www.atlassian.com/software/jira/bitbucket-integration)

    Menghubungkan dan mengotomatisasi proses antara Bitbucket dan Jira, sehingga tim dapat melihat status pengembangan, kode, dan penyebaran dalam satu tempat. <br>
    beberapa fitur diantaranya :

    - Melihat dan membuat cabang dan _pull request_ dari panel pengembangan Jira
    - Melihat dan mengedit tiket Jira dari dalam UI Bitbucket
    - Membuat aturan otomatisasi berdasarkan pemicu seperti komit atau permintaan tarik
    - Melihat isu-isu Jira yang ditugaskan kepada Anda dari dalam Bitbucket
    - Membuat tiket Jira langsung dari dalam komentar permintaan tarik
    - Melihat dan berinteraksi dengan isu-isu Jira di tab isu-isu Jira di Bitbucket


2. [Atlassian Open DevOps](https://www.atlassian.com/solutions/devops)

    sebuah platform yang mengintegrasikan alat-alat Atlassian dan mitra untuk membangun dan mengoperasikan perangkat lunak dengan mudah. Tim dapat memilih alat-alat yang mereka inginkan atau membawa alat-alat yang sudah ada.

## Perbandingan

| Komponen        | Github | Gitlab | Bitbucket |
|-----------------|--------|--------|-----------|
| Maintenance     | 4      | 4      | 4         |
| Reputable       | 4      | 4      | 4         |
| Compatibility   | 4      | 4      | 4         |
| Community       | 4      | 4      | 3         |
| Documentation   | 4      | 4      | 3         |
| Licensing       | 4      | 4      | 4         |
| Extensible      | 3      | 3      | 4         |
| Size            | 3      | 4      | 4         |
| **Total Score** | 30     | 31     | 30        |