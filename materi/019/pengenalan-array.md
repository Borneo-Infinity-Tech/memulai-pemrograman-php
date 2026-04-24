# Pengenalan Array

Dalam pemrograman, kita sering bekerja dengan banyak data sekaligus.

Contohnya:

- daftar nama siswa dalam satu kelas
- daftar produk dalam toko
- daftar nilai ujian

Jika kita menggunakan variabel biasa, kita harus membuat banyak variabel:

```php
$nama1 = "Budi";
$nama2 = "Ani";
$nama3 = "Siti";
```

❌ Kekurangan:

- Tidak rapi
- Sulit dikelola jika datanya banyak
- Tidak efisien

Untuk mengatasi hal tersebut, PHP menyediakan **array**, yaitu sebuah struktur data yang dapat menyimpan banyak nilai dalam satu variabel.

---

## Pengertian Array

Array adalah variabel yang dapat menyimpan lebih dari satu nilai dalam satu tempat. Bayangkan array seperti sebuah **kotak yang berisi beberapa barang**.

Contoh: Bayangkan array seperti rak buku:

```
Rak Buku:
+-----------------+
| Buku A          |
| Buku B          |
| Buku C          |
+-----------------+
```

## Konsep Penting dalam Array

Array bisa menyimpan banyak data dengan tipe yang sama atau berbeda:

```
+-----------------+
| "Buku A"        |
| 20              |
| true            |
+-----------------+
```

Penjelasan:

- "Buku A" → string
- 20 → angka
- true → boolean

👉 Artinya array bisa fleksibel menyimpan berbagai jenis data.

Array memiliki index (Index adalah nomor posisi dari setiap elemen dalam array.), Setiap data dalam array memiliki **index (posisi)**

**Penting:** Index dimulai dari **0,** Bukan dari 1

```
Rak Buku:
+---------------------+
| 0 → Buku A          |
| 1 → Buku B          |
| 2 → Buku C          |
+---------------------+
```

## Cara Membuat Array di PHP

Ada dua cara umum untuk membuat array di PHP.

Menggunakan fungsi `array()`

```php
$buah = array("Apel", "Jeruk", "Mangga");
```

Menggunakan tanda kurung siku `[]`

```php
$buah = ["Apel", "Jeruk", "Mangga"];
```

Kedua cara tersebut menghasilkan array yang sama.

### **Isi Array**

Setiap data dalam array disebut **elemen**.

```php
$buah = ["Apel", "Jeruk", "Mangga"];
```

Ilustrasi Posisi

<table><tbody><tr><td>Index</td><td>0</td><td>1</td><td>2</td></tr><tr><td>Data</td><td>Apel</td><td>Jeruk</td><td>Mangga</td></tr></tbody></table>

## Mengakses Data dalam Array

Untuk mengambil data dari array, kita gunakan index.

`$nama_variabel[index]`

Contoh:

```php
$buah = ["Apel", "Jeruk", "Mangga"];

echo $buah[0]; // Output: Apel
echo $buah[1]; // Output: Jeruk
echo $buah[2]; // Output: Mangga
```

## Kapan Menggunakan Array?

- Menyimpan banyak data dalam satu variabel
- Data memiliki jenis yang sama (misalnya semua nama atau semua angka)
- Ingin mengelola data secara lebih rapi

Array adalah konsep dasar yang sangat penting dalam PHP. Dengan memahami array, kita dapat menyimpan dan mengelola banyak data dengan lebih mudah dan rapi.

Materi ini masih merupakan pengenalan dasar. Pada tahap selanjutnya, kita akan mempelajari cara menggunakan array dengan lebih lanjut.

---

## [Latihan](materi/019/latihan.md)
