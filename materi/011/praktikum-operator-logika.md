# Praktikum - Operator Logika

Petunjuk: Kerjakan soal di bawah ini dengan membuat kode PHP dari setiap soal.

Pada setiap file PHP tambahkan kode ini di bagian awal setelah pembuka `<?php`

```php
/**
* Nama: Tuliskan Nama Kalian
* Tanggal: Isikan tanggal praktikum
*/
```

---

## Soal 1 – Lampu dan Televisi

**Konteks:**

Andi ingin menyalakan lampu ruang tamu dan televisi hanya jika kedua stop kontak tersambung listrik.

**Tugas:**

Buat program PHP yang menampilkan `true` jika **lampu** dan **televisi** keduanya tersambung (gunakan operator `&&` atau `AND`, dan `false` jika salah satunya tidak.

```php
<?php
$lampu = true;
$tv = false;

// Tuliskan kode logika di bawah ini
$hasil = ...; // Gunakan operator logika yang sesuai
var_dump($hasil);
?>
```

## Soal 2 – Login Aplikasi

**Konteks:**

Seseorang bisa masuk ke aplikasi jika **username benar** atau **password benar** (anggap hanya salah satu perlu benar untuk latihan ini).

**Tugas:**

Gunakan operator `||` atau `OR` untuk memeriksa apakah login berhasil.

```php
<?php
$usernameBenar = false;
$passwordBenar = true;

// Tuliskan kode logika di bawah ini
$login = ...;
var_dump($login);
?>
```

## Soal 3 – Pergi ke Sekolah

**Konteks:**

Budi hanya bisa berangkat ke sekolah jika **tidak hujan** dan **ada kendaraan**.

**Tugas:**

Gunakan operator `&& (AND)` dan `!` untuk menentukan apakah Budi bisa berangkat ke sekolah. Cetak hasilnya (`true` atau `false`).

```php
<?php
$hujan = true;
$adaKendaraan = true;

// Tuliskan kode logika di bawah ini
$bisaBerangkat = ...;
var_dump($bisaBerangkat);
?>
```

## Soal 4 – Membaca Buku

**Konteks:**

Dina membaca buku hanya kalau **punya waktu luang** dan **tidak mengantuk**.

**Tugas:**

Gunakan kombinasi `&&` dan `!` untuk menentukan apakah Dina membaca buku.

```php
<?php
$punyaWaktu = true;
$mengantuk = false;

// Tuliskan kode logika di bawah ini
$membacaBuku = ...;
var_dump($membacaBuku);
?>
```

## Soal 5 - Nilai Cukup atau Tidak

**Konteks:**

Ani mendapat nilai **75** dari batas kelulusan **70**.

Buat program yang menampilkan **true** jika nilai Ani **lebih besar atau sama dengan** batas kelulusan.

```php
<?php
$nilai = 75;
$batas = 70;

// Tuliskan kode di bawah ini
$lulus = ...;
var_dump($lulus);
?>
```

📘*Petunjuk:* Gunakan operator `>=` untuk membandingkan.

## Soal 6 - Berat Barang dan Ongkir Gratis

**Konteks:**

Sebuah toko memberikan **gratis ongkir** jika berat barang **lebih dari 5 kg** **dan** total harga **lebih dari Rp100.000**.  
Tentukan apakah pelanggan mendapat gratis ongkir atau tidak.

```php
<?php
$berat = 6; // dalam kg
$harga = 120000;

// Tuliskan kode di bawah ini
$gratisOngkir = ...; // Gunakan kombinasi > dan &&
var_dump($gratisOngkir);
?>
```

📘*Petunjuk:* Gunakan `&&` (dan logika) untuk menggabungkan dua kondisi.

## Soal 7 - Diskon Hari Belanja

**Konteks:**

Sebuah toko memberikan diskon jika **total belanja lebih dari Rp200.000** **dan** **jumlah barang minimal 3**.  
Gunakan operator logika untuk menentukan apakah diskon berlaku.

```php
<?php
$totalBelanja = 250000;
$jumlahBarang = 2;

// Tuliskan kode di bawah ini
$dapatDiskon = ...; // Gunakan kombinasi > dan &&
var_dump($dapatDiskon);
?>
```

## Soal 8 - Kehadiran di Sekolah

**Konteks:**

Siswa dinyatakan **rajin** jika **jumlah hari hadir lebih dari atau sama dengan 25** dari **30 hari**, dan **tidak pernah terlambat**.

```php
<?php
$hadir = 26;
$terlambat = false;

// Tuliskan kode di bawah ini
$rajin = ...; // Gunakan kombinasi >= dan !
var_dump($rajin);
?>
```

📘*Petunjuk:* Gunakan `!` untuk membalik nilai dari `$terlambat`.

## Soal 9 - Nilai Akhir Siswa

**Konteks:**

Seorang siswa dinyatakan **naik kelas** jika **rata-rata nilai** tiga pelajaran **≥ 75** dan **tidak ada nilai yang di bawah 60**.

**Tugas:**

Gunakan kombinasi operator aritmatika dan logika untuk menentukan hasilnya (`true` atau `false`).

```php
<?php
$matematika = 80;
$ipa = 70;
$bahasa = 85;

// Tuliskan kode di bawah ini
$rata = ...;
$naikKelas = ...; // Gunakan kombinasi >=, &&, dan >
var_dump($naikKelas);
?>
```

📘*Petunjuk:* Hitung dulu rata-rata, lalu gabungkan dua kondisi logika.

## Soal 10 - Keuangan Bulanan

**Konteks:**

Dika akan **menabung bulan ini** jika **sisa uang setelah pengeluaran ≥ 50000** dan **pendapatan bulan ini > pengeluaran**.

**Tugas:**

Gunakan operator aritmatika (`-`) dan logika (`>=`, `&&`, `>`).

```php
<?php
$pendapatan = 1000000;
$pengeluaran = 950000;

// Tuliskan kode di bawah ini
$sisa = ...;
$menabung = ...;
var_dump($menabung);
?>
```

## Soal 11 - Pemeriksaan Kendaraan

**Konteks:**

Sebuah kendaraan dinyatakan **siap jalan** jika:

- BBM lebih dari 10 liter
- Tekanan ban antara 30 sampai 35 psi
- Rem berfungsi baik (true)

Gunakan operator logika gabungan dan bandingkan nilai tekanan ban menggunakan kombinasi `>`, `<`, dan `&&`.

```php
<?php
$bbm = 12; // liter
$tekananBan = 33; // psi
$remBaik = true;

// Tuliskan kode di bawah ini
$siapJalan = ...;
var_dump($siapJalan);
?>
```

📘 _Petunjuk:_ Gunakan `(kondisi1 && kondisi2 && kondisi3)`.

## Soal 12 - Bonus Karyawan

**Konteks:**

Seorang karyawan mendapat **bonus** jika:

- **Jam kerja ≥ 160 jam per bulan**,
- dan **nilai performa ≥ 80**,
- atau **lembur lebih dari 10 jam**.

Gunakan kombinasi `&&` dan `||` dengan operator aritmatika sederhana.

```php
<?php
$jamKerja = 155;
$lembur = 12;
$performa = 85;

// Tuliskan kode di bawah ini
$bonus = ...;
var_dump($bonus);
?>
```

📘 _Petunjuk:_ Gunakan `(A && B) || C` untuk gabungan kondisi.

## Soal 13 - Perbandingan Gaji dan Biaya Hidup

**Konteks:**

Seorang pegawai ingin tahu apakah **gajinya cukup untuk hidup layak**. Ia dianggap “cukup” jika:

- Gaji dikurangi total pengeluaran masih **lebih dari 1 juta**, **dan**
- Pengeluaran bulanan **tidak lebih dari 70%** dari gajinya.

```php
<?php
$gaji = 6000000;
$pengeluaran = 4000000;

// Tuliskan kode di bawah ini
$sisa = $gaji - $pengeluaran;
$persentase = ($pengeluaran / $gaji) * 100;

$cukup = ($sisa > 1000000) && ($persentase <= 70);
var_dump($cukup);
?>
```

🧠 _Latihan:_ tulis ulang rumus `$cukup` di atas sendiri dan pahami kenapa harus dua kondisi.

## Soal 14 - Tarif Listrik Rumah Tangga

**Konteks:**

Hitung apakah **tagihan listrik melebihi batas wajar**.  
Tagihan dianggap **tidak wajar** jika:

- **Pemakaian kWh > 400**, **atau**
- **Biaya lebih dari 20% dari gaji bulanan**, **dan**
- **Bukan rumah subsidi**.

```php
<?php
$kwh = 450;
$biaya = 800000;
$gaji = 3500000;
$subsidi = false;

// Tuliskan kode di bawah ini
$persen = ($biaya / $gaji) * 100;
$tidakWajar = ($kwh > 400 || $persen > 20) && !$subsidi;
var_dump($tidakWajar);
?>
```

## Soal 15 - Keamanan Login

**Konteks:**

Pengguna dianggap **berhasil login aman** jika:

- Username dan password benar, **dan**
- Jumlah percobaan login **kurang dari 3**, **atau**
- Akun sudah di-_whitelist_ oleh admin.

```php
<?php
$usernameBenar = true;
$passwordBenar = true;
$percobaan = 2;
$whitelist = false;

// Tuliskan kode di bawah ini
$loginAman = (($usernameBenar && $passwordBenar) && $percobaan < 3) || $whitelist;
var_dump($loginAman);
?>
```
