# Operator Aritmatika

Operator aritmatika adalah simbol yang melakukan operasi matematika pada operand (nilai/variabel). Di PHP, operator ini bekerja pada **integer** dan **float (double)**. Hasil operasi mengikuti tipe data operand misalnya, jika ada salah satu float, hasil umumnya float.

## Daftar Operator Aritmatika

### 1) Penjumlahan `+`

Menjumlahkan dua nilai.

```php
<?php
$a = 10;
$b = 2.5;

echo $a + $b;
// Output: 12.5 (float, karena ada float)
?>
```

### 2) Pengurangan `-`

Mengurangkan dua nilai.

```php
<?php
echo 7 - 4;
// Output 3
?>
```

### 3) Perkalian `*`

Mengalikan dua nilai.

```php
<?php
echo 6 * 3;
// Output 18
?>
```

### 4) Pembagian `/`

Membagi dua nilai.

```php
<?php
echo 7 / 2;  // Output: 3.5 (berbentuk float)
echo 8 / 2; // 4
?>
```

### 5) Modulus (sisa bagi) `%`

Mengembalikan sisa dari pembagian bilangan bulat.

```php
<?php
echo 10 % 3;
// Output 1
?>
```

**Catatan:** Hanya bermakna untuk tipe data integer.

### 6) Pangkat `**`

Memangkatkan nilai kiri dengan eksponen di kanan.

```php
<?php
echo 2**3; // 2 pangkat 3, Output: 8
echo 5**2; // Output: 25
?>
```

## Contoh Lengkap

### Aritmatika dasar

```php
<?php
$a = 15;
$b = 4;
echo $a + $b; // Output: 19
echo $a - $b; // Output: 11
echo $a * $b; // Output: 60
echo $a / $b; // Output: 3.75
echo $a % $b; // Output: 3
?>
```

### Pangkat & Pengelompokan

```php
<?php
echo (5 + 2) / 3; // Output: 2.333
echo (10 + 3) - 1 * 2; // Output: 11

echo 2 ** 4; // Output: 16
echo 3 ** 3; // Output: 27
?>
```

### Membuat Kalkulator Sederhana

```php
<?php
$angka1 = readline("Masukkan Angka Pertama: ");
$angka2 = readline("Masukkan Angka Kedua: ");

$jumlah = $angka1 + $angka2;
$kurang = $angka1 - $angka2;
$kali = $angka1 * $angka2;
$bagi = $angka1 / $angka2;
$modulus = $angka1 % $angka2;

echo "Hasil Penjumlahan = $jumlah \n";
echo "Hasil Pengurangan = $kurang \n";
echo "Hasil Perkalian = $kali \n";
echo "Hasil Pembagian = $bagi \n";
echo "Sisa Hasil Bagi = $modulus \n";
?>
```

- ### [Praktikum](/materi/011/praktikum-operator-aritmatika.md)
- ### [Praktikum 2](/materi/011/praktikum-operator-aritmatika-2.md)

