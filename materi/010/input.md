# Input CLI di PHP

## Apa itu Input CLI?

**CLI (Command Line Interface)** adalah cara menjalankan program lewat **terminal / command prompt**, bukan lewat browser. Di PHP, kita bisa meminta pengguna mengetik sesuatu saat program berjalan, lalu membaca input tersebut ke dalam variabel.

## Fungsi `readline()`

Fungsi bawaan PHP untuk membaca input dari CLI.

Bentuk umum:

```php
$variabel = readline("Pesan untuk user: ");
```

Cara Kerja:

1. Menampilkan teks prompt ke layar.
2. Program menunggu sampai user mengetik.
3. Nilai yang diketik user (string) disimpan ke variabel.

**Contoh:**

```php
<?php
$nama = readline("Masukkan nama Anda: ");
echo "Halo, $nama!\n";
?>
```

Kalau user ketik `Indira`, maka output:

```
Masukkan nama Anda: Indira
Halo, Indira!
```

## Tipe Data Input

Semua input dari `readline()` selalu berupa string.

Kalau ingin jadi angka (`int` atau `float`), perlu dikonversi (casting).

```php
<?php
$umur = readline("Masukkan umur: ");  // masih string
$umur = (int)$umur;                  // ubah jadi integer

$tinggi = (float)readline("Masukkan tinggi badan: "); // langsung float

var_dump($umur, $tinggi);
?>
```

Jika user ketik `20` dan `165.5`, output:

```
int(20)
float(165.5)
```

## Membaca Beberapa Input

Kita bisa panggil `readline()` lebih dari sekali untuk ambil banyak data.

```php
<?php
$nama = readline("Masukkan Nama: ");
$umur = (int)readline("Masukkan Umur: ");
echo "Nama Anda {$nama}, umur {$umur} tahun.\n";
?>
```

---

## Mari Mencoba

Buat file PHP dengan berisi kode berikut.

```php
<?php
$nama = readline("Masukkan Nama: ");
$umur = (int)readline("Masukkan Umur: ");
$tinggi = (float)readline("Masukkan Tinggi badan: ");

echo "Halo $nama!\n";
echo "Umur: $umur tahun\n";
echo "Tinggi: $tinggi cm\n";
?>
```

Jalankan kode PHP tersebut. Apa yang tampil di prompt ?

## Referensi Tambahan

- [PHP readline() Function](https://www.geeksforgeeks.org/php/php-readline-function/)

---

## [Praktikum](praktikum.md)
