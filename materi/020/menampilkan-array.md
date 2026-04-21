# Menampilkan Array dengan Perulangan

Setelah sebelumnya mempelajari **pengenalan array**, kita sudah tahu bahwa array digunakan untuk menyimpan banyak data dalam satu variabel.

```php
$buah = ["Apel", "Jeruk", "Mangga"];
```

Masalahnya, bagaimana cara menampilkan semua isi array tersebut?

Kalau jumlah datanya banyak, tentu tidak efisien jika ditampilkan satu per satu secara manual. Di sinilah kita menggunakan **perulangan (looping)**.

## Menampilkan Array Menggunakan Perulangan `for`

Perulangan `for` digunakan jika kita mengetahui jumlah data dalam array.

Untuk array, biasanya kita menggunakan fungsi:

```php
count()
```

untuk mengetahui jumlah elemen.

**Contoh:**

```php
<?php
$buah = ["Apel", "Jeruk", "Mangga"];

for ($i = 0; $i < count($buah); $i++) {
    echo $buah[$i] . "\n";
}
?>
```

### **Penjelasan**

- `$i = 0` → mulai dari index pertama
- `$i < count($buah)` → selama masih ada data
- `$i++` → tambah index setiap perulangan
- `$buah[$i]` → mengambil isi array berdasarkan index

## Menampilkan Array Menggunakan Perulangan `while`

Perulangan `while` akan berjalan selama kondisi bernilai **true**.

**Contoh**

```php
<?php
$buah = ["Apel", "Jeruk", "Mangga"];

$i = 0;
while ($i < count($buah)) {
    echo $buah[$i] . "\n";
    $i++;
}
?>
```

### Penjelasan

- `$i = 0` → inisialisasi awal
- `while ($i < count($buah))` → kondisi perulangan
- `$i++` → jangan lupa ditambah agar tidak infinite loop

## Menampilkan Array Menggunakan Perulangan `foreach`

`foreach` dibuat khusus untuk array, jadi lebih sederhana dan sering digunakan.

**Contoh:**

```php
<?php
$buah = ["Apel", "Jeruk", "Mangga"];

foreach ($buah as $item) {
    echo $item . "\n";
}
?>
```

### **Penjelasan**

- `$buah` → array
- `$item` → setiap isi array akan disimpan ke variabel ini secara otomatis

**Contoh dengan Index**

```php
<?php
$buah = ["Apel", "Jeruk", "Mangga"];

foreach ($buah as $index => $item) {
    echo "Index ke-$index: $item \n";
}
?>
```

Dalam PHP, menampilkan array bisa dilakukan dengan berbagai jenis perulangan. Namun dalam praktik sehari-hari:

- Gunakan `foreach` untuk kemudahan dan kejelasan kode
- Gunakan `for` **atau** `while` jika butuh kontrol lebih terhadap index

Memahami ketiga cara ini sangat penting karena akan sering digunakan saat mengolah data, terutama dari database.
