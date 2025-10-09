# Operator Logika

Operator logika digunakan dalam PHP untuk **membandingkan dua atau lebih kondisi (ekspresi boolean)** dan menghasilkan **nilai** `**true**` **atau** `**false**`.

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
