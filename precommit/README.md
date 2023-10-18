# Precommit

## Husky

### Pendahuluan Husky

Husky adalah alat yang dirancang untuk mempermudah penggunaan Githooks, yang merupakan skrip yang dapat dijalankan sebelum atau sesudah operasi Git tertentu seperti commit atau push. Berikut adalah beberapa poin penting mengenai Husky:

1. **Peningkatan Commit**: 
   Husky membantu dalam meningkatkan commit Anda dengan memungkinkan Anda untuk menjalankan linter pada pesan commit, menjalankan tes, dan menjalankan linting kode sebelum melakukan commit atau push ke repositori Git.

2. **Penegakan Kebijakan**:
   Dengan menggunakan Husky, tim dapat menegakkan kebijakan dan memastikan konsistensi di antara anggota tim dengan menjalankan skrip khusus sebelum atau sesudah operasi Git terjadi. Ini dapat mencegah commit yang tidak diinginkan dari ditambahkan ke repositori dan memberi tahu anggota tim jika ada perubahan yang perlu dilakukan.

3. **Pengaturan Githooks**:
   Husky memudahkan proses pengaturan Githooks, memungkinkan developer untuk bekerja dengan Githooks lebih efisien dan menjalankan semua skrip yang perlu dijalankan pada berbagai tahapan. Dengan mempermudah proses pengaturan Githooks, developer dapat menciptakan solusi yang efektif lebih cepat.

4. **Manajemen Githooks**:
   Husky populer sebagai manajer Githooks yang mengotomatiskan tugas-tugas sebelum melakukan commit atau push perubahan. Husky membantu dalam menjaga standar pemrograman, menjalankan tes, dan memastikan commit Anda mengikuti pedoman yang telah ditetapkan, yang pada akhirnya membantu dalam mengotomatiskan atau menegakkan tindakan dalam alur kerja Git Anda.

Dengan fungsionalitas ini, Husky menjadi alat penting dalam membantu developer untuk mengotomatiskan dan menstandarkan proses developeran, sehingga membantu dalam meningkatkan kualitas kode dan kolaborasi tim.

#### Referensi

