# Apa Itu Tipe Data?

Tipe data adalah klasifikasi jenis data atau bentukan dari suatu data. Ia menjelaskan suatu data: dari jenis apakah ia tersusun? Apakah bilangan riil? Atau kah bilangan pecahan? Atau kah ia data yang tersusun dari bentukan karakter?

Intinya tipe data adalah klasifikasi jenis dari data yang kita ingin simpan dalam sebuah variabel. Hampir seluruh bahasa pemrograman yang ada mendukung berbagai macam jenis tipe data, seperti: integer untuk bilangan rill, boolean untuk `true` dan `false`, string untuk kumpulan karakter, dan sebagainya [1](https://id.wikipedia.org/wiki/Tipe_data).

### Macam-Macam Tipe Data Dalam PHP

Ada berbagai macam tipe data: mulai dari tipe data asli dan tipe data buatan. Untuk PHP sendiri, ia mendukung setidaknya 8 tipe data skalar. Akan tetapi dalam pertemuan ini, sementara kita akan fokuskan dahulu pada pembahasn 5 tipe data saja, karena 5 tipe data ini adalah tipe data yang paling dasar. 5 tipe data tersebut adalah:
| Tipe Data | Keterangan |
| --------- | ---------- |
| Integer | Tipe data yang berupa bilangan bulat. Contoh: 1, 2, 3, 4, 5, dan seterusnya. |
| Float | Tipe data yang berupa bilangan riil. Contoh: 1.1, 2.2, 3.3, 4.4, 5.5, dan seterusnya. |
| String | Tipe data yang berupa kumpulan karakter/teks yang diapit oleh tanda `''` atau `""`. Contoh: "Hello World", "Halo Dunia", "Aku Superman", dan seterusnya. |
| Boolean | Tipe data yang berupa `true` atau `false`. |
| Array | Tipe data yang berupa kumpulan / himpunan data. |

PHP adalah bahasa pemrograman yang bersifat _dinamic typing_, yang artinya ia tidak memiliki aturan ketat terhadap pendefinisian tipe data pada setiap variabel. PHP akan otomatis menentukan tipe data dari suatu variabel tertentu ketika program dijalankan.

## Apa itu Variabel?

Variabel adalah suatu "wadah" yang digunakan untuk menyimpan suatu data atau nilai. Kita bisa menyimpan berbagai macam data dari berbagai macam tipe, misalkan kita menyimpan data teks untuk nama mahasiswa, atau data desimal untuk nilai ipk mahasiswa, dan seterusnya.

### Peraturan Penamaan Variabel

Untuk menyimpan suatu data pada variabel, kita perlu memberi nama terhadap variabel tersebut.

Dalam PHP, terdapat beberapa peraturan dalam pemberian nama variabel sebagaimana pada tabel berikut:

| Peraturan                                  | Keterangan                                                                                                                                                                                                                                                        |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| diawali tanda `$`                          | Setiap nama variabel dalam bahasa pemrograman PHP didefinisikan dengan tanda `$` lalu diikuti oleh nama variabel itu sendiri                                                                                                                                      |
| nama diawali huruf atau _underscore_ (`_`) | Nama variabel PHP harus diawali huruf, atau tanda underscore (`_`). Kita bisa membuat variabel dengan nama `$_nilai` atau `$nilai123` akan **tetapi tidak bisa membuat variabel dengan nama** `$1nilai`                                                           |
| case sensitive                             | PHP membedakan huruf besar dan kecil dalam penamaan variabel. Maka variabel `$nilai`, `$niLai` dan juga `$nIlAi` dianggap 3 variabel yang berbeda                                                                                                                 |
| hanya boleh huruf dan angka                | nama variabel hanya boleh tersusun dari huruf `[a-z]` atau `[A-Z]`, dan juga angka `[0-9]`. Kita tidak bisa memberi nama variabel misalkan dengan tanda `^` atau `&` dan lain sebagainya. Kita juga tidak bisa menggunakan `spasi` dalam penamaan variabel di PHP |
| inisiasi dengan tanda `=`                  | Kita bisa memberi nilai terhadap suatu variabel dengan menggunakan operator sama dengan (`=`). Contoh: `$nama = "Nurul Huda";`                                                                                                                                    |

:::note[NB]
Penamaan suatu variabel disarankan agar menggunakan nama yang sesuai dengan tugas variabel tersebut. Misalkan menggunakan nama `$nilaiMatematika` untuk menyimpan nilai matematika, dan tidak menggunakan nama `$a` untuk menyimpan nama hari misalnya.
:::

## Pembuatan Variabel

Untuk pembuatan variabel dalam PHP, kombinasi sintaksnya adalah sebagai berikut:

```php
<?php

$namaVariabel = [nilai variabel];
```

Bagian `$namaVariabel` adalah nama yang anda berikan untuk variabel tersebut, sedangkan `[nilai variabel]` adalah nilai yang akan anda masukkan ke dalam variabel tersebut.

Nilai variabel ini lah yang menentukan tipe data dari variabel itu sendiri. Jika anda memasukkan angka, maka tipe datanya menjadi tipe data numeric (_integer/float_), jika anda masukkan `true`/`false` maka jadinya adalah `boolean`, dan seterusnya.

### Tipe Data Integer

Tipe data yang pertama adalah `integer`. Ia adalah tipe data yang digunakan untuk menyimpan bilangan bulat.

Kita akan membuat variabel dengan tipe data `integer` lalu menampilkannya dengan perintah `echo`. Kita juga bisa menampilkan tipe data dari variabel tersebut dengan perintah `var_dump`.

Perhatikan kode program berikut:

```php
<?php
# inisiasi dan inisialisasi variabel
$a = 10;
$b = 5;
$c = $a + 5;
$d = $b + (10 * 5);
$e = $d - $c;

# Tampilkan data dengan perintah echo
echo "Variabel a: {$a} <br>";
echo "Variabel b: {$b} <br>";
echo "Variabel c: {$c} <br>";
echo "Variabel d: {$d} <br>";
echo "Variabel e: {$e} <br>";

# mengetahui tipe data dari variabel
var_dump($e);
```

Kode program di atas akan menghasilkan output seperti berikut:

```cli
Variable a: 10
Variable b: 5
Variable c: 15
Variable d: 55
Variable e: 40
int(40)
```

### Tipe Data Float

Untuk tipe data `float`, caranya sama saja dengan `integer`. Hanya saja, ia menerima data desimal dengan angka `.` sebagai pembaginya.

Perhatikan dan praktikkan contoh berikut:

```php
<?php

$nilaiMatematika = 5.1;
$nilaiIPA = 6.7;
$nilaiBahasaIndonesia = 9.3;

# hitung nilai rata-rata
$rataRata = ($nilaiMatematika + $nilaiIPA + $nilaiBahasaIndonesia) / 3;

# Tampilkan data

echo "Matematika: {$nilaiMatematika} <br>";
echo "IPA: {$nilaiIPA} <br>";
echo "Bahasa Indonesia: {$nilaiBahasaIndonesia} <br>";
echo "Rata-rata: {$rataRata} <br>";

# lihat tipe data dari variabel $rataRata
var_dump($rataRata);
```

Kode program di atas akan menghasilkan output seperti berikut:

```cli
Matematika: 5.1
IPA: 6.7
Bahasa Indonesia: 9.3
Rata-rata: 7.0333333333333
float(7.0333333333333)
```

### Tipe Data Boolean

Tipe data `boolean` hanya bisa menampung nilai `true` atau `false`.

Tipe data ini adalah tipe data yang paling simpel, akan tetapi butuh logika yang kuat untuk bisa memanfaatkannya dengan benar.

Berikut ini contoh penggunaan tipe data `boolean` pada PHP:

```php
<?php

$apakahSiswaLulus = true;
$apakahSiswaSudahUjian = false;

var_dump($apakahSiswaLulus);
echo "<br>";
var_dump($apakahSiswaSudahUjian);
```

Output:

```cli
bool(true)
bool(false)
```

### Tipe Data String

Tipe data `string` adalah tipe data yang digunakan untuk menyimpan teks. Semua teks tersebut diapit oleh tanda petik satu (`''`) mau pun tanda pentik dua (`""`).

Pada contoh-contoh di atas, sebenarnya kita telah menggunakan tipe data ini ketika kita memanggil fungsi `echo` yang diikuti setelahnya dengan teks.

Akan tetapi data `string` tersebut tidak kita simpan ke dalam sebuah variabel. Akan tetapi langsung kita tampilkan dengan perintah `echo`.

Sekarang, saya akan beri contoh bagaimana membuat variabel, lalu mengisinya dengan data `string`.

Perhatikan kode program berikut:

```php
<?php

$namaDepan = "Ibnu"; # pakai tanda petik dua
$namaBelakang = 'Jakaria'; # pakai tanda petik satu

# menggabungkan dua variabel dengan tanda
# petik dua
$namaLengkap = "{$namaDepan} {$namaBelakang}";

# anda juga bisa menggabungkan string dengan menggunakan tanda titik (.)
$namaLengkap2 = $namaDepan . ' ' . $namaBelakang;

# [Tampilkan Data]
# kita bisa memasukkan variabel lain jika menggunakan tanda petik dua
echo "Nama Depan: {$namaDepan} <br>";
# ada pun jika pakai tanda petik satu, kita tidak bisa memasukkan variabel
# di dalam string akan tetapi menggabungkannya dengan operator titik (.)
echo 'Nama Belakang: ' . $namaBelakang . '<br>';

echo $namaLengkap;
```

Output:

```cli
Nama Depan: Ibnu
Nama Belakang: Jakaria
Ibnu Jakaria
```

Terdapat beberapa hal yang perlu dibahas terkait tipe data string. Seperti misalnya memotong teks string, me-replace suatu kata dalam string, mengubah string menjadi UPPERCASE atau menjadi lowercase, dan sebagainya.

Hal tersebut akan kita pelajari pada akhir-akhir pembelajaran PHP dasar ini pada pembahasan: `Belajar Memanipulasi String Dalam PHP`.

### Tipe Data Array

Tipe data `array` berfungsi untuk menyimpan himpunan data. Himpunan data tersebut diapit oleh tanda kurung siku (`[]`).

Sebagai contoh, saya memiliki 3 mahasiswa, dan saya ingin menyimpan ketiga nama mahasiswa dalam variabel.

Maka saya bisa melakukan hal tersebut dengan menggunakan tipe data `array` sebagai berikut:

```php
<?php

$listMahasiswa = ["Wahid Abdullah", "Elmo Bachtiar", "Lendis Fabri"];
```

Untuk mengakses isi dari variabel `array`, kita bisa menggunakan indeks. Indeks dimulai dari `0`. Sehingga jika saya akan menampilkan nama pertama dari variabel `$listMahasiswa`, saya akan menggunakan indeks `0` seperti di bawah:

```php
<?php

echo $listMahasiswa[0]; // "Wahid Abdullah"
```

Contoh di atas masih sangat sederhana sekali. Array merupakan tipe data yang cukup kompleks. Kalian tidak akan mempelajarinya sampai detil pada tahap ini agar tidak terlalu membingungkan.
