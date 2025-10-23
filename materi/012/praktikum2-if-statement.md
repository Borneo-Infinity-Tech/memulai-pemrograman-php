# Praktikum - `if` Praktikum

Petunjuk: Kerjakan soal di bawah ini dengan membuat kode PHP dari setiap soal.

Pada setiap file PHP tambahkan kode ini di bagian awal setelah pembuka `<?php`

```php
/**
* Nama: Tuliskan Nama Kalian
* Tanggal: Isikan tanggal praktikum
*/
```

## Soal 1 — Cek Umur Dewasa

**Deskripsi:**

Buat program yang meminta pengguna memasukkan umur.

Jika umur **lebih dari atau sama dengan 18**, tampilkan pesan **“Anda sudah dewasa.”**

Kode (salin ke file `cek_umur.php`):

```php
<?php
$umur = readline("Masukkan umur Anda: ");

if ($umur >= 18) {
    echo "Anda sudah dewasa.";
}
?>
```

## Soal 2 — Cek Angka Positif

**Tujuan:** Melatih logika dasar dengan input angka.

**Deskripsi:**

Buat program yang meminta pengguna memasukkan sebuah angka.

Jika angka tersebut **lebih dari 0**, tampilkan pesan **“Angka positif.”**

**Petunjuk:**

Gunakan `readline()` untuk menerima input, lalu `if` untuk memeriksa kondisinya.

## Soal 3 — Cek Nama Spesial

**Tujuan:** Melatih perbandingan teks (string).

**Deskripsi:**

Buat program yang meminta pengguna memasukkan nama.

Jika nama yang dimasukkan adalah **“Andi”**, tampilkan pesan **“Halo, Andi!”**

**Petunjuk:**

Gunakan tanda kutip `" "` untuk membandingkan string di dalam `if`.

## Soal 4 — Cek Total Belanja Diskon

**Deskripsi:**

Buat program yang meminta pengguna memasukkan total belanja.

Jika total belanja **lebih dari 100000**, tampilkan pesan **“Anda mendapat diskon 10%”** dan hitung jumlah setelah diskon.

Kode (salin ke file `diskon.php`):

```php
<?php
$total = readline("Masukkan total belanja: ");

if ($total > 100000) {
    $diskon = $total * 0.1;
    $bayar = $total - $diskon;
    echo "Anda mendapat diskon 10%.\n";
    echo "Total yang harus dibayar: Rp $bayar";
}
?>
```

## Soal 5 — Cek Kelulusan Berdasarkan Nilai Rata-Rata

**Deskripsi:**

Program meminta pengguna memasukkan **3 nilai ujian**, lalu menghitung **rata-ratanya**. Jika rata-rata **≥ 70**, tampilkan **“Anda lulus.”**

**Petunjuk:**

Buat 3 input untuk 3 nilai, lakukan perhitungan rata-rata nilai, dan lakukan pengecekan menggunakan `if`.

## Soal 6 — Cek Gaji Setelah Bonus

**Deskripsi:**

Buat program yang meminta pengguna memasukkan **gaji pokok**.

Jika gaji pokok **lebih dari atau sama dengan 5000000**, berikan **bonus 500000** dan tampilkan total gajinya.

**Petunjuk:**

Buat input untuk memasukkan gaji pokok. lakukan pengecekan dengan if, apabila kondisi benar tambahkan gaji pokok dengan bonus lalu tampilkan total gaji.
