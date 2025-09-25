# Operator Penugasan (Assignment)

Operator penugasan digunakan untuk memberi nilai ke variabel. Bentuk paling dasar adalah `=`, sementara bentuk gabungan (seperti `+=`, `.=`) menjalankan operasi lalu menugaskan hasilnya kembali ke variabel yang sama.

**Contoh**

```php
<?php
$x = 10;      // x menjadi 10
$x = $x + 3;  // x menjadi 13 (setelah penjumlahan manual)
$x += 3;      // cara singkat: sama dengan x = x + 3
?>
```

## Daftar Operator Penugasan di PHP

### 1) Penugasan dasar

`=` menetapkan nilai kanan ke variabel kiri.

```php
<?php
$a = 5;
$b = $a;      // b menjadi 5
?>
```

### 2) Gabungan aritmatika

Dipakai untuk hitung lalu simpan kembali ke variabel yang sama.

- `+=` tambah
- `-=` kurang
- `*=` kali
- `/=` bagi
- `%=` sisa bagi
- `**=` pangkat

**Contoh**

```php
<?php
$x = 10;

$x += 5;   // 15   (x = x + 5)
$x *= 2;   // 30   (x = x * 2)
$x /= 4;   // 7.5  (bisa jadi float)
$x %= 3;   // 1    (sisa bagi)

$y = 2; $y **= 3; // 8
?>
```

### 3) Gabungan String

Dipakai untuk menyambung string. `.=` (concat & simpan lagi)

**Contoh**

```php
<?php
$s = "Halo";
$s .= ", Indira";   // "Halo, Indira"
$s .= "!";        // "Halo, Indira!"
?>
```
