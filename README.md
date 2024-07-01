# Laravel Docker Environment

![Docker](https://img.shields.io/badge/Docker-3.8-blue)
![PHP](https://img.shields.io/badge/PHP-8.2-blue)
![Laravel](https://img.shields.io/badge/Laravel-10.x-orange)

## Deskripsi

Proyek ini menyediakan lingkungan Docker lengkap untuk menjalankan aplikasi Laravel. Ini termasuk PHP 8.2 dengan FPM, Nginx sebagai server web, MySQL untuk basis data, dan Adminer sebagai antarmuka basis data.

## Daftar Isi

1. [Prasyarat](#prasyarat)
2. [Instalasi](#instalasi)
3. [Struktur Docker](#struktur-docker)
4. [Penggunaan](#penggunaan)
5. [Konfigurasi Tambahan](#konfigurasi-tambahan)
   
## Prasyarat

- Docker 20.10 atau lebih baru
- Docker Compose 1.29 atau lebih baru

## Instalasi

1. **Clone repository ini**:
   ```bash
   git clone https://github.com/Leonardo12SH/Docker-For-Laravel.git
   cd Docker-For-Laravel
# Laravel Docker Environment

![Docker](https://img.shields.io/badge/Docker-3.8-blue)
![PHP](https://img.shields.io/badge/PHP-8.2-blue)
![Laravel](https://img.shields.io/badge/Laravel-10.x-orange)

## Deskripsi

Proyek ini menyediakan lingkungan Docker lengkap untuk menjalankan aplikasi Laravel. Ini termasuk PHP 8.2 dengan FPM, Nginx sebagai server web, MySQL untuk basis data, dan Adminer sebagai antarmuka basis data.

## Daftar Isi

1. [Prasyarat](#prasyarat)
2. [Instalasi](#instalasi)
3. [Struktur Docker](#struktur-docker)
4. [Penggunaan](#penggunaan)
5. [Konfigurasi Tambahan](#konfigurasi-tambahan)
6. [Contributing](#contributing)
7. [Lisensi](#lisensi)
8. [Kontak](#kontak)

## Prasyarat

- Docker 20.10 atau lebih baru
- Docker Compose 1.29 atau lebih baru

## Instalasi

1. **Clone repository ini**:
   ```bash
   git clone https://github.com/Leonardo12SH/Docker-For-Laravel.git
   cd Docker-For-Laravel
2. **Salin file contoh konfigurasi**:
   ```bash
   cp .env.example .env
3. **Jalankan Docker Compose**:
   ```bash
   docker-compose up -d --build

**Penggunaan**
Setelah Docker Compose selesai berjalan, Anda dapat mengakses layanan berikut:

Laravel: http://localhost:8001
Adminer: http://localhost:8080
MySQL: Host localhost, Port 3306, User root, Password admin123
Untuk menjalankan perintah Laravel Artisan atau Composer, gunakan:
  ```bash
  docker-compose exec app php artisan
  docker-compose exec app composer
```

**Konfigurasi Tambahan**
Pengaturan Nginx
File konfigurasi Nginx (default.conf) berada di ./docker/nginx/default.conf. Anda bisa mengubahnya sesuai kebutuhan.

**Pengaturan PHP**
Konfigurasi PHP (php.ini) berada di ./docker/php/php.ini. Ubah pengaturan ini jika diperlukan.

**Penggunaan Volume**
Volume digunakan untuk menyinkronkan kode sumber lokal dengan container Docker, memastikan perubahan kode Anda secara otomatis tersedia di container.




