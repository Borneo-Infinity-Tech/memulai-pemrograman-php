# Operator Perbandingan

**Operator perbandingan** dipakai untuk membandingkan dua nilai dan menghasilkan **boolean** : `true` atau `false`. Operator ini sering digunakan pada **kondisi** (misal. `if`, `while`).

## Daftar Operator Perbandingan PHP

### 1) Sama / Tidak Sama

- `==` (sama, **loose**)
  Bandingkan nilai dengan konversi tipe bila perlu.

  **Contoh:** `"5" == 5` nilai `true`

- `===` (identik, **strict**)

  Nilai dan tipe data harus sama.

  **Contoh:** `"5" === 5` nilai `false`

- `!=` (tidak sama, **loose**)

  True jika nilainya beda (boleh konversi tipe).

  **Contoh:** `7 != "7.0"` nilai `false`

- `!==` (tidak identik, **strict**)

  True jika nilai atau tipe berbeda.

  **Contoh:** `7 !== 7.0` nilai `true`

### 2) Lebih Kecil/Besar

- `<` (lebih kecil)

  **Contoh:** `3 < 5` nilai `true`

- `>` (lebih besar)

  **Contoh:** `10 > 2` nilai `true`

- `<=` (lebih kecil atau sama)

  **Contoh:** `5 <= 5` nilai `true`

- `>=` (lebih besar atau sama)

  **Contoh:** `6 >= 7` nilai `true`
