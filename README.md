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
![Screenshot_20210515-061020_Chrome](https://user-images.githubusercontent.com/81820421/118347702-637bff00-b56f-11eb-8c86-e8a75ded4879.jpg)


Uji coba apakah server sudah berkerja dengan baik http://127.0.0.1 atau http://localhost Tampil halaman utama XAMPP jika server sudah berkerja dengan baik. • Dokumen Website Semua file website tempatkan di direktori: \xampp\htdocs
• Database MySQL Direktori: \xampp\mysql
Manajemen database: http://localhost/phpmyadmin

# Memulai PHP 
Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)
![Screenshot_20210515-121005_Chrome](https://user-images.githubusercontent.com/81820421/118348769-a4c3dd00-b576-11eb-8b2c-8551dfff060b.jpg)


Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL: http://localhost/lab7_php_dasar/
![Screenshot_20210515-130030_Chrome](https://user-images.githubusercontent.com/81820421/118349887-a9d85a80-b57d-11eb-9c14-f5feadc23b61.jpg)


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
Kemudian untuk mengakses hasilnya melalui URL: http://localhost/lab7_php_dasar/php_dasar.php

![Screenshot_20210515-130259_Chrome](https://user-images.githubusercontent.com/81820421/118349921-ed32c900-b57d-11eb-8a34-0fc63019dd4b.jpg)

# Variabel PHP 
Menambahkan variable pada program.

![Screenshot_20210515-130403_Chrome](https://user-images.githubusercontent.com/81820421/118349948-0fc4e200-b57e-11eb-9ac3-0c5765c6d3be.jpg)

# Predefine variabel Get $
~~~
<h2>Predefine Variable</h2>
    <?php 
        echo 'Selamat Datang ' . $_GET['nama'];
    ?>
~~~

![20210515_130745](https://user-images.githubusercontent.com/81820421/118350010-9974af80-b57e-11eb-9c2e-05ef01338fa7.jpg)


# Membuat Form Input 
~~~
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>PHP Dasar</title>
    </head>
    <body>
    <h2>Form Input</h2>
    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
    <?php
        echo 'Selamat Datang' . $_POST['nama'];
    ?>
    </body>
</html>
~~~
![20210515_132426](https://user-images.githubusercontent.com/81820421/118350455-f709fb80-b580-11eb-8ab9-afae80afe6b3.jpg)



# Operator 
~~~ 
<h2>Operator</h2>
    <?php
        $gaji = 1000000;
        $pajak = 0.1;
        $thp = $gaji - ($gaji*$pajak);
            echo "Gaji sebelum pajak = Rp. $gaji <br>";
            echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>

~~~ 

![20210515_132642](https://user-images.githubusercontent.com/81820421/118350504-4a7c4980-b581-11eb-8e58-ab5f17d0a08f.jpg)



# Kondisi IF 
~~~
<h2>Kondisi IF</h2>
    <?php
        $nama_hari = date("l");
            if ($nama_hari == "Sunday") {
        echo "Minggu";
            } elseif ($nama_hari == "Monday") {
        echo "Senin";
            } else {
        echo "Selasa";
        }
    ?>
~~~



# Kondisi switch 
~~~
<h2>Kondisi Switch</h2>
    <?php
        $nama_hari = date("l");
            switch ($nama_hari) {
            case "Sunday":
        echo "Minggu";
            break;
            case "Monday":
    echo "Senin";
            break;
            case "Tuesday":
    echo "Selasa";
            break;
            default:
    echo "Sabtu";
            }
    ?>
~~~
![20210515_132838](https://user-images.githubusercontent.com/81820421/118350545-90391200-b581-11eb-9b27-0630bdee511a.jpg)

# Kondisi perulangan For 
~~~ 
<h2>Perulangan For</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
        }
        echo "Perulangan Menurun dari 10 ke 1 <br />";
            for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
        }
    ?>
~~~

![20210515_133151](https://user-images.githubusercontent.com/81820421/118350646-21a88400-b582-11eb-86ff-326c64ce22a7.jpg)


# Perulangan While 

~~~
 <h2>Perulangan While</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
        }
    ?>
~~~

Foto 

# Perulangan Dowhile
~~~

<h2>Perulangan Dowhile</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            do {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
            } while ($i<=10);
    ?>
~~~
![Screenshot_20210515-133359_Chrome](https://user-images.githubusercontent.com/81820421/118350674-46046080-b582-11eb-8cff-82722b46ee81.jpg)


# Pertanyaan dan Tugas 
Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir. Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.

~~~
<h2>Tugas</h2>
    <form method="post">
            <label>Nama Lengkap: </label>
            <input type="text" name="nama">
            <br>
            <label>Tempat Lahir: </label>
            <input type="text" name="tempat_lahir">
            <br>
            <label>Tanggal Lahir: </label>
            <input type="date" name="tgl_lahir">
            <br>
            <label>Alamat: </label>
            <input type="text" name="alamat">
            <br>
            <label>Pekerjaan:
            <select name='pekerjaan'>
                <option value='Programmer'>Prgrammer</option>
                <option value='Software Enginer'>Software Enginer</option>
                <option value='IT Konsultan'>IT Konsultan</option>
                <option value='Database Enginer'>Database Enginer</option>
            </select>
            </label>
            <br>
            <input type="submit" value="Kirim">
    </form>
    <h2>Output</h2>
    <?php
        echo '<br> Nama Lengkap : ' . $_POST['nama'];
        echo '<br> Tempat Lahir : ' . $_POST['tempat_lahir'];
        echo '<br> Alamat : ' . $_POST['alamat'];
            $tgl_lahir = @$_POST['tgl_lahir'];
            $lahir = new DateTime($tgl_lahir);
            $hari_ini = new DateTime();
            $diff = $hari_ini->diff($lahir);
        echo "<br> Usia : ". $diff->y ." Tahun";
        echo "<br> Pekerjaan : ". $_POST['pekerjaan'];
            $pekerjaan = @$_POST['pekerjaan'];
            if($pekerjaan == "Prgrammer"){
                echo '<br> Gaji : Rp. 10.000.000,-';
            }
            elseif($pekerjaan == "Software Enginer"){
                echo '<br> Gaji : Rp. 19.500.000,-';
            }
            elseif($pekerjaan == "IT Konsultan"){
                echo '<br> Gaji : Rp. 14.000.000,-';
            }
            elseif($pekerjaan == "Database Enginer"){
                echo '<br> Gaji : Rp. 12.000.000,-';
            }
    ?>
~~~

![20210515_133614](https://user-images.githubusercontent.com/81820421/118350746-a85d6100-b582-11eb-970f-378a87c5a078.jpg)











