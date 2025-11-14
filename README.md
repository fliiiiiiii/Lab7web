# 🖥️ Praktikum Pemrograman Web - PHP Dasar
**Nama:** Rafli Anugrah Ramadhan 
**NIM:** 312410351  
**Kelas:** TI 24A4  
**Mata Kuliah:** Pemrograman Web  
**Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom. 

## 📸 Tampilan Program

1. Memulai PHP

<img width="224" height="103" alt="image" src="https://github.com/user-attachments/assets/2160655b-42a3-46fb-94ab-196541f6d80c" />

2. PHP Dasar

KODE:

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
</body>
</html>
```
HASIL:

<img width="208" height="88" alt="image" src="https://github.com/user-attachments/assets/adc7f54c-f6b2-4901-a72e-11f1a73ed1ae" />

3.  VARIABLE PHP

KODE:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>

    <?php
    // Menampilkan teks Hello World
    echo "Hello World<br>";

    // Menampilkan subjudul di bawah Hello World
    echo "<h2>Menggunakan Variabel</h2>";

    // Deklarasi variabel
    $nim = "312410351";
    $nama = "Rafli Anugrah";

    // Menampilkan isi variabel
    echo "NIM : " . $nim . "<br>";
    echo "Nama : " . $nama;
    ?>
</body>
</html>
```

HASIL:

<img width="196" height="86" alt="image" src="https://github.com/user-attachments/assets/d10f3cde-56b7-4773-a01a-dc2e37e7261d" />


4. PREDEFINE VARIABLE

KODE:

``` html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Predefine Variable</title>
</head>
<body>
    <h1>Predefine Variable</h1>

    <?php
    if (isset($_GET['nama'])) {
        echo 'Selamat Datang ' . $_GET['nama'];
    } else {
        echo 'Selamat Datang, Rafli Anugrah!';
    }
    ?>
</body>
</html>
```

HASIL:

<img width="203" height="110" alt="image" src="https://github.com/user-attachments/assets/12c06997-eb0b-46ed-ab0f-892682f831dc" />

5. FROM INPUT

KODE:

``` html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Form Input</title>
</head>
<body>
    <h2>Form Input</h2>

    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>

    <?php
    // Menampilkan teks di bawah form
    echo 'Selamat Datang Rafli Anugrah';
    ?>
</body>
</html>
```

HASIL:

<img width="209" height="101" alt="image" src="https://github.com/user-attachments/assets/2d920046-4d82-405e-b223-fcf090190f61" />

6. OPERATOR, KONDISI IF, KONDISI SWITCH, PERULANGAN FOR

KODE:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Operator</title>
</head>
<body>
    <h2>Operator</h2>
    <?php
    $gaji = 1000000;
    $pajak = 0.1;
    $thp = $gaji - ($gaji * $pajak);
    echo "Gaji sebelum pajak = Rp. $gaji <br>";
    echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
</body>
</html>



<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Kondisi IF</title>
</head>
<body>
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
</body>
</html>



<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Kondisi Switch</title>
</head>
<body>
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
</body>
</html>



<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan For</title>
</head>
<body>
    <h2>Perulangan For</h2>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    for ($i = 1; $i <= 10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
    }

    echo "<br>Perulangan Menurun dari 10 ke 1 <br />";
    for ($i = 10; $i >= 1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    ?>
</body>
</html>
```

HASIL:

<img width="507" height="533" alt="image" src="https://github.com/user-attachments/assets/3fd3b402-a8ca-4ff2-9436-ada86ef3b8ce" />

7. PERULANGAN WHILE

``` html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan While</title>
</head>
<body>
    <h2>Perulangan While</h2>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i = 1;
    while ($i <= 10) {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    }
    ?>
</body>
</html>
```

HASIL:

<img width="172" height="185" alt="image" src="https://github.com/user-attachments/assets/bdbed136-79fa-4bc7-a7b0-8b06e9cf1ccd" />

8. PERULANGAN DO WHILE

KODE:

```hmtl
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Perulangan Do While</title>
</head>
<body>
    <h2>Perulangan Do...While</h2>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i = 1;
    do {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    } while ($i <= 10);
    ?>
</body>
</html>
```

HASIL:

<img width="218" height="181" alt="image" src="https://github.com/user-attachments/assets/acadec0c-b159-4f51-b275-0355f1edb3a0" />

9. FORM INPUT DATA DIRI

KODE:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Program PHP - Data Diri</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            background: #f2f2f2;
        }
        h2 {
            color: #333;
        }
        form {
            background: white;
            padding: 20px;
            border-radius: 10px;
            width: 350px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        label {
            display: block;
            margin-top: 10px;
        }
        input, select, button {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }
        .result {
            margin-top: 30px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            width: 350px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>

<h2>Form Input Data Diri</h2>

<form method="post" action="">
    <label>Nama:</label>
    <input type="text" name="nama" required>

    <label>Tanggal Lahir:</label>
    <input type="date" name="tanggal_lahir" required>

    <label>Pekerjaan:</label>
    <select name="pekerjaan" required>
        <option value="">-- Pilih Pekerjaan --</option>
        <option value="Programmer">Programmer</option>
        <option value="Desainer">Desainer</option>
        <option value="Data Analyst">Data Analyst</option>
        <option value="Guru">Guru</option>
        <option value="Dokter">Dokter</option>
    </select>

    <button type="submit" name="submit">Tampilkan</button>
</form>

<?php
if (isset($_POST['submit'])) {
    $nama = $_POST['nama'];
    $tgl_lahir = $_POST['tanggal_lahir'];
    $pekerjaan = $_POST['pekerjaan'];

    // Hitung umur
    $lahir = new DateTime($tgl_lahir);
    $hari_ini = new DateTime();
    $umur = $hari_ini->diff($lahir)->y;

    // Tentukan gaji berdasarkan pekerjaan
    switch ($pekerjaan) {
        case "Programmer":
            $gaji = 10000000;
            break;
        case "Desainer":
            $gaji = 8000000;
            break;
        case "Data Analyst":
            $gaji = 12000000;
            break;
        case "Guru":
            $gaji = 6000000;
            break;
        case "Dokter":
            $gaji = 15000000;
            break;
        default:
            $gaji = 0;
    }

    echo "<div class='result'>";
    echo "<h3>Hasil Data Diri</h3>";
    echo "Nama: <b>$nama</b><br>";
    echo "Tanggal Lahir: <b>" . date("d-m-Y", strtotime($tgl_lahir)) . "</b><br>";
    echo "Umur: <b>$umur tahun</b><br>";
    echo "Pekerjaan: <b>$pekerjaan</b><br>";
    echo "Gaji: <b>Rp " . number_format($gaji, 0, ',', '.') . "</b>";
    echo "</div>";
}
?>

</body>
</html>
```

HASIL:

<img width="322" height="478" alt="image" src="https://github.com/user-attachments/assets/147ffa90-046c-47fa-8a64-73891326fc1d" />


## 📚 Deskripsi

Repository ini berisi kumpulan program dasar **PHP** yang digunakan untuk memahami konsep fundamental dalam pemrograman web berbasis server.  
Setiap file berisi topik dan konsep berbeda, mulai dari penggunaan variabel, operator, kondisi, perulangan, hingga form input data diri dengan perhitungan otomatis.

---

## 📂 Daftar File

| No | Nama File | Deskripsi |
|----|------------|-----------|
| 1 | **phpdasar.php** | Menampilkan teks “Hello World” dan penggunaan variabel. |
| 2 | **predefine.php** | Menampilkan penggunaan variabel predefine `$_GET`. |
| 3 | **forminput.php** | Menampilkan form input sederhana dengan output teks. |
| 4 | **operator.php** | Contoh operasi aritmatika sederhana dalam PHP. |
| 5 | **kondisi_if.php** | Contoh penggunaan pernyataan `if`, `elseif`, dan `else`. |
| 6 | **kondisi_switch.php** | Contoh penggunaan pernyataan `switch`. |
| 7 | **perulangan_for.php** | Contoh perulangan `for` naik dan menurun. |
| 8 | **perulangan_while.php** | Contoh perulangan menggunakan `while`. |
| 9 | **perulangan_dowhile.php** | Contoh perulangan menggunakan `do...while`. |
| 10 | **datadiri.php** | Program utama: form input nama, tanggal lahir, dan pekerjaan yang menampilkan hasil umur serta gaji. |

---

## 💡 Penjelasan Singkat Program Utama (Data Diri)

Program **Data Diri** merupakan latihan integrasi beberapa konsep PHP:
- **Form Input (POST Method)** untuk mengambil data dari user.  
- **Pengolahan Data** seperti perhitungan umur otomatis berdasarkan tanggal lahir.  
- **Kondisi Switch** untuk menentukan gaji berdasarkan pilihan pekerjaan.  
- **Output Dinamis** yang menampilkan hasil dalam bentuk tabel rapi.

### 💼 Daftar Gaji Berdasarkan Pekerjaan:
| Pekerjaan | Gaji (Rp) |
|------------|------------|
| Programmer | 10.000.000 |
| Desainer | 8.000.000 |
| Data Analyst | 12.000.000 |
| Guru | 6.000.000 |
| Dokter | 15.000.000 |

---

## ⚙️ Cara Menjalankan Program

1. Simpan semua file `.php` ke dalam folder `htdocs` (misalnya `C:\xampp\htdocs\phpdasar`).
2. Jalankan **XAMPP**, lalu aktifkan **Apache**.
3. Buka browser dan ketik:

























































