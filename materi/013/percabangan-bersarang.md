# Materi PHP: Percabangan Bersarang (Nested Conditional)

Dalam pemrograman, sering kali kita harus mengambil keputusan berdasarkan beberapa kondisi sekaligus. Tidak semua keputusan bisa diselesaikan hanya dengan satu kondisi `if` atau `else`. Kadang, setelah sebuah kondisi terpenuhi, kita masih perlu memeriksa kondisi lain di dalamnya.

Untuk menangani kasus seperti ini, PHP menyediakan konsep **percabangan bersarang** (_nested conditional_). Percabangan bersarang adalah percabangan yang berada di dalam percabangan lain. Materi ini akan membahas pengertian, konsep, struktur, dan contoh penggunaan percabangan bersarang dalam PHP secara mudah dipahami.

## Pengertian Percabangan Bersarang

**Percabangan bersarang** adalah kondisi `if`, `else if`, atau `else` yang berada di dalam kondisi `if`, `else if`, atau `else` lainnya.

Artinya:

- Satu keputusan bergantung pada keputusan sebelumnya
- Program melakukan pengecekan kondisi secara bertahap

Contoh kasus sederhana:

> Jika nilai siswa ≥ 75, maka lulus.  
> Jika lulus, periksa apakah nilainya ≥ 90 untuk menentukan predikat.

## Struktur Dasar Percabangan Bersarang

Struktur umum percabangan bersarang di PHP:

```php
if (kondisi_1) {
    if (kondisi_2) {
        // kode dijalankan jika kondisi_1 dan kondisi_2 benar
    } else {
        // kode dijalankan jika kondisi_1 benar, kondisi_2 salah
    }
} else {
    // kode dijalankan jika kondisi_1 salah
}
```

**Penjelasan**

- `kondisi_1` dicek terlebih dahulu
- Jika `kondisi_1` bernilai **true**, maka program masuk ke percabangan di dalamnya
- Di dalamnya, `kondisi_2` akan dicek

## Contoh 1: Menentukan Kelulusan dan Predikat Nilai

```php
<?php
$nilai = 85;

if ($nilai >= 75) {
    echo "Status: Lulus <br>";

    if ($nilai >= 90) {
        echo "Predikat: A";
    } else {
        echo "Predikat: B";
    }
} else {
    echo "Status: Tidak Lulus";
}
?>
```

**Penjelasan**

1.  Program mengecek apakah `$nilai >= 75`
2.  Jika **true**, maka status **Lulus**
3.  Di dalam kondisi lulus, program mengecek lagi:
    1.  Jika nilai ≥ 90 → Predikat A
    2.  Jika tidak → Predikat B
4.  Jika nilai \< 75 → Tidak Lulus

## Contoh 2: Login dengan Hak Akses

```php
<?php
$username = "admin";
$password = "12345";

if ($username == "admin") {
    if ($password == "12345") {
        echo "Login berhasil sebagai Admin";
    } else {
        echo "Password salah";
    }
} else {
    echo "Username tidak ditemukan";
}
?>
```

**Penjelasan**

- Program pertama mengecek `username`
- Jika username benar, baru mengecek `password`
- Jika username salah, pengecekan password tidak dilakukan

## Contoh 3: Percabangan Bersarang dengan `else if`

```php
<?php
$umur = 17;

if ($umur >= 18) {
    echo "Dewasa";
} else {
    if ($umur >= 13) {
        echo "Remaja";
    } else {
        echo "Anak-anak";
    }
}
?>
```

**Penjelasan**

1.  Jika umur ≥ 18 → Dewasa
2.  Jika tidak:
    1.  Umur ≥ 13 → Remaja
    2.  Selain itu → Anak-anak

## Kapan Menggunakan Percabangan Bersarang?

Gunakan percabangan bersarang jika:

- Keputusan kedua bergantung pada keputusan pertama
- Logika program tidak bisa dipisahkan
- Ingin proses pengecekan yang lebih terstruktur

Namun, **hindari terlalu banyak percabangan bersarang**, karena:

- Kode menjadi sulit dibaca
- Sulit dirawat dan dikembangkan

## Tips Menggunakan Percabangan Bersarang

1.  Gunakan indentasi (spasi/tab) agar kode mudah dibaca
2.  Jangan membuat percabangan terlalu dalam
3.  Jika logika terlalu kompleks, pertimbangkan:
    1.  Menggunakan `else if`
    2.  Menggunakan `switch`
    3.  Memecah kode ke dalam fungsi

Percabangan bersarang dalam PHP sangat berguna untuk menangani kondisi yang saling bergantung. Dengan memahami konsep ini, kita dapat membuat program yang lebih cerdas dan sesuai dengan kebutuhan logika yang kompleks.

Kunci utama dalam menggunakan percabangan bersarang adalah **menjaga kode tetap rapi, mudah dibaca, dan tidak berlebihan**. Dengan latihan dan pemahaman yang baik, percabangan bersarang akan menjadi alat yang sangat membantu dalam pemrograman PHP.

---

[Praktikum](/materi/013/praktikum/01.md)
