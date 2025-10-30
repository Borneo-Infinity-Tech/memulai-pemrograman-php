# Program Pertama PHP

Langkah pertama dalam belajar PHP adalah menampilkan teks sederhana ke layar. Biasanya kita memulai dengan program klasik **“Hello World”**.

Buat file dengana nama **HelloWorld.php**.

![Program Pertama PHP](/img/program-pertama-php-01.png)

Tulisakan kode di bawah ini.

**Contoh Kode:**

```php
<?php
echo "Halo, Dunia!";
?>
```

**Penjelasan:**

- `<?php` → menandai **awal dari kode PHP**.
- `echo` → digunakan untuk **menampilkan teks atau isi** ke layar.
- `"Halo, Dunia!"` → teks yang ingin ditampilkan (harus diapit tanda kutip).
- `?>` → menandai **akhir dari kode PHP** (boleh ditulis, tapi sering juga diabaikan jika file berisi hanya PHP).

Jalankan kode melalui terminal, dengan mengetikan perintah **php** diikuti dengan nama file dalam kasus ini nama file kita **HelloWorld.php**

```
php HelloWorld.php
```

![Program Pertama PHP](/img/program-pertama-php-02.png)

Tekan Enter untuk melihat hasil akhir program. Maka akan tampil tulisan Hallo, Dunia! pada terminal.

![Program Pertama PHP](/img/program-pertama-php-03.png)

## Menampilkan Beberapa Baris Teks

Kita juga bisa menampilkan beberapa teks sekaligus menggunakan beberapa perintah `echo`.

```php
<?php
echo "Selamat datang di dunia PHP!\n";
echo "Mari kita belajar bersama.\n";
?>
```

#### **Penjelasan:**

- `echo` digunakan untuk **menampilkan teks** ke layar.
- Tanda `\n` digunakan untuk **membuat baris baru** di terminal.

Jika dijalankan, hasilnya akan seperti ini:

```
Selamat datang di dunia PHP!
Mari kita belajar bersama.
```

## Penggabungan Teks

Kita bisa menggabungkan beberapa teks menggunakan tanda **titik (**`.`**)** di PHP.

```php
<?php
echo "Halo" . " Dunia!" . "\n";
echo "Belajar " . "PHP " . "itu mudah!\n";
?>
```

**Hasil di terminal:**

```
Halo Dunia!
Belajar PHP itu mudah!
```

#### **Penjelasan:**

- Tanda `**.**` digunakan untuk **menggabungkan (concatenate)** teks.
- PHP akan menampilkan hasil gabungan tersebut sebagai satu kalimat utuh.

Selamat! Kamu sudah berhasil membuat dan menjalankan **program pertama PHP melalui terminal**.  
Kamu juga telah mempelajari cara menggunakan `echo` untuk menampilkan teks dan membuat baris baru dengan `\n`.

Ini adalah langkah awal yang penting dalam memahami dasar bahasa PHP. Teruslah berlatih agar semakin terbiasa dengan sintaks PHP dan cara kerjanya di terminal.
