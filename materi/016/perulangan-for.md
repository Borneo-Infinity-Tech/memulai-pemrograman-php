# Perulangan `for`

Dalam pemrograman PHP, sering kali kita harus menjalankan sebuah perintah yang sama secara berulang-ulang. Contohnya menampilkan angka 1 sampai 10, mencetak daftar nama, atau menampilkan data secara berurutan. Jika perintah tersebut ditulis satu per satu, kode akan menjadi panjang dan kurang efisien. Untuk mengatasi hal tersebut, PHP menyediakan struktur **perulangan** `**for**`. Perulangan ini sangat berguna ketika kita sudah mengetahui berapa kali suatu perintah akan diulang.

## Pengertian Perulangan `for`

Perulangan `for` adalah perulangan yang digunakan ketika jumlah pengulangan sudah diketahui sejak awal. Perulangan ini akan menjalankan sebuah blok kode selama kondisi yang ditentukan bernilai benar (true).

Perulangan `for` terdiri dari tiga bagian utama, yaitu:

1.  **Inisialisasi** → nilai awal perulangan
2.  **Kondisi** → syarat agar perulangan terus berjalan
3.  **Perubahan nilai** → proses perubahan nilai (biasanya bertambah atau berkurang)

## Struktur Dasar Perulangan `for`

Struktur dasar perulangan `for` dalam PHP adalah sebagai berikut:

```
for (inisialisasi; kondisi; perubahan_nilai) {
    // kode yang akan diulang
}
```

Penjelasan:

- **Inisialisasi**: dijalankan satu kali di awal perulangan
- **Kondisi**: dicek setiap kali sebelum perulangan dijalankan
- **Perubahan nilai**: dijalankan setiap kali perulangan selesai satu putaran

## Contoh Perulangan `for`

Contoh menampilkan angka 1 sampai 5:

```php
for ($i = 1; $i <= 5; $i++) {
    echo $i;
}
```

Penjelasan:

- `$i = 1` → nilai awal perulangan
- `$i <= 5` → perulangan berjalan selama nilai `$i` kurang dari atau sama dengan 5
- `$i++` → nilai `$i` bertambah 1 setiap perulangan

Hasil yang ditampilkan adalah:

```
12345
```

### **Contoh Perulangan** `for` **dengan Teks**

Menampilkan teks berulang kali:

```php
for ($i = 1; $i <= 3; $i++) {
    echo "Belajar PHP<br>";
}
```

Kode di atas akan menampilkan teks **"Belajar PHP"** sebanyak 3 kali.

### **Perulangan** `for` **dengan Penambahan dan Pengurangan**

Perulangan `for` tidak hanya bisa bertambah, tetapi juga bisa berkurang.

**Contoh bertambah:**

```php
for ($i = 1; $i <= 10; $i++) {
    echo $i;
}
```

Perulangan ini akan menampilkan angka dari 1 sampai 9.

**Contoh berkurang:**

```php
for ($i = 5; $i >= 1; $i--) {
    echo $i;
}
```

## Manfaat Menggunakan Perulangan `for`

Beberapa manfaat penggunaan perulangan `for` dalam PHP:

- Kode menjadi lebih singkat dan rapi
- Mudah digunakan untuk perulangan dengan jumlah tertentu
- Mengurangi pengulangan penulisan kode
- Cocok untuk proses data yang berurutan

Perulangan `for` merupakan salah satu perulangan dasar yang sangat penting dalam PHP. Perulangan ini digunakan ketika jumlah pengulangan sudah diketahui. Dengan memahami cara kerja inisialisasi, kondisi, dan perubahan nilai, kita dapat menggunakan perulangan `for` dengan baik dan benar.

Pemahaman perulangan `for` akan menjadi dasar untuk mempelajari perulangan lainnya serta pengolahan data yang lebih kompleks dalam pemrograman PHP.

---

[Latihan Soal Perulangan for](/materi/016/latihan.md)
