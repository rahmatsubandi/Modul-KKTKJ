# Praktik

#### 1. Number

**Soal:**
Buatlah program yang menghitung luas dan keliling lingkaran. Untuk `jari-jari lingkaran` silakan kalian masukan nomor absen kalian sendiri.

Output yang diharapkan (Misalnya `jari-jari lingkaran` saya adalah 2):

```cli
Luas lingkaran: 12.57
Keliling lingkaran: 12.57
```

**Pembahasan:**
Gunakan rumus:

- Luas = π \* r²
- Keliling = 2 _ π _ r

#### 2. String

**Soal:**
Buatlah program untuk memasukkan kalimat dan kemudian menghitung jumlah kata, huruf vokal, dan huruf konsonan dalam kalimat tersebut. Kalian harus mendefinisikan terlebih dahulu kalimat yang ingin di hitung jumlah katanya, misalnya `Ini bapak de budi`.

Output yang diharapkan:

```cli
Jumlah kata: 4
Jumlah huruf vokal: 7
Jumlah huruf konsonan: 7
```

**Pembahasan:**
Gunakan metode string seperti `.split()` dan iterasi untuk menghitung huruf.

#### 3. List

**Soal:**
Buatlah variabel `angka` dengan berisikan 5 data integer, simpan dalam list, kemudian hitung dan tampilkan angka terbesar dan terkecil dari list tersebut.

Output yang diharapkan (Misalkan angka saya `2,4,70,29,50`):

```cli
Angka terbesar: 70
Angka terkecil: 2
```

**Pembahasan:**
Gunakan fungsi `max()` dan `min()` untuk menemukan angka terbesar dan terkecil.

#### 4. Tuple

**Soal:**
Buatlah program yang membuat tuple berisi nama-nama buah (Nama buahnya bebas), lalu tampilkan buah kedua dan terakhir dalam tuple tersebut.

Output yang diharapkan (Misalkan buah yang ada di list saya `apel, jeruk, pisang, mangga, kiwi`):

```cli
Buah kedua: jeruk
Buah terakhir: kiwi
```

**Pembahasan:**
Gunakan indeks untuk mengakses elemen dalam tuple.

#### 5. Dictionary

**Soal:**
Buatlah program yang menampilkan data agen (nama dan umur) dalam dictionary. Silakan kalian definisikan `nama` dan `umur` sesuai keinginan kalian, lalu tampilkan data agen yang telah didefinisikan.

Output yang diharapkan (Misalkan buah yang ada di list saya `apel, jeruk, pisang, mangga, kiwi`):

```cli
Data agen:
Nama: John Wick, Umur: 99
```

**Pembahasan:**
Gunakan metode dictionary seperti `dict[key]` untuk menyimpan dan mengakses data.

#### 6. Tanggal & Waktu

**Soal:**
Buatlah program yang menampilkan tanggal dan waktu saat ini. Selain itu, tampilkan hari dalam seminggu untuk tanggal tersebut.

Output yang diharapkan:

```cli
Tanggal dan waktu saat ini: 2024-10-14 18:43:54.910162
Hari dalam seminggu: Monday
```

**Pembahasan:**
Gunakan modul `datetime` untuk mendapatkan tanggal dan waktu saat ini.

#### 7. Fungsi

**Soal:**
Definisikanlah fungsi yang menerima dua parameter (`bilangan1` dan `bilangan2`) untuk angka nya bisa menggunakan nomor absen kalian dan teman kalian, selanjutnya kembalikan hasil penjumlahan, pengurangan, dan perkalian dari kedua bilangan tersebut. Panggil fungsi tersebut dengan bilangan yang diinginkan.

Output yang diharapkan (Misalnya pada `bilangan1` saya membuat valuenya 27 dan `bilangan2` valuenya 3) maka outputnya:

```cli
Penjumlahan: 30
Pengurangan: 24
Perkalian: 81
```

**Pembahasan:**
Definisikan fungsi dan gunakan `return` untuk mengembalikan nilai.
