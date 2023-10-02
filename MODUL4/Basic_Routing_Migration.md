## Basic Routing dan Migration
1. Menambahkan endpoint dengan method GET pada aplikasi dengan menambahkan beberapa baris kode. ![Cuplikan layar 2023-09-27 090648](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/de6815bc-8596-4ad3-a5ec-c12d5d6a25c5)

2. Menambahkan method POST, PUT, PATCH, DELETE, dan OPTIONS. ![Cuplikan layar 2023-09-27 091129](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a9e88908-fef6-4fab-828d-45367dbcc6bf)

3. Menginstall extensions `thunder client`. ![Cuplikan layar 2023-09-27 091214](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/679ac8fb-f3e4-41c7-a8d8-2d134cda6083)

4. Membuat request dan mengakses url yang sudah ditambahkan dengan methodnya. ![Cuplikan layar 2023-10-02 130717](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/cc4dd5ab-6c82-4f67-b3ea-be43c4dfb7b7)

5. Pada langkah migrasi database ini yang pertama dilakukan adalah mengubah konfigurasi pada `.env`. ![Cuplikan layar 2023-09-27 130436](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/cfc6a62b-f2da-4a64-b526-05a0b863b9cb)

6. Menambahkan beberapa kode pada file app.php di dalam folder bootstrap. ![Cuplikan layar 2023-09-27 130527](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/75ab5408-c945-47b0-86cf-648df19af6a3)

7. Menjalankan beberapa command untuk membuat file migration. ![Cuplikan layar 2023-09-27 130917](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/374fe455-9f55-4eb0-9005-441417fde7bb)

8. Mengubah fungsi up pada file migrasi `create_users_table`. ![Cuplikan layar 2023-09-27 131131](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/cc8ca6a8-51a7-40f1-b4d3-120d0011838d)

9. Mengubah fungsi up pada file migrasi `create_products_table`. ![Cuplikan layar 2023-09-27 131206](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/4a37307b-678f-4bfe-a69f-96d372081ba0)

10. Menjalankan command `php artisan migrate`. ![Cuplikan layar 2023-09-27 131636](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9ac023fe-1058-431e-9f38-c83cc755d1cf)
