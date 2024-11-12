# Apa itu PHP?

Kita masuk dari pembahasan yang pertama, yaitu tentang file PHP.

File PHP adalah file yang berekstensi `*.php`, diawali dengan sintaks `<?php` dan diakhiri dengan sintaks `?>`.

Contoh:

```php
<?php

echo "Halo dunia!";
```

> {quote} **Kode 1:** Hello world dengan php

Atau bisa kalian singkat dengan:

```php
<?= "Halo dunia!"; ?>
```

Tanda `<?=` adalah singkatan dari `<?php echo`.

Jika file murni PHP saja, tidak bercampur dengan file yang lain. Kita boleh untuk tidak menutup file tersebut dengan `?>` seperti contoh pada **Kode 1** di atas. Dan ini adalah cara yang disarankan.

Ada pun jika kode program kita bercampur dengan “konten” non-php. Maka kita perlu menggunakan sintaks penutup (`?>`) untuk memperjelas mana yang harus dieksekusi sebagai file php, dan mana yang bukan.

Perhatikan kode program pada **Kode 2** di bawah di mana sintaks PHP bercampur dengan sintaks HTML.

```php
<!DOCTYPE html>
<html>
  <body>

    <h1>Halaman HTML</h1>
    <?php
    echo "Halo dunia!";
    ?>

  </body>
</html>
```

> {quote} **Kode 2:** Hello world php yang bercampur dengan konten non php

Kode program pada contoh **Kode 2** di atas harus disimpan dengan ekstensi `.php`. Jika tidak, maka itu akan dianggap teks HTML biasa.

## Komentar dalam File PHP

Kita telah mengetahui dari contoh di atas bahwasanya sintaks php adalah semua yang diapit oleh tag `<?php` dan `?>`. Akan tetapi, ada satu bagian file php yang keberadaannya seperti tidak ada, alias tidak dianggap: yaitu baris komentar.

Baris komentar dalam php ada 2 jenis: _inline_ dan _multiple_ lines. Anda bisa memanfaatkan komentar dalam PHP untuk menulis catatan tentang fungsi atau alur dari kode program yang anda tulis.

### Contoh Komentar Inline

Pada PHP, ada dua cara untuk mendefinisikan komentar _inline_. Yang pertama seperi umumnya komentar pada bahasa pemrograman yang lain, yaitu menggunakan sintaks _double slash_ (`//`). Dan cara yang kedua adalah dengan menggunakan tanda pagar atau _hashtag_ (`#`).

Perhatikan contoh pada **Kode 3** berikut:

```php
<?php

# Ini adalah komentar satu baris dengan tanda pagar (#)
// ini juga komentar satu baris tapi dengan tanda double-slash (//)
echo "Halo dunia!";
```

> {quote} **Kode 3:** komentar inline php

### Contoh Komentar Multiple-Lines

Jenis komentar yang kedua adalah komentar _multiple lines_. Ia diawali tanda `/**` dan diakhiri dengan tanda `*/`.
Agar lebih bagus, biasanya setiap baris komentar akan ditambahkan tanda bintang `*`.

```php
<?php

/**
 * Terkadang anda ingin menggunakan komentar dalam bentuk beberapa baris
 * Anda bisa menulisnya seperti ini
 *
 * NB: Ini biasa digunakan untuk menjelaskan logika/alur program yang cukup panjang
 */

echo "Halo dunia!";
```

> {quote} **Kode 4:** komentar multiple-lines php

Seperti yang anda saksikan pada **Kode 3** dan **Kode 4**, kita bisa menambahkan komentar pada file php kita tanpa mempengaruhi program kita sama sekali. Untuk komentar _inline_, kita bisa menggunakan tanda `#` mau pun tanda `//`. Ada pun untuk _multiple lines_, anda bisa menggunakan tanda `/**` dan ditutup dengan tanda `*/`.
