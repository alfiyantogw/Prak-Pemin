# Register, Authentication dan Authorization
## Register
1. Memastikan terdapat tabel users pada aplikasi.
![Cuplikan layar 2023-10-31 075852](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1ceb8e88-fb39-4e50-b30e-701ab1745e7a)

2. Memastikan adanya model `User.php`.
![Cuplikan layar 2023-10-30 153951](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ef04086b-0077-4437-8ccd-579413fa8439)

3. Membuat file `AuthController.php` dan isi file tersebut dengan sintaks dibawah ini.
![Cuplikan layar 2023-10-30 154134](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b1546424-6328-4da2-906f-e3cdc70ff2fb)

4. Menambahkan group route pada `routes/web.php`.
![Cuplikan layar 2023-10-30 154251](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f95ff9aa-d9f1-4334-bd0b-605998fde9e4)

5. Menjalankan aplikasi pada endpoint `/auth/register` dengan ini body seperti dibawah ini menggunakan postman.
![Cuplikan layar 2023-10-30 154632](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3dfb2bb8-7145-4476-85dd-b1da79ac40d6)

## Authentication
1. Membuat fungsi `login(Request $request)` pada file `AuthController.php`.
![Cuplikan layar 2023-10-30 154753](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b8d02b51-6cae-4b11-81c7-30b5d66e8131)

2. Menambahkan route pada file `web.php`.
![Cuplikan layar 2023-10-30 155734](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b91f3faa-9073-43a4-8ceb-defd06f08c41)

3. Menjalankan aplikasi pada endpoint `/auth/login` dengan ini body seperti dibawah ini menggunakan postman.
![Cuplikan layar 2023-10-30 160031](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b39a39a2-d884-4b54-85a4-b25a0583d845)

## Token
1. Menjalankan perintah dibawhah ini untuk membuat migrasi baru.
![Cuplikan layar 2023-10-30 160403](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9d215e4e-7941-4e94-9a48-d6a5ba3e5f4b)

2. Menambahkan sintaks dibawah ini pada file migration yang dibuat pada langkah sebelumnya.
![Cuplikan layar 2023-10-30 160523](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/65ab02cb-7aee-4476-9b6d-2c23ed3384d5)

3. Menambahkan atribut token di `$fillable` pada `User.php`.
![Cuplikan layar 2023-10-30 160927](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/adc0f597-0b80-42c7-858a-aac90933a9da)

4. Menambahkan baris berikut pada file `AuthController.php`.
![Cuplikan layar 2023-10-30 161509](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f2c52d7e-8132-4bfc-870e-15a89a24f8d0)

5. Menjalankan perintah dibawah ini untuk menjalankan migrasi terbaru.
![Cuplikan layar 2023-10-30 161759](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/7567a946-2617-4637-ada4-ad53f16d00a7)

6. Menjalankan aplikasi pada endpoint `/auth/login` dengan ini body seperti dibawah ini menggunakan postman, dan salin token yang didapat ke notepad.
![Cuplikan layar 2023-10-30 162323](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/850764de-9d05-416a-b619-0f7fdfbaefb6)

## Authorization
1. Membuat file `Authorization.php` pada folder `App/Http/Middleware` dan isi dengan sintaks dibawah ini.
![Cuplikan layar 2023-10-30 170615](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9aa54124-5ff7-4209-bcf8-40865ccd75f9)

2. Menambahkan middleware yang baru dibuat pada `bootstrap/app.php.`.
![Cuplikan layar 2023-10-30 170615](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/435b1306-65f3-496b-a8af-5d90d3ad4f70)

3. Membuat fungsi `home()` pada `HomeController.php`.
![Cuplikan layar 2023-10-31 075657](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1bf64f80-26ae-449c-84e7-ca616b121fbf)

4. Menambahkan route pada file `web.php`.
![Cuplikan layar 2023-10-30 171201](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/df902636-aaa7-4f39-a862-50de37521324)

5. Menjalankan alikasi pada endpoint `/home` dengan memasukkan nilai token yang telah didapat sebelumnya.
![Cuplikan layar 2023-10-30 184517](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/8238feda-da21-414b-9856-fee83582290f)
