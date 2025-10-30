# Variabel pada PHP

## Pendahuluan

Dalam kehidupan sehari-hari, kita sering kali membutuhkan wadah untuk menyimpan sesuatu. Misalnya:

- Dompet untuk menyimpan uang 💰
- Tas untuk menyimpan buku 🎒
- Kulkas untuk menyimpan makanan 🥦

Nah, dalam **pemrograman**, kita juga membutuhkan **wadah untuk menyimpan data**. Wadah tersebut disebut _**variabel**_.

Di dalam PHP, **variabel digunakan untuk menyimpan nilai** seperti teks, angka, atau bahkan hasil perhitungan agar bisa digunakan kembali di bagian lain dari program.

---

## Apa Itu Variabel?

**Variabel** adalah tempat atau wadah untuk menyimpan data di dalam memori komputer.

Data ini bisa berupa:

- Angka (misalnya: 10, 100, 3.14)
- Teks (misalnya: "Halo Dunia")
- Nilai logika (benar/salah atau `true/false`)

Di PHP, semua variabel **selalu diawali dengan tanda** `**$**` **(dolar)**, diikuti oleh nama variabelnya.

**Contoh:**

```php
<?php
$nama = "Indira";
$umur = 20;
$tinggi = 170.5;
?>
```

Pada contoh di atas:

- `$nama` menyimpan teks `"Rakhmat"`
- `$umur` menyimpan angka `20`
- `$tinggi` menyimpan angka desimal `170.5`

## Aturan Penulisan Variabel di PHP

Saat membuat variabel, ada beberapa aturan yang harus kamu ingat:

- WAJIB diawali tanda `$`
- Nama variabel harus dimulai dengan huruf atau garis bawah (`_`)
- Tidak boleh diawali dengan angka
- Tidak boleh ada spasi di dalam nama variabel
- Huruf besar dan kecil dianggap berbeda (_case-sensitive_)

**Contoh Benar:**

```php
$namaLengkap = "Indira Putri";
$_alamat = "Jakarta";
$umur2 = 25;
```

**Contoh Salah:**

```php
$2umur = 25;    // ❌ Salah: diawali angka
$nama lengkap = "Indira"; // ❌ Salah: ada spasi
```

## Contoh Lain Penulisan Variabel

Bayangkan kamu sedang membuat program kasir sederhana di toko.

```php
<?php
$namaBarang = "Roti";
$harga = 15000;
$stok= 20;


echo "Nama Barang: $namaBarang \n";
echo "Harga: Rp $harga \n";
echo "Stok Tersedia: $stok \n";
?>
```

**Penjelasan:**

- `$namaBarang` menyimpan nama barang.
- `$harga` menyimpan harga per barang.
- `$stok` menyimpan jumlah stok barang yang tersedia.

Hasilnya akan menampilkan:

```
Nama Barang: Roti
Harga: Rp 15000
Stok Tersedia: 20
```

## Mengubah Nilai Variabel

Kamu juga bisa **mengganti isi variabel kapan saja**.

```php
<?php
$warna = "Merah";
echo $warna;

$warna = "Biru";
echo $warna;
?>
```

Di sini, nilai `$warna` berubah dari **"Merah"** menjadi **"Biru"**.

Setelah mempelajari materi ini, kamu sudah memahami dasar dari penggunaan **variabel dalam PHP**. Variabel adalah pondasi penting dalam setiap program, karena hampir semua hal yang kita lakukan — mulai dari menyimpan data pengguna, menghitung nilai, hingga menampilkan hasil — melibatkan variabel.

**Ingat:** variabel ibarat kantong ajaib dalam program — kamu bisa menyimpan apapun di dalamnya dan menggunakannya kapan pun dibutuhkan.
