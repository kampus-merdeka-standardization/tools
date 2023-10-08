# Tools Documentation

## Repo

## Artifact

### JFrog Artifactory

JFrog Artifactory adalah solusi DevOps universal yang menyediakan otomatisasi dan manajemen end-to-end dari binari dan artefak 
melalui proses pengiriman aplikasi yang meningkatkan produktivitas dalam ekosistem pengembangan Anda.

Ini memungkinkan kebebasan pilihan dengan mendukung lebih dari 25 paket perangkat lunak, semua platform CI/CD utama, dan 
alat-alat DevOps yang sudah Anda gunakan. Artifactory siap untuk Kubernetes dengan mendukung kontainer, Docker, Helm Charts, 
dan menjadi registri Kubernetes dan Docker Anda, serta dilengkapi dengan CLI penuh dan API REST yang dapat disesuaikan dengan 
ekosistem Anda.

#### Main Features and Functionality

- **Lingkungan Hibrid dan Multi-Cloud**: Anda dapat meng-host Artifactory di infrastruktur Anda sendiri, di Cloud, atau menggunakan 
solusi SaaS untuk fleksibilitas dan pilihan maksimum. 


- **Manajemen Repositori Binari Universal**: Artifactory menawarkan solusi universal yang mendukung semua format paket utama, 
termasuk Alpine, Maven, Gradle, Docker, Cargo, Conda, Conan, Debian, Go, Helm, Vagrant, YUM, P2, Ivy, NuGet, PHP, NPM, RubyGems, 
PyPI, Bower, CocoaPods, GitLFS, Opkg, SBT, Swift, Terraform, dan lainnya. 


- **Metadata yang Luas**: Artifactory menyediakan metadata lengkap untuk semua format paket utama baik untuk artefak maupun 
folder. Ini termasuk metadata yang berasal dari paket itu sendiri, metadata kustom yang ditambahkan oleh pengguna seperti 
properti yang dapat dicari, dan metadata yang dihasilkan secara otomatis oleh alat-alat seperti informasi build dan lainnya. 


- **Artifactory sebagai Registri Kubernetes Anda**: Artifactory memungkinkan Anda untuk mendeploy mikro layanan berkontainer 
ke klaster Kubernetes karena ia berfungsi sebagai manajer repositori universal untuk semua kebutuhan CI/CD Anda, tidak peduli 
di mana mereka berjalan di organisasi Anda. 


- **Skalabilitas Besar**: Mendukung berbagai kemampuan penyimpanan skala enterprise termasuk S3 Object Storage, Google Cloud 
Storage, Azure Blob Storage, dan Filestore Sharding, memberikan skalabilitas tak terbatas, pemulihan bencana, dan stabilitas 
dan keandalan yang tak tertandingi. 


- **Replikasi**: Kemampuan replikasi unik dari Artifactory memastikan lokalitas dalam topologi jaringan apa pun dan untuk 
metodologi pengembangan apa pun. 


- **Ketersediaan Tinggi**: Solusi HA aktif/aktif penuh dengan failover langsung dan upgrade produksi tanpa gangguan. 


- **Integrasi CI Server Lanjutan dengan Alat Build**: JFrog Artifactory mendukung integrasi build, baik Anda menjalankan 
build di salah satu server CI umum yang digunakan saat ini, di server CI berbasis cloud, atau mandiri tanpa server CI.


- **Automasi Berbasis API Kustom**: Artifactory mengekspos API REST yang luas yang memberikan akses ke fitur-fiturnya di 
seluruh siklus pengembangan.


- **Pencarian Lanjutan dengan Bahasa Kueri Artifactory**: AQL (Artifactory Query Language) memberikan fleksibilitas tak 
terbatas dalam pencarian artefak.


- **Artifactory Cloud dengan Distribusi CDN**: JFrog Artifactory Cloud dengan solusi CDN CloudFront dari Amazon memungkinkan 
pengguna Enterprise untuk mengelola, mengendalikan, dan mendistribusikan volume tinggi distribusi perangkat lunak melintasi 
lokasi yang berbeda. Solusi CDN terintegrasi sepenuhnya menghilangkan kebutuhan untuk menangani kompleksitas mengatur sistem 
CDN Caching eksternal terpisah.

