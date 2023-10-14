# Linter

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
