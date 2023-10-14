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
