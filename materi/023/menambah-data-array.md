# Menambahkan Data Baru ke Dalam Array pada PHP

Pada materi sebelumnya, kita sudah belajar tentang **pengenalan array**, **array terindeks**, **array asosiatif**, **array multidimensi**, serta cara **menampilkan isi array** menggunakan `echo`,  dan perulangan seperti `for` atau `foreach`.

Pada materi ini, kita akan melanjutkan pembahasan dengan mempelajari cara **menambahkan data baru ke dalam array** pada PHP. Materi ini penting karena dalam pemrograman, data sering kali tidak langsung lengkap dari awal. Kadang kita perlu menambahkan data baru setelah array dibuat.

Contohnya, kita memiliki daftar nama siswa, lalu ada siswa baru yang masuk. Maka, kita perlu menambahkan nama siswa tersebut ke dalam array.

---

## Menambahkan Data ke Array Terindeks

Array terindeks adalah array yang menggunakan angka sebagai index. Index array di PHP dimulai dari angka `0`.

Contoh array terindeks:

```php
$buah = ["Apel", "Jeruk", "Mangga"];
```

Isi array tersebut adalah:

```php
Index 0 = Apel
Index 1 = Jeruk
Index 2 = Mangga
```

### **1 Menambahkan Data dengan Tanda Kurung Siku Kosong**

Cara paling umum untuk menambahkan data baru ke array terindeks adalah menggunakan tanda kurung siku kosong `[]`.

```php
$buah = ["Apel", "Jeruk", "Mangga"];

$buah[] = "Pisang";


print_r($buah);
```

Hasil:

```php
Array
(
    [0] => Apel
    [1] => Jeruk
    [2] => Mangga
    [3] => Pisang
)
```

Penjelasan:

```php
$buah[] = "Pisang";
```

Artinya, PHP akan menambahkan data `"Pisang"` ke posisi index berikutnya secara otomatis.

Karena index terakhir sebelumnya adalah `2`, maka data baru akan masuk ke index `3`.

### **2 Menambahkan Lebih dari Satu Data**

Kita juga bisa menambahkan beberapa data baru satu per satu.

```php
$buah = ["Apel", "Jeruk"];

$buah[] = "Mangga";
$buah[] = "Pisang";
$buah[] = "Anggur";

print_r($buah);
```

Hasil:

```php
Array
(
    [0] => Apel
    [1] => Jeruk
    [2] => Mangga
    [3] => Pisang
    [4] => Anggur
)
```

## Menambahkan Data ke Array Asosiatif

Array asosiatif adalah array yang menggunakan nama key atau kunci, bukan angka.

Contoh:

```php
$siswa = [
    "nama" => "Andi",
    "kelas" => "XI RPL",
    "umur" => 17
];
```

Pada array tersebut:

```php
key "nama" berisi "Andi"
key "kelas" berisi "XI RPL"
key "umur" berisi 17
```

### **1 Menambahkan Data Baru dengan Key Baru**

Untuk menambahkan data baru ke array asosiatif, kita bisa menuliskan nama key baru.

```php
$siswa = [
    "nama" => "Andi",
    "kelas" => "XI RPL",
    "umur" => 17
];

$siswa["alamat"] = "Makassar";

print_r($siswa);
```

Hasil:

```php
Array
(
    [nama] => Andi
    [kelas] => XI RPL
    [umur] => 17
    [alamat] => Makassar
)
```

Penjelasan:

```php
$siswa["alamat"] = "Makassar";
```

Artinya, kita menambahkan data baru dengan key `"alamat"` dan nilai `"Makassar"`.

### **2 Menambahkan Beberapa Data Baru**

```php
$siswa = [
    "nama" => "Andi",
    "kelas" => "XI RPL"
];

$siswa["umur"] = 17;
$siswa["alamat"] = "Makassar";
$siswa["jurusan"] = "Rekayasa Perangkat Lunak";

print_r($siswa);
```

Hasil:

```php
Array
(
    [nama] => Andi
    [kelas] => XI RPL
    [umur] => 17
    [alamat] => Makassar
    [jurusan] => Rekayasa Perangkat Lunak
)
```

## Menambahkan Data ke Array Multidimensi

