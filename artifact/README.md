# Artifact

## JFrog Artifactory

JFrog Artifactory adalah solusi DevOps universal yang menyediakan otomatisasi dan manajemen end-to-end dari binari dan artefak 
melalui proses pengiriman aplikasi yang meningkatkan produktivitas dalam ekosistem pengembangan Anda.

Ini memungkinkan kebebasan pilihan dengan mendukung lebih dari 25 paket perangkat lunak, semua platform CI/CD utama, dan 
alat-alat DevOps yang sudah Anda gunakan. Artifactory siap untuk Kubernetes dengan mendukung kontainer, Docker, Helm Charts, 
dan menjadi registri Kubernetes dan Docker Anda, serta dilengkapi dengan CLI penuh dan API REST yang dapat disesuaikan dengan 
ekosistem Anda.

### Main Features and Functionality

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

### Referensi

- [JFrog Artifactory Documentation](https://jfrog.com/help/r/jfrog-artifactory-documentation/jfrog-artifactory)

## AWS CodeArtifact

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

### How does CodeArtifact work?

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

### Referensi

- [User Guide AWS CodeArtifact](https://docs.aws.amazon.com/codeartifact/latest/ug/welcome.html)

## Docker Hub

Docker Hub adalah layanan yang disediakan oleh Docker untuk menemukan dan berbagi citra kontainer.

Docker Hub merupakan repositori _image_ _container_ terbesar di dunia dengan berbagai sumber konten termasuk pengembang komunitas _container_, proyek _open source_, dan _independent software vendors_[ISV] yang membangun dan mendistribusikan kode mereka dalam kontainer.

### Tugas apa saja yang bisa dilakukan di Docker Hub ?
1. [Membuat dan mengelola tim dan organisasi](https://docs.docker.com/docker-hub/orgs/)
2. [Membuat perusahaan](https://docs.docker.com/docker-hub/creating-companies/)
3. [Menerapkan proses masuk [_sign in_]](https://docs.docker.com/docker-hub/configure-sign-in/)
4. Menyiapkan [SSO](https://docs.docker.com/single-sign-on/) dan [SCIM](https://docs.docker.com/docker-hub/scim/)
5. Gunakan [pemetaan Grup](https://docs.docker.com/docker-hub/group-mapping/)
6. [Melaksanakan audit domain](https://docs.docker.com/docker-hub/domain-audit/)
7. [Gunakan Manajemen Akses _Image_](https://docs.docker.com/docker-hub/image-access-management/) untuk mengontrol akses pengembang ke jenis gambar tertentu
8. [Mengaktifkan Manajemen Akses Registri](https://docs.docker.com/desktop/hardened-desktop/registry-access-management/)

## Perbandingan

| Komponen        | JFrog | AWS CodeArtifact | Docker Hub |
|-----------------|-------|------------------|------------|
| Maintenance     | 4     | 4                | 4          |
| Reputable       | 4     | 4                | 4          |
| Compatibility   | 4     | 4                | 4          |
| Community       | 4     | 3                | 3          |
| Documentation   | 4     | 4                | 3          |
| Licensing       | 4     | 3                | 4          |
| Extensible      | 3     | 3                | 4          |
| Size            | 4     | 4                | 4          |
| **Total Score** | 31    | 29               | 30         |