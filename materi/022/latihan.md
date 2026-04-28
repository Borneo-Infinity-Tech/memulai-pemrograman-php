# Praktikum Array Multidimensi

**Kerjakan soal di bawah ini dengan jawaban yang tepat!**

## Soal 1

Diberikan data siswa berikut:

- Nama: Alya Amanda, Umur: 16, Kelas: XI RPL
- Nama: Muhammad Akbar, Umur: 17, Kelas: XI TKJ
- Nama: Aurelia, Umur: 16, Kelas: XI MM

**Tugas:**

1.  Ubah data siswa di atas ke dalam bentuk **array multidimensi numerik (terindeks)** di PHP.
2.  Tampilkan setiap data siswa menggunakan **echo**, tanpa menggunakan perulangan (looping).

```php
<?php
$siswa = [
    ["Alya Amanda", 16, "XI RPL"],
    ["Muhammad Akbar", 17, "XI TKJ"],
    ["Aurelia", 16, "XI MM"]
];

// Menampilkan data tanpa perulangan
echo "Nama: " . $siswa[0][0] . ", Umur: " . $siswa[0][1] . ", Kelas: " . $siswa[0][2];
echo "<br>";
echo "Nama: " . $siswa[1][0] . ", Umur: " . $siswa[1][1] . ", Kelas: " . $siswa[1][2];
echo "<br>";
echo "Nama: " . $siswa[2][0] . ", Umur: " . $siswa[2][1] . ", Kelas: " . $siswa[2][2];
?>
```

## Soal 2

Diberikan data siswa berikut:

- Nama: Alya Amanda, Umur: 16, Kelas: XI RPL
- Nama: Muhammad Akbar, Umur: 17, Kelas: XI TKJ
- Nama: Aurelia, Umur: 16, Kelas: XI MM

**Tugas:**

1.  Ubah data siswa di atas ke dalam bentuk **array multidimensi numerik (terindeks)** di PHP.
2.  Tampilkan seluruh data siswa menggunakan **perulangan** `**foreach**`.

```php
<?php
$siswa = [
    ["Alya Amanda", 16, "XI RPL"],
    ["Muhammad Akbar", 17, "XI TKJ"],
    ["Aurelia", 16, "XI MM"]
];

// Menampilkan data menggunakan foreach
foreach ($siswa as $data) {
    echo "Nama: " . $data[0] . ", Umur: " . $data[1] . ", Kelas: " . $data[2];
    echo "<br>";
}
?>
```

## Soal 3

Perhatikan data produk berikut dalam bentuk tabel:

<table><tbody><tr><td><strong>Nama Produk</strong></td><td><strong>Harga</strong></td><td><strong>Stok</strong></td></tr><tr><td>Laptop</td><td>7000000</td><td>5</td></tr><tr><td>Mouse</td><td>150000</td><td>20</td></tr><tr><td>Keyboard</td><td>300000</td><td>15</td></tr><tr><td>Monitor</td><td>2000000</td><td>8</td></tr></tbody></table>

**Tugas:**

1.  Ubah data pada tabel di atas ke dalam bentuk **array multidimensi numerik (terindeks)** di PHP.
2.  Tampilkan seluruh data produk tersebut ke layar menggunakan **perulangan** `**foreach**`.
3.  Format output:

```
Produk: Laptop, Harga: 7000000, Stok: 5
```

**Ketentuan:**

- Gunakan array terindeks (numerik), bukan array asosiatif.
- Tidak boleh menyalin kode dari contoh sebelumnya.
- Gunakan `foreach` untuk menampilkan data.
- Gunakan `echo` untuk output.

## Soal 4

Perhatikan data film berikut dalam bentuk tabel:

| Judul Film | Tahun | Genre   | Durasi (menit) | Rating |
| ---------- | ----- | ------- | -------------- | ------ |
| Inception  | 2010  | Sci-Fi  | 148            | 8.8    |
| Parasite   | 2019  | Drama   | 132            | 8.6    |
| Avengers   | 2012  | Action  | 143            | 8.0    |
| Coco       | 2017  | Animasi | 105            | 8.4    |

**Tugas:**

1.  Ubah data pada tabel di atas ke dalam bentuk **array multidimensi numerik (terindeks)** di PHP.
2.  Tampilkan seluruh data film tersebut ke layar menggunakan **perulangan** `**foreach**`.
3.  Format output:

```
Film: Inception, Tahun: 2010, Genre: Sci-Fi, Durasi: 148 menit, Rating: 8.8
```

**Ketentuan:**

- Gunakan array terindeks (numerik), bukan array asosiatif.
- Tidak boleh menyalin kode dari contoh sebelumnya.
- Gunakan `foreach` untuk menampilkan data.
- Gunakan `echo` untuk output.

## Soal 5

Perhatikan data menu makanan berikut dalam bentuk tabel:

| Nama Menu   | Kategori | Harga | Kalori | Stok |
| ----------- | -------- | ----- | ------ | ---- |
| Nasi Goreng | Makanan  | 20000 | 450    | 10   |
| Es Teh      | Minuman  | 5000  | 120    | 25   |
| Mie Ayam    | Makanan  | 15000 | 380    | 8    |
| Jus Alpukat | Minuman  | 12000 | 250    | 12   |

**Tugas:**

1.  Ubah data pada tabel di atas ke dalam bentuk **array multidimensi numerik (terindeks)** di PHP.
2.  Tampilkan seluruh data menu tersebut ke layar menggunakan **perulangan** `**foreach**`.
3.  Format output:

```
Menu: Nasi Goreng, Kategori: Makanan, Harga: 20000, Kalori: 450, Stok: 10
```

**Ketentuan:**

- Gunakan array terindeks (numerik), bukan array asosiatif.
- Tidak boleh menyalin kode dari contoh sebelumnya.
- Gunakan `foreach` untuk menampilkan data.
- Gunakan `echo` untuk output.