1. Husky - GitHub Pages. (n.d.). Retrieved from [Husky - GitHub Pages](https://typicode.github.io/husky).
2. Getting Started with Git Hooks and Husky | Tower Blog. (n.d.). Retrieved from [Tower Blog](https://www.git-tower.com/blog/git-hooks-husky).
3. How to Use Husky and Git Hooks to Automate Actions - GitKraken. (n.d.). Retrieved from [GitKraken](https://www.gitkraken.com/learn/git/tutorials/how-to-use-husky-git-hooks-tutorial).
4. Streamlining Git Workflows with Husky - eddy.hashnode.dev. (n.d.). Retrieved from [eddy.hashnode.dev](https://eddy.hashnode.dev/streamlining-git-workflows-with-husky).


### Cara Kerja Husky
Husky adalah alat yang memungkinkan pengguna untuk menjalankan skrip selama berbagai bagian dari alur kerja Git. Berikut adalah bagaimana Husky bekerja:

1. Integrasi dengan Git Hooks:
Husky bekerja dengan mengintegrasikan objek ke dalam file package.json Anda yang mengonfigurasi Husky untuk menjalankan skrip yang Anda tentukan. Ini memanfaatkan Githooks untuk memungkinkan Anda mengaitkan ke berbagai event Git seperti pre-commit dan pre-push​1.

2. Automasi Skrip:
Anda dapat menggunakan Husky untuk lint pesan commit, menjalankan tes, lint kode, dll., saat Anda melakukan commit atau push. Husky mendukung semua Githooks di sisi klien, memungkinkan otomatisasi berbagai tugas selama proses developeran​​.

3. Pengaturan Githooks:
Husky membantu developer bekerja dengan Githooks lebih efisien dan menjalankan semua skrip yang perlu bekerja pada berbagai tahapan. Dengan mempermudah proses pengaturan Githooks, developer dapat menciptakan solusi yang efektif lebih cepat​.

4. Direktori Husky:
Saat diatur, Husky akan membuat direktori di root proyek Anda yang disebut .husky, di dalamnya Anda akan menemukan hook pre-commit dengan instruksi untuk menjalankan `npm test`. Anda dapat memperbarui instruksi tersebut ke yarn test jika Anda menggunakan yarn. Ini akan menjalankan skrip tes "jika Anda memiliki" sebelum bahkan memungkinkan Anda membuat pesan commit​4.

Dengan cara ini, Husky menyediakan alat otomatisasi yang kuat dan fleksibel yang dapat membantu developer menjaga kualitas kode seiring berjalannya waktu.

#### Referensi:
- [How to add commit hooks to git with husky to automate code tasks - FreeCodeCamp​](https://www.freecodecamp.org/news/how-to-add-commit-hooks-to-git-with-husky-to-automate-code-tasks)

- [Husky - GitHub Pages - Husky Official Documentation​](https://typicode.github.io/husky/)​​

### Kelebihan dan kekurangan Husky

#### Kelebihan:
1. **Berbagi dan Menyimpan Versi Hook**:
   Husky memungkinkan hook yang dapat dibagi dan memiliki versi, dengan hook ditetapkan melalui skrip npm seperti tugas lainnya dalam proyek. Ini membuatnya mudah untuk melacak perubahan pada Githooks di seluruh tim.

2. **Otomatisasi Tugas-tugas Git**:
   Husky otomatis mengotomatiskan tugas-tugas sebelum melakukan commit atau push perubahan, seperti menjalankan tes atau linting kode. Ini membantu memastikan standar pemrograman dipatuhi dan mencegah kesalahan dari dicommit ke repositori.

#### Kekurangan:
1. **Penggunaan Khusus**:
   Beberapa perintah Git dapat digunakan untuk melewati hook Husky, seperti `--no-verify` flag dengan `git commit` atau mengatur variabel lingkungan `HUSKY` ke `0` untuk melewati hook saat push. Ini dapat membuka peluang bagi pengguna untuk melewati kontrol kualitas yang ditetapkan oleh Husky, yang pada gilirannya dapat mengurangi efektivitas Husky dalam menjaga konsistensi kode.

2. **Alternatif Lain**:
   Terdapat beberapa alternatif lain untuk Husky yang mungkin menawarkan pendekatan yang berbeda atau fitur tambahan. Misalnya, pengguna dapat mengatur Githooks secara manual atau menggunakan perangkat lunak lain untuk mengelola Githooks.

#### Referensi:
- Medium: [Taming the husky. Easy and shareable git hooks for JS…](https://medium.com/@david.palecek/taming-the-husky-easy-and-shareable-git-hooks-for-js-projects-94d0a19f4b6d)
- eddy.hashnode.dev: [Streamlining Git Workflows with Husky](https://eddy.hashnode.dev/streamlining-git-workflows-with-husky)
- leonardomontini.dev: [Git Hooks with Husky — Leonardo Montini](https://leonardomontini.dev/git-hooks-with-husky)
- dev.to: [Git hook is the excellent alternative to Husky - DEV Community](https://dev.to/litvin/git-hook-is-the-excellent-alternative-to-husky-3ed)

### Cara Install Husky

Untuk menginstal Husky di proyek Anda, ikuti langkah-langkah berikut:

1. **Instalasi Husky**:
   - Jalankan perintah berikut di terminal proyek Anda:
     ```bash
     npm install husky --save-dev
     ```
   - Alternatifnya, Anda juga dapat menggunakan Yarn untuk menginstal Husky:
     ```bash
     yarn add husky --dev
     ```

2. **Mengaktifkan Githooks**:
   - Setelah Husky terinstal, jalankan perintah berikut untuk mengaktifkan Githooks:
     ```bash
     npx husky install
     ```

3. **Pengaturan Otomatis**:
   - Edit file `package.json` di proyek Anda untuk menjalankan perintah `husky install` secara otomatis setelah instalasi:
     ```json
     {
       "scripts": {
         "prepare": "husky install"
       }
     }
     ```

Langkah-langkah ini akan menginstal Husky di proyek Anda dan mengaturnya untuk menjalankan Githooks yang Anda definisikan. Anda juga dapat mengikuti panduan yang lebih mendetail di dokumentasi resmi Husky atau sumber lainnya untuk memahami lebih lanjut tentang konfigurasi dan penggunaan Husky.

#### Referensi:
- FreeCodeCamp: [How to Add Commit Hooks to Git with Husky to Automate Code Tasks](https://www.freecodecamp.org/news/how-to-add-commit-hooks-to-git-with-husky-to-automate-code-tasks).
- Tower Blog: [Getting Started with Git Hooks and Husky](https://www.git-tower.com/blog/git-hooks-husky).
- Husky - GitHub Pages: [Getting started | husky - GitHub Pages](https://typicode.github.io/husky).
- GitKraken: [How to Use Husky and Git Hooks to Automate Actions - GitKraken](https://www.gitkraken.com/learn/git/tutorials/how-to-use-husky-git-hooks-tutorial).



### Cara Pakai Husky

Setelah Husky terinstal di proyek Anda, berikut adalah langkah-langkah untuk mengatur dan menggunakan Husky untuk menjalankan Githooks:

1. **Membuat Hook**:
   - Pertama, buat direktori untuk hook Anda, misalnya `src/hooks`.
   - Di dalam direktori ini, buat file untuk setiap hook yang ingin Anda gunakan, misalnya `pre-commit.js`.

2. **Mendaftarkan Hook di Husky**:
   - Buka file `package.json` proyek Anda, lalu tambahkan konfigurasi Husky seperti berikut:
     ```json
     "husky": {
       "hooks": {
         "pre-commit": "node src/hooks/pre-commit.js"
       }
     }
     ```
   Dalam contoh ini, Husky akan menjalankan skrip `pre-commit.js` setiap kali Anda mencoba melakukan commit.

3. **Menulis Kode Hook**:
   - Di dalam file hook (misalnya `pre-commit.js`), tulis kode yang ingin Anda jalankan. Misalnya, Anda mungkin ingin menjalankan ESLint pada file yang telah diubah:
     ```javascript
     const { execSync } = require('child_process');

     function run(command) {
       try {
         console.log(execSync(command).toString());
       } catch (error) {
         console.error(error.stdout.toString());
         process.exit(1);
       }
     }

     run('npx eslint . --fix');
     ```

4. **Menjalankan Hook**:
   - Sekarang, setiap kali Anda mencoba melakukan commit, Husky akan menjalankan hook `pre-commit` yang telah Anda tetapkan, menjalankan ESLint pada file yang telah diubah.

5. **Menyesuaikan atau Menambah Hook Lain**:
   - Anda dapat menambahkan lebih banyak hook atau menyesuaikan hook yang ada dengan cara yang sama. Cukup tambahkan entri baru ke bagian `hooks` di konfigurasi Husky di file `package.json` Anda, dan buat file hook terkait di direktori `src/hooks` atau di lokasi lain yang Anda pilih.




## GitHooks

Git hooks adalah skrip yang berjalan secara otomatis setiap kali suatu peristiwa tertentu terjadi di dalam repositori Git. Mereka memungkinkan Anda untuk menyesuaikan perilaku internal Git dan memicu tindakan yang dapat disesuaikan pada titik-titik kunci dalam siklus pengembangan.

Hooks yang dijalankan selama proses pembuatan commit
Kasus penggunaan umum untuk Git hooks meliputi mendorong kebijakan commit, mengubah lingkungan proyek tergantung pada kondisi repositori, dan mengimplementasikan alur kerja integrasi berkelanjutan. Namun, karena skrip dapat disesuaikan secara tak terbatas, Anda dapat menggunakan Git hooks untuk mengotomatisasi atau mengoptimalkan hampir semua aspek alur kerja pengembangan Anda.

### Penggunaan

1. **Navigasi ke Repositori Git Anda:**
   Buka terminal atau command prompt dan navigasi ke direktori repositori Git Anda.

2. **Buat atau Ubah Hook `pre-commit`:**
   Anda perlu membuat atau mengedit skrip hook `pre-commit`. Anda dapat melakukannya dengan mengikuti langkah-langkah berikut:

   a. Buka direktori `.git/hooks` dalam repositori Anda. Ini adalah direktori yang berisi semua hooks Git.

   b. Cari atau buat file bernama `pre-commit` (tanpa ekstensi). Jika file ini sudah ada, Anda dapat mengeditnya; jika tidak, Anda dapat membuatnya.

   c. Tambahkan skrip yang ingin Anda jalankan sebelum commit. Misalnya, berikut adalah contoh skrip sederhana untuk memeriksa sintaksis file PHP sebelum commit:

      ```bash
      #!/bin/sh
      php -l $(git rev-parse --show-toplevel)/$(git diff --cached --name-only) || exit 1
      ```

      Pastikan untuk memberikan izin eksekusi ke file `pre-commit`:

      ```bash
      chmod +x .git/hooks/pre-commit
      ```

3. **Uji Hook `pre-commit`:**
   Sekarang, hook `pre-commit` telah diatur. Saat Anda mencoba melakukan commit, skrip ini akan dijalankan sebelumnya. Anda dapat mencoba melakukan commit untuk melihat apakah skrip berfungsi dengan baik.

   ```bash
   git commit -m "Pesan commit Anda"
   ```

   Jika skrip melarang commit (misalnya, jika ada kesalahan dalam skrip atau pemeriksaan yang gagal), Anda harus memperbaiki masalah tersebut sebelum Anda dapat melakukan commit.

4. **Kustomisasi Hook `pre-commit`:**
   Anda dapat mengkustomisasi skrip `pre-commit` sesuai dengan kebutuhan Anda. Anda dapat menambahkan pemeriksaan lain, menjalankan tes, atau tindakan lain yang diperlukan sebelum commit dilakukan.

### Kelebihan dan kekurangan Githooks dibandingkan precommit lain

**Kelebihan Git Hooks (pre-commit):**

1. **Terintegrasi Dengan Git:**
   Git hooks adalah bagian dari Git itu sendiri, sehingga tidak memerlukan instalasi atau konfigurasi tambahan. Mereka sudah ada di dalam setiap repositori Git.

2. **Kustomisasi Tanpa Tambahan Alat:**
   Anda dapat mengkustomisasi hook `pre-commit` dengan mudah sesuai dengan kebutuhan proyek Anda tanpa harus menginstal alat tambahan. Ini membuatnya mudah digunakan dan didistribusikan dalam tim.

3. **Kendali Penuh:**
   Dengan Git hooks, Anda memiliki kendali penuh atas tindakan apa yang dijalankan sebelum commit. Anda dapat menentukan skrip yang tepat sesuai dengan kebijakan dan kebutuhan proyek Anda.

4. **Berjalan Secara Lokal:**
   Git hooks berjalan secara lokal di repositori setiap kali seseorang melakukan commit. Ini memungkinkan Anda untuk melakukan pemeriksaan sebelum commit terjadi tanpa ketergantungan pada server atau infrastruktur tambahan.

**Kekurangan Git Hooks (pre-commit):**

1. **Tidak Portable:**
   Git hooks spesifik untuk repositori tertentu. Jika Anda ingin menerapkan aturan yang sama di banyak repositori, Anda perlu mengkonfigurasi hook `pre-commit` di setiap repositori tersebut secara terpisah.

2. **Keterbatasan Bahasa dan Fungsionalitas:**
   Git hooks biasanya ditulis dalam shell script (biasanya bash) dan memiliki keterbatasan dalam hal bahasa dan fungsionalitas yang tersedia. Anda mungkin perlu menggunakan alat tambahan atau bahasa yang berbeda untuk tindakan yang lebih kompleks.

3. **Keterbatasan Sekuritas:**
   Jika pengembang memiliki akses langsung ke repositori Git, mereka dapat dengan mudah melewati atau mematikan Git hooks jika mereka ingin melakukannya. Ini dapat mengurangi keefektifan penerapan aturan.

4. **Kesulitan Pemeliharaan:**
   Dalam proyek yang besar atau dengan banyak repositori, pemeliharaan dan sinkronisasi hooks `pre-commit` dapat menjadi tantangan. Memastikan bahwa setiap repositori memiliki hook yang sesuai dengan kebijakan dapat menjadi pekerjaan tambahan.