# Praktikum - `if...elseif...else` statement

Petunjuk: Kerjakan soal di bawah ini dengan membuat kode PHP dari setiap soal.

Pada setiap file PHP tambahkan kode ini di bagian awal setelah pembuka \`\<?php\`

```php
/**
* Nama: Tuliskan Nama Kalian
* Tanggal: Isikan tanggal praktikum
*/
```

## Soal 1: Menentukan Kelulusan Siswa

**Deskripsi:**

Buat program PHP untuk menentukan apakah siswa **lulus** atau **tidak lulus** berdasarkan nilai ujian.

- Siswa **lulus** jika nilai ≥ 60.
- Siswa **tidak lulus** jika nilai \< 60.

**Kode dasar (salin dan lengkapi):**

```php
<?php
$nilai = 75; // Ubah nilai ini untuk mencoba nilai lain

if (__________) {
    echo "Selamat, Anda LULUS!";
} else {
    echo "Maaf, Anda TIDAK LULUS.";
}
?>
```

**Tugas:**

Lengkapi kondisi pada `if` agar program menampilkan hasil yang sesuai berdasarkan nilai siswa.

## Soal 2: Menentukan Bilangan Positif atau Negatif

**Deskripsi:**

Buat program PHP untuk menentukan apakah suatu bilangan merupakan **bilangan positif**, **negatif**, atau **nol**.

**Kode dasar (salin dan lengkapi):**

```php
<?php
$angka = -7; // Ubah nilai ini untuk mencoba angka lain

if (__________) {
    echo "Bilangan positif";
} elseif (__________) {
    echo "Bilangan negatif";
} else {
    echo "Bilangan nol";
}
?>
```

**Tugas:**

Lengkapi bagian yang kosong (`__________`) dengan kondisi yang sesuai agar program bekerja dengan benar.

## Soal 3: Menghitung Nilai Akhir Siswa

**Deskrispi:**

Seorang siswa memiliki dua komponen nilai:

- Nilai tugas (40%)
- Nilai ujian (60%)

Siswa dinyatakan **lulus** jika nilai akhir ≥ 60, dan **tidak lulus** jika nilai akhir \< 60.

**Tugas:**

1.  Minta pengguna (atau gunakan variabel) untuk memasukkan nilai tugas dan nilai ujian.
2.  Hitung **nilai akhir** dengan rumus: `nilai_akhir = (0.4 * nilai_tugas) + (0.6 * nilai_ujian)`
3.  Gunakan **if...else** untuk menampilkan apakah siswa **LULUS** atau **TIDAK LULUS**.
4.  Tampilkan nilai akhir di layar.

## Soal 4: Menghitung Biaya Perjalanan

**Deskripsi:**

Sebuah layanan travel mengenakan biaya perjalanan berdasarkan jarak tempuh:

- Jika jarak **≤ 50 km**, tarif per km = **Rp2.000**.
- Jika jarak **\> 50 km**, tarif per km = **Rp1.800** (diskon tarif jarak jauh).

**Tugas:**

1.  Minta pengguna memasukkan **jarak perjalanan (dalam km)**.
2.  Tentukan tarif per km berdasarkan aturan di atas.
3.  Hitung **total biaya perjalanan = jarak × tarif per km**.
4.  Tampilkan **jarak**, **tarif per km**, dan **total biaya perjalanan**.

## Soal 5: Menghitung Diskon Pembelian

**Deskripsi:**

Sebuah toko memberikan diskon berdasarkan total belanja pelanggan:

- Jika total belanja lebih dari **500.000**, pelanggan mendapat **diskon 20%**.
- Jika total belanja antara **200.000 hingga 500.000**, pelanggan mendapat **diskon 10%**.
- Jika total belanja kurang dari **200.000**, **tidak ada diskon**.

**Tugas:**

1.  Minta pengguna (melalui input atau variabel) untuk memasukkan total belanja.
2.  Hitung total yang harus dibayar setelah diskon (jika ada).
3.  Tampilkan **total belanja**, **besar diskon**, dan **total bayar akhir**.

## Soal 6: Menentukan Grade Nilai

**Deskripsi:**

Buat program untuk menentukan **grade huruf** berdasarkan **nilai angka** yang dimasukkan.

<table><tbody><tr><td>Nilai</td><td>Grade</td></tr><tr><td>80 - 100</td><td>A</td></tr><tr><td>70 - 79</td><td>B</td></tr><tr><td>60 - 69</td><td>C</td></tr><tr><td>50 - 59</td><td>D</td></tr><tr><td>&lt; 50</td><td>E</td></tr></tbody></table>

**Kode dasar (salin dan lengkapi):**

```php
<?php
$nilai = 75; // Ubah nilai ini untuk mencoba nilai lain

