# if...else Statement

## Pendahuluan

Dalam kehidupan sehari-hari, kita sering dihadapkan pada **pengambilan keputusan**. Misalnya:

```
Jika hujan turun, maka saya akan membawa payung.
Jika tidak hujan, maka saya tidak akan membawa payung.
```

Contoh di atas menggambarkan **percabangan logika** — ada dua kemungkinan tindakan tergantung pada kondisi tertentu. Dalam pemrograman, kita bisa membuat komputer **“berpikir dan memilih tindakan”** dengan cara yang sama menggunakan **percabangan if...else**.

---

## if...else Statement

`if...else` statement adalah struktur logika dalam PHP yang digunakan untuk **menjalankan perintah tertentu hanya jika suatu kondisi benar**, dan **menjalankan perintah lain jika kondisi tersebut salah**.

Secara umum, bentuk penulisannya seperti ini:

```
if (kondisi) {
    // kode yang dijalankan jika kondisi benar (TRUE)
} else {
    // kode yang dijalankan jika kondisi salah (FALSE)
}
```

**Penjelasan**

- `if` berarti “jika”. Bagian ini akan dicek dulu apakah kondisinya benar (`TRUE`).
- `else` berarti “jika tidak”. Bagian ini dijalankan jika kondisi `if` tidak terpenuhi (`FALSE`).
- **Kondisi** biasanya berupa ekspresi logika, misalnya `>`, `<`, `==`, `!=`, `>=`, `<=`.

## Contoh Sederhana dari Kehidupan Sehari-hari

### **Contoh 1:**

Bayangkan kamu ingin menentukan apakah kamu bisa menonton film di bioskop berdasarkan umurmu.

### **Contoh Kasus:**

Seseorang hanya boleh menonton film jika **usia ≥ 17 tahun**.

**Contoh Kode PHP:**

```php
<?php
$umur = 16;

if ($umur >= 17) {
    echo "Kamu boleh menonton film ini.";
} else {
    echo "Maaf, kamu belum cukup umur untuk menonton film ini.";
}
?>
```

**Penjelasan:**

- PHP akan memeriksa apakah `$umur` lebih besar atau sama dengan 17.
- Jika **ya (TRUE)**, maka pesan “Kamu boleh menonton film ini.” akan tampil.
- Jika **tidak (FALSE)**, maka program akan menampilkan pesan “Maaf, kamu belum cukup umur untuk menonton film ini.”

### **Contoh 2**

Misalnya, kita ingin menentukan apakah seseorang harus membawa payung atau tidak.

```php
<?php
$cuaca = "hujan";

if ($cuaca == "hujan") {
    echo "Bawa payung sebelum keluar rumah!";
} else {
    echo "Cuaca cerah, tidak perlu membawa payung.";
}
?>
```

**Penjelasan:**

- Jika nilai variabel `$cuaca` adalah `"hujan"`, maka program menampilkan pesan **“Bawa payung sebelum keluar rumah!”**.
- Jika nilai `$cuaca` **bukan "hujan"**, maka program menampilkan **“Cuaca cerah, tidak perlu membawa payung.”**

Dengan `if...else`, kamu bisa membuat program yang **lebih cerdas dan interaktif**, karena mampu **mengambil keputusan** seperti manusia.
