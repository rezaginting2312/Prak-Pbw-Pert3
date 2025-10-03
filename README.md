# Prak-Pbw-Pert3
# LaraPress - Aplikasi Blog Sederhana
LaraPress adalah aplikasi blog sederhana yang dibangun menggunakan Laravel 12 untuk tujuan pembelajaran dan pengembangan keterampilan web development.
<img width="1917" height="1079" alt="image" src="https://github.com/user-attachments/assets/0767c983-15fa-473b-98c8-349f824bba92" />
Tampilan halaman utama LaraPress
📋 Tentang Proyek
Proyek ini dibuat sebagai bagian dari pembelajaran Laravel framework. LaraPress mendemonstrasikan konsep-konsep dasar Laravel seperti routing, views, dan struktur MVC.
🚀 Fitur yang Sudah Diimplementasikan
1. Halaman Utama (Welcome Page)
Mengubah tampilan default Laravel menjadi halaman sederhana
Menampilkan judul "Selamat Datang di LaraPress"
Struktur HTML yang bersih dan minimal
2. Halaman Tentang Kami
Route: /tentang-kami
Menampilkan informasi tentang LaraPress
Menjelaskan tujuan proyek sebagai pembelajaran Laravel 12

📁 Struktur File yang Dimodifikasi
File yang Dibuat/Dimodifikasi:
resources/views/welcome.blade.php

Mengubah tampilan default Laravel yang kompleks menjadi struktur HTML sederhana
Menampilkan pesan sambutan untuk pengunjung blog
resources/views/about.blade.php (BARU)

File view baru untuk halaman "Tentang Kami"
Berisi informasi tentang LaraPress sebagai proyek pembelajaran
routes/web.php

Menambahkan route baru /tentang-kami yang mengarah ke view about.blade.php
## 🛠️ Langkah-langkah Implementasi

Step 1: Modifikasi Halaman Welcome
Mengubah file resources/views/welcome.blade.php dari tampilan default Laravel (266 baris) menjadi HTML sederhana:
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Datang di LaraPress</title>
</head>
<body>
    <h1>Selamat Datang di Blog LaraPress</h1>
    <p>Ini adalah halaman utama dari aplikasi blog kita.</p>
</body>
</html>

Step 2: Membuat Route Baru
Menambahkan route baru di routes/web.php:

Route::get('/tentang-kami', function () {
    return view('about');
});

Step 3: Membuat View About
Membuat file baru resources/views/about.blade.php:
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tentang Kami - LaraPress</title>
</head>
<body>
    <h1>Tentang LaraPress</h1>
    <p>LaraPress adalah aplikasi blog sederhana yang dibuat dengan Laravel 12.</p>
    <p>Proyek ini dibuat untuk tujuan pembelajaran dan pengembangan keterampilan.</p>
</body>
</html>

## 💻 Teknologi yang Digunakan
Framework: Laravel 12
PHP Version: 8.x
Database: SQLite (default)
Frontend: Blade Template Engine, HTML, CSS
Build Tool: Vite

📦 Instalasi
Clone repository ini:
git clone https://github.com/adiwp/pbw.git
cd pro1
Install dependencies:
composer install
npm install
Buat file .env:
cp .env.example .env
Generate application key:
php artisan key:generate
Jalankan development server:
php artisan serve
Akses aplikasi di browser:
http://localhost:8000

📸 Screenshot
Halaman Utama

<img width="1918" height="1073" alt="image" src="https://github.com/user-attachments/assets/9d7d7d75-6784-4ca6-9b52-14842fbd62d7" />

Tentang kami
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b9f008b5-6445-4b00-9715-b58ebc5287d6" />

Kontak
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a7cab039-2d1a-435a-a35c-107eda684917" />

## Kesimpulan
Praktikum ini berhasil memperkenalkan dasar-dasar penggunaan Laravel. Mahasiswa mampu menginstal dan menjalankan proyek Laravel, memahami alur kerja request–route–view–response, serta membuat dan menghubungkan halaman statis sederhana. Dengan pemahaman ini mahasiswa memiliki fondasi untuk melanjutkan ke materi Laravel yang lebih kompleks pada pertemuan selanjutnya.

