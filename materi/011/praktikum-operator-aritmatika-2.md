# Praktikum - Operator Aritmatika 2

Petunjuk: Kerjakan soal di bawah ini dengan membuat kode PHP dari setiap soal.

Pada setiap file PHP tambahkan kode ini di bagian awal setelah pembuka `<?php`

```php
/**
* Nama: Tuliskan Nama Kalian
* Tanggal: Isikan tanggal praktikum
*/
```

---

## Soal 1 - Split Bill (Patungan Makanan)

**Tujuan:** membagi tagihan rata dengan biaya layanan.

**Input:** total tagihan, biaya layanan (%), jumlah orang.

**Proses:** `total_akhir = total * (1 + biaya_layanan/100)` → `per_orang = total_akhir / orang`

**Output:** `Perorang: Rp. <per_orang>`

## Soal 2 - Estimasi Biaya Bensin

**Tujuan:** menghitung kebutuhan liter dan biaya perjalanan.

**Input:** jarak (km), konsumsi (km/liter), harga per liter.

**Proses:** `liter = jarak / konsumsi` → `biaya = liter * harga`

**Output:**

- `Keperluan bensin: <liter> L`
- `Biaya: <biaya dalam integer>`

## Soal 3 - BMI (Indeks Massa Tubuh)

**Tujuan:** menghitung indeks massa tubuh.

**Input:** berat (kg), tinggi (cm)

**Proses:** ubah tinggi ke meter → `BMI = berat / (tinggi ** 2)`

**Output:** `BMI: <Hasil perhitungan BMI>`

## Soal 4 - Konversi Kurs: Rupiah → USD

**Tujuan:** menghitung USD diterima setelah biaya admin.

**Input:** rupiah ditukar, kurs (Rp per 1 USD), biaya admin (%)

**Proses:** `rp_bersih = rupiah * (1 - admin/100)` → `usd = rp_bersih / kurs`

**Output:** `Konversi USD: <usd>`

## Soal 5 - Tarif Parkir Flat

**Tujuan:** menghitung total parkir

**Input:** biaya masuk, tarif per jam, durasi dalam jam

**Proses:** `total = masuk + (per_jam * jam)`

**Output:** `Total Bayar: <total>`

## Soal 6 - Efektivitas Paket Data

**Tujuan:** menghitung sisa kuota dan biaya per GB yang terpakai.

**Input:** kuota awal (GB), pemakaian harian rata-rata (MB), jumlah hari terpakai, harga paket (Rp).

**Proses:**

- `terpakai_GB = (pemakaian_MB * hari) / 1024`
- `sisa_GB = kuota_awal - terpakai_GB`
- `biaya_per_GB = harga / kuota_awal`
- `biaya_efektif = (terpakai_GB / kuota_awal) * harga`

**Output:**

- `Terpakai: <terpakai_GB> GB`
- `Sisa: <sisa_GB> GB`
- `Biaya/GB: Rp <biaya_per_GB>`
- `Biaya Efektif: Rp <Biaya_efektif>`

## Soal 7 - Cicilan Flat per Bulan

**Tujuan:** menghitung angsuran bulanan dengan bunga **flat.**

**Input:** harga barang, DP (%), bunga flat per tahun (%), tenor (bulan).

**Proses:**

- `nominal dp = harga * (dp/100)`
- `pokok = harga - nominal dp`
- `bunga_total = pokok * (bunga_tahun/100) * (tenor/12)`
- `total_bayar = pokok + bunga_total`
- `angsuran_bulanan = total_bayar / tenor`

**Output:**

- `DP: Rp <nominal dp>`
- `Poko pinjaman: Rp <pokok>`
- `Total bunga: Rp <bunga_total>`
- `Angsuran perbulan: Rp <angsuran_bulanan>`

