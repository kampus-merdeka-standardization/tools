# Linter

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
