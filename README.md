# Praktikum Pemrograman Web 2 - Pertemuan 2
# Ricko Syahputra
# NIM 24454010023
# prodi TI semester 5
# tanggal 17-09-2026

## Deskripsi
Aplikasi "Modul Tiket Baca Saja" menggunakan framework Laravel dengan menerapkan pola arsitektur MVC (Model-View-Controller). Aplikasi ini berfokus pada pemisahan tanggung jawab (Separation of Concerns) antara Route, Controller, dan View.

## Endpoint (Route) Aplikasi
Sesuai dengan penugasan praktikum, aplikasi ini menyediakan tiga endpoint berikut:
- `GET /tickets` : Menampilkan daftar tiket dengan output Blade HTML.
- `GET /tickets/{ticket}` : Menampilkan detail tiket dengan output Blade HTML, dilengkapi constraint berupa angka pada parameter URL.
- `GET /api/tickets/{ticket}` : Menampilkan detail tiket dalam format JSON.

## Teknologi
- PHP dan Laravel
- Composer
- Blade Templating (sebagai View)
- Git
*(Catatan: Penggunaan Vue, Vite, Node.js, dan NPM dihilangkan karena pada materi ini tampilan dirender sepenuhnya di sisi server menggunakan Blade).*

## Instalasi Aplikasi
Karena aplikasi tidak lagi dipisah antara backend dan frontend (monolithic MVC), instalasi cukup dijalankan pada root project Laravel:
```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan serve
