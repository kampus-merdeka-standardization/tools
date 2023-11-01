# Dependency Manager

## Node Package Manager (NPM)

NPM adalah registri perangkat lunak terbesar di dunia. Di dalamnya terdapat lebih dari 800.000 package yang siap digunakan. 
NPM mengelola package Javascript untuk menginstal modul, berbagi dependensi, dan berbagi tool. Dengan jumlah package yang 
banyak tersebut, seorang developer dapat terbantu terutama dalam soal waktu pembuatan aplikasi.

### Cara Kerja NPM

NPM memiliki 2 fungsi dalam kerja pemrograman. Berikut merupakan 2 fungsi dari package manager ini:
1. Sebagai repositori online: berfungsi untuk menerbitkan project open source Node.js. Artinya, NPM menjadi wadah yang bisa 
digunakan para developer untuk mempublikasikan dan membagikan project Node.js mereka. 
2. Sebagai command line:  dapat digunakan oleh developer untuk menginstal dan mengunduh package, serta mengelola versi dan 
dependensi yang diperlukan saat proses pembuatan project.

Untuk bisa menggunakan NPM, kamu harus menginstal Node.js terlebih dahulu. Hal ini dikarenakan NPM dan Node.js berada dalam 
1 paket aplikasi, yaitu Node.js. Kamu bisa mendownloadnya di [Nodejs.org](https://nodejs.org/en).

### Command NPM

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

### Cara Install NPM

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

### Referensi
- [Apa Itu NPM (Node Package Manager)?](https://www.dewaweb.com/blog/apa-itu-npm/)

## Yarn

### Pendahuluan

Yarn adalah manajer paket yang cepat, andal, dan aman yang dapat digunakan untuk mengelola dependensi di proyek kode Anda. Ini dirancang untuk membantu pengembang mengelola dan mengautomasi pengelolaan dependensi perangkat lunak dengan efisien, sehingga memungkinkan fokus pada penulisan kode yang sebenarnya untuk aplikasi mereka. Yarn memastikan bahwa versi dependensi yang diinstal di lingkungan pengembangan lokal Anda sesuai dengan yang diinstal di lingkungan produksi, sehingga mengurangi "itu bekerja di mesin saya" masalah.

Beberapa alasan mengapa Yarn populer di kalangan pengembang antara lain:

- **Kecepatan**: Yarn menawarkan kecepatan instalasi paket yang lebih cepat dibandingkan dengan npm (Node Package Manager) karena mengoptimalkan proses pengunduhan dan mengurangi waktu tunggu.
- **Keandalan**: Dengan lockfile yang dihasilkan (yarn.lock), Yarn memastikan bahwa struktur node_modules dan versi paket yang diinstal adalah konsisten di semua lingkungan.
- **Keamanan**: Yarn memiliki mekanisme keamanan yang kuat untuk memastikan integritas paket yang diinstal, dan menawarkan resolusi konflik otomatis yang dapat membantu menghindari dependensi yang konflik atau cacat.
  
Yarn dikembangkan oleh Facebook, Google, Exponent, dan Tilde. Sejak peluncurannya, Yarn telah menjadi pilihan populer di kalangan pengembang karena peningkatan kinerja dan fitur-fitur andal yang ditawarkannya.

### Referensi:

- [npm vs Yarn: Which Package Manager Should You Choose?](https://www.keycdn.com/blog/npm-vs-yarn) 
- [Yarn vs npm - Best Package Manager 2021](https://buttercms.com/blog/yarn-vs-npm-best-package-manager-2021)
- [Yarn Package Manager: An Improvement over npm](https://auth0.com/blog/yarn-package-manager-an-improvement-over-npm/)
- [What is Yarn? Yarn vs Npm](https://www.educative.io/edpresso/what-is-yarn-yarn-vs-npm)

### Cara Kerja Yarn

Yarn adalah sebuah manajer dependensi yang cepat, dapat diandalkan, dan aman yang dirancang untuk menangani paket dependensi di proyek-proyek perangkat lunak. Berikut adalah beberapa aspek utama dari cara kerja Yarn:

1. **Mengelola Dependensi:**
   - Yarn memungkinkan pengembang untuk menginstal, mengupdate, dan menghapus dependensi proyek dengan mudah melalui command-line interface (CLI) yang sederhana.
   - Dependensi yang dideklarasikan dalam berkas `package.json` dan berkas kunci `yarn.lock` yang menjamin konsistensi dependensi di seluruh lingkungan dan tim pengembangan.

2. **Caching:**
   - Yarn mencache setiap paket yang telah diunduh, sehingga tidak perlu mengunduh paket yang sama lagi di masa mendatang. Ini berarti instalasi yang lebih cepat bahkan pada instalasi ulang atau di mesin lain yang memiliki cache yang sama.

3. **Resolusi Versi:**
   - Yarn memiliki algoritma resolusi yang kuat yang bekerja untuk menyelesaikan konflik versi dependensi dan memastikan versi yang benar dari setiap paket diinstal di proyek Anda.

4. **Integritas Proyek:**
   - Yarn menggunakan berkas kunci (`yarn.lock`) untuk mengunci versi dependensi proyek, memastikan bahwa setiap anggota tim memiliki konsistensi versi paket, terlepas dari kapan mereka menginstalnya.

5. **Keamanan:**
   - Yarn memiliki fitur untuk mengecek dan melaporkan kelemahan keamanan potensial dalam proyek Anda.

6. **Performa:**
   - Yarn dilakukan hampir semuanya secara bersamaan untuk memaksimalkan penggunaan sumber daya, yang berarti instalasi yang bahkan lebih cepat.

7. **Workspaces:**
   - Yarn mendukung workspaces yang memungkinkan pengembang untuk mengelola dependensi monorepo dengan lebih baik, memungkinkan sharing code dan dependensi antar proyek dengan lebih efisien.

8. **Plug 'n' Play (PnP):**
   - Yarn memperkenalkan konsep Plug 'n' Play yang menghilangkan tahap `node_modules` dan memungkinkan penggunaan langsung dependensi tanpa tahap instalasi tradisional.

### Referensi:

- [npm - Yarn](https://www.npmjs.com/package/yarn)
- [Official Yarn Documentation](https://yarnpkg.com/)
- [Wikipedia - Yarn (package manager)](https://en.wikipedia.org/wiki/Yarn_(package_manager))
- [State of JavaScript - Yarn](https://2022.stateofjs.com/en-US/technologies/package-managers/)
- [Yarn - Official Architecture Overview](https://yarnpkg.com/advanced/architecture)

#### Command Yarn
1. **Menambahkan Dependensi**: 
   - `yarn add [package]`: Perintah ini digunakan untuk menambahkan sebuah paket sebagai dependensi ke dalam proyek Anda.
   - `yarn add [package]@[version]`: Menambahkan versi spesifik dari sebuah paket.
   - `yarn add --dev [package]`: Menambahkan paket sebagai dependensi pengembangan.
   - `yarn add --peer [package]`: Menambahkan paket sebagai dependensi sejawat.
   - `yarn add --optional [package]`: Menambahkan paket sebagai dependensi opsional.

2. **Meningkatkan Versi Dependensi**:
   - `yarn upgrade [package]`: Meningkatkan versi paket ke versi terbaru.
   - `yarn upgrade [package]@[version]`: Meningkatkan versi paket ke versi spesifik.

3. **Menghapus Dependensi**:
   - `yarn remove [package]`: Menghapus paket dari daftar dependensi proyek Anda.

4. **Memasang Dependensi**:
   - `yarn install`: Memasang semua dependensi yang terdaftar di file `package.json`.

5. **Menjalankan Skrip**:
   - `yarn run [script]`: Menjalankan skrip yang ditentukan di file `package.json`.

6. **Inisialisasi Proyek Baru**:
   - `yarn init`: Membuat file `package.json` baru untuk proyek Anda.

7. **Mengecek Versi Yarn**:
   - `yarn --version`: Menampilkan versi Yarn yang saat ini terpasang.

8. **Mengunci Versi Dependensi**:
   - `yarn lock`: Membuat atau memperbarui file `yarn.lock` untuk mengunci versi dependensi.

9. **Menjalankan Server Lokal**:
   - `yarn start`: Menjalankan server lokal untuk proyek Anda.

10. **Membuat Build Produksi**:
    - `yarn build`: Membuat build produksi dari proyek Anda.

11. **Menjalankan Tes**:
    - `yarn test`: Menjalankan tes di proyek Anda.

12. **Menjalankan Pemeriksaan Format dan Lint**:
    - `yarn lint`: Menjalankan pemeriksaan format dan lint pada kode sumber proyek Anda.

Perintah-perintah di atas merupakan sebagian dari perintah yang tersedia di Yarn. Setiap perintah memiliki opsi dan flag tambahan yang dapat digunakan untuk mengatur perilakunya. Untuk informasi lebih lanjut tentang perintah Yarn, Anda dapat mengunjungi dokumentasi resmi Yarn.

### Referensi:
- [Yarn Commands (Official Documentation)](https://classic.yarnpkg.com/en/docs/cli/)
- [Yarn Command Cheat Sheet](https://devhints.io/yarn)
- [Managing dependencies with Yarn](https://classic.yarnpkg.com/en/docs/managing-dependencies/)

## Cara Install Yarn

Sebelum Anda mulai menggunakan Yarn, Anda perlu menginstalnya pada sistem Anda. Berikut ini adalah beberapa metode instalasi Yarn:

### Melalui npm (Node Package Manager)

Direkomendasikan untuk menginstal Yarn melalui npm yang merupakan bagian dari instalasi Node.js. Setelah Node.js dan npm terinstal, jalankan perintah berikut untuk menginstal dan memperbarui Yarn:

```bash
npm install --global yarn
```

### Melalui Paket Manager Sistem Operasi

Yarn juga dapat diinstal melalui manajer paket dari sistem operasi yang Anda gunakan. Berikut adalah beberapa contoh:

- Pada Alpine Linux (3.6+), gunakan perintah:
```bash
apk add yarn
```

- Pada sistem operasi berbasis Debian seperti Ubuntu, gunakan perintah:
```bash
sudo apt-get update && sudo apt-get install yarn
```

- Pada sistem operasi berbasis Red Hat seperti Fedora, gunakan perintah:
```bash
sudo dnf install yarn
```

### Melalui Skrip Instalasi

Yarn menyediakan skrip instalasi yang dapat dijalankan di terminal untuk menginstal Yarn pada sistem macOS dan Unix umum:

```bash
curl -o- -L https://yarnpkg.com/install.sh | bash
```

Untuk menginstal versi tertentu dari Yarn, gunakan perintah berikut dan gantikan `[version]` dengan nomor versi Yarn yang diinginkan:

```bash
curl -o- -L https://yarnpkg.com/install.sh | bash -s -- --version [version]
```

### Melalui Tarball

Yarn dapat diinstal dengan mengunduh tarball dan mengekstraknya di mana saja pada sistem Anda:

```bash
cd /opt
wget https://yarnpkg.com/latest.tar.gz
tar zvxf latest.tar.gz
# Yarn is now in /opt/yarn-[version]/
```

Sebelum mengekstrak Yarn, disarankan untuk memverifikasi tarball menggunakan GPG:

```bash
wget -qO- https://dl.yarnpkg.com/debian/pubkey.gpg | gpg --import
wget https://yarnpkg.com/latest.tar.gz.asc
gpg --verify latest.tar.gz.asc
# Look for "Good signature from 'Yarn Packaging'" in the output
```

### Konfigurasi Path

Jika Yarn tidak ditemukan dalam PATH Anda, ikuti langkah-langkah berikut untuk menambahkannya sehingga dapat dijalankan dari mana saja:

1. Tambahkan ini ke profil Anda: `export PATH="$PATH:/opt/yarn-[version]/bin"` (path mungkin berbeda tergantung di mana Anda mengekstrak Yarn)
2. Di terminal, log in dan log out untuk menerapkan perubahan

Untuk mengakses eksekutabel Yarn secara global, Anda perlu mengatur variabel lingkungan `PATH` di terminal Anda. Untuk melakukan ini, tambahkan `export PATH="$PATH:`yarn global bin`"` ke profil Anda, atau jika Anda menggunakan shell Fish, jalankan perintah `set -U fish_user_paths (yarn global bin) $fish_user_paths`.

### Referensi:
- [Dokumentasi Resmi Yarn](https://classic.yarnpkg.com/en/docs/install)
- [Panduan Instalasi Yarn di Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-20-04)
- [Panduan Instalasi Yarn di Linode](https://www.linode.com/docs/guides/how-to-install-yarn-on-ubuntu-and-debian/)
- [Panduan Instalasi Yarn di Hostinger](https://www.hostinger.com/tutorials/how-to-install-node-js-ubuntu)
- [Panduan Instalasi Yarn di Github](https://github.com/yarnpkg/yarn)


### Cara Install Yarn

Berikut adalah panduan untuk menginstal Yarn pada berbagai sistem operasi:

## Di Windows:
1. Unduh [installer Yarn](https://classic.yarnpkg.com/latest.msi).
2. Jalankan file yang telah diunduh dan ikuti petunjuk pada layar untuk menyelesaikan instalasi.

## Di macOS:
1. Gunakan Homebrew, sebuah manajer paket untuk sistem operasi macOS. Buka terminal dan ketik perintah berikut:
   ```bash
   brew install yarn
   ```
   Atau anda dapat mengunduh installer dari [situs resmi Yarn](https://classic.yarnpkg.com/en/docs/install/#mac-stable).

## Di Linux:
Untuk Linux, anda dapat melihat [dokumentasi resmi Yarn](https://classic.yarnpkg.com/en/docs/install/#debian-stable) untuk petunjuk instalasi pada distribusi Linux yang berbeda.

Mohon dicatat bahwa terdapat dua versi dari Yarn: Yarn Classic dan Yarn Berry. Link di atas adalah untuk Yarn Classic. Jika anda ingin menggunakan Yarn Berry, anda dapat mengikuti panduan instalasi dari [situs resmi Yarn Berry](https://yarnpkg.com/getting-started/install).

### Referensi:
- [Installasi Yarn di macOS](https://tecadmin.net/install-yarn-macos/)
- [Dokumentasi Resmi Yarn](https://classic.yarnpkg.com/en/docs/install)

## Composer

### Pendahuluan

Composer merupakan alat manajemen dependensi yang digunakan dalam pengembangan perangkat lunak PHP. Dengan Composer, pengembang dapat mendeklarasikan perpustakaan atau library yang diperlukan oleh proyek mereka, dan Composer akan mengatur (menginstal/memperbarui) perpustakaan tersebut untuk mereka. Ini membantu pengembang untuk mengelola perpustakaan dan paket yang diperlukan oleh aplikasi dengan lebih efisien dan terstruktur. Berikut adalah poin-poin penting mengenai Composer:

1. **Manajemen Dependensi**: Composer memungkinkan pengembang untuk mendeklarasikan dan mengelola dependensi atau perpustakaan yang diperlukan oleh proyek mereka dalam suatu format yang standar dan terstruktur.

2. **Instalasi dan Pembaruan Perpustakaan**: Composer menyederhanakan proses instalasi dan pembaruan perpustakaan dengan otomatis mengelola dependensi tersebut, sehingga pengembang tidak perlu melakukan proses ini secara manual.

3. **Komunitas PHP**: Composer dianggap sebagai manajer dependensi pilihan utama dalam komunitas PHP, membantu memudahkan penginstalan, pembaruan, dan penggunaan paket pihak ketiga. Paket-paket ini dapat dihosting oleh repositori publik maupun pribadi, dengan sebagian besar proyek populer mempublish ke Packagist, sebuah repositori paket PHP terkenal.

4. **Integrasi dengan Framework Modern**: Composer digunakan di hampir semua framework PHP modern seperti Symfony, CakePHP, dan Laravel. Ini merupakan alat yang sangat direkomendasikan untuk mengatasi masalah fundamental dalam banyak proyek web.

5. **Menyederhanakan Pengembangan**: Dengan menggunakan Composer, pengembang dapat fokus pada menulis kode untuk aplikasi mereka, sementara manajemen dependensi diurus oleh Composer, ini menciptakan proses pengembangan yang lebih efisien dan terorganisir.

Composer bukanlah manajer paket dalam arti yang sama seperti Yum atau Apt, namun lebih difokuskan pada manajemen dependensi pada level aplikasi. Hal ini sangat penting untuk memahami peran dan manfaat Composer dalam ekosistem pengembangan PHP.

### Referensi:
- [getcomposer.org - Introduction](https://getcomposer.org/doc/00-intro.md)
- [w3resource.com - A gentle introduction to composer as a dependency manager](https://www.w3resource.com/php/composer/a-gentle-introduction-to-composer-as-a-dependency-manager.php)
- [howtogeek.com - How to Install and Use Composer, PHP's Dependency Manager](https://www.howtogeek.com/662594/how-to-install-and-use-composer-phps-dependency-manager/)
- [udemy.com - Composer - The Ultimate Guide for PHP Dependency Management](https://www.udemy.com/course/composer-php-dependency-manager/)


## Cara Kerja Composer

1. **Definisi Dependensi**:
   - Semua dependensi proyek Anda didefinisikan dalam file `composer.json` yang terletak di direktori teratas proyek Anda.
   - Di dalam file `composer.json`, Anda perlu menentukan key `require` untuk mencantumkan paket-paket yang dibutuhkan oleh proyek Anda, bersama dengan versi yang diinginkan.

2. **Mencari dan Mengunduh Dependensi**:
   - Composer akan mencari paket-paket yang didefinisikan dalam file `composer.json` di repositori yang telah diatur.
   - Repositori default adalah Packagist.org, tetapi Anda juga dapat menentukan repositori lainnya.
   - Composer kemudian menggunakan informasi versi dari VCS (Sistem Kontrol Versi) paket untuk menemukan versi paket yang paling cocok dengan keterbatasan versi yang Anda tentukan dalam file `composer.json`.

3. **Menyelesaikan Dependensi**:
   - Composer menyelesaikan semua dependensi yang terdaftar dalam file `composer.json` dan menuliskan semua paket dan versi tepat mereka ke dalam file `composer.lock`.
   - Hal ini memastikan bahwa semua orang yang bekerja pada proyek ini terkunci pada versi dependensi yang sama.

4. **Menginstal Dependensi**:
   - Setelah dependensi diselesaikan, Composer kemudian mengunduh file-file dependensi ke dalam direktori `vendor` di proyek Anda.
   - Direktori `vendor` adalah lokasi konvensional untuk semua kode pihak ketiga dalam proyek.

5. **Penguncian Versi**:
   - File `composer.lock` memastikan bahwa semua pengembang dalam tim, server CI, mesin produksi, dll., menggunakan versi yang sama dari dependensi, yang mengurangi potensi bug yang mempengaruhi hanya beberapa bagian dari penyebaran.
   - Hal ini juga memungkinkan Anda untuk merasa percaya diri bahwa dependensi yang diinstal masih berfungsi bahkan jika banyak versi baru dari dependensi tersebut telah dirilis sejak file `composer.lock` dibuat.

6. **Pembaruan Dependensi**:
   - Untuk memperbarui dependensi, Anda dapat menjalankan perintah `update` yang akan menyelesaikan dependensi lagi dan memperbarui file `composer.lock` dengan versi terbaru yang sesuai dengan batasan versi dalam file `composer.json`.

Dengan demikian, Composer memudahkan pengelolaan dependensi dalam proyek PHP, memastikan konsistensi antar lingkungan, dan memudahkan integrasi dan pengujian kode.

Referensi:
- [Dokumentasi Resmi Composer](https://getcomposer.org/doc/01-basic-usage.md)

### Command Composer

#### 1. `composer init`

- Menginisialisasi paket Composer baru di direktori saat ini dan meminta detail paket seperti nama, deskripsi, penulis, dan dependensi.

#### 2. `composer install` atau `composer i`

- Mengunduh dan menginstal semua pustaka dan dependensi yang diuraikan dalam file composer.lock. Jika file tidak ada, akan mencari composer.json dan melakukan hal yang sama, sekaligus membuat file composer.lock.

#### 3. `composer update` atau `composer u` atau `composer upgrade`

- Memperbarui dependensi pustaka ke versi terbaru yang sesuai dengan batasan yang ditentukan dalam file composer.json.

#### 4. `composer require` atau `composer r`

- Menambahkan paket baru ke file composer.json dan mengunduhnya.

#### 5. `composer remove` atau `composer rm`

- Menghapus paket dari file composer.json dan juga menghapusnya dari direktori vendor.

#### 6. `composer dump-autoload` atau `composer dumpautoload`

- Mengoptimalkan muatan otomatis dengan meregenerasi file autoload yang diperlukan.

#### 7. `composer self-update` atau `composer selfupdate`

- Memperbarui Composer itu sendiri ke versi terbaru.

#### 8. `composer create-project`

- Membuat proyek baru berdasarkan paket yang ada.

#### 9. `composer validate`

- Memvalidasi file composer.json dan composer.lock.

#### 10. `composer run-script` atau `composer run`

- Menjalankan skrip yang ditentukan dalam file composer.json.

#### 11. `composer search`

- Mencari paket di Packagist yang sesuai dengan kata kunci yang diberikan.

#### 12. `composer show` atau `composer info`

- Menampilkan informasi tentang paket yang diinstal atau paket yang tersedia.

Dan masih banyak lagi perintah lainnya yang dapat Anda temukan dalam dokumentasi resmi Composer. Untuk melihat daftar lengkap perintah yang tersedia, Anda dapat menjalankan `composer` atau `composer list` di antarmuka baris perintah, kemudian `--help` dikombinasikan dengan salah satu dari perintah tersebut dapat memberikan informasi lebih lanjut. Sebagai tambahan, Composer menggunakan `symfony/console` sehingga Anda dapat memanggil perintah dengan nama singkat jika tidak ambigu.

Referensi:

- [DevOpsSchool - Composer User Guide & Commands](https://www.devopsschool.com/blog/what-is-composer-and-its-user-guide-commands/)
- [Devhints.io - Composer Cheatsheet](https://devhints.io/composer)
- [Thomas Venturini - The Most Common Composer Commands](https://thomasventurini.com/articles/the-most-common-composer-commands)
- [Composer - Command-line interface / Commands](https://getcomposer.org/doc/03-cli.md)


### Menginstall Composer

### 1. Menginstal Composer di Shared Hosting, Linux, atau macOS:

Langkah-langkah berikut digunakan untuk menginstal Composer di akun hosting bersama, Linux (PC atau sistem berbasis server), dan macOS:

1. Hubungkan ke akun hosting Anda menggunakan koneksi SSH (hanya berlaku untuk hosting bersama dan cloud). Jika tidak, buka jendela terminal di Linux atau macOS.
2. Unduh Composer dari situs web resmi dengan perintah berikut:
```bash
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
```
Pastikan PHP telah terinstal sebelumnya jika Anda menggunakan macOS atau Linux.

3. Verifikasi tanda tangan installer (SHA-384) untuk memastikan file installer tidak korup:
```bash
php -r "if (hash_file('sha384', 'composer-setup.php') === '55ce33d7678c5a611085589f1f3ddf8b3c52d662cd01d4ba75c0ee0459970c2200a51f492d557530c71c15d8dba01eae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
```
Ambil perintah SHA-384 terbaru dari [halaman unduhan Composer](https://getcomposer.org/download/).

4. Setelah verifikasi, instal Composer secara lokal atau global:
   - Instalasi Lokal:
   ```bash
   php composer-setup.php
   ```
   - Instalasi Global:
   ```bash
   php composer-setup.php --install-dir=/usr/local/bin --filename=composer
   ```
5. Setelah proses instalasi selesai, hapus installer:
```bash
php -r "unlink('composer-setup.php');"
```
6. Akhirnya, uji instalasi Composer:
```bash
composer
```

### 2. Menginstal Composer di Windows:

1. Instal PHP di komputer Anda. Kami merekomendasikan menggunakan [XAMPP](https://www.apachefriends.org/index.html) karena prosesnya sederhana dan dapat diselesaikan dalam beberapa menit.
2. Setelah XAMPP terinstal, unduh [versi terbaru Composer](https://getcomposer.org/download/).
3. Jalankan wizard setup Composer. Ketika ditanya untuk mengaktifkan mode pengembang, abaikan dan lanjutkan dengan installer.
4. Sebuah jendela akan muncul dan meminta Anda untuk menemukan baris perintah PHP. Lokasi default adalah `C:/xampp/php/php.exe`. Setelah lokasi dipilih, klik Next.
5. Anda akan diminta dengan jendela Pengaturan Proxy. Biarkan kotak tidak dicentang dan lewati bagian ini dengan menekan Next. Kemudian, pada jendela terakhir, klik Install.
6. Setelah menyelesaikan instalasi, buka Command Prompt. Tekan pintasan CTRL + R, dan ketik cmd. Klik OK.
7. Gunakan perintah berikut dan tekan Enter:
```bash
composer
```
Perintah di atas akan mengembalikan hasil berikut:
```plaintext
______
/ ____/___ ____ ___ ____ ____ ________ _____
/ / / __ / __ `__ / __ / __ / ___/ _ / ___/
/ /___/ /_/ / / / / / / /_/ / /_/ (__ ) __/ /
____/____/_/ /_/ /_/ .___/____/____/___/_/
/_/
Composer version 2.4.2 2022-09-14 16:11:15
```

Referensi:
- [Hostinger Guide](https://www.hostinger.com/tutorials/how-to-install-composer)

## Apache Maven 🪶🪶🪶

Salah satu _Build Automation Tool_ yang populer pada kalangan _developer_ Java adalah **Maven**. _Build Automation_ adalah proses otomatisasi pembangunan perangkat lunak yang bertujuan untuk mempermudah pengembang dalam mengelola dan mengotomatisasi tugas-tugas yang terkait dengan kompilasi, pengujian, dan distribusi kode sumber. Maven adalah salah satu alat (tool) yang digunakan dalam build automation di dunia pengembangan perangkat lunak, khususnya dalam proyek-proyek berbasis Java.

Ada opsi lain selain **Apache Maven**, seperti **Gradle**. Gradle sendiri populer untuk kalangan programmer bahasa **Kotlin**.

Untuk lebih lengkapnya, kita bisa langsung melihat pada dokumentasi-nya langsung pada tautan https://maven.apache.org/guides/getting-started/index.html

### Instalasi Maven [^](#)

- Maven dibuat menggunakan bahasa pemrograman java yang notabene-nya multiplatform, jadi segala jenis OS dapat menginstallnya pada tautan [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi)

- Seletah instalasi `zip` file, kemudian ekstrak pada direktori yang kita inginkan

- Masukkan lokasi direktori kedalam environment variable dengan nama variable `MAVEN_HOME`

- Masukkan lokasi `bin` direktori dari maven ke dalam `Path` di dalam environment variable

- Kedua langkah diatas kurang lebih sama dengan cara menambahkan environment variable untuk java yang dapat dilihat pada laman [**<u>ini</u>**](/java-standardization/README.md#b-instalasi-jdk-)

- Pastikan dengan mencoba perintah
    ```
    mvn --version
    ```

    kalau berhasil akan muncul detail versi maven seperti

    ```
    Apache Maven 3.9.4 (dfbb324ad4a7c8fb0bf182e6d91b0ae20e3d2dd9)
    Maven home: C:\Program Files\Maven\apache-maven-3.9.4
    Java version: 17.0.2, vendor: Oracle Corporation, runtime: C:\Program Files\Java\jdk-17.0.2
    Default locale: en_US, platform encoding: Cp1252
    OS name: "windows 11", version: "10.0", arch: "amd64", family: "windows"
    ```
    versi mungkin berbeda sesuai yang kita install sebelumnya

### Membuat Project [^](#)
- Buka terminal pada direktori dimana project akan disimpan
- Ketik
    ```sh
    mvn archetype:generate
    ```
- Akan muncul berbagai template, kemudian carilah `maven-archetype-quickstart`
    ```
    Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): : maven-archetype-quickstart
    Choose archetype:
    1: remote -> com.github.ywchang:maven-archetype-quickstart (Provide up-to-date java quickstart archetype)
    2: remote -> com.haoxuer.maven.archetype:maven-archetype-quickstart (a simple maven archetype)
    3: remote -> org.apache.maven.archetypes:maven-archetype-quickstart (An archetype which contains a sample Maven project.)
    Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): 3:
    ```
    pilih nomor 3 dan enter

- Pilih versi
    ```
    Choose org.apache.maven.archetypes:maven-archetype-quickstart version:
    1: 1.0-alpha-1
    2: 1.0-alpha-2
    3: 1.0-alpha-3
    4: 1.0-alpha-4
    5: 1.0
    6: 1.1
    7: 1.3
    8: 1.4
    Choose a number: 8:
    ```
    default terpilih nomor 8, kita bisa tinggal tekan enter

- 
    ```
    Define value for property 'groupId':
    ```
    Tulislah nama untuk `groupId` sesuai yang kita inginkan.<br/>`groupId` biasanya merepresentasikan nama company. Misal kita isi dengan **company-name**

- 
    ```
    Define value for property 'artifactId':
    ```
    Tulislah nama untuk `artifactId` sesuai yang kita inginkan.<br/>`artifactId` merepresentasikan nama project kita. Misal kita isi dengan **demo-maven**

- 
    ```
    Define value for property 'version' 1.0-SNAPSHOT: :
    ```
    Tulislah versi aplikasi project kita. Default `1.0-SNAPSHOT`, kita bisa langsung enter bila ingin menggunakan default version.

- 
    ```
    Define value for property 'package' company-name: :
    ```
    Ini merupakan package pada main program kita. Biasanya penamaan package dinamai secara terbalik dari nama domain kita. Contoh, jika domain kita adalah **example.com**, maka package dapat dinamai **com.example.maven**.<br/>Misal kita isi dengan **com.example.maven**

- 
    ```
    Confirm properties configuration:
    groupId: company-name
    artifactId: demo-maven
    version: 1.0-SNAPSHOT
    package: com.example.maven
    Y: :
    ```
    Tekan `Y` (atau langsung enter, karena secara default sudah 'Y') jika detail yang diberikan sudah sesuai dengan apa yang kita isi 

- Project siap di gunakan

### Struktur Maven Project [^](#)
```
nama-project/
├── pom.xml
└── src/
    ├── main/
    |   └── java/
    |       └── com.example.app/
    |           └── App.java
    └── test/
        └── java/
            └── com.example.app/
                └── AppTest.java
```

##### Penjelasan Struktur kode di atas :
- `src.main.java.com.example.app` merupakan lokasi dimana kode program java ditempatkan

- `src.test.java.com.example.app` merupakan lokaasi dimana unit test program java ditempatkan

- `pom.xml` merupakan inti dari konfigurasi project Maven. Ini merupakan file konfigurasi yang berisi sebagian besar informasi yang diperlukan untuk membangun project sesuai yang kita inginkan.

### Maven Lifecycle [^](#)

- `validate`: validate the project is correct and all necessary information is available
- `clean`: Deleting the target folder (where the compilation results are stored)
- `compile`: compile the source code of the project
- `test`: test the compiled source code using a suitable unit testing framework. These tests should not require the code be packaged or deployed
- `package`: take the compiled code and package it in its distributable format, such as a JAR.
- `integration-test`: process and deploy the package if necessary into an environment where integration tests can be run
- `verify`: run any checks to verify the package is valid and meets quality criteria
- `install`: install the package into the local repository, for use as a dependency in other projects locally
- `deploy`: done in an integration or release environment, copies the final package to the remote repository for sharing with other developers and projects.
- untuk lebih lengkapnya, bisa dilihat pada dokumentasi nya langsung https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html

##### Cara menjalankan lifecycle :
Cara menjalankan lifecycle, cukup dengan menggunakan perintah `mvn namalifecycle`. Bisa juga lebih dari satu seperti `mvn clean test install`

### Dependency [^](#)
Dalam pembuatan aplikasi, sering kali kita butuh library dari luar untuk mendukung kemudahan kita dalam mengembangkan aplikasi. Tanpa Build Automation Tool seperti Apache Maven ini, akan banyak sekali yang harus dilakukan ketika kita ingin menambahkan library luar.

Untuk mencari dependency dari luar, kita bisa mencarinya pada :
- https://central.sonatype.com/
- https://mvnrepository.com/

Kemudian kita bisa menambahkan dependency yang kita butuhkan kedalam `pom.xml` pada bagian 
```xml
<dependencies>
    <!-- letakkan disini -->
</dependencies>
```

contoh : 
```xml
<dependencies>
    <dependency>
        <groupId>com.google.code.gson</groupId>
        <artifactId>gson</artifactId>
        <version>2.10.1</version>
    </dependency>
</dependencies>
```

### Repository [^](#)
Saat kita menambahkan dependency, maven akan mencari dependecy tersebut pada berbagai repository yang maven miliki. 

Terkadang kita ingin maven mencarinya pada repository yang kita inginkan, contoh repository pribadi atau milik perusahaan

untuk kita kita bisa menambahkannya pada bagian 
```xml
<repositories>
    <!-- letakkan disini -->
</repositories>
```

contoh :
```xml
<repositories>
    <repository>
        <id>id</id>
        <name>name</name>
        <url>url</url>
    </repository>
</repositories>
```

## Go Modules

Go modules meruapakan manajemen dependensi resmi untuk Go. Modules ini diperkenalkan pertama kali di `go1.11`, sebemum itu
pengembangan project Go dilakukan dalam `GOPATH`. Modules digunakan untuk menginisialisasi sebuah project, sekaligus melakukan
manajemen terhadap 3rd party atau library lain yang dipergunakan. Modules penggunaannya adalah lewat CLI. Dan jika teman-teman
sudah sukses meng-install Go, maka otomatis bisa mempergunakan Go Modules.

### Inisialisasi Project Menggunakan Go Modules

Command `go mod init` dingunakan untuk menginisialisasi project baru.
Skema penulisan command `go mod`:
```shell
go mod init <nama-project>
```
Untuk nama project, umumnya adalah simakan dengan nama direktori, tapi bisa saja sebenarnya menggunakan nama yang lain.
> Nama project dan nama module merupakan istilah yang sama

Eksekusi perintah `go mod init` menghasilkan satu buah file baru bernama `go.mod`. File ini digunakan oleh Go toolchain
untuk menandai bahwa folder di mana file tersebut berada adalah folder project.

Cukup itu saja cara inisialisasi project di Go. Sebenarnya selain Go Modules, setup project di Go juga bisa menggunakan
`$GOPATH`. Tapi inisialisasi project dengan GOPATH sudah outdate dan kurang dianjurkan untuk project-project yang dikembangkan
menggunakan Go versi terbaru (1.14 ke atas).