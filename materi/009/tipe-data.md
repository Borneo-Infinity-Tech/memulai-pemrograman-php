# Tipe Data

**Tipe data** adalah **klasifikasi nilai** yang menentukan **bentuk data** dan **operasi** apa saja yang bisa dilakukan pada data tersebut.

Contoh sederhana:

- Angka `10` → bisa dijumlahkan (`10 + 5`).
- Teks `"10"` → dianggap string, sehingga kalau dijumlahkan dengan teks lain akan digabung (`"10" . "5"` → `"105"`).

Jadi, tipe data penting supaya komputer tahu cara memperlakukan sebuah nilai.

Dalam PHP, tipe data ditentukan secara otomatis (dynamic typing). Artinya, kita tidak perlu menulis `int x = 10;` seperti di Java/C, cukup tulis `$x = 10;` dan PHP akan menganggapnya integer.

## **Tipe Data Dasar di PHP**

### Integer

Tipe data berupa bilangan bulat, positif, negatif, atau nol.

**Contoh nilai:** `-5`, `0`, `42`, `2025`

**Contoh kode:**

```php
<?php
$umur = 21;
var_dump($umur); // int(21)
?>
```

### Float (atau Double)

Tipe data angka pecahan atau bilangan desimal.

**Contoh nilai:** `3.14`, `-0.5`, `2.5e3` (artinya 2500)

**Contoh kode:**

```php
<?php
$pi = 3.14;
$diskon = 0.15;
var_dump($pi, $diskon);
?>
```

### String

Tipe data yang berisi teks, kumpulan karakter.

**Contoh nilai:** `"Halo"`, `'PHP'`, `"123"` (walau isinya angka, tapi dianggap teks).

**Contoh kode:**

```php
<?php
$nama = "Rani";
$pesan = 'Belajar PHP';
var_dump($nama, $pesan);
?>
```

### Boolean

Tipe data logika, hanya punya dua kemungkinan: **benar** (`true`) atau **salah** (`false`).

**Contoh nilai:** `true`, `false`

**Contoh kode:**

```php
<?php
$isStudent = true;
$isAdmin = false;
var_dump($isStudent, $isAdmin);
?>
```

### Null

Tipe data khusus yang berarti **tidak ada nilai**.

**Contoh nilai:** `null`

**Contoh kode:**

```php
<?php
$data = null;
var_dump($data); // NULL
?>
```

## Referensi Tambahan Materi

- [w3schools PHP Data Type](https://www.w3schools.com/php/php_datatypes.asp)
- [geekforgeeks.org PHP Data Type](https://www.geeksforgeeks.org/php/php-data-types/)
