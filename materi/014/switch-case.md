# Switch…Case Statement

Dalam pemrograman PHP, sering kali kita perlu membuat keputusan berdasarkan suatu nilai. Misalnya: menentukan nama hari berdasarkan angka, menentukan grade nilai, atau memilih menu berdasarkan input pengguna.

Biasanya, kondisi seperti ini bisa dibuat menggunakan `if...else`. Namun, jika kondisi yang dicek **banyak dan berdasarkan satu variabel yang sama**, penggunaan `if...else` menjadi panjang dan kurang rapi.

Untuk mengatasi hal tersebut, PHP menyediakan **Switch…Case Statement**, yaitu struktur kontrol yang digunakan untuk memilih satu dari banyak kemungkinan berdasarkan nilai tertentu. Struktur ini membuat kode lebih **ringkas, mudah dibaca, dan terstruktur**.

## Pengertian Switch…Case

`switch...case` adalah pernyataan percabangan di PHP yang digunakan untuk membandingkan **satu nilai** dengan beberapa kemungkinan nilai lainnya.

Jika nilai yang diuji cocok dengan salah satu `case`, maka kode di dalam `case` tersebut akan dijalankan.

## Struktur Dasar Switch…Case

Berikut struktur umum `switch...case` dalam PHP:

```
switch (variabel) {
    case nilai1:
        // kode yang dijalankan jika variabel == nilai1
        break;
    case nilai2:
        // kode yang dijalankan jika variabel == nilai2
        break;
    default:
        // kode yang dijalankan jika tidak ada case yang cocok
}
```

### Penjelasan:

- **switch (variabel)**  
  Variabel yang nilainya akan diperiksa.
- **case nilai:**  
  Nilai pembanding dari variabel.
- **break;**  
  Digunakan untuk menghentikan proses `switch` setelah sebuah `case` dijalankan.
- **default:**  
  Dijalankan jika tidak ada `case` yang sesuai.

## Contoh 1: Menentukan Nama Hari

```php
<?php
$hari = 3;

switch ($hari) {
    case 1:
        echo "Senin";
        break;
    case 2:
        echo "Selasa";
        break;
    case 3:
        echo "Rabu";
        break;
    case 4:
        echo "Kamis";
        break;
    case 5:
        echo "Jumat";
        break;
    case 6:
        echo "Sabtu";
        break;
    case 7:
        echo "Minggu";
        break;
    default:
        echo "Nomor hari tidak valid";
}
?>
```

**Penjelasan:**

Karena nilai `$hari` adalah `3`, maka program akan menampilkan **“Rabu”**.

## Contoh 2: Menentukan Grade Nilai

```php
<?php
$grade = "B";

switch ($grade) {
    case "A":
        echo "Sangat Baik";
        break;
    case "B":
        echo "Baik";
        break;
    case "C":
        echo "Cukup";
        break;
    case "D":
        echo "Kurang";
        break;
    default:
        echo "Grade tidak dikenal";
}
?>
```

**Penjelasan:**

Switch membandingkan nilai `$grade` dengan setiap `case`. Karena bernilai `"B"`, maka hasilnya adalah **“Baik”**.

## Pentingnya Break pada Switch…Case

Jika kita **tidak menggunakan** `**break;**`, maka PHP akan menjalankan **case berikutnya**, meskipun kondisinya tidak cocok. Hal ini disebut _fall-through_.

**Contoh tanpa break:**

```php
<?php
$angka = 1;

switch ($angka) {
    case 1:
        echo "Satu ";
    case 2:
        echo "Dua ";
    case 3:
        echo "Tiga ";
}
?>
```

**Output**:

```php
Satu Dua Tiga
```

Karena tidak ada `break`, semua `case` setelah yang cocok ikut dijalankan.

## Menggabungkan Beberapa Case

Beberapa `case` dapat menjalankan kode yang sama.

```php
<?php
$nilai = "A";

switch ($nilai) {
    case "A":
    case "B":
        echo "Lulus";
        break;
    case "C":
        echo "Remedial";
        break;
    default:
        echo "Tidak lulus";
}
?>
```

**Penjelasan:**  
Jika nilai `"A"` atau `"B"`, hasilnya tetap **“Lulus”**.

## Kapan Menggunakan Switch…Case?

Gunakan `switch...case` jika:

- Kondisi didasarkan pada **satu variabel**
- Nilai yang dicek bersifat **tetap (konstan)**
- Jumlah kondisi **banyak**

Gunakan `if...else` jika:

- Kondisi kompleks (menggunakan operator logika `&&`, `||`)
- Perbandingan rentang nilai (misalnya: `>`, `<`)

Switch…Case Statement merupakan salah satu struktur kontrol penting dalam PHP yang membantu programmer membuat percabangan dengan lebih rapi dan mudah dipahami. Dengan memahami cara kerja `switch`, penggunaan `case`, `break`, dan `default`, kita dapat menulis kode yang lebih efisien dan terstruktur.

Penguasaan `switch...case` akan sangat membantu dalam pembuatan aplikasi PHP, terutama saat menangani banyak pilihan kondisi berbasis satu nilai.
