Selamat datang! Di bawah ini, saya akan memberikan tutorial lengkap untuk HTML dan CSS dasar, dilengkapi dengan studi kasus sederhana untuk menggambarkan bagaimana HTML dan CSS dapat digunakan bersama-sama untuk membuat tampilan website yang menarik. Tutorial ini akan mencakup langkah-langkah dasar untuk membuat struktur HTML, menggabungkan CSS untuk mengatur tampilan, dan studi kasus sederhana untuk menggambarkan penerapan keduanya. Mari kita mulai!

## Bagian 1: Pengenalan HTML

HTML (HyperText Markup Language) adalah bahasa markup yang digunakan untuk membangun struktur dasar sebuah halaman web. Hal ini memungkinkan kita untuk menentukan elemen-elemen pada halaman dan bagaimana elemen-elemen tersebut berinteraksi satu sama lain.

### Langkah 1: Membuat Struktur Dasar HTML

Buatlah sebuah file dengan ekstensi `.html`. Kami akan menyebutnya sebagai `index.html`. Struktur dasar HTML terdiri dari elemen `<html>`, `<head>`, dan `<body>`.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Website</title>
</head>
<body>

</body>
</html>
```

### Langkah 2: Menambahkan Konten ke Halaman

Kita bisa menambahkan berbagai elemen ke dalam `<body>` untuk membangun konten pada halaman. Contoh berikut menambahkan sebuah judul, sebuah paragraf, dan sebuah gambar:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Website</title>
</head>
<body>
    <h1>Selamat Datang di Contoh Website</h1>
    <p>Ini adalah contoh paragraf. Silakan ganti dengan konten yang sesuai.</p>
    <img src="gambar-contoh.jpg" alt="Gambar Contoh">
</body>
</html>
```

## Bagian 2: Pengenalan CSS

CSS (Cascading Style Sheets) digunakan untuk mengatur tampilan dari elemen-elemen HTML. Dengan CSS, kita bisa mengubah warna, ukuran, letak, dan berbagai aspek tampilan lainnya.

### Langkah 3: Menerapkan CSS Internal

Kita bisa menggunakan CSS internal dengan menambahkan elemen `<style>` di dalam bagian `<head>` dari dokumen HTML.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Website</title>
    <style>
        h1 {
            color: blue;
            text-align: center;
        }

        p {
            font-size: 18px;
        }

        img {
            display: block;
            margin: 0 auto;
        }
    </style>
</head>
<body>
    <h1>Selamat Datang di Contoh Website</h1>
    <p>Ini adalah contoh paragraf dengan tampilan yang berbeda.</p>
    <img src="gambar-contoh.jpg" alt="Gambar Contoh">
</body>
</html>
```

### Langkah 4: Menerapkan CSS Eksternal

Alternatifnya, kita bisa menggunakan CSS eksternal dengan membuat file terpisah dengan ekstensi `.css`. Kami akan menyebutnya sebagai `style.css`. File ini kemudian akan dihubungkan dengan dokumen HTML menggunakan elemen `<link>`.

Buatlah file baru dengan nama `style.css` dan tambahkan kode berikut:

```css
/* style.css */

h1 {
    color: blue;
    text-align: center;
}

p {
    font-size: 18px;
}

img {
    display: block;
    margin: 0 auto;
}
```

Kemudian, pada `index.html`, tambahkan elemen `<link>` untuk menghubungkan file CSS tersebut:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Selamat Datang di Contoh Website</h1>
    <p>Ini adalah contoh paragraf dengan tampilan yang berbeda.</p>
    <img src="gambar-contoh.jpg" alt="Gambar Contoh">
</body>
</html>
```

## Studi Kasus: Membuat Halaman Portofolio Sederhana

Sekarang, kita akan mencoba membuat halaman portofolio sederhana menggunakan HTML dan CSS. Halaman ini akan memiliki beberapa bagian seperti header, daftar portofolio, dan kontak.

### Langkah 5: Membuat Struktur Halaman

Buatlah file baru dengan nama `portfolio.html` dan gunakan kode berikut sebagai struktur halaman:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Portofolio Saya</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Portofolio Saya</h1>
        <nav>
            <ul>
                <li><a href="#home">Beranda</a></li>
                <li><a href="#portofolio">Portofolio</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Halo, Selamat Datang di Portofolio Saya</h2>
        <p>Selamat datang di halaman portofolio saya. Ini adalah tempat saya memamerkan proyek-proyek yang telah saya kerjakan.</p>
    </section>

    <section id="portofolio">
        <h2>Portofolio</h2>
        <!-- Tambahkan proyek-proyek Anda di sini -->
    </section>

    <section id="kontak">
        <h2>Kontak</h2>
        <p>Jika Anda tertarik bekerja sama, silakan hubungi saya melalui email: example@example.com</p>
    </section>
</body>
</html>
```

### Langkah 6: Menerapkan Tampilan dengan CSS

Gunakan file `style.css` yang sudah dibuat sebelumnya untuk mengatur tampilan halaman portofolio. Berikut ini adalah contoh CSS untuk mengatur tampilan header dan beberapa elemen lainnya:

```css
/* style.css */

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    padding: 10px;
    text-align: center;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}



nav ul li a {
    color: #fff;
    text-decoration: none;
}

section {
    padding: 20px;
}

section h2 {
    border-bottom: 2px solid #333;
    padding-bottom: 10px;
}
```

