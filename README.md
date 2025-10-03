# Praktikum Laravel 1 - LaraPress

## 📚 Deskripsi
Praktikum ini memperkenalkan dasar-dasar framework Laravel. Pada pertemuan ini mahasiswa belajar menginstal proyek Laravel baru, menjalankan server development lokal, dan membuat halaman statis sederhana menggunakan Route dan View.

## 📝 Langkah-langkah Praktikum

### 1. Instalasi Laravel “LaraPress”
- Buka terminal/command line (Laragon/XAMPP).
- Navigasi ke folder root server lokal (contoh: `C:\laragon\www`).
- Jalankan perintah:
  ```bash
  composer create-project laravel/laravel LaraPress
  ```
- Tunggu hingga Composer selesai mengunduh paket Laravel.

### 2. Menjalankan Server Development
- Masuk ke folder proyek:
  ```bash
  cd LaraPress
  ```
- Jalankan server bawaan Laravel:
  ```bash
  php artisan serve
  ```
- Buka browser dan akses `http://127.0.0.1:8000`.

### 3. Memahami Alur Dasar Laravel (Route → View)
- Buka proyek di VS Code.
- Edit file `routes/web.php` untuk mendefinisikan route:
  ```php
  Route::get('/', function () {
      return view('welcome');
  });
  ```
- Modifikasi file tampilan `resources/views/welcome.blade.php` dengan HTML sederhana.
- Refresh browser untuk melihat perubahan.

### 4. Membuat Halaman Statis Baru (“Tentang Kami”)
- Tambah route baru di `routes/web.php`:
  ```php
  Route::get('/tentang-kami', function () {
      return view('about');
  });
  ```
- Buat file `resources/views/about.blade.php` berisi HTML halaman “Tentang Kami”.
- Tambahkan link navigasi di kedua view:
  - Di `welcome.blade.php`:
    ```html
    <a href="/tentang-kami">Lihat Halaman Tentang Kami</a>
    ```
  - Di `about.blade.php`:
    ```html
    <a href="/">Kembali ke Halaman Utama</a>
    ```

### 5. Tugas Mandiri (Opsional)
- Buat halaman statis baru bernama **Kontak**.
- Akses melalui `/kontak` dan tambahkan info kontak fiktif.
- Tambahkan link navigasi antarhalaman.

## Halaman Utama
<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/9ea4c7c4-7ff9-4fb5-b935-44a519a214fe" />

## Tentang kami
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/399b4e67-1ad9-4b7a-8583-85319378cad8" />

## Kontak
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e5d42012-7926-459f-9cc0-35a7766cd666" />

## ✅ Kesimpulan Praktikum
Praktikum ini membekali mahasiswa dengan pemahaman dasar framework Laravel.

Mahasiswa berhasil:
- Menginstal proyek Laravel baru dengan Composer.
- Menjalankan server development lokal menggunakan Artisan.
- Membuat dan menghubungkan halaman statis dengan mendefinisikan **Route** dan **View**.

Dengan langkah ini mahasiswa sudah memahami siklus permintaan paling dasar di Laravel (**Request → Route → View → Response**) sebagai fondasi untuk mengembangkan fitur Laravel yang lebih kompleks pada praktikum berikutnya.
