# Documenting

## Markdown

Referensi :
- [Panduan Lengkap Belajar Menulis dengan Markdown untuk Pemula](https://www.petanikode.com/markdown-pemula/)
- [Markdown: Apa itu, Cara dan Kenapa Menggunakannya](https://dewabiz.com/markdown/)

Markdown adalah bahasa markup yang ringan dan sederhana, dirancang untuk mempermudah penulisan dan membaca dokumen berbasis web. Dibuat oleh John Gruber pada tahun 2004, Markdown menggunakan sintaks pemformatan teks biasa, dengan tujuan untuk dikonversi menjadi format HTML terstruktur.

File Markdown dapat kita simpan dengan ekstensi `.markdown` atau `.md`. Contoh: `belajar-menulis.md` atau `belajar-menulis.markdown`.

Saat ini markdown sudah digunakan untuk:

- Dokumentasi
- SSG (Static Site Generator)
- CMS seperti Ghost, Wordpress, Tumblr, dll.
- Penulisan Buku
- Format teks pada chat: Telegram, WA, Facebook
- dll.

Berikut beberapa contoh dasar format Markdown:

### Editor untuk menulis markdown file
Untuk editornya biasanya _text editor_ atau IDE sudah memiliki bawaan untuk men-_generate_ markdown file. jika tidak ada, bisa install plugin atau ekstensi untuk menulis markdown file, seperti contoh pada visual studio code, kita bisa menambahkan ekstensi [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)

### Membuat Heading

Membuat Heading atau judul di markdown dapat dibuat dengan tanda pagar #. Contoh:
```
# Heading 1
## Heading 2
### Heading 3
```

hasilnya menjadi seperti :

# Heading 1
## Heading 2
### Heading 3
---

### _Styling text_

Untuk membuat teks miring kita bisa menggunakan karakter bintang `*` atau underscores `_` , seperti berikut: `*Text Miring*` atau `_Text Miring_`, hasilnya menjadi _Text Miring_.

Kamu bisa menggunakan dua bintang atau dua underscores untuk memformat teks secara tebal atau strong, seperti berikut: `**Teks Tebal**` atau `__Teks Tebal__`, hasilnya akan menjadi **Text Tebal**.


### Membuat List

Kamu bisa menggunakan bintang `*` atau strip `-` untuk membuat list dengan poin bulat, seperti berikut:
```
- Kuning
    - merah
- Biru
- Hijau
```
dan hasilnya :
- Kuning
    - Merah
- Biru
- Hijau

Dan dengan angka kamu bisa membuat ordered list, seperti berikut:
```
1. List Pertama
2. List Kedua
3. List Ketiga
```

dan hasilnya : 
1. List Pertama
2. List Kedua
3. List Ketiga

### _Hyperlink_

Jika kamu ingin membuat link atau dalam tag html `<a>` gunakan sintaks berikut: `[Text Link](https://youtube.com)`, dan hasilnya menjadi [Text Link](https://youtube.com). Atau kita juga bisa menulis link-nya secara langsung seperti `https://youtube.com` jika kita ingin menulis tanpa _alternative text_, hasilnya seperti : https://youtube.com


### Menyisipkan Gambar

Dan untuk menampilkan gambar kamu bisa menggunakan sintaks berikut: `![alt text](https://unair.ac.id/wp-content/uploads/2022/08/kucing.jpg)`. hasilnya menjadi ![alt text](https://unair.ac.id/wp-content/uploads/2022/08/kucing.jpg)

### Membuat Kutipan
Pada HTML, kita mengenal tag `<blockquote>` untuk membuat kutipan. Pada markdown, kita bisa membuatnya seperti ini: 
```
> To be or not to be, that is the question.
```
dan hasilnya menjadi :

> To be or not to be, that is the question.

### Menulis _Inline Code_
Inline code sangat sering digunakan dalam teks. Cara membuatnya adalah seperti
```
`apt-get`
```

dan hasilnya menjadi : `apt-get`

### Menulis _Source Code_
Source code sering ditulis dengan markdown. Lalu menggunakan **Prism.js** untuk syntax higlighting.

```
    ```java
    public class HelloWorld {
        public static void main(String[] argumen){
            System.out.println("Hello World!");
        }
    }
    ```
```

dan hasilnya menjadi :
```java
public class HelloWorld {
    public static void main(String[] argumen){
        System.out.println("Hello World!");
    }
}
```

Tanda ``` berfungsi untuk menulis _source code_. Lalu pada pembuka kita tambahkan nama bahasanya agar teksnya berwarna (__syntax highligting__).

### Membuat Tabel
Tabel di markdown dapat dibuat dengan cara sperti ini:
```
| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |
```

dan hasilnya menjadi :
| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |

### Membuat Garis Horizontal
Garis horizontal atau `<hr>`, dapat kita buat dengan tanda `---`.

contoh :

```
ini adalah paragraf

---

ini paragraf ke dua
```

dan hasilnya :

ini adalah paragraf

---

ini paragraf ke dua

## Confluence

Confluence adalah salah satu bagian dari Atlassian Suite, yaitu sebuah perusahaan di Australia yang berfokus dalam pengembangan 
perangkat lunak, manajemen konten, dan sebagainya. Confluence adalah sebuah aplikasi yang memungkinkan penggunanya untuk 
melakukan kolaborasi dan berbagi pengetahuan secara efisien. Aplikasi ini memungkinkan penggunanya untuk menulis, mengedit, memberikan komentar, dan menyelesaikan pekerjaan secara bersamaan 
di dalam interface Confluence.

Pada dasarnya Confluence tidak berbeda jauh dengan Google Docs. Akan tetapi, dalam hal berkolaborasi aplikasi ini lebih luas 
dibandingkan dengan Google Docs. Perbedaan antara Confluence dan Google Docs juga terletak dalam struktur halaman depannya. 
Confluence juga menyediakan fitur mention, like, dan berbagi komentar di dalam satu dokumen sehingga kamu dan rekan timmu dapat langsung berdiskusi untuk mengubah konten.

### Kelebihan

- _Tools_ yang hebat untuk pekerjaan kolaborasi bersama
- Mengintegrasikan semua halaman dan informasi
- Menawarkan sejumlah besar _template_ dan makro untuk menyederhanakan tugas
- Opsi kontrol akses dan izin yang kuat

### Kekurangan

- Fungsionalitas tingkat lanjut bisa jadi agak mahal
- Beberapa fitur yang dibutuhkan hanya tersedia sebagai plugin berbayar
- Pengguna mungkin merasa kesulitan untuk menyesuaikan dan beradaptasi dengan _software interface_

### Referensi

- [Confluence: Aplikasi Penunjang Kolaborasi Para Pekerja](https://glints.com/id/lowongan/confluence-adalah/)
- [Confluence Review 2023: Features, Pros And Cons](https://www.forbes.com/advisor/business/software/confluence-review/)