#### Referensi

- [JFrog Artifactory Documentation](https://jfrog.com/help/r/jfrog-artifactory-documentation/jfrog-artifactory)

### AWS CodeArtifact

AWS CodeArtifact adalah layanan penyimpanan artefak yang aman, sangat dapat diskalakan, dan dikelola yang membantu organisasi 
menyimpan dan berbagi paket perangkat lunak untuk pengembangan aplikasi. Anda dapat menggunakan CodeArtifact dengan alat-alat 
build dan manajer paket populer seperti NuGet CLI, Maven, Gradle, npm, yarn, pip, dan twine. CodeArtifact membantu mengurangi 
kebutuhan Anda untuk mengelola sistem penyimpanan artefak sendiri atau khawatir tentang skalabilitas infrastrukturnya. Tidak 
ada batasan pada jumlah atau ukuran total paket yang dapat Anda simpan di repositori CodeArtifact.

Anda dapat membuat koneksi antara repositori CodeArtifact pribadi Anda dengan repositori publik eksternal, seperti npmjs.com 
atau Maven Central. CodeArtifact akan mengambil dan menyimpan paket secara on-demand dari repositori publik ketika mereka 
diminta oleh manajer paket. Hal ini membuatnya lebih nyaman untuk mengonsumsi dependensi open-source yang digunakan oleh 
aplikasi Anda dan membantu memastikan bahwa mereka selalu tersedia untuk build dan pengembangan. Anda juga dapat menerbitkan 
paket-paket pribadi ke repositori CodeArtifact. Ini membantu Anda berbagi komponen perangkat lunak properti antara beberapa 
aplikasi dan tim pengembangan dalam organisasi Anda.

#### How does CodeArtifact work?

CodeArtifact menyimpan paket perangkat lunak dalam repositori. Repositori bersifat poliglot—satu repositori dapat berisi 
paket-paket dari jenis yang didukung apa pun. Setiap repositori CodeArtifact adalah anggota dari satu domain CodeArtifact. 
Kami merekomendasikan agar Anda menggunakan satu domain produksi untuk organisasi Anda dengan satu atau lebih repositori. 
Sebagai contoh, Anda mungkin menggunakan setiap repositori untuk tim pengembangan yang berbeda. Paket-paket dalam repositori 
Anda kemudian dapat ditemukan dan dibagikan di seluruh tim pengembangan Anda.

Untuk menambahkan paket ke repositori, konfigurasikan manajer paket seperti npm atau Maven untuk menggunakan endpoint (URL) 
repositori. Anda kemudian dapat menggunakan manajer paket tersebut untuk menerbitkan paket ke repositori. Anda juga dapat 
mengimpor paket open-source ke dalam repositori dengan mengkonfigurasikannya dengan koneksi eksternal ke repositori publik 
seperti npmjs, NuGet Gallery, Maven Central, atau PyPI.

Anda dapat membuat paket-paket dalam satu repositori tersedia untuk repositori lain dalam domain yang sama. Untuk melakukannya, 
konfigurasikan satu repositori sebagai upstream dari yang lain. Semua versi paket yang tersedia untuk repositori upstream 
juga tersedia untuk repositori downstream. Selain itu, semua paket yang tersedia untuk repositori upstream melalui koneksi 
eksternal ke repositori publik juga tersedia untuk repositori downstream.

#### Referensi

- [User Guide AWS CodeArtifact](https://docs.aws.amazon.com/codeartifact/latest/ug/welcome.html)

## Dependency Manager

### Node Package Manager (NPM)

NPM adalah registri perangkat lunak terbesar di dunia. Di dalamnya terdapat lebih dari 800.000 package yang siap digunakan. 
NPM mengelola package Javascript untuk menginstal modul, berbagi dependensi, dan berbagi tool. Dengan jumlah package yang 
banyak tersebut, seorang developer dapat terbantu terutama dalam soal waktu pembuatan aplikasi.

#### Cara Kerja NPM

NPM memiliki 2 fungsi dalam kerja pemrograman. Berikut merupakan 2 fungsi dari package manager ini:
1. Sebagai repositori online: berfungsi untuk menerbitkan project open source Node.js. Artinya, NPM menjadi wadah yang bisa 
digunakan para developer untuk mempublikasikan dan membagikan project Node.js mereka. 
2. Sebagai command line:  dapat digunakan oleh developer untuk menginstal dan mengunduh package, serta mengelola versi dan 
dependensi yang diperlukan saat proses pembuatan project.

Untuk bisa menggunakan NPM, kamu harus menginstal Node.js terlebih dahulu. Hal ini dikarenakan NPM dan Node.js berada dalam 
1 paket aplikasi, yaitu Node.js. Kamu bisa mendownloadnya di [Nodejs.org](https://nodejs.org/en).

#### Command NPM

- **npm init**

Perintah yang paling sering digunakan dalam penggunaan NPM adalah npm init. Perintah ini berfungsi untuk menginisialisasi 
project. Cara menggunakannya pun cukup mudah, cukup mengetikan npm init, kemudian tekan **Enter**.

Diharuskan menjawab beberapa pertanyaan terkait project. Berikut beberapa pertanyaan yang ada pada proses inisialisasi:
- Nama project 
- Versi project 
- Deskripsi project 
- Entry point (File utama dalam project, secara default adalah index.js)
- Test command (Perintah untuk uji coba)
- Repositori git 
- Keywords (Kata kunci, seperti hastag)
- Lisensi project

Jika menginginkan pengaturan default saat inisialisasi project, bisa tekan **Enter** untuk melewati setiap pertanyaan 
di atas. Setelah selesai, akan melihat file baru di folder project dengan nama package.json.

- **npm init – –yes**

Jika ingin menginisialisasi project tetapi tidak ingin mengisi data-data project seperti nama, versi, dan lain-lain. Gunakan 
perintah npm init – – yes. Dengan menggunakan parameter – – yes, semua pertanyaan inisialisasi akan terisi secara otomatis.

- **npm install**

Untuk menginstall package (module), gunakan perintah **npm install <module>**. Ganti kata **<module>** dengan nama package 
yang ingin diinstall. Setelah menjalankan perintah **npm install**, folder node_module akan terbuat secara otomatis. Dan 
semua package yang kamu install akan masuk ke folder tersebut. Package yang diinstall juga akan terdaftar pada file package.json 
sebagai dependencies.

#### Cara Install NPM

Untuk dapat menjalankan perintah npm, diharuskan menginstall Node.js terlebih dahulu. Berikut ini cara install NPM di Windows 
dan Mac.

- **Cara install NPM di Windows**

Untuk install NPM di Windows, harus download terlebih dahulu Node.js di [nodejs.org](https://nodejs.org/en).

![npm-download](https://dwblog-ecdf.kxcdn.com/wp-content/uploads/2022/04/download-npm-windows.png)

Jika belum familiar dengan Node.js, anda bisa memilih versi yang recomended. Setelah selesai download aplikasi Node.js, 
silahkan langsung install di PC. Untuk pilihan pada saat instalasi Node.js, silahkan pilih default semua dengan cara klik 
next sampai selesai.

Cek hasil instalasi NPM dengan cara buka command prompt, kemudian ketik **npm –v** dan klik **Enter**. Jika instalasi sudah 
berhasil, maka akan muncul angka pada command prompt. Angka tersebut adalah versi dari NPM yang sudah terinstall.

- **Cara install NPM di Mac**

Buat pengguna Mac, silahkan download terlebih dahulu aplikasinya di [nodejs.org](https://nodejs.org/en/download). Pilih macOS Installer, selanjutnya ikuti 
perintah yang ada sampai selesai.

![npm-download](https://dwblog-ecdf.kxcdn.com/wp-content/uploads/2022/04/download-npm-mac-1024x749.png)

#### Referensi
- [Apa Itu NPM (Node Package Manager)?](https://www.dewaweb.com/blog/apa-itu-npm/)
