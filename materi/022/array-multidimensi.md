# Array Multidimesi

Pada materi sebelumnya, kita sudah belajar:

- Array terindeks (menggunakan angka sebagai indeks)
- Array asosiatif (menggunakan key berupa teks)
- Menampilkan array menggunakan perulangan

Sekarang, kita akan belajar tentang **array multidimensi**.

Array multidimensi adalah **array yang berisi array lain di dalamnya**. Dengan kata lain, ini adalah array bersarang (nested array).

## Apa itu Array Multidimensi?

Array multidimensi adalah array yang memiliki lebih dari satu dimensi.

Contoh sederhana:

```php
$data = [
    ["Andi", 20],
    ["Budi", 21],
    ["Citra", 19]
];
```

Struktur:

- $data\[0\]\[0\] → "Andi"
- $data\[0\]\[1\] → 20
- $data\[1\]\[0\] → "Budi"

---

## Jenis Array Multidimensi

### **Array 2 Dimensi**

Array yang memiliki baris dan kolom (seperti tabel)

Contoh:

```php
$nilai = [
    [80, 85, 90],
    [75, 70, 88],
    [92, 87, 89]
];
```

### **Array Multidimensi Asosiatif**

Gabungan array asosiatif di dalam array:

```php
$mahasiswa = [
    [
        "nama" => "Andi",
        "umur" => 20,
        "jurusan" => "Informatika"
    ],
    [
        "nama" => "Budi",
        "umur" => 21,
        "jurusan" => "Sistem Informasi"
    ]
];
```

## Cara Mengakses Data

### **Array 2 Dimensi**

```php
echo $data[0][0]; // Andi
echo $data[1][1]; // 21
```

### **Array Asosiatif Multidimensi**

```php
echo $mahasiswa[0]["nama"]; // Andi
echo $mahasiswa[1]["jurusan"]; // Sistem Informasi
```

## Menampilkan Data dengan Perulangan

### **Menggunakan** `for`

```php
$angka = [
    [1, 2, 3],
    [4, 5, 6]
];

for ($i = 0; $i < count($angka); $i++) {
    for ($j = 0; $j < count($angka[$i]); $j++) {
        echo $angka[$i][$j] . " ";
    }
    echo "\n";
}
```

### **Menggunakan** `foreach`

```php
foreach ($angka as $baris) {
    foreach ($baris as $nilai) {
        echo $nilai . " ";
    }
    echo "\n";
}
```

`foreach` lebih mudah dibaca dan sering digunakan.

## Contoh Kasus Sederhana

Menampilkan data siswa:

```php
$siswa = [
    [
        "nama" => "Andi",
        "nilai" => 85
    ],
    [
        "nama" => "Budi",
        "nilai" => 75
    ]
];

foreach ($siswa as $s) {
    echo "Nama: " . $s["nama"] . "\n";

    if ($s["nilai"] >= 80) {
        echo "Status: Lulus \n\n";
    } else {
        echo "Status: Tidak Lulus \n\n";
    }
}
```

## Kapan Menggunakan Array Multidimensi?

Array multidimensi digunakan ketika:

- Data berbentuk tabel (baris dan kolom)
- Data lebih dari satu kelompok
- Contoh:
  - Data siswa
  - Data produk
  - Data nilai kelas

## Hal Penting yang Perlu Diingat

- Array multidimensi adalah array di dalam array
- Indeks bisa berupa angka atau key (jika asosiatif)
- Gunakan perulangan bersarang (nested loop) untuk menampilkan data
- Struktur harus rapi agar mudah dibaca

---

Array multidimensi sangat berguna untuk mengelola data yang kompleks, seperti data tabel atau kumpulan data yang saling berhubungan. Dengan memahami konsep ini, kamu bisa membuat program yang lebih terstruktur dan kuat.
