# Proyek 4: Permainan Tebak Angka

### Penjelasan Proyek

Proyek ini adalah permainan tebak angka di mana pengguna harus menebak angka yang dihasilkan secara acak oleh program. Program memberikan umpan balik apakah tebakan pengguna terlalu tinggi, terlalu rendah, atau benar.

#### Fitur

- Menghasilkan angka acak antara 1 hingga 100.
- Memberikan umpan balik kepada pengguna setelah setiap tebakan.
- Menghitung jumlah tebakan yang diperlukan untuk menemukan angka yang benar.

#### Langkah-Langkah

1. Gunakan modul `random` untuk menghasilkan angka acak.
2. Buat loop untuk meminta tebakan dari pengguna.
3. Berikan umpan balik berdasarkan tebakan pengguna.
4. Tampilkan jumlah tebakan setelah pengguna berhasil menebak angka.

#### Deskripsi Detail

- Menggunakan loop `while` untuk terus meminta tebakan hingga pengguna berhasil.
- Menggunakan variabel untuk menyimpan angka acak dan jumlah tebakan.

#### Contoh Output yang Diharapkan

```cli
Selamat datang di permainan Tebak Angka!
Saya telah memilih angka antara 1 hingga 100. Coba tebak!
Masukkan tebakan Anda: 50
Tebakan Anda terlalu rendah. Coba lagi!
Masukkan tebakan Anda: 75
Tebakan Anda terlalu tinggi. Coba lagi!
Masukkan tebakan Anda: 62
Selamat! Anda berhasil menebak angka 62 dalam 3 tebakan.
```
