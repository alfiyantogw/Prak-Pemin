# Register, Authentication dan Authorization
## Register
1. Memastikan terdapat tabel users pada aplikasi.
2. Memastikan adanya model `User.php`.
3. Membuat file `AuthController.php` dan isi file tersebut dengan sintaks dibawah ini.
4. Menambahkan group route pada `routes/web.php`.
5. Menjalankan aplikasi pada endpoint `/auth/register` dengan ini body seperti dibawah ini menggunakan postman.

## Authentication
1. Membuat fungsi `login(Request $request)` pada file `AuthController.php`.
2. Menambahkan route pada file `web.php`.
3. Menjalankan aplikasi pada endpoint `/auth/login` dengan ini body seperti dibawah ini menggunakan postman.

## Token
1. Menjalankan perintah dibawhah ini untuk membuat migrasi baru.
2. Menambahkan sintaks dibawah ini pada file migration yang dibuat pada langkah sebelumnya.
3. Menambahkan atribut token di `$fillable` pada `User.php`.
4. Menambahkan baris berikut pada file `AuthController.php`.
5. Menjalankan perintah dibawah ini untuk menjalankan migrasi terbaru.
6. Menjalankan aplikasi pada endpoint `/auth/login` dengan ini body seperti dibawah ini menggunakan postman, dan salin token yang didapat ke notepad.

## Authorization
1. Membuat file `Authorization.php` pada folder `App/Http/Middleware` dan isi dengan sintaks dibawah ini.
2. Menambahkan middleware yang baru dibuat pada `bootstrap/app.php.`.
3. Membuat fungsi `home()` pada `HomeController.php`.
4. Menambahkan route pada file `web.php`.
5. Menjalankan alikasi pada endpoint `/home` dengan memasukkan nilai token yang telah didapat sebelumnya.
