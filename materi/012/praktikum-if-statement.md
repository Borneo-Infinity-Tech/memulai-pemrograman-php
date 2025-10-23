# Praktikum - `if` Praktikum

Petunjuk: Kerjakan soal di bawah ini dengan membuat kode PHP dari setiap soal.

Pada setiap file PHP tambahkan kode ini di bagian awal setelah pembuka `<?php`

```php
/**
* Nama: Tuliskan Nama Kalian
* Tanggal: Isikan tanggal praktikum
*/
```

## Soal 1 — Mengecek Nama Pengguna

**Tujuan:** Melatih penggunaan `if` dengan perbandingan string.

**Instruksi:**  
Buat program yang menampilkan **"Halo, Budi!"** jika variabel `$nama` bernilai `"Budi"`.

**Kode dasar (salin ke file** `cek_nama.php`**):**

```php
<?php
$nama = "Budi"; // ubah nilainya untuk mencoba

if ($nama == "Budi") {
    echo "Halo, Budi!";
}
?>
```

## Soal 2 — Mengecek Umur di Atas 10 Tahun

**Tujuan:** Melatih `if` dengan perbandingan angka sederhana.

**Instruksi:**  
Buat program yang menampilkan **"Anda sudah remaja"** jika umur lebih dari 10 tahun.

**Kode dasar (salin ke file** `cek_umur.php`**):**

```php
<?php
$umur = 12; // ubah nilainya untuk mencoba

if ($umur > 10) {
    echo "Anda sudah remaja.";
}
?>
```

## Soal 3 — Mengecek Angka Sama Dengan 10

**Tujuan:** Melatih `if` dengan kondisi kesetaraan.

**Instruksi:**  
Buat program yang menampilkan **"Angka adalah 10"** jika variabel `$angka` bernilai 10.

**Kode dasar (salin ke file** `cek_angka10.php`**):**

```php
<?php
$angka = 10; // ubah nilainya untuk mencoba

if ($angka == 10) {
    echo "Angka adalah 10.";
}
?>
```

## Soal 4 — Cek Anggota Klub

**Instruksi:**

Sebuah klub hanya menerima anggota dengan nama **“Rina”**.  
Buat program yang memeriksa apakah nama seseorang adalah “Rina”.  
Jika iya, tampilkan pesan bahwa orang tersebut **anggota klub**.

_Petunjuk berpikir:_  
Bagaimana cara membandingkan nilai teks dalam variabel dengan teks tertentu?

## Soal 5 — Cek Suhu Panas

**Instruksi:**

Buat program yang menampilkan pesan **“Cuaca panas hari ini”** jika suhu (`$suhu`) lebih dari 30.  
Jika suhu di bawah atau sama dengan 30, tidak menampilkan apa pun.

_Petunjuk berpikir:_  
Gunakan logika perbandingan angka dan pikirkan kapan kondisi suhu > 30 itu benar.

## Soal 6 — Cek Nilai Bonus

**Instruksi:**

Perusahaan memberi bonus jika karyawan bekerja lebih dari **5 tahun**.  
Buat program yang memeriksa lama bekerja (`$lama_kerja`) dan menampilkan pesan **“Anda mendapat bonus!”** jika memenuhi syarat.

💡 _Petunjuk berpikir:_  
Gunakan `if` dengan kondisi sederhana berbasis angka, dan bayangkan beberapa contoh nilai untuk menguji kebenarannya.

## Soal 7 — Cek Usia dan Status Pelajar

**Deskripsi:**  
Seseorang hanya boleh mendapatkan kartu pelajar jika **umur di bawah 18 tahun** **dan** statusnya adalah **pelajar**.  
Buat program yang menampilkan pesan **“Anda berhak mendapatkan kartu pelajar”** jika kedua syarat tersebut terpenuhi.

💡 _Petunjuk berpikir:_  
Gunakan operator logika `&&` karena **dua kondisi harus benar sekaligus**.  
Pikirkan: apa yang terjadi jika salah satu kondisi salah?

## Soal 8 — Cek Diskon Akhir Pekan

**Deskripsi:**  
Sebuah toko memberikan diskon jika **hari adalah Sabtu atau Minggu**.  
Buat program yang menampilkan pesan **“Diskon spesial hari ini!”** jika hari termasuk dua hari tersebut.

💡 _Petunjuk berpikir:_  
Gunakan operator logika `||` karena **cukup salah satu kondisi benar** agar pesan muncul.  
Coba bayangkan nilai `$hari = "Sabtu"` dan `$hari = "Senin"` untuk menguji logikanya.

## Soal 9 — Cek Login Sederhana

**Deskripsi:**  
Buat program yang memeriksa apakah nama pengguna adalah `"admin"` **dan** kata sandinya `"1234"`.  
Jika kedua kondisi benar, tampilkan **“Login berhasil”**.

💡 _Petunjuk berpikir:_  
Gunakan `&&` antara dua perbandingan string.  
Coba pikirkan apa yang akan terjadi jika hanya satu dari dua data benar.

---

## [Praktikum 2]


