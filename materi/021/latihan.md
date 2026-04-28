# Praktikum Array Assosiatif

**Kerjakan soal di bawah ini dengan jawaban yang tepat!**

## Soal 1

Terdapat data siswa sebagai berikut:

- Nama: Budi
- Kelas: XI RPL
- Umur: 16
- Sekolah: SMK ISFI Banjarmasin
- Lulus: false

Data tersebut kita ubah kedalam bentuk **array asosiatif** seperti kode di bawah ini dan kita tampilkan datanya.

```php
<?php
$siswa = [
    "nama" => "Budi",
    "kelas" => "XI RPL",
    "umur" => 16,
    "sekolah" => "SMK ISFI Banjarmasin",
    "lulus" => false
];

$status = $siswa["lulus"] === false ? "Belum Lulus" : "Lulus";

echo "Nama: $siswa[nama] \n";
echo "Kelas: $siswa[kelas] \n";
echo "Umur: $siswa[umur] \n";
echo "Sekolah: $siswa[sekolah] \n";
echo "Lulus; $status \n";
?>
```

Tampilkan datanya ke layar.

## Soal 2

Diberikan data karyawan berikut:

- Nama: Andi
- Jabatan: Manager
- Gaji: 8000000
- Status: Tetap

Ubah data tersebut ke dalam bentuk **array asosiatif pada PHP**, lalu tampilkan seluruh data **tanpa menggunakan perulangan**.

## Soal 3

Diberikan data sebuah **produk toko online** sebagai berikut:

- Nama Produk: Laptop ASUS
- Harga: 7500000
- Stok: 10
- Kategori: Elektronik

Ubah data tersebut ke dalam bentuk **array asosiatif pada PHP**, lalu tampilkan seluruh data **tanpa menggunakan perulangan**.

## Soal 4

Terdapat data siswa sebagai berikut:

- Nama: Aurel Alana
- Kelas: X RPL
- Umur: 17
- Sekolah: SMK ISFI Banjarmasin

Data tersebut kita ubah kedalam bentuk **array asosiatif** seperti kode di bawah ini dan kita tampilkan datanya menggunakan perulangan `foreach`.

```php
<?php
$siswa = [
    "nama" => "Aurel Alana",
    "kelas" => "X RPL",
    "umur" => 17,
    "sekolah" => "SMK ISFI Banjarmasin"
];

foreach ($siswa as $key => $value) {
    echo "$key: $value \n";
}
?>
```

## Soal 5

Diberikan data sebuah **buku di perpustakaan** sebagai berikut:

- Judul: Laskar Pelangi
- Pengarang: Andrea Hirata
- Tahun Terbit: 2005
- Penerbit: Bentang Pustaka

Ubah data tersebut ke dalam bentuk **array asosiatif pada PHP**, lalu tampilkan seluruh data **menggunakan perulangan**.

## Soal 6

Diberikan data **transaksi belanja di minimarket** sebagai berikut:

- Nama Barang: Indomie Goreng
- Harga: 3500
- Jumlah Beli: 3
- Total: 10500

Buatlah **array asosiatif pada PHP** dari data tersebut, lalu tampilkan seluruh data **menggunakan perulangan**.

Diberikan data **transaksi belanja di minimarket** sebagai berikut:

- Nama Barang: Indomie Goreng
- Harga: 3500
- Jumlah Beli: 3
- Total: 10500

Buatlah **array asosiatif pada PHP** dari data tersebut, lalu tampilkan seluruh data **menggunakan perulangan**.

---

[Lanjut Array Multidimensi](materi/022/latihan.md)
