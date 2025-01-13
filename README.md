# IuranWargaApp

## Pendahuluan
Ini adalah project Laravel yang dikembangkan untuk mata kuliah Pemrograman Web. Project ini adalah aplikasi manajemen iuran warga.

## Prasyarat
- [XAMPP](https://www.apachefriends.org/index.html) (untuk Apache dan MySQL)
- [Composer](https://getcomposer.org/) (untuk mengelola dependensi PHP)
- PHP versi yang sesuai dengan requirement Laravel

## Langkah-langkah Instalasi

1. **Clone Repository**
   ```bash
   git clone https://github.com/username/IuranWargaApp.git
   cd IuranWargaApp
   ```

2. **Jalankan XAMPP**
   - Aktifkan Apache dan MySQL di XAMPP Control Panel.

3. **Buat Database**
   - Buka [phpMyAdmin](http://localhost/phpmyadmin).
   - Buat database baru dengan nama `ilovepemweb`.

4. **Instalasi Dependensi**
   ```bash
   composer install
   ```

5. **Konfigurasi Environment**
   - Salin file `.env.example` menjadi `.env`.
   - Atur konfigurasi database di file `.env`:
     ```env
     DB_CONNECTION=mysql
     DB_HOST=127.0.0.1
     DB_PORT=3306
     DB_DATABASE=ilovepemweb
     DB_USERNAME=root
     DB_PASSWORD=
     ```

6. **Generate Application Key**
   ```bash
   php artisan key:generate
   ```

7. **Migrasi Database**
   ```bash
   php artisan migrate
   ```

8. **Jalankan Server**
   ```bash
   php artisan serve
   ```

9. **Akses Aplikasi**
   - Buka browser dan akses [http://localhost:8000](http://localhost:8000).

## Catatan
- Pastikan semua service di XAMPP berjalan dengan baik.
- Jika ada error, periksa kembali langkah-langkah di atas dan pastikan semua prasyarat sudah terpenuhi.

## Kontribusi
Jika Anda ingin berkontribusi, silakan fork repository ini dan buat pull request.
