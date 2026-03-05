# Perulangan `do...while`

Setelah mempelajari perulangan **for** dan **while**, pada materi ini kita akan mempelajari jenis perulangan lainnya dalam PHP yaitu **do...while**. Perulangan ini merupakan **perulangan ketiga** yang sering digunakan dalam pemrograman PHP untuk menjalankan suatu perintah secara berulang.

Berbeda dengan perulangan **for** dan **while** yang memeriksa kondisi di awal perulangan, pada **do...while** proses akan **dijalankan terlebih dahulu**, kemudian setelah itu baru dilakukan pengecekan kondisi apakah perulangan perlu dilanjutkan atau tidak. Oleh karena itu, perulangan **do...while** memiliki karakteristik khusus yaitu **kode di dalamnya pasti dijalankan minimal satu kali**.

Perulangan ini sering digunakan pada situasi di mana suatu proses harus terjadi terlebih dahulu sebelum dilakukan pengecekan kondisi, seperti pada **program menu, validasi input pengguna, atau proses yang harus dijalankan setidaknya satu kali**. Pada materi ini akan dibahas mengenai **pengertian perulangan do...while, struktur penulisan, cara kerja, serta contoh penggunaannya dalam PHP** agar lebih mudah dipahami dan dapat diterapkan dalam pembuatan program.

## Pengertian Perulangan `do...while`

Perulangan **do...while** adalah jenis perulangan yang akan:

1.  Menjalankan kode terlebih dahulu
2.  Setelah itu baru memeriksa kondisi
3.  Jika kondisi **true**, maka perulangan akan diulang
4.  Jika kondisi **false**, maka perulangan berhenti

Artinya, **kode di dalam do pasti dijalankan minimal satu kali**, walaupun kondisi tidak terpenuhi.

## Struktur Penulisan `do...while`

Struktur dasar perulangan **do...while** dalam PHP adalah sebagai berikut:

```php
do {
    // kode yang dijalankan
} while (kondisi);
```

Penjelasan:

- **do** → tempat menuliskan kode yang akan dijalankan
- **while(kondisi)** → kondisi untuk menentukan apakah perulangan diulang atau tidak
- Jika kondisi **true**, perulangan akan kembali ke **do**
- Jika kondisi **false**, program keluar dari perulangan

## Contoh Sederhana `do...while`

Contoh menampilkan angka **1 sampai 5.**

```php
<?php

$angka = 1;

do {
    echo $angka . "\n";
    $angka++;
} while ($angka <= 5);

?>
```

Hasil output

```
1
2
3
4
5
```

### Penjelasan

1.  Variabel `$angka` bernilai **1**
2.  Program masuk ke blok **do**
3.  Menampilkan angka
4.  `$angka` ditambah 1
5.  Setelah itu baru diperiksa kondisi `$angka <= 5`
6.  Jika masih benar, perulangan diulang

**Contoh lain:**

```php
<?php

$i = 1;

do {
    echo "Belajar PHP itu menyenangkan \n";
    $i++;
} while ($i <= 3);

?>
```

Output

```
Belajar PHP itu menyenangkan
Belajar PHP itu menyenangkan
Belajar PHP itu menyenangkan
```

**Contoh Program Menghitung Total**

```php
<?php

$i = 1;
$total = 0;

do {
    $total += $i;
    $i++;
} while ($i <= 5);

echo "Total = " . $total;

?>
```

Output

```
Total = 15
```

## Kapan Menggunakan `do...while`?

Perulangan **do...while** biasanya digunakan ketika:

1.  Program **harus dijalankan minimal sekali**
2.  Input atau proses harus dilakukan sebelum pengecekan
3.  Program menu sederhana
4.  Sistem login atau validasi input

Contoh sederhana pada **menu program**.

```php
<?php

$pilihan = 1;

do {
    echo "Menu Program <br>";
    echo "1. Lihat Data <br>";
    echo "2. Tambah Data <br>";
    echo "3. Keluar <br>";

    $pilihan++;

} while ($pilihan <= 3);

?>
```

Perulangan **do...while** merupakan salah satu struktur kontrol dalam PHP yang digunakan untuk menjalankan kode secara berulang. Keunikan dari perulangan ini adalah **kode di dalam blok do akan selalu dijalankan minimal satu kali**, karena kondisi diperiksa setelah kode dijalankan.

Dengan memahami konsep **do...while**, programmer dapat membuat program yang lebih fleksibel, terutama ketika suatu proses perlu dijalankan terlebih dahulu sebelum kondisi diperiksa.

Menguasai perulangan seperti **do...while**, `while`, dan `for` merupakan dasar penting dalam pemrograman PHP karena sangat sering digunakan dalam pengolahan data, perhitungan, maupun pembuatan sistem aplikasi.
