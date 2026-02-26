# Perulangan `while`

Dalam pemrograman, sering kali kita perlu menjalankan sebuah perintah secara berulang-ulang. Misalnya menampilkan angka dari 1 sampai 10, mencetak daftar nama, atau memproses data dalam jumlah banyak. Untuk melakukan hal tersebut, kita menggunakan **perulangan (looping)**.

Salah satu jenis perulangan dalam PHP adalah **while**. Perulangan `while` digunakan untuk menjalankan kode selama suatu kondisi bernilai **true (benar)**. Jika kondisi bernilai **false (salah)**, maka perulangan akan berhenti.

Perulangan `while` biasanya digunakan ketika kita belum tahu pasti berapa kali perulangan akan dilakukan, tetapi kita tahu kondisi kapan perulangan harus berhenti.

## Pengertian Perulangan `while`

Perulangan `while` adalah struktur kontrol dalam PHP yang akan mengeksekusi blok kode secara berulang selama kondisi yang diberikan bernilai true.

Artinya:

- Cek kondisi dulu
- Jika benar → jalankan kode
- Cek lagi kondisi
- Jika masih benar → jalankan lagi
- Jika salah → berhenti

## Struktur Dasar Perulangan `while`

Berikut bentuk umum penulisan while:

```
while (kondisi) {
    // kode yang dijalankan berulang
}
```

Penjelasan:

- `while` → kata kunci perulangan
- `(kondisi)` → syarat agar perulangan berjalan
- `{}` → blok kode yang akan diulang

## Contoh Perulangan `while`

Contoh 1: Menampilkan Angka 1 sampai 5

```php
<?php
$angka = 1;

while ($angka <= 5) {
    echo "Angka ke-" . $angka . "<br>";
    $angka++;
}
?>
```

Penjelasan:

- `$angka` dimulai dari 1
- Selama `$angka <= 5`, maka perulangan berjalan
- `$angka++` artinya nilai bertambah 1 setiap perulangan
- Jika `$angka` sudah lebih dari 5, perulangan berhenti

Output:

```
Angka ke-1
Angka ke-2
Angka ke-3
Angka ke-4
Angka ke-5
```

### **Penting: Increment dan Infinite Loop**

Di dalam perulangan while, kita harus memastikan kondisi bisa menjadi false. Jika tidak, maka akan terjadi **infinite loop (perulangan tanpa akhir)**.

Contoh salah:

```
<?php
$angka = 1;

while ($angka <= 5) {
    echo $angka;
}
?>
```

Kesalahan:

- Tidak ada `$angka++`
- Nilai `$angka` tidak pernah berubah
- Kondisi selalu true
- Program akan berjalan terus tanpa henti

Contoh Menghitung Jumlah Total

```php
<?php
$i = 1;
$total = 0;

while ($i <= 5) {
    $total += $i;
    $i++;
}

echo "Total = " . $total;
?>
```

Penjelasan:

- Menjumlahkan angka 1 sampai 5
- `$total += $i` artinya total = total + i

Hasil:

```
Total = 15
```

## Kapan Menggunakan While?

Gunakan while ketika:

- Jumlah perulangan belum diketahui pasti
- Perulangan tergantung kondisi tertentu
- Mengambil data dari database
- Membaca file sampai akhir

Jika jumlah perulangan sudah pasti (misalnya 1 sampai 10), biasanya lebih sering menggunakan `for`.

Perulangan `while` dalam PHP adalah salah satu struktur kontrol yang sangat penting untuk mengulang suatu perintah selama kondisi tertentu masih terpenuhi. While bekerja dengan cara mengecek kondisi terlebih dahulu sebelum menjalankan kode.

Dengan memahami cara kerja while, cara membuat kondisi yang benar, serta menghindari infinite loop, kita dapat membuat program yang lebih dinamis dan efisien.

Teruslah berlatih membuat berbagai variasi perulangan agar semakin memahami logika pemrograman. Semakin sering mencoba, semakin mudah memahami konsepnya.