Array multidimensi adalah array yang memiliki array lain di dalamnya.

Contoh:

```php
$daftarSiswa = [
    [
        "nama" => "Andi",
        "kelas" => "XI RPL"
    ],
    [
        "nama" => "Budi",
        "kelas" => "XI TKJ"
    ]
];
```

Array tersebut berisi beberapa data siswa. Setiap siswa disimpan dalam bentuk array asosiatif.

### **1 Menambahkan Data Baru ke Array Multidimensi**

Misalnya kita ingin menambahkan siswa baru.

```php
$daftarSiswa = [
    [
        "nama" => "Andi",
        "kelas" => "XI RPL"
    ],
    [
        "nama" => "Budi",
        "kelas" => "XI TKJ"
    ]
];

$daftarSiswa[] = [
    "nama" => "Citra",
    "kelas" => "XI MM"
];

print_r($daftarSiswa);
```

Hasil:

```php
Array
(
    [0] => Array
        (
            [nama] => Andi
            [kelas] => XI RPL
        )

    [1] => Array
        (
            [nama] => Budi
            [kelas] => XI TKJ
        )

    [2] => Array
        (
            [nama] => Citra
            [kelas] => XI MM
        )
)
```

Penjelasan:

```php
$daftarSiswa[] = [
    "nama" => "Citra",
    "kelas" => "XI MM"
];
```

Artinya, kita menambahkan satu array baru ke dalam array utama `$daftarSiswa`.

## Menampilkan Array Setelah Ditambahkan Data

Setelah data ditambahkan, kita bisa menampilkannya menggunakan `foreach`.

Contoh array terindeks:

```php
$buah = ["Apel", "Jeruk"];

$buah[] = "Mangga";
$buah[] = "Pisang";

foreach ($buah as $b) {
    echo $b . "\n";
}
```

Hasil:

```php
Apel
Jeruk
Mangga
Pisang
```

Contoh array asosiatif:

```php
$siswa = [
    "nama" => "Andi",
    "kelas" => "XI RPL"
];

$siswa["umur"] = 17;

foreach ($siswa as $key => $value) {
    echo $key . " : " . $value . "\n";
}
```

Hasil:

```php
nama : Andi
kelas : XI RPL
umur : 17
```

Contoh array multidimensi:

```php
$daftarSiswa = [
    [
        "nama" => "Andi",
        "kelas" => "XI RPL"
    ],
    [
        "nama" => "Budi",
        "kelas" => "XI TKJ"
    ]
];

$daftarSiswa[] = [
    "nama" => "Citra",
    "kelas" => "XI MM"
];

foreach ($daftarSiswa as $siswa) {
    echo "Nama: " . $siswa["nama"] . "\n";
    echo "Kelas: " . $siswa["kelas"] . "\n\n";
}
```

Hasil:

```php
Nama: Andi
Kelas: XI RPL

Nama: Budi
Kelas: XI TKJ

Nama: Citra
Kelas: XI MM
```

## Contoh Studi Kasus Sederhana

Misalnya kita memiliki data produk toko.

```php
$produk = [
    [
        "nama" => "Buku",
        "harga" => 5000
    ],
    [
        "nama" => "Pulpen",
        "harga" => 3000
    ]
];
```

Kemudian ada produk baru yang ingin ditambahkan.

```php
$produk[] = [
    "nama" => "Penghapus",
    "harga" => 2000
];
```

Lalu kita tampilkan semua data produk.

```php
foreach ($produk as $p) {
    echo "Nama Produk: " . $p["nama"] . "<br>";
    echo "Harga: Rp" . $p["harga"] . "<br><br>";
}
```

Hasil:

```php
Nama Produk: Buku
Harga: Rp5000

Nama Produk: Pulpen
Harga: Rp3000

Nama Produk: Penghapus
Harga: Rp2000
```

---

Dengan memahami cara menambahkan data baru ke dalam array, kita dapat mengelola data dengan lebih fleksibel di dalam program PHP. Materi ini sangat berguna ketika kita membuat aplikasi yang berhubungan dengan daftar data, seperti data siswa, data barang, data nilai, data pengguna, dan sebagainya.
