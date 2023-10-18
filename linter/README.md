# Linter

## SonarLint

Referensi: [Linter IDE Tool & Real-Time Software for Code with SonarLint | Sonar](https://www.sonarsource.com/products/sonarlint/)

SonarLint adalah ekstensi IDE gratis yang membantu kita menemukan dan memperbaiki masalah dalam kode kita secara _real-time_. Ini berfungsi seperti pemeriksa ejaan, SonarLint menyoroti masalah dalam kode dan memungkinkan kita untuk menulis kode yang lebih baik dengan melakukan analisis saat kita menulis kode untuk mendeteksi kesalahan umum, bug yang rumit, dan _hotspots_.

SonarLint mendukung berbagai bahasa pemrograman dan tersedia untuk diinstal dari _marketplace_ IDE, tinggal kita cari `sonarlint` dan install. Atau pada website https://www.sonarsource.com/products/sonarlint/ dan install sesuai IDE yang digunakan.

Beberapa fitur utama SonarLint meliputi:
- Analisis real-time: Memberikan umpan balik instan saat Anda menulis kode.
- Perbaikan cepat: Menyarankan solusi yang disesuaikan dengan kode spesifik Anda sehingga Anda dapat memperbaiki masalah yang ditandai secara real-time.
- Aturan dan pengaturan analisis tim yang disatukan: Dengan terhubung ke SonarQube atau SonarCloud, aturan dan pengaturan analisis disinkronkan ke SonarLint, menyelaraskan tim di sekitar standar Clean Code tunggal.

## Checksyle (java)

Referensi : [checkstyle – Checkstyle 10.12.4](https://checkstyle.sourceforge.io/)

Checkstyle adalah sebuah alat pengembangan yang sangat berguna bagi para programmer dalam menulis kode Java sesuai dengan standar penulisan. Dengan kemampuan otomatisasinya, Checkstyle membantu menghemat waktu dan tenaga manusia dalam proses pengecekan kode. Yang membuat Checkstyle sangat fleksibel adalah kemampuannya untuk dikonfigurasi sesuai dengan hampir semua standar penulisan yang ada, termasuk contoh file konfigurasi untuk Sun Code Conventions dan Google Java Style. Alat ini sangat komprehensif dalam memeriksa berbagai aspek kode sumber, mulai dari masalah desain kelas, metode, layout, hingga format. Integrasi Checkstyle ke dalam proses build atau lingkungan pengembangan menjadi lebih mudah berkat plugin-plugin yang disediakan, termasuk yang tersedia untuk Ant, Maven, Eclipse, dan juga plugin pihak ketiga untuk IDE lainnya. Selain itu, Checkstyle mengikuti versi Romantis dan Semantiknya sendiri, hanya dibatasi oleh versi minimal JRE. Untuk detail lebih lanjut mengenai keterbatasannya, dapat merujuk pada daftar keterbatasan lengkap yang disediakan.

### Cara Download
Rilis terbaru dari Checkstyle dapat diunduh dari [halaman rilis GitHub](https://github.com/checkstyle/checkstyle/releases/), atau [Maven central](https://central.sonatype.com/search?q=g:com.puppycrawl.tools%20%20a:checkstyle&smo=true).

Jika Anda ingin hidup di ujung tombak, Anda bisa [_checkout_](https://github.com/checkstyle/checkstyle) kode pengembangan saat ini dari GitHub dan mengkompilasinya sendiri. Atau gunakan [jitpack.io](https://jitpack.io/) untuk membangun dan mendapatkan artefak yang kita butuhkan (kita bahkan bisa membangun repo bercabang).


### _Related Tools_
Checkstyle sangat berguna jika kita mengintegrasikannya ke dalam proses build atau lingkungan pengembangan kita. Distribusinya meliputi:

1. Sebuah [_Ant Task_](https://checkstyle.sourceforge.io/anttask.html).
2. [_command line_](https://checkstyle.sourceforge.io/cmdline.html) _interface_ (CLI).

Selain itu, plug-in ditulis oleh pihak ketiga. Beberapa di antaranya masih didasarkan pada rilis Checkstyle 2.4, meskipun ada banyak perbaikan sejak saat itu. Plug-in yang dikenal adalah:

| IDE / _Build tool_ | _Main_/_Initial Author_ | _Available from_ | _Remarks_ |
| :------ | :------ | :------ | :------ |
| IntelliJ IDEA |	James Shiell | [_Checkstyle-idea Project Page_](https://github.com/jshiell/checkstyle-idea) | Provides real-time and on-demand scanning. |
| Visual Studio Code | Sheng Chen |	[vscode-checkstyle](https://marketplace.visualstudio.com/items?itemName=shengchen.vscode-checkstyle) | Checkstyle for Microsoft Visual Studio Code
| ... | ... | ... | ... |

dan masih banyak yang lainnya, dapat dilihat pada https://checkstyle.sourceforge.io/#Related_Tools_Active_Tools


## PMD

referensi :
- [PMD](https://pmd.github.io/)

PMD adalah alat analisis kode sumber. Alat ini dapat menemukan cacat pemrograman umum seperti variabel yang tidak digunakan, blok penangkapan kosong, pembuatan objek yang tidak perlu, dan sebagainya. PMD mendukung berbagai bahasa pemrograman seperti Java, JavaScript, Salesforce.com Apex dan Visualforce, PLSQL, Apache Velocity, XML, XSL.

Selain itu, PMD juga mencakup CPD (Copy-Paste Detector), yang dapat menemukan kode yang duplikat dalam berbagai bahasa pemrograman.

PMD dapat digunakan dalam proses _linting_, yaitu proses analisis statis pada kode untuk mendeteksi kesalahan pemrograman, bug, kesalahan gaya dan format, dan entri yang mencurigakan. Dengan menggunakan PMD dalam linting, Anda dapat memastikan kode Anda mengikuti standar tertentu dan lebih efisien.

### Cara menggunakan PMD
Berikut adalah beberapa langkah untuk menggunakan PMD:

1. **Pilih Bahasa Pemrograman**: PMD mendukung berbagai bahasa pemrograman seperti Java, JavaScript, Salesforce.com Apex dan Visualforce, PLSQL, Apache Velocity, XML, XSL.

2. **Atur Aturan PMD**: Anda perlu mengonfigurasi aturan PMD dalam pengaturan plugin dan memilih versi PMD yang sesuai.

3. **Integrasi dengan IDE**: PMD dapat diintegrasikan sebagai inspeksi dalam IDE seperti [IntelliJ](https://plugins.jetbrains.com/plugin/15412-pmd-idea), sehingga file yang sedang dibuka dapat dipindai "_on the fly_". Selain Intellij Idea, PMD juga dapat diintegrasikan dengan IDE lainnya, seperti pada VSCode, kita bisa mencari ekstensi "PMD" lalu install

4. **Pemindaian Kode**: Anda dapat menjalankan kode Anda melalui linter dan mendapatkan pemberitahuan dini tentang kesalahan pemrograman, bug, kesalahan gaya dan format, dan entri yang mencurigakan¹.

5. **Perbaikan Cepat**: Untuk beberapa aturan umum, perbaikan cepat tersedia⁸.

6. **Analisis Kode**: Anda juga dapat memeriksa jenis variabel, menghapus variabel yang tidak digunakan, dan membuat kode Anda lebih efisien.


## GolangCI-Lint

`golangci-lint` adalah Go linters runner yang cepat. Ia menjalankan linter secara paralel, menggunakan caching, mendukung 
konfigurasi `yaml`, memiliki integrasi dengan semua major IDE dan menyertakan lusinan linter.

### Fitur

- [Very fast](https://golangci-lint.run/usage/performance): menjalankan linter secara paralel, menggunakan kembali cache build Go, dan menyimpan hasil analisis cache. 
- YAML-based [configuration](https://golangci-lint.run/usage/configuration). 
- [Integrations](https://golangci-lint.run/usage/integrations) dengan VS Code, Sublime Text, GoLand, GNU Emacs, Vim, Atom, GitHub Actions. 
- [A lot of linters](https://golangci-lint.run/usage/linters) disertakan, tidak perlu menginstalnya. 
- Jumlah minimum [false positives](https://golangci-lint.run/usage/false-positives) karena pengaturan default disetel. 
- Keluaran bagus dengan warna, baris kode sumber, dan pengidentifikasi yang ditandai.

### Instalasi

- GitHub Actions

  Direkomendasikan menggunakan [our GitHub Action](https://github.com/golangci/golangci-lint-action) untuk menjalankan `golangci-lint` 
  di CI untuk proyek GitHub. Ini [fast and uses smart caching](https://github.com/golangci/golangci-lint-action#performance) 
  di dalamnya dan bisa jauh lebih cepat daripada instalasi _simple binary_.

- Other CI

  Penting untuk memiliki CI yang dapat direproduksi: jangan mulai membuat semua build gagal secara bersamaan. Dengan golangci-lint 
  hal ini dapat terjadi jika Anda menggunakan opsi `--enable-all` dan linter baru ditambahkan atau bahkan tanpa `--enable-all` 
  saat satu linter upstream ditingkatkan.

  **PENTING**: Sangat disarankan untuk menginstal versi golangci-lint tertentu yang tersedia di [releases page](https://github.com/golangci/golangci-lint/releases).

  Berikut adalah contoh install golangci-lint dengan v1.54.2:
  ```shell
  # binary will be $(go env GOPATH)/bin/golangci-lint
  curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin v1.54.2

  # or install it into ./bin/
  curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s v1.54.2

  # In alpine linux (as it does not come with curl by default)
  wget -O- -nv https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s v1.54.2

  golangci-lint --version
  ```

- Local
  
  - Binaries
    
    ```shell
    # binary will be $(go env GOPATH)/bin/golangci-lint
    curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin v1.54.2

    golangci-lint --version
    ```

  - Docker

    ```shell
    docker run --rm -v $(pwd):/app -w /app golangci/golangci-lint:v1.54.2 golangci-lint run -v
    ```

    Mempertahankan cache di antara proses yang berurutan:
    ```shell
    docker run --rm -v $(pwd):/app -v ~/.cache/golangci-lint/v1.54.2:/root/.cache -w /app golangci/golangci-lint:v1.54.2 golangci-lint run -v
    ```

    Colored output:
    ```shell
    docker run -t --rm -v $(pwd):/app -w /app golangci/golangci-lint:v1.54.2 golangci-lint run -v
    ```
  - macOS
    Anda dapat menginstal binary release di macOS menggunakan brew:
    ```shell
    brew install golangci-lint
    brew upgrade golangci-lint
    ```
  - Install from Source
    Note: instalasi `go install`/`go get` tersebut tidak dijamin berhasil. Direkomendasikan menggunakan _binary installation_.
    ```shell
    go install github.com/golangci/golangci-lint/cmd/golangci-lint@v1.54.2
    ```

### Penggunaan

Untuk menjalankan golangci-lint, jalankan:
```shell
golangci-lint run
```
Sama saja dengan seperti ini:
```shell
golangci-lint run ./...
```
Anda dapat memilih direktori dan file mana yang akan dianalisis:
```shell
golangci-lint run dir1 dir2/... dir3/file1.go
```
Direktori TIDAK dianalisis secara rekursif. Untuk menganalisisnya, tambahkan `/...` secara rekursif ke _path_.

GolangCI-Lint dapat digunakan dengan konfigurasi nol. Secara default, linter berikut diaktifkan:
```shell
$ golangci-lint help linters
Enabled by default linters:
errcheck: errcheck is a program for checking for unchecked errors in Go code. These unchecked errors can be critical bugs in some cases [fast: false, auto-fix: false]
gosimple (megacheck): Linter for Go source code that specializes in simplifying code [fast: false, auto-fix: false]
govet (vet, vetshadow): Vet examines Go source code and reports suspicious constructs, such as Printf calls whose arguments do not align with the format string [fast: false, auto-fix: false]
ineffassign: Detects when assignments to existing variables are not used [fast: true, auto-fix: false]
staticcheck (megacheck): It's a set of rules from staticcheck. It's not the same thing as the staticcheck binary. The author of staticcheck doesn't support or approve the use of staticcheck as a library inside golangci-lint. [fast: false, auto-fix: false]
unused (megacheck): Checks Go code for unused constants, variables, functions and types [fast: false, auto-fix: false]
```
Berikan `-E/--enable` untuk mengaktifkan linter dan `-D/--disable` untuk menonaktifkan:
```shell
golangci-lint run --disable-all -E errcheck
```

### Referensi 

- [Dokumentasi golangci-lint](https://golangci-lint.run/)

## SwiftLint

_Tools_ untuk menerapkan gaya dan konvensi Swift, berdasarkan pada [GitHub Swift Style Guide](https://github.com/github/swift-style-guide) 
yang sekarang diarsipkan. SwiftLint menerapkan aturan panduan gaya yang diterima secara umum oleh komunitas Swift. Aturan-aturan 
ini dijelaskan dengan baik dalam panduan gaya populer seperti [Kodeco's Swift Style Guide](https://github.com/kodecocodes/swift-style-guide).

### Instalasi

[Homebrew](http://brew.sh/):
```shell
brew install swiftlint
```

[CocoaPods](https://cocoapods.org/):
Cukup tambahkan baris berikut ke Podfile Anda:
```shell
pod 'SwiftLint'
```

Ini akan mengunduh binari dan dependensi SwiftLint di `Pods/` selama eksekusi `pod install` berikutnya dan memungkinkan Anda 
untuk memanggilnya melalui `${PODS_ROOT}/SwiftLint/swiftlint` dalam Fase Pembuatan Skrip Anda.

Ini adalah cara yang disarankan untuk menginstal versi SwiftLint tertentu karena mendukung instalasi versi yang disematkan, 
bukan hanya versi terbaru (seperti halnya Homebrew).

Perhatikan bahwa ini akan menambahkan biner SwiftLint, biner dependensinya, dan distribusi pustaka biner Swift ke direktori 
`Pods/`, jadi memeriksa direktori ini ke SCM seperti git tidak disarankan.

[Mint](https://github.com/yonaskolb/mint):
```shell
$ mint install realm/SwiftLint
```

### Command Line

```shell
$ swiftlint help
OVERVIEW: A tool to enforce Swift style and conventions.

USAGE: swiftlint <subcommand>

OPTIONS:
  --version               Show the version.
  -h, --help              Show help information.

SUBCOMMANDS:
  analyze                 Run analysis rules
  docs                    Open SwiftLint documentation website in the default web browser
  generate-docs           Generates markdown documentation for all rules
  lint (default)          Print lint warnings and errors
  reporters               Display the list of reporters and their identifiers
  rules                   Display the list of rules and their identifiers
  version                 Display the current version of SwiftLint

  See 'swiftlint help <subcommand>' for detailed help.
```
Jalankan `swiftlint` di direktori yang berisi file Swift ke lint. Direktori akan dicari secara rekursif.

Untuk menentukan daftar file saat menggunakan `lint` atau `analyze` (seperti daftar file yang dimodifikasi oleh Xcode yang 
ditentukan oleh plugin [`ExtraBuildPhase`](https://github.com/norio-nomura/ExtraBuildPhase) Xcode, atau file yang dimodifikasi 
di _working tree_ berdasarkan `git ls-files -m`), Anda dapat melakukannya dengan meneruskan opsi `--use-script-input-files` 
dan mengatur variabel instan berikut: `SCRIPT_INPUT_FILE_COUNT` dan `SCRIPT_INPUT_FILE_0, SCRIPT_INPUT_FILE_1`...`SCRIPT_INPUT_FILE_{SCRIPT_INPUT_FILE_COUNT - 1}.`

### Referensi

- [SwiftLint GitHub](https://github.com/realm/SwiftLint)



## ESlint

### ESLint: Pengantar
ESLint adalah alat analisis kode statis yang dirancang untuk mengidentifikasi dan melaporkan pola dalam kode ECMAScript/JavaScript, dengan tujuan membuat kode menjadi lebih konsisten dan menghindari bug. Setiap aturan dalam ESLint adalah plugin, dan Anda dapat menambahkan lebih banyak plugin pada saat runtime. ESLint diciptakan oleh Nicholas C. Zakas pada Juni 2013 sebagai utilitas linting JavaScript sumber terbuka. Alat ini sering digunakan untuk menemukan pola bermasalah atau kode yang tidak sesuai dengan pedoman gaya tertentu. ESLint ditulis menggunakan Node.js untuk menyediakan lingkungan runtime yang cepat dan instalasi yang mudah melalui npm.

ESLint menganalisis kode secara statis untuk cepat menemukan masalah, dan terintegrasi dengan sebagian besar editor teks. ESLint dapat dijalankan sebagai bagian dari pipeline integrasi terus menerus, dan banyak masalah yang ditemukan oleh ESLint dapat diperbaiki secara otomatis. Selain itu, aturan dalam ESLint dapat dikonfigurasi, dan aturan kustom dapat ditentukan dan dimuat. ESLint mencakup masalah kualitas kode dan masalah gaya kode.

#### Referensi:
1. ESLint Official Documentation: [Getting Started with ESLint - Pluggable JavaScript Linter](https://eslint.org/docs/user-guide/getting-started).
2. DEV Community: [ESLint: What, Why, When, How](https://dev.to/codemouse92/eslint-what-why-when-how-5cf3).
3. Wikipedia: [ESLint](https://en.wikipedia.org/wiki/ESLint).
4. Sampig GitHub: [Introduction to ESLint](https://sampig.github.io/blog/introduction-to-eslint).


### Cara Kerja ESLint

#### Analisis Kode Sumber:
ESLint menganalisis kode sumber Anda untuk mencari kesalahan dan pelanggaran terhadap praktik terbaik. Alat ini membantu Anda membuat kode lebih konsisten dan menghindari bug​​.

#### Penerapan Aturan:
ESLint bekerja dengan mem-parsing kode Anda dan menerapkan set aturan yang dapat Anda konfigurasi atau sesuaikan. Aturan-aturan ini dapat didasarkan pada praktik terbaik, standar pemrograman, atau preferensi Anda sendiri​​.

#### Perbaikan Otomatis:
ESLint memiliki kemampuan untuk memperbaiki masalah secara otomatis. Perbaikan yang dibuat oleh ESLint sadar sintaks sehingga Anda tidak akan mengalami kesalahan yang diperkenalkan oleh algoritma temukan-dan-ganti tradisional​3.

#### Konfigurasi:
ESLint sepenuhnya dapat dikonfigurasi. Anda dapat mengonfigurasinya dengan file .eslintrc.{js,yml,json} dan menambahkan aturan, plugin, dan konfigurasi individu. Tingkat kesalahan dari aturan dapat diatur ke salah satu dari tiga nilai: "off" atau 0 untuk mematikan aturan, "warn" atau 1 untuk mengaktifkan aturan sebagai peringatan, dan "error" atau 2 untuk mengaktifkan aturan sebagai kesalahan​1​.

#### Struktur Internal:
Di tingkat yang lebih dalam, ESLint memiliki beberapa komponen penting seperti bin/eslint.js yang merupakan pembungkus sederhana untuk bootstrap ESLint, lib/api.js yang mengekspos objek yang berisi kelas publik, dan lib/cli.js yang merupakan inti dari CLI ESLint​.

Referensi:
- [Dokumentasi Resmi ESLint: Getting Started with ESLint​](https://eslint.org/docs/latest/use/getting-started)
- [LinkedIn: ESLint Tutorial for Beginners: Benefits and Tips](https://www.linkedin.com/pulse/eslint-tutorial-begin)

### Kelebihan dan Kekurangan ESLint

#### Kelebihan:
1. **Deteksi Otomatis Masalah:**
   ESLint secara otomatis menganalisis kode untuk mencari potensi bug dan kesalahan sesuai dengan standar atau konvensi yang telah ditetapkan dalam konfigurasi ESLint. Hal ini memungkinkan pengembang untuk mendapatkan umpan balik cepat mengenai apakah kode mereka sudah sesuai dengan praktik terbaik atau apakah ada bagian kode yang berpotensi menyebabkan bug di masa mendatang.

2. **Perbaikan Otomatis:**
   ESLint memiliki fitur untuk memperbaiki otomatis kode yang salah sesuai dengan aturan yang ditetapkan, sehingga memudahkan pengembang untuk memperbaiki kesalahan dengan cepat.

3. **Kustomisasi:**
   ESLint memungkinkan pengembang untuk mengkustomisasi konfigurasi, parser, dan aturan sesuai dengan kebutuhan proyek mereka. Ini juga mencakup dukungan untuk TypeScript dan banyak pustaka atau kerangka kerja populer lainnya seperti React dan Vue, dengan banyak plugin tersedia untuk memperluas fungsionalitasnya.

4. **Integrasi Mudah:**
   ESLint mudah diintegrasikan dengan alat dan editor kode lain, serta memiliki .eslintignore file untuk menghindari pemeriksaan file tertentu, mirip dengan .gitignore.

5. **Deteksi Vulnerabilitas Keamanan:**
   ESLint membantu dalam mendeteksi vulnerabilitas keamanan dalam kode, yang merupakan keuntungan besar untuk memastikan keamanan aplikasi.

6. **Pencegahan Kesalahan Sintaksis dan Global yang Tidak Disengaja:**
   ESLint membantu mencegah kesalahan sintaksis dan variabel global yang tidak disengaja yang mungkin lolos tanpa diketahui dalam bahasa yang dinamis seperti JavaScript.

#### Kekurangan:
1. **Kemungkinan Positif Palsu atau Negatif Palsu:**
   Terkadang, ESLint dapat melaporkan positif palsu atau negatif palsu, yang bisa menjadi masalah dalam proyek besar dan kompleks.

2. **Kurva Belajar:**
   Mungkin ada kurva belajar untuk mengonfigurasi dan memahami semua aturan dan opsi yang tersedia di ESLint, terutama untuk pengguna baru atau tim yang belum familiar dengan linter.

3. **Konfigurasi dan Pemeliharaan:**
   ESLint memerlukan konfigurasi awal dan pemeliharaan berkelanjutan untuk memastikan bahwa itu tetap efektif dan relevan dengan kebutuhan proyek.

Referensi:
- Rivki, M. (n.d.). Kenalan dengan ESLint, Linter Javascript. Retrieved from [rivki.dev](https://rivki.dev)
- Why and how to use ESLint in your project - IBM Developer. (n.d.). Retrieved from [IBM Developer](https://developer.ibm.com)
- Pros and Cons for using ESLint for Software Security - Codiga. (n.d.). Retrieved from [Codiga](https://www.codiga.io)
- Understanding the Real Advantages of Using ESLint - Rangle. (n.d.). Retrieved from [Rangle](https://rangle.io)


### Cara Install ESLint

#### Prasyarat:
Sebelum memulai instalasi ESLint, pastikan bahwa Node.js versi `^12.22.0`, `^14.17.0`, atau `>=16.0.0` sudah terinstal pada sistem Anda. Jika Anda menggunakan distribusi Node.js resmi, dukungan SSL sudah terintegrasi dalam instalasi tersebut.

#### Langkah-langkah Instalasi:
1. **Instalasi Lokal**:
   - Buka terminal pada sistem Anda.
   - Jalankan perintah berikut untuk menginstal dan mengonfigurasi ESLint:
     ```bash
     npm init @eslint/config
     ```
   - Jika Anda ingin menggunakan konfigurasi berbagi tertentu yang di-host di npm, Anda dapat menggunakan opsi `--config` dan menentukan nama paket:
     ```bash
     # npm 7+
     npm init @eslint/config -- --config semistandard

     # atau (prefix `eslint-config` adalah opsional)
     npm init @eslint/config -- --config eslint-config-semistandard

     # ⚠️ npm 6.x tanpa tanda dash ganda ekstra:
     npm init @eslint/config --config semistandard
     ```
   - Setelah konfigurasi awal, Anda dapat menjalankan ESLint pada file atau direktori mana saja seperti ini:
     ```bash
     npx eslint yourfile.js

     # atau

     yarn run eslint yourfile.js
     ```
   Catatan: Perintah `npm init @eslint/config` mengasumsikan bahwa Anda sudah memiliki file `package.json`. Jika belum, pastikan untuk menjalankan `npm init` atau `yarn init` sebelumnya.

2. **Instalasi Global**:
   - Untuk menginstal ESLint secara global sehingga dapat digunakan di seluruh sistem, jalankan perintah berikut:
     ```bash
     npm install -g eslint
     ```
   - Untuk memeriksa instalasi dan melihat versi ESLint, jalankan perintah berikut:
     ```bash
     eslint -v
     ```
   - Untuk mengetahui di mana ESLint diinstal (asumsikan MacOS/Linux), Anda dapat menjalankan perintah berikut:
     ```bash
     whereis eslint
     ```
   - Setelah instalasi global, Anda dapat menjalankan ESLint pada file atau direktori mana saja dari mana saja dalam sistem Anda.

#### Referensi:
- ESLint - [Getting Started with ESLint](https://eslint.org/docs/latest/use/getting-started)
- Stack Overflow - [How to install ESLint globally?](https://stackoverflow.com/questions/59404272/how-to-install-eslint-globally)
- npm - [ESLint on npmjs.com](https://www.npmjs.com/package/eslint)
- Microsoft - [Linting JavaScript in Visual Studio](https://learn.microsoft.com/en-us/visualstudio/ide/how-to-linting-javascript)

### Cara Pakai ESLint

Menggunakan ESLint untuk memeriksa kode Anda bisa membantu meningkatkan kualitas kode dan menjaga konsistensi gaya penulisan kode di seluruh proyek. Berikut adalah langkah-langkah dasar untuk menggunakan ESLint:

1. **Konfigurasi ESLint**:
   - Setelah instalasi, buat file konfigurasi ESLint dengan menjalankan `eslint --init` di direktori proyek Anda. Ini akan membimbing Anda melalui proses pembuatan file konfigurasi ESLint (`.eslintrc`).
   - Anda juga dapat menyesuaikan konfigurasi ESLint sesuai kebutuhan proyek dengan mengedit file `.eslintrc` atau file konfigurasi lain yang relevan.

2. **Menjalankan ESLint**:
   - Jalankan ESLint pada file atau direktori tertentu dengan perintah `eslint [your file/directory]`. Misalnya, `eslint src/` akan memeriksa semua file di direktori `src`.
   - Anda juga dapat menambahkan skrip ke file `package.json` Anda untuk menjalankan ESLint. Misalnya: 
     ```json
     "scripts": {
       "lint": "eslint src/"
     }
     ```
     Kemudian, Anda dapat menjalankan ESLint dengan perintah `npm run lint`.

3. **Memeriksa Hasil**:
   - ESLint akan melaporkan kesalahan dan peringatan pada terminal. Setiap masalah akan memiliki penjelasan singkat dan lokasi baris/karakter di mana masalah itu terjadi.
   - Anda juga dapat menggunakan flag `--fix` untuk memperbaiki otomatis sebagian masalah yang terdeteksi. Misalnya, `eslint src/ --fix`.

4. **Integrasi dengan Editor**:
   - Banyak editor teks dan IDE memiliki plugin ESLint yang memungkinkan Anda untuk melihat hasil linting secara real-time saat Anda mengetik kode.
   - Contoh plugin termasuk ESLint plugin untuk Visual Studio Code, Sublime Text, atau Atom.

5. **Menggunakan Plugins dan Aturan Kustom**:
   - ESLint mendukung plugin dan aturan kustom. Jika Anda ingin menambahkan aturan atau perangkat tambahan tertentu, Anda dapat menginstal plugin terkait dan memperbarui konfigurasi ESLint Anda untuk memasukkan plugin atau aturan tersebut.

6. **Memelihara Konfigurasi ESLint**:
   - Secara berkala, perbarui konfigurasi ESLint Anda untuk mencocokkan evolusi kebutuhan proyek dan tim Anda.
   - Pertimbangkan untuk menggunakan konfigurasi berbagi atau ekstensi untuk menjaga konfigurasi ESLint Anda tetap konsisten di seluruh proyek atau organisasi.