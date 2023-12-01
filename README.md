# Lab9Web
**PHP Modular**
<hr>

**Instruksi Praktikum**
1. Persiapkan text editor misalnya VSCode.<br>
2. Buat folder baru dengan nama lab9_php_modular pada docroot webserver
(htdocs)<br>
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya
<hr>

# **1 & 2**
![image](https://github.com/Luxcario/Lab9Web/assets/116184002/61356b6d-3dc6-4c1d-b091-9fef8fd56367)
<br>
# **3. Langkah Praktikum**<br>
**Buat file baru dengan nama header.php**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Modularisasi</title>
    <link rel="sttylesheet" href="style.css" type="text/stylesheet" media="screen">
</head>
<body>
    <div class="container">
        <header>
            <h1>Modularisasi Menggunakan Require</h1>
        </header>
        <nav>
            <a href="home.php">Home</a>
            <a href="about.php">Tentang</a>
            <a href="contact.php">Kontak</a>
        </nav>
    </div>
</body>
</html>
```

![image](https://github.com/Luxcario/Lab9Web/assets/116184002/61befa61-ff12-4aa1-9c96-e0a4098b705a)

<hr>

**Buat file baru dengan nama footer.php**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div class="container">
        <footer>
            <p>&copy; 2021, Informatika, Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```
![image](https://github.com/Luxcario/Lab9Web/assets/116184002/63bf9eb5-61c6-4a22-aee5-82da6fe840ea)
<hr>

**Buat file baru dengan nama home.php**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php require('header.php');?>

    <div class="content"></div>
</body>
</html>
```
![image](https://github.com/Luxcario/Lab9Web/assets/116184002/af7d53a5-6286-4c5a-8666-c4babb65cbe9)

<hr>

**Buat file baru dengan nama about.php**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php require('header.php');?>

    <div class="content">
        <h2>Ini halaman Home</h2>
        <p>Ini adalah bagian content dari halaman.</p>
        <?php require ('footer.php');?>
    </div>
</body>
</html>
```
![image](https://github.com/Luxcario/Lab9Web/assets/116184002/959246a6-5e2f-4e39-a3c5-0420ccc4a82f)
<hr>

**CSS**
```
    <link rel="stylesheet" href="style.css" type="text/stylesheet" media="screen">
    <style>
        body{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        .container{
            display: block;
            align-items: center;
            justify-content: center;
            height: auto;
            background: #778899;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        }
        nav{
            background-color: rgb(211, 211, 211);
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        nav a{
            margin: 10px;
            color: green;
            font-size: 20px;
        }
    </style>
```
<br>
Untuk mengakses hasil gunakan URL : http://localhost/lab9_php_modular/ <br>
hasil
![image](https://github.com/Luxcario/Lab9Web/assets/116184002/9f541eb4-8231-4902-984c-3e2ce98f0436)
<hr>

**Pertanyaan dan Tugas**
Implementasikan konsep modularisasi pada kode program praktikum 8 tentang database, sehingga setiap halamannya memiliki template tampilan yang sama<br>
