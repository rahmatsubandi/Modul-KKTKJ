# Tugas

### Manajemen Data Buku

Buatlah program manajemen data buku yang memungkinkan pengguna untuk melakukan beberapa operasi dasar terkait buku. Program ini harus dapat:

1. Menambahkan buku ke dalam daftar.
2. Menampilkan semua buku yang ada dalam daftar.
3. Menghapus buku berdasarkan judul.
4. Mencari buku berdasarkan nama penulis.

### Langkah-langkah yang Harus Dilakukan

1. **Buat Kelas Buku**

   - **Definisikan Kelas**: Buatlah kelas bernama `Buku`.
   - **Atribut Kelas**: Kelas ini harus memiliki dua atribut:
     - `judul`: untuk menyimpan judul buku.
     - `penulis`: untuk menyimpan nama penulis buku.
   - **Metode `__str__`**: Buatlah metode ini untuk mengembalikan string yang menampilkan informasi buku dalam format "judul oleh penulis".

2. **Buat Daftar Buku**

   - **Inisialisasi List**: Buatlah sebuah list kosong bernama `daftar_buku` untuk menyimpan objek-objek buku yang ditambahkan.

3. **Buat Fungsi untuk Menambahkan Buku**

   - **Fungsi `tambah_buku`**: Buatlah fungsi ini yang menerima dua parameter: `judul` dan `penulis`.
   - **Validasi Input**: Pastikan bahwa input judul dan penulis tidak kosong.
   - **Buat Objek Buku**: Jika valid, buat objek `Buku` baru dan tambahkan ke dalam `daftar_buku`.
   - **Berikan Umpan Balik**: Tampilkan pesan konfirmasi bahwa buku telah ditambahkan.

4. **Buat Fungsi untuk Menampilkan Buku**

   - **Fungsi `tampilkan_buku`**: Buatlah fungsi ini untuk menampilkan semua buku dalam daftar.
   - **Cek Daftar Kosong**: Jika daftar kosong, tampilkan pesan yang sesuai. Jika tidak, tampilkan semua buku dengan memanggil metode `__str__`.

5. **Buat Fungsi untuk Menghapus Buku**

   - **Fungsi `hapus_buku`**: Buatlah fungsi ini yang menerima parameter `judul`.
   - **Filter Daftar Buku**: Hapus buku dari `daftar_buku` berdasarkan judul yang diberikan (gunakan pencarian case-insensitive).
   - **Berikan Umpan Balik**: Tampilkan pesan konfirmasi apakah buku berhasil dihapus atau tidak ditemukan.

6. **Buat Fungsi untuk Mencari Buku**

   - **Fungsi `cari_buku_berdasarkan_penulis`**: Buatlah fungsi ini yang menerima parameter `penulis`.
   - **Pencarian Case-Insensitive**: Cari buku berdasarkan nama penulis dan tampilkan hasilnya.
   - **Berikan Umpan Balik**: Tampilkan semua buku yang ditemukan atau pesan jika tidak ada.

7. **Buat Menu Utama**
   - **Loop Menu**: Buatlah loop yang terus menampilkan menu hingga pengguna memilih untuk keluar.
   - **Opsi Menu**: Tampilkan opsi untuk menambahkan, menampilkan, menghapus, mencari buku, dan keluar.
   - **Input Pilihan**: Ambil input dari pengguna dan jalankan fungsi yang sesuai berdasarkan pilihan yang dipilih.

#### Kriteria

- Input `judul` dan `penulis` tidak boleh kosong.
- Pencarian buku tidak `case-sensitive`.
- Program harus memberikan umpan balik yang jelas kepada pengguna, terutama saat buku ditambahkan, dihapus, atau tidak ditemukan.

#### Output yang Diharapkan

- Ketika menambahkan buku: "Buku `'judul'` telah ditambahkan."
- Ketika menampilkan buku: "Daftar Buku: judul oleh penulis."
- Ketika menghapus buku: "Buku `'judul'` telah dihapus." atau "Buku `'judul'` tidak ditemukan."
- Ketika mencari buku: "Hasil Pencarian: judul oleh penulis." atau "Tidak ditemukan buku oleh penulis tersebut."

### Pengumpulan Tugas:

Silakan kumpulkan di link berikut:

[https://forms.gle/UWChnuCVgHyamypJ9](https://forms.gle/UWChnuCVgHyamypJ9)

:::danger[CATATAN]
Pengumpulan tugas paling lambat **27 Oktober 2024 Pukul 21:00 WIB**.
Tidak ada toleransi dengan alasan yang kurang jelas.
:::

:::note[Kutipan dalam tugas]

Ingin menyerah? Klik [di sini](<https://cdn0-production-images-kly.akamaized.net/E-hI3mzWgOEG2JxOFSBzCsHRFLs=/640x640/smart/filters:quality(75):strip_icc():format(webp)/kly-media-production/medias/4269258/original/073485600_1671687164-FkZR3RfacAAXsYR.jpg>) untuk mendapatkan semangat baru.

:::