if (__________) {
    echo "Grade: A";
} elseif (__________) {
    echo "Grade: B";
} elseif (__________) {
    echo "Grade: C";
} elseif (__________) {
    echo "Grade: D";
} else {
    echo "Grade: E";
}
?>
```

**Tugas:**

Lengkapi bagian kondisi `__________` agar program menampilkan grade yang sesuai.

## Soal 7: Menentukan Kategori Umur

**Deskripsi:**

Buat program untuk menentukan kategori umur seseorang.

<table><tbody><tr><td>Umur</td><td>Kategori</td></tr><tr><td>0 - 5 tahun</td><td>Balita</td></tr><tr><td>6 - 12 tahun</td><td>Anak-anak</td></tr><tr><td>13 - 17 tahun</td><td>Remaja</td></tr><tr><td>18 - 59 tahun</td><td>Dewasa</td></tr><tr><td>≥ 60 tahun</td><td>Lansia</td></tr></tbody></table>

**Kode dasar (salin dan lengkapi):**

```php
<?php
$umur = 20; // Ubah nilai ini untuk mencoba umur lain

if (__________) {
    echo "Kategori: Balita";
} elseif (__________) {
    echo "Kategori: Anak-anak";
} elseif (__________) {
    echo "Kategori: Remaja";
} elseif (__________) {
    echo "Kategori: Dewasa";
} else {
    echo "Kategori: Lansia";
}
?>
```

**Tugas:**

Lengkapi bagian `__________` dengan kondisi yang tepat untuk menampilkan kategori umur sesuai aturan.

## Soal 8: Menghitung Potongan Harga

**Deskripsi:**

Sebuah toko memberikan potongan harga berdasarkan **total belanja pelanggan** sebagai berikut:

<table><tbody><tr><td><strong>Total Belanja</strong></td><td><strong>Potongan Harga</strong></td></tr><tr><td>≥ Rp500.000</td><td>15% dari total belanja</td></tr><tr><td>200.000 – 499.999</td><td>10% dari total belanja</td></tr><tr><td>&lt; Rp200.000</td><td>5% dari total belanja</td></tr></tbody></table>

**Tugas:**

1.  Buat program PHP yang meminta input **total belanja**.
2.  Gunakan `**if...elseif...else**` untuk menentukan **persentase potongan harga**.
3.  Hitung dan tampilkan:
    1.  Potongan harga
    2.  Total yang harus dibayar setelah potongan

## Soal 9: Menghitung Biaya Pengiriman Barang

**Deskripsi:**

Sebuah jasa ekspedisi menentukan biaya kirim berdasarkan **berat barang (dalam kg)**:

<table><tbody><tr><td><strong>Berat Barang</strong></td><td><strong>Tarif per kg</strong></td></tr><tr><td>≤ 5 kg</td><td>Rp10.000 per kg</td></tr><tr><td>6 – 10 kg</td><td>Rp9.000 per kg</td></tr><tr><td>&gt; 10 kg</td><td>Rp8.000 per kg</td></tr></tbody></table>

**Tugas:**

1.  Buat program PHP yang meminta input **berat barang**.
2.  Tentukan **tarif per kg** menggunakan `**if...elseif...else**`.
3.  Hitung dan tampilkan:
    1.  Berat barang
    2.  Tarif per kg
    3.  Total biaya pengiriman

---
