# Lab7Web
# Pemograman Web
~~~
Nama   = Endrik
NIM    = 311910088
Kelas  = TI.19.C.1
Universitas Pelita Bangsa
~~~
# Langkah-langkah Praktikum
Download aplikasi XAMPP
pilih versi portable untuk memudahkan proses installasi. Kemudian extract file tersebut, seusikan direktorinya (misal: d:\xampp).

# Menjalankan Web Server 
Untuk menjalankan web server dari menu XAMPP Control.

Foto

Uji coba apakah server sudah berkerja dengan baik http://127.0.0.1 atau http://localhost Tampil halaman utama XAMPP jika server sudah berkerja dengan baik. • Dokumen Website Semua file website tempatkan di direktori: \xampp\htdocs
• Database MySQL Direktori: \xampp\mysql
Manajemen database: http://localhost/phpmyadmin

# Memulai PHP 
Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)
Foto 

Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL: http://localhost/lab7_php_dasar/

Foto 

# PHP Dasar 

Buat file baru dengan nama php_dasar.php pada directory tersebut. Kemudian buat kode seperti berikut.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
</body>
</html>
~~~
