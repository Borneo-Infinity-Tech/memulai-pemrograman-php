# Array Asosiatif

Pada materi sebelumnya, kita sudah belajar:

- Pengertian array
- Array terindeks (menggunakan angka sebagai indeks)
- Menampilkan array dengan perulangan

Sekarang, kita akan belajar tentang **array asosiatif**. Berbeda dengan array terindeks, array asosiatif menggunakan **kata (key)** sebagai pengganti angka untuk mengakses data. Ini sangat berguna ketika kita ingin memberi nama pada setiap data agar lebih mudah dipahami.

## Apa itu Array Asosiatif?

Array asosiatif adalah array yang menggunakan **key (kunci) berupa teks** untuk menyimpan nilai.

**Contoh:**

```php
$mahasiswa = [
    "nama" => "Andi",
    "umur" => 20,
    "jurusan" => "Informatika"
];
```

**Penjelasan**:

- "nama" adalah key → nilainya "Andi"
- "umur" adalah key → nilainya 20
- "jurusan" adalah key → nilainya "Informatika"

## Cara Membuat Array Asosiatif

**Menggunakan tanda kurung siku \[\]**

```php
$buah = [
    "apel" => "Merah",
    "pisang" => "Kuning",
    "anggur" => "Ungu"
];
```

**Menggunakan fungsi** `array()`

```php
$buah = array(
    "apel" => "Merah",
    "pisang" => "Kuning",
    "anggur" => "Ungu"
);
```

## Mengakses Data dalam Array Asosiatif

Untuk mengambil data, gunakan key:

```php
echo $mahasiswa["nama"];     // Andi
echo $mahasiswa["umur"];     // 20
echo $mahasiswa["jurusan"];  // Informatika
```

## Menampilkan Array dengan Perulangan

Menggunakan `foreach`

```php
foreach ($mahasiswa as $key => $value) {
    echo "$key : $value \n";
}
```

**Penjelasan**:

- `$key` → nama indeks (contoh: nama, umur)
- `$value` → isi data

## Contoh Kasus Sederhana

Misalnya data satu siswa:

```php
$siswa = [
    "nama" => "Budi",
    "nilai" => 85,
    "kelas" => "XI RPL"
];

if ($siswa["nilai"] >= 80) {
    echo $siswa["nama"] . " Lulus";
} else {
    echo $siswa["nama"] . " Tidak Lulus";
}
```

## Perbedaan Array Terindeks dan Asosiatif

<table><tbody><tr><td><strong>Array Terindeks</strong></td><td><strong>Array Asosiatif</strong></td></tr><tr><td>Menggunakan angka</td><td>Menggunakan teks (key)</td></tr><tr><td>Contoh: <code>$data[0]</code></td><td>Contoh: <code>$data["nama"]</code></td></tr><tr><td>Cocok untuk daftar</td><td>Cocok untuk data berlabel</td></tr></tbody></table>

## Hal Penting yang Perlu Diingat

- Key harus unik (tidak boleh sama)
- Lebih mudah dibaca dibanding array terindeks
- Sangat cocok untuk data seperti:
  - Biodata
  - Data siswa
  - Data produk

---

Array asosiatif sangat membantu dalam mengelola data yang memiliki label atau keterangan. Dengan menggunakan key, kita bisa mengakses data dengan lebih jelas dan mudah dipahami.
