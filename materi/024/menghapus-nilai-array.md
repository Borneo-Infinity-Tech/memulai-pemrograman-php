# Menghapus Nilai pada Array di PHP

Pada materi sebelumnya, kita sudah mempelajari beberapa hal penting tentang array di PHP, seperti membuat, menampilkan, dan menambahkan data ke array, langkah berikutnya adalah mempelajari cara **menghapus nilai atau data dari array**. Menghapus data pada array sangat penting karena dalam program nyata, data sering berubah. Misalnya:

- menghapus nama siswa dari daftar,
- menghapus produk dari keranjang belanja,
- menghapus data pengguna,

## Menghapus Data Array Menggunakan `unset()`

Perintah `unset()` digunakan untuk menghapus elemen array berdasarkan **index** atau **key**.

**Contoh pada Array Terindeks**

```php
$buah = ["Apel", "Jeruk", "Mangga", "Pisang"];

unset($buah[1]);

print_r($buah);
```

**Hasil**

```php
Array
(
    [0] => Apel
    [2] => Mangga
    [3] => Pisang
)
```

Penjelasan:

Data dengan index `1`, yaitu `"Jeruk"`, berhasil dihapus. Namun, index array tidak otomatis berurutan kembali. Index yang tersisa adalah `0`, `2`, dan `3`.

Jika ingin merapikan index, gunakan `array_values()`.

```php
$buah = array_values($buah);

print_r($buah);
```

Hasil:

```php
Array
(
    [0] => Apel
    [1] => Mangga
    [2] => Pisang
)
```

## Menghapus Data pada Array Asosiatif

Array asosiatif menggunakan **key berupa nama**, bukan angka index.

Contoh:

```php
$siswa = [
    "nama" => "Andi",
    "kelas" => "XI RPL",
    "umur" => 17
];

unset($siswa["umur"]);

print_r($siswa);
```

Hasil:

```php
Array
(
    [nama] => Andi
    [kelas] => XI RPL
)
```

Penjelasan:

Data dengan key `"umur"` dihapus dari array.

## Menghapus Data pada Array Multidimensi

Array multidimensi adalah array di dalam array.

Contoh data siswa:

```php
$siswa = [
    [
        "nama" => "Andi",
        "kelas" => "XI RPL"
    ],
    [
        "nama" => "Budi",
        "kelas" => "XI TKJ"
    ],
    [
        "nama" => "Citra",
        "kelas" => "XI MM"
    ]
];
```

**Menghapus Satu Data Siswa**

```php
unset($siswa[1]);

print_r($siswa);
```

**Hasil:**

```php
Array
(
    [0] => Array
        (
            [nama] => Andi
            [kelas] => XI RPL
        )

    [2] => Array
        (
            [nama] => Citra
            [kelas] => XI MM
        )
)
```

Data siswa dengan index `1`, yaitu Budi, berhasil dihapus.

Agar index kembali berurutan:

```php
$siswa = array_values($siswa);
```

---

Menghapus data pada array adalah kemampuan penting dalam pemrograman PHP. Dengan memahami berbagai cara penghapusan array, kita bisa mengatur data dengan lebih fleksibel. Dengan menguasai materi ini, kita dapat membuat program PHP yang lebih dinamis, misalnya program daftar siswa, keranjang belanja, data produk, dan sistem pengelolaan data lainnya.
