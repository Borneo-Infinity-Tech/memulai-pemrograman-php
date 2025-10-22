# `if` Statement

## Pendahuluan

Dalam pemrograman, sering kali kita perlu membuat keputusan berdasarkan suatu **kondisi**. Misalnya:

- Jika nilai lebih dari 70, maka tampilkan “Lulus”.
- Jika umur lebih dari 17, maka tampilkan “Dewasa”.

Untuk membuat logika semacam ini di PHP, kita menggunakan **if statement** — yaitu struktur yang memungkinkan program menjalankan suatu perintah **hanya jika kondisi tertentu benar (true)**.

## Pengertian `if` Statement

**IF statement** adalah pernyataan kondisi dalam PHP yang digunakan untuk mengeksekusi kode **hanya jika kondisi bernilai benar (true)**. Jika kondisi bernilai salah (false), maka blok kode tersebut **tidak akan dijalankan**.

Struktur umumnya seperti ini:

```php
if (kondisi) {
    // kode yang akan dijalankan jika kondisi benar
}
```

Penjelasan:

- `if` adalah kata kunci.
- `(kondisi)` adalah ekspresi logika yang akan diperiksa.
- Jika kondisi bernilai **true**, maka blok kode di dalam `{}` dijalankan.
- Jika kondisi bernilai **false**, blok kode tersebut dilewati (tidak dieksekusi).

## Contoh Sederhana

```php
<?php
$umur = 20;

if ($umur >= 18) {
    echo "Anda sudah dewasa.";
}
?>
```

Penjelasan:

- Variabel `$umur` bernilai `20`.
- PHP memeriksa kondisi `($umur >= 18)`.
- Karena 20 lebih besar atau sama dengan 18, maka kondisi bernilai **true**.
- Maka hasilnya:

```
Anda sudah dewasa.
```

Jika `$umur` bernilai `15`, maka kondisi tersebut bernilai **false**, dan **tidak ada output** yang ditampilkan.

## Contoh Kedua: Pengecekan Sederhana

```php
<?php
$nilai = 80;

if ($nilai > 75) {
    echo "Selamat, Anda lulus ujian!";
}
?>
```

Penjelasan

- Program akan menampilkan pesan _“Selamat, Anda lulus ujian!”_ hanya jika nilai lebih dari 75.
- Jika nilai 75 atau kurang, maka tidak ada pesan yang muncul sama sekali.

Kondisi di dalam `if` biasanya menggunakan **operator perbandingan.** Kita juga bisa menggabungkan beberapa kondisi menggunakan **operator logika**.

**Contoh:**

```php
<?php
$umur = 25;
$status = "aktif";

if ($umur > 18 && $status == "aktif") {
    echo "Anda memenuhi syarat.";
}
?>
```

Penjelasan:

- Kondisi hanya dianggap benar jika **keduanya benar**.
- Karena `$umur > 18` dan `$status == "aktif"`, maka hasilnya:

```
Anda memenuhi syarat.
```

## Kesimpulan

- `if` digunakan untuk **menjalankan kode hanya ketika kondisi benar (true)**.
- Jika kondisi salah (false), maka tidak terjadi apa-apa.
- `if` bisa digunakan untuk memeriksa satu atau beberapa kondisi sekaligus.
- Operator perbandingan (`==`, `>`, `<`, dll.) dan logika (`&&`, `||`) sering digunakan dalam `if`.

---

## [Praktikum](/materi/012/praktikum-if-statement.md)
