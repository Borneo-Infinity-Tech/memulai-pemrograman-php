# if...elseif...else Statement

## Pendahuluan

Dalam kehidupan sehari-hari, kita sering membuat keputusan berdasarkan kondisi tertentu. Contohnya:

- Jika hujan, kita membawa payung.
- Jika tidak hujan tapi mendung, kita membawa jas hujan.
- Jika cerah, kita tidak perlu membawa apa pun.

Dalam pemrograman, logika pengambilan keputusan seperti ini disebut **percabangan**. PHP menyediakan beberapa bentuk percabangan, dan salah satu yang paling umum digunakan adalah `**if...elseif...else**` **statement**.

## Pengertian `if...elseif...else` Statement

Pernyataan `**if...elseif...else**` digunakan dalam PHP untuk **menjalankan bagian kode tertentu berdasarkan kondisi yang diuji**. Dengan kata lain, program akan **mengecek satu per satu kondisi yang diberikan** dan **menjalankan perintah yang sesuai dengan kondisi yang benar (true)**. Jika semua kondisi salah (false), maka bagian `else` akan dijalankan sebagai “jalan terakhir”.

Struktur dasarnya adalah sebagai berikut:

```php
if (kondisi1) {
    // Kode dijalankan jika kondisi1 benar
} elseif (kondisi2) {
    // Kode dijalankan jika kondisi1 salah, tapi kondisi2 benar
} else {
    // Kode dijalankan jika semua kondisi salah
}
```

**Penjelasan singkat tiap bagian:**

- `if` → Mengecek kondisi pertama. Jika benar, kode di dalamnya dijalankan.
- `elseif` → Mengecek kondisi lain jika kondisi sebelumnya salah. Bisa ada satu atau lebih.
- `else` → Dijalankan jika semua kondisi sebelumnya salah.

Struktur ini membantu program untuk **mengambil keputusan secara berurutan** — dari kondisi pertama hingga terakhir.

## Contoh

Misalnya kita ingin membuat program yang memberi saran berdasarkan kondisi cuaca.

```php
<?php
$cuaca = "mendung";

if ($cuaca == "hujan") {
    echo "Bawa payung ya!";
} elseif ($cuaca == "mendung") {
    echo "Sebaiknya bawa jas hujan, siapa tahu hujan.";
} else {
    echo "Cerah sekali, tidak perlu bawa apa-apa!";
}
?>
```

**Penjelasan:**

1.  Program akan memeriksa apakah `$cuaca` bernilai `"hujan"`. Jika iya, menampilkan “Bawa payung ya!”.
2.  Jika bukan `"hujan"`, maka akan memeriksa kondisi berikutnya: `"mendung"`. Jika benar, menampilkan “Sebaiknya bawa jas hujan...”.
3.  Jika tidak memenuhi kedua kondisi di atas, maka bagian `else` dijalankan dan menampilkan “Cerah sekali, tidak perlu bawa apa-apa!”.

**Contoh Lain: Menentukan Nilai Huruf Berdasarkan Skor**

```php
<?php
$nilai = 82;

if ($nilai >= 90) {
    echo "Nilai kamu: A";
} elseif ($nilai >= 75) {
    echo "Nilai kamu: B";
} elseif ($nilai >= 60) {
    echo "Nilai kamu: C";
} else {
    echo "Nilai kamu: D";
}
?>
```

**Penjelasan:**

- Jika nilai 90 ke atas → tampilkan “A”
- Jika 75–89 → tampilkan “B”
- Jika 60–74 → tampilkan “C”
- Jika di bawah 60 → tampilkan “D”

Dengan `if...elseif...else`, program bisa menilai siswa otomatis berdasarkan angka yang diberikan. `if...elseif...else` adalah **dasar penting dalam logika pemrograman** yang harus dikuasai oleh setiap programmer. Melalui percabangan ini, program dapat “berpikir” dan mengambil keputusan layaknya manusia. Teruslah berlatih membuat contoh sederhana dengan berbagai kondisi yang berbeda, agar kamu terbiasa memahami alur logika program.

\`“Logika yang baik akan menghasilkan program yang cerdas.” 💡💻\`
