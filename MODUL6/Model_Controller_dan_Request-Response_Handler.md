# Model, Controller dan Request-Response Handler
### Model
1. Memastikan adanya table users pada aplikasi.
![Cuplikan layar 2023-10-18 130422](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/606b387a-589e-4645-8214-119219a8f3e6)

2. Mengganti isi dari file `User.php` pada path `app/Models`dengan
   menggunakan sintkas dibawah ini.
![Cuplikan layar 2023-10-18 130822](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/8813d3ac-cecb-4887-bb7f-ac29bd337a75)

### Controller
1. Membuat salinan dari file `ExampleController.php` pada folder `app/Http/Controllers` dengan nama `HomeController.php` serta membuat function index dengan sintaks dibawah ini.
![Cuplikan layar 2023-10-18 132030](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/03a7ea35-be38-4660-a03f-1524d0b7a276)

2. Mengubah route pada file `routes/web/php` seperti dibawwah ini.
![Cuplikan layar 2023-10-18 132235](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/8b63720d-b066-47ff-b129-fdf83a62796d)

3. Menjalakan aplikasi dengan memasukkan `localhost:8000` pada browser sehingga muncul tampilan seperti dibawah ini.
![Cuplikan layar 2023-10-18 132514](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/38a86fce-b263-4d9a-b77f-b39880e00e3d)

### Request Handler
1. Melakukan import library request pada file `HomeController.php`.
![Cuplikan layar 2023-10-18 134644](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b7a70158-cce6-454e-a26c-508e01aec6d6)

2. Merubaha `function index()` menjadi seperti dibawah ini.
![Cuplikan layar 2023-10-18 135036](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ec3aa971-e772-45b9-bdf7-df1da6949c4c)

3. Menjalankan kembali aplikasi terssebut.
![Cuplikan layar 2023-10-18 135110](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a0b4a149-46e0-4a7a-96d6-c517a5e04cd8)

### Response Handler
1. Melakukan import library response pada file `HomeController.php`.
![Cuplikan layar 2023-10-18 135156](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/bfaac642-a609-416d-aca7-0fca140895a6)

2. Membuat `function hello()`.
![Cuplikan layar 2023-10-18 135435](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/885d8f01-df26-48ec-ba0d-4919c6a807f4)

3. Menambahkan route `/hello` pada file `routes/web.php`.
![Cuplikan layar 2023-10-18 135553](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a144b670-7cbd-4144-a340-657c9ee9b322)

4. Menjalankan aplikasi pada route /hello.
![Cuplikan layar 2023-10-18 135636](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f9afe191-81b3-4bcc-817c-a12236140db7)

### Ppenerapan
1. Melakukan import model User dengan menambahkan sintaks berikut pada file `HomeController.php`.
![Cuplikan layar 2023-10-18 135808](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/020283c7-7813-411c-8b40-1b31d3aa8908)

2. Menambahkan `function defaultUser()`, `function createUseer()`, dan `function getUsers()`.
![Cuplikan layar 2023-10-18 135940](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/54e4eb72-0f2d-4b86-824e-98fa9166af71)

3. Menambahkan route untuk setiap function yang telah dibuat sebelumnya.
![Cuplikan layar 2023-10-18 140122](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/53576d1b-07bd-4ccd-b998-aa47d7659a13)

4. Menjalankan aplikasi pada route `/users/default` menggunakan Postman.
![Cuplikan layar 2023-10-18 140553](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1012871c-43a8-4fd4-9fb5-a3b1fdfb7392)

5. Menjalankan kembali aplikasi melalui Postman pada route `/users/new` dengan mengisi field body seperti dibawah ini.
![Cuplikan layar 2023-10-18 141004](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/d1fd4b92-2c81-4c9a-bdfd-c82f6604e70d)

6. Menjalankan aplikasi pada route `/users/all`.
   ![Cuplikan layar 2023-10-20 075728](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1af08027-26c6-4bd1-b738-64af5ed8c0d6)
