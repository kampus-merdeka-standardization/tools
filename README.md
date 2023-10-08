# Tools Documentation

## Repo

## Artifact

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
