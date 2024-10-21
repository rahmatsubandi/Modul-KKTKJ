# Praktik

### 1. Modul

**Soal:**
Buatlah sebuah modul Python yang berisi dua fungsi:

- `tambah(a, b)`: mengembalikan hasil penjumlahan dari `a` dan `b`.
- `kurang(a, b)`: mengembalikan hasil pengurangan dari `a` dan `b`.

Definisikan `a` dan `b` sesuai dengan nomor absen kalian dan teman kalian.
Setelah itu, panggilah kedua fungsi tersebut di bawahnya dan cetak hasilnya.

Output yang diharapkan (Misalnya pada `a` saya membuat valuenya 10 dan `b` valuenya 5):

```cli
Hasil tambah: 15
Hasil kurang: 5
```

**Pembahasan:**
Karna kita menggunakan Google Colab kalian tidak perlu menuliskan `import` modul, cukup definisikan fungsi dan panggil fungsi tersebut.

### 2. File I/O

**Soal:**
Buatlah sebuah program yang:

- Meminta input dari pengguna untuk menuliskan beberapa kalimat.
- Menyimpan kalimat-kalimat tersebut dalam sebuah list.
- Setelah pengguna selesai memasukkan kalimat (dengan menekan Enter tanpa mengetik apa pun), program harus menampilkan semua kalimat yang telah dimasukkan beserta jumlah karakter dari setiap kalimat.

Output yang diharapkan (Misalnya pengguna memasukkan kalimat "aku ingin bebas", "siap grak", dan "ashiapppp"):

```cli
Masukkan kalimat (tekan Enter untuk selesai):
aku ingin bebas
siap grak
ashiapppp


Kalimat yang telah dimasukkan:
- aku ingin bebas (15 karakter)
- siap grak (9 karakter)
- ashiapppp (9 karakter)
```

**Pembahasan:**
Setiap kalimat yang dimasukkan oleh pengguna akan disimpan dalam list. Setelah pengguna menekan Enter tanpa mengetik apa pun, program akan menampilkan semua kalimat yang telah dimasukkan beserta jumlah karakter dari setiap kalimat.
Kalian bisa menggunakan `input()` untuk meminta input dari pengguna dan `len()` untuk menghitung jumlah karakter dari kalimat yang dimasukkan.

### 3. Exception

**Soal:**
Buatlah program yang meminta input angka dari pengguna dan melakukan pembagian 100 dengan angka tersebut.

- Jika pengguna memasukkan angka 0, program harus menangani exception dan menampilkan pesan "Tidak bisa membagi dengan nol!".
- Jika input bukan angka, tampilkan pesan "Input tidak valid! Masukkan angka."

Output yang diharapkan (Misalnya pengguna memasukkan angka 20):

```cli
Masukkan angka: 20
Hasil pembagian 100 dengan 20.0 adalah 5.0
```

**Pembahasan:**
Kalian bisa menggunakan `try` dan `except` untuk menangani exception. Jika pengguna memasukkan angka 0, program akan menampilkan pesan "Tidak bisa membagi dengan nol!". Jika input bukan angka, program akan menampilkan pesan "Input tidak valid! Masukkan angka.".

### 4. Object & Class

**Soal:**
Buatlah sebuah class `Mobil` yang memiliki atribut:

- `merk`
- `tahun`
- `warna`

Class tersebut harus memiliki metode:

- `deskripsi()`: yang mengembalikan string yang menjelaskan mobil tersebut, misalnya "Mobil merk Toyota, tahun 2020, warna merah."

Kemudian, buatlah program yang meminta pengguna untuk memasukkan nilai untuk `merk`, `tahun`, dan `warna`, lalu tampilkan deskripsi mobil menggunakan metode `deskripsi()`.

Output yang diharapkan (Misalnya pengguna memasukkan merk "Toyota", tahun "2020", dan warna "merah"):

```cli
Mobil merk Toyota, tahun 2018, warna Hitam.
```

**Pembahasan:**
Kalian bisa menggunakan `input()` untuk meminta input dari pengguna dan membuat objek dari class `Mobil` dengan atribut yang sesuai. Kemudian, panggil metode `deskripsi()` untuk menampilkan deskripsi mobil tersebut.
Jangan lupa untuk `tahun` yang kalian inputkan harus bertipe `int`. Lalu buat variabel `mobil_user` untuk membuat objek dari class `Mobil`, dan print deskripsi mobil tersebut.
