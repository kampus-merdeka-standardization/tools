# IDE

## VS Code

Visual Studio Code adalah kode editor yang ringan namun _powerful_ yang berjalan di desktop dan tersedia untuk Windows, 
macOS dan Linux. Muncul dengan dukungan bawaan untuk JavaScript, TypeScript dan Node.js dan memiliki ekosistem ekstensi yang 
kaya untuk bahasa dan runtime lain (seperti C++, C#, Java, Python, PHP, Go, .NET).

### Kelebihan

- Visual Studio Code menawarkan dukungan hebat untuk berbagai bahasa pemrograman, termasuk Java, Python, C++, JavaScript, 
dan banyak lagi.
- Visual Studio Code menawarkan banyak fitur yang menjadikannya editor kode yang hebat. Beberapa fitur utama mencakup integrasi 
Git, alat debugging, dan ekstensi yang memungkinkan Anda menyesuaikan alur kerja Anda.
- Visual Studio Code sangat dapat di-_customize_, memungkinkan Anda mengonfigurasi antarmuka dan pintasan keyboard sesuai 
keinginan Anda. Ini menjadikannya pilihan tepat bagi pengembang yang ingin menyesuaikan lingkungan pengkodean dengan kebutuhan 
spesifik mereka.
- Visual Studio Code memiliki komunitas _developer_ yang besar yang membuat dan memelihara ekstensi dan plugin yang menambahkan 
fungsionalitas baru ke editor.
- Visual Studio Code cepat dan efisien, dengan ukuran yang kecil. Ini menjadikannya pilihan tepat bagi pengembang yang menginginkan 
editor kode yang tidak memperlambat komputer mereka.

### Kekurangan

- Visual Studio Code bisa sangat membingungkan bagi pemula yang baru mengenal coding dan mungkin tidak memerlukan semua fitur 
yang ditawarkan.
- Visual Studio Code terkadang terasa memerlukan lebih banyak konfigurasi dibandingkan editor kode lainnya. Hal ini dapat 
menjadi kerugian bagi pengembang yang lebih memilih pengaturan yang lebih efisien
- Visual Studio Code bisa memakan banyak sumber daya, terutama saat menjalankan banyak ekstensi atau proyek yang lebih besar.

### Install

- #### **macOS**
1. [Download Visual Studio Code](https://go.microsoft.com/fwlink/?LinkID=534106)
2. Jika _archive_, ekstrak isi _archive_. Klik dua kali untuk beberapa browser atau pilih ikon 'kaca pembesar' dengan Safari.
3. Seret Visual Studio Code.app ke folder Aplikasi, sehingga tersedia di MacOS Launchpad.
4. Buka VS Code dari folder Aplikasi, dengan mengklik dua kali ikon tersebut.
5. Tambahkan VS Code ke Dock Anda dengan mengklik kanan ikon yang terletak di Dock, untuk membuka menu konteks dan memilih 
**Options**, **Keep in Dock**.

- #### Linux
  
  - Debian and Ubuntu based distributions 
    
    Cara termudah untuk menginstal Visual Studio Code untuk distribusi berbasis Debian/Ubuntu adalah mengunduh dan menginstal 
    paket [.deb (64-bit)](https://go.microsoft.com/fwlink/?LinkID=760868), atau melalui baris perintah dengan:
    ```shell
    sudo apt install ./<file>.deb
    
    # Jika Anda menggunakan distribusi Linux yang lebih lama, Anda harus menjalankan ini:
    # sudo dpkg -i <file>.deb
    # sudo apt-get install -f # Install dependencies
    ```
    
  - RHEL, Fedora, and CentOS based distributions

    Saat ini kami mengirimkan Kode VS 64-bit yang stabil dalam repositori yum, skrip berikut akan menginstal kunci dan repositori:
    ```shell
    sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
    sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
    ```
    Kemudian perbarui cache paket dan instal paket menggunakan `dnf` (Fedora 22 ke atas):
    ```shell
    dnf check-update
    sudo dnf install code # or code-insiders
    ```
    Atau pada versi lama menggunakan `yum`:
    ```shell
    yum check-update
    sudo yum install code # or code-insiders
    ```
  - openSUSE and SLE-based distributions

    Repositori yum di atas juga berfungsi untuk sistem berbasis openSUSE dan SLE, skrip berikut akan menginstal _key_ dan repositori:
    ```shell
    sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
    sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/vscode.repo'
    ```
    Kemudian perbarui cache paket dan instal paket menggunakan:
    ```shell
    sudo zypper refresh
    zypper install code
    ```

- #### Windows
1. Unduh [Visual Studio Code installer](https://go.microsoft.com/fwlink/?LinkID=534107) untuk Windows.
2. Setelah diunduh, jalankan penginstal (VSCodeUserSetup-{version}.exe). Ini hanya akan memakan waktu satu menit.
3. Secara default, VS Code diinstal di `C:\Users\{Username}\AppData\Local\Programs\Microsoft VS Code`.

Alternatifnya, Anda juga dapat mengunduh [Zip archive](https://code.visualstudio.com/docs/?dv=winzip), mengekstraknya, dan 
menjalankan Kode dari sana.

> **Tip**: _Setup_ akan menambahkan Visual Studio Code ke `%PATH%` Anda, jadi dari konsol Anda dapat mengetik 'code .' untuk 
> membuka VS Code pada folder itu. Anda perlu me-restart konsol Anda setelah instalasi agar perubahan pada variabel lingkungan 
> `%PATH%` dapat diterapkan.

### Referensi

- [VS Code Documentation](https://code.visualstudio.com/docs)
- [What are the advantages and disadvantages of using Visual Studio Code or Atom?](https://medium.com/@ssc.ahmed.926748/what-are-the-advantages-and-disadvantages-of-using-visual-studio-code-or-atom-d3132bf1af85)


## Xcode

### Pendahuluan

Xcode adalah Integrated Development Environment (IDE) yang dibuat oleh Apple untuk mendukung pengembangan perangkat lunak di semua platform Apple seperti Mac, iPhone, iPad, Apple Watch, dan Apple TV. Alat ini mendukung berbagai bahasa pemrograman, termasuk Swift, dan menyediakan seperangkat alat untuk para pengembang dalam mendesain, mengkode, menguji, men-debug, dan menerapkan aplikasi mereka.

#### Fungsi dan Fitur Utama:
1. **Pengembangan Aplikasi**: 
   - Xcode adalah suite alat yang digunakan pengembang untuk membangun aplikasi untuk platform Apple. Alat ini mengelola seluruh alur kerja pengembangan, mulai dari penciptaan aplikasi hingga pengujian, optimalisasi, dan pengajuan ke App Store.
   - Dengan Xcode, pengembang dapat mengembangkan aplikasi untuk iOS, watchOS, tvOS, dan macOS. Xcode menawarkan berbagai fitur untuk mempercepat proses pengembangan aplikasi, termasuk editor kode, alat desain grafis, kerangka kerja debugging, dan lainnya.

2. **Antarmuka Pengguna**:
   - Xcode menyatukan desain antarmuka pengguna, pengkodean, pengujian, debugging, dan pengajuan ke App Store dalam satu alur kerja terpadu. Ini termasuk editor kode kelas dunia, alat pratinjau SwiftUI bawaan yang menampilkan UI aplikasi Anda saat Anda memodifikasi kode.

3. **Tersedia Gratis**:
   - Rilis terkini dari Xcode tersedia untuk diunduh secara gratis dari Mac App Store, memudahkan akses untuk para pengembang yang ingin mulai menggunakan alat ini untuk pengembangan aplikasi mereka.

#### Sejarah:
- Xcode pertama kali diluncurkan pada tahun 2003, yang menjadikannya sebagai salah satu IDE yang telah mapan dan terus berkembang untuk mendukung pengembangan aplikasi di ekosistem Apple.

#### Referensi:
1. Core Commerce: [What is Xcode and What Can You Do With It?](https://www.corecommerce.com/blog/what-is-xcode-and-what-can-you-do-with-it/).
2. Apple Developer Documentation: [Xcode](https://developer.apple.com/documentation/xcode).
3. Blue Zorro: [How to Code Xcode: A Complete Tutorial For Beginners](https://bluezorro.com/how-to-code-xcode-a-complete-tutorial-for-beginners/).
4. Apple Developer Support: [Xcode](https://developer.apple.com/support/xcode/).

### Cara Kerja Xcode
#### Struktur Dasar dan Fungsionalitas:
1. **Alat Pengembangan**:
   - Xcode adalah kumpulan alat pengembangan yang dirancang untuk membuat aplikasi untuk Mac, iPhone, iPad, Apple Watch, dan Apple TV. Xcode merupakan IDE (Integrated Development Environment) yang mencakup banyak alat untuk desain antarmuka pengguna, pengkodean, pengujian, debugging, dan pengajuan ke App Store. Xcode mengonversi kode sumber menjadi kode mesin atau file kode biner dan memungkinkan pengembang untuk mengotomatisasi folder proyek mereka.
   - Xcode adalah suite alat yang digunakan pengembang untuk membangun aplikasi untuk platform Apple. Ini mengelola seluruh alur kerja pengembangan, mulai dari penciptaan aplikasi hingga pengujian, optimalisasi, dan pengajuan ke App Store.

2. **Antarmuka Pengguna**:
   - Xcode terdiri dari lima area utama: Navigator, Editor, Utility Area, Toolbar, dan Debug Area. Pengguna dapat menyesuaikan ukuran pane-pane ini dan menampilkan atau menyembunyikan area-area tertentu sesuai kebutuhan via tombol "View" di sudut kanan atas.

3. **Pengkodean dan Antarmuka Pengguna**:
   - Pengembang dapat menulis kode dalam Editor Area, membangun antarmuka pengguna dengan menggunakan Storyboards atau SwiftUI, dan mengonfigurasi elemen dengan Utility Area.

4. **Pengujian dan Debugging**:
   - Xcode dilengkapi dengan iOS Simulator untuk menguji aplikasi, dan Debug Console untuk mengidentifikasi dan memperbaiki bug. Pengembang juga dapat menjalankan dan membangun proyek mereka menggunakan Toolbar.

5. **Manajemen Proyek**:
   - Alat ini juga mencakup berbagai alat untuk mengelola file proyek dan sumber daya, serta membantu dalam mengkonfigurasi proyek atau workspace untuk menggunakan Xcode Cloud, yang memudahkan pengembang dalam membangun dan mengoptimalkan aplikasi atau kerangka kerja mereka dengan Xcode Cloud.

#### Proses Kerja (Workflow):
1. **Pengembangan Aplikasi**:
   - Mulai dengan membuat proyek baru atau membuka proyek yang ada, kemudian tulis kode dan desain antarmuka pengguna.
   - Selanjutnya, bangun dan jalankan aplikasi untuk pengujian, baik di simulator atau perangkat nyata.
   - Identifikasi dan perbaiki bug dengan menggunakan Debug Console.
   - Optimalisasi aplikasi dan siapkan untuk pengajuan ke App Store.

#### Referensi:
1. Apple Developer Support: [Xcode](https://developer.apple.com/support/xcode/).
2. Apple Developer Documentation: [Xcode](https://developer.apple.com/documentation/xcode).
3. BrowserStack: [What is Xcode: Features, Installation, Uses, Advantages](https://www.browserstack.com/guide/what-is-xcode).
4. Apple Developer: [Configuring your first Xcode Cloud workflow](https://developer.apple.com/documentation/xcode/configuring-your-first-xcode-cloud-workflow).
5. CodeWithChris: [Xcode Tutorial for Beginners](https://codewithchris.com/xcode-tutorial/).

### Kelebihan dan Kekurangan Xcode
#### Kelebihan Xcode:
1. **Desain Antarmuka**:
   - Desain antarmuka pengguna Xcode cukup sederhana dan user-friendly, memudahkan para pengembang untuk membangun dan menguji aplikasi mereka.
   
2. **Pengujian dan Debugging**:
   - Xcode memungkinkan pengujian setiap bagian kode untuk memperbaiki proses debugging, dan juga memiliki simulasi bawaan yang memudahkan pengujian aplikasi.

3. **Optimasi Kinerja**:
   - Xcode menyediakan peluang untuk mempelajari profil dan analisis heap, yang membantu pengembang dalam mengoptimalkan kinerja aplikasi mereka.

4. **Kolaborasi Tim**:
   - Alat-alat yang tersedia dalam Xcode memungkinkan kolaborasi tim, penting dalam lingkungan kerja remote.

5. **Instalasi Mudah**:
   - Mudah untuk diatur dan berfungsi dengan sempurna, bahkan pada Android.

6. **Pengembangan Multi-platform**:
   - Xcode mendukung pengembangan aplikasi untuk semua platform Apple seperti macOS, iOS, watchOS, tvOS, dan juga memungkinkan testing responsif aplikasi menggunakan Xcode iPhone Simulator.

#### Kekurangan Xcode:
1. **Keterbatasan Kompatibilitas**:
   - Xcode hanya kompatibel dengan produk Apple, yang mungkin membatasi penggunaan di luar ekosistem Apple.

2. **Kesulitan dalam Bekerja dengan Banyak Jendela**:
   - Ketidakmampuan untuk mengaktifkan konteks kerja berbasis tab membuat penggunaan banyak jendela menjadi tantangan.

3. **Kurangnya Alat Tertentu**:
   - Beberapa ulasan mencatat bahwa Xcode mungkin kurang beberapa alat yang ada di IDE lain, seperti yang lebih baik mendukung untuk bahasa pemrograman tertentu selain Swift dan Objective-C.

#### Referensi:
1. Talent500 Blog: [XCode: The best IDE for iOS Development](https://www.talent500.co/blog/what-is-xcode-and-what-can-you-do-with-it).
2. PeerSpot: [Apple Xcode pros and cons](https://www.peerspot.com/products/apple-xcode/reviews).
3. Mechlin Software Technology Pvt: [How To Use Xcode and its advantages?](https://mechlintech.com/how-to-use-xcode-and-its-advantages).
4. Software Testing Help: [Xcode Tutorial - What Is Xcode And How To Use It](https://www.softwaretestinghelp.com/xcode-tutorial-what-is-xcode-and-how-to-use-it).
5. BrowserStack: [Using Xcode iOS Simulator for Responsive Testing](https://www.browserstack.com/guide/using-xcode-ios-simulator-for-responsive-testing).


### Cara Install Xcode
#### Langkah 1: Unduh Xcode
- **Melalui App Store**:
  1. Buka App Store pada Mac Anda.
  2. Masuk dengan ID Apple Anda.
  3. Cari Xcode dalam App Store.
  4. Klik install atau update.
- **Melalui Situs Pengembang Apple** (Disarankan untuk versi spesifik atau versi lama):
  1. Buka bagian "more" pada [situs pengembang Apple](https://developer.apple.com/download/more/).
  2. Masuk dengan ID Apple Anda.
  3. Ketikkan versi yang diinginkan, lalu unduh file `Xcode_x_x_x.xip`.
  4. Setelah file diunduh, klik pada file `.xip` untuk mengekstraknya. Laptop Anda akan mengekstraknya ke folder yang sama tempat Anda mengunduhnya. Proses ekstraksi ini otomatis.
  5. (Opsional) Setelah diekstrak, ganti nama aplikasinya menjadi “Xcode11.x.x” jika Anda menggunakan beberapa versi.
  6. Seret aplikasi ke folder Aplikasi.
  7. (Opsional) Atur versi Xcode baru sebagai default dengan membuka Terminal dan mengetikkan `sudo xcode-select -switch /Applications/Xcodex.x.x.app`. Gantikan `x.x.x` dengan nomor versi. Misalnya: `Xcode11.4.1.app`.

#### Langkah 2: Instal Command Line Tools (CLT)
- Jika Anda memiliki lebih dari satu pengguna pada komputer Anda, Anda perlu memperbarui CLT untuk setiap pengguna.
- Unduh file `.dmg` CLT dari [situs pengembang Apple](https://developer.apple.com/download/more/).
- Jika ini adalah instalasi Xcode pertama Anda, Anda mungkin dapat memperbarui dengan Terminal Anda dengan mengetikkan `xcode-select --install`.
- Setelah file `.dmg` selesai diunduh, klik dua kali file untuk membukanya dan ikuti petunjuk untuk menginstal CLT.

#### Langkah 3: Buka Xcode
- Buka folder Aplikasi dan buka versi baru dari Xcode. Jika Anda mengganti nama Xcode, pastikan Anda membuka aplikasi yang benar.
- Xcode mungkin akan meminta Anda untuk menginstal komponen tambahan. Klik install dan tunggu beberapa menit.
- Setelah komponen terinstal, Xcode akan meluncurkan. Anda harus dapat mengambil proyek lama Anda dan melanjutkan dari mana Anda berhenti.

#### Sumber:
1. FreeCodeCamp: [How to Download Xcode and Install it on Your Mac](https://www.freecodecamp.org/news/how-to-download-and-install-xcode).
2. MarketSplash: [How To Install Xcode On Your Mac](https://marketsplash.com/how-to-install-xcode-on-mac).
3. Andrew Hoog: [3 ways to install Xcode on macOS [2023]](https://www.andrewhoog.com/post/how-to-install-xcode).