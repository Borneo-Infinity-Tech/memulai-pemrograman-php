# Operator Logika

Operator logika digunakan dalam PHP untuk **membandingkan dua atau lebih kondisi (ekspresi boolean)** dan menghasilkan **nilai** `true` **atau** `false`.

Biasanya operator ini digunakan untuk menentukan kebenaran dari pernyataan majemuk, seperti “apakah dua kondisi sama-sama benar” atau “apakah salah satu kondisi benar”.

## Daftar Operator Logika PHP

### Operator `&&` dan `AND`

Operator ini akan menghasilkan **true** hanya jika **semua kondisi** bernilai **true**. Jika salah satu kondisi **false**, hasil akhirnya **false**.

**Contoh:**

```php
<?php
$a = true;
$b = true;
$c = false;

echo ($a && $b); // true
echo "<br>";
echo ($a && $c); // false
?>
```

### Operator `||` dan `OR`

Operator ini menghasilkan **true** jika **setidaknya satu** dari kondisi bernilai **true**. Hanya akan menghasilkan **false** jika **semua kondisi false**.

**Contoh:**

```php
<?php
$a = true;
$b = false;

echo ($a || $b); // true (karena salah satu benar)
echo "<br>";
echo ($b || false); // false (karena dua-duanya salah)
?>
```

### Operator `!` NOT

Operator ini berfungsi untuk **membalikkan nilai logika**. Jika nilai aslinya `true`, maka hasilnya `false`. Jika nilai aslinya `false`, maka hasilnya `true`.

**Contoh:**

```php
<?php
$a = true;
$b = false;

echo !$a; // false (karena dibalik)
echo "<br>";
echo !$b; // true (karena dibalik)
?>
```

## [Praktikum](/materi/011/praktikum-operator-logika.md)
