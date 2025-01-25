# KasirKue
membuat fitur kasir untuk pedagang kue

# Cara Menjalankannya

# Buat Database:
Buat database menggunakan database management system yang Anda gunakan (misalnya MySQL).
# Buat Tabel items:
Buat tabel untuk model Items yang memiliki struktur:
id (primary key)
name (string)
qty_stock (integer)
price (float)
# Buat table users:
Buat tabel Users mungkin memiliki:
id (primary key)
username (string)
password (string)
role (string)

Sambungkan Aplikasi ke Database:
Pastikan pengaturan koneksi database di file models/items.js dan models/users.js sesuai dengan databasenya.

# Cara Kerja Web

# Framework dan Library:
Aplikasi menggunakan Express.js sebagai framework server.
Menggunakan EJS sebagai view engine untuk merender halaman HTML secara dinamis.
# Library lain yang digunakan:
jsonwebtoken untuk otentikasi berbasis token.
dotenv untuk mengelola variabel lingkungan.
cookie-parser untuk menangani cookie.

#Fungsi Utama:
Otentikasi: Middleware authToken memastikan bahwa hanya pengguna yang masuk (logged in) yang bisa mengakses rute tertentu.
# Manajemen Barang:
Menampilkan daftar barang di halaman kasir (/kasir).
Menambah, mengedit, dan menghapus barang melalui API.
Mengatur stok barang berdasarkan transaksi.
# Pendapatan:
Pendapatan harian, mingguan, dan bulanan disimpan sementara di server dan diperbarui setelah setiap transaksi.

# API dan Tampilan:
API untuk manajemen barang, pencarian, dan transaksi.
Halaman web untuk login, daftar barang, dan formulir penambahan/edit barang.

# Port Server:
Server berjalan di http://127.0.0.1:5000.

# Catatan: codingan masih dalam tahap pengembangan disebabkan karena fitur kasir yang masih belum berjalan seperti yang diinginkan.
