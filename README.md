<p align="center"><a href="http://rw-academica-21.herokuapp.com/" target="_blank"><img src="public/img/Screenshot%202021-11-24%20at%2004-39-35%20Academica.png"></a></p>

## About Academica

Academica adalah website bertema edukasi yang mengimplementasikan autensikasi user menggunakan `session dan cookie`. Halaman `dashboard` hanya dapat di akses oleh pengguna yang telah mendaftar. Website ini dibuat untuk menyelesaikan Ujian Tengah Semester mata kuliah Rekayasa Web.

## Build With

Academica dibangun dengan bantuan framework seperti:
- [Laravel](https://laravel.com)
- [Tailwind CSS](https://tailwindcss.com/)
- [AlpineJS](https://alpinejs.dev/)
- [MySQL](https://www.mysql.com/)

## Panduan Installasi

Dibawah ini merupakan panduan untuk menginstall Academica pada komputer lokal anda. Silahkan ikuti langkah-langkah berikut:

### Prerequisites

Aplikasi yang dibutuhkan untuk menjalankan Academica di komputer anda:
1. Git
   ```bash
    git --version
    # contoh output
    git version 2.33.1.windows.1
   ```
2. Composer
    ```bash
    composer --version
    # contoh output
    2.1.9 2021-10-05 09:47:38
    ```
3. NodeJS dan NPM
   ```bash
    node --version
    # contoh output
    v16.13.0

    npm --version
    # contoh output
    8.1.3
   ```
4. MySQL

    MySQL bisa menggunakan Aplikasi GUI seperti `Laragon` atau `XAMPP`. 

### Memulai Installasi

1. Clone Repository ini
   ```bash
   # clone repository
   git clone https://github.com/Galangaidil/rw-academica-21.git

   # masuk kedalam direktori rw-academica-21
   cd rw-academica-21
   ```
2. Install Package dari Composer
   ```
   composer install
   ```
3. Install Package dari NPM
    ```
    npm i
    ```
4. Menjalankan `Laravel Mix`
    ```
    npm run dev
    ```
5. Mengcopy isi file `.env.example` ke `.env`
   ```bash
   # untuk Linux && MacOS
   cp .env.example .env
   
   # untuk Windows
   copy .env.example .env
   ```
6. Membuat `APP_KEY`
   ```
   php artisan key:generate
   ```
7. Buatlah database dengan nama **rw-academica-21**
8. Menjalankan `migration` dan mengisikan data user dengan `seeder`
   ```
   php artisan migrate:refresh --seed
   ```
9.  Menjalankan server
    ```
    php artisan serve
    ```
10. Congratulation, Sekarang Academica dapat di akses di [http://localhost:8000](http://localhost:8000)

## Kontak

Follow sosial media saya di:
- Instagram [@galangaidilakbar](https://www.instagram.com/galangaidilakbar/)
- Twitter [@galangaidilakbr](https://twitter.com/galangaidilakbr)


## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
