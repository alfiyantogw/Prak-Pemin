![Cuplikan layar 2023-10-27 144134](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e73b928a-63eb-484a-a842-72a51ee0a22f)# Relasi One-to-Many dan Many-to-Many
## Pembuatan Tabel
1. Memastikan sudah ada database dengan nama `lumenpost`.
![Cuplikan layar 2023-10-29 200756](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e5f7a995-16aa-468a-bb7e-fd0fd64c57f4)

2. Mengubah konfigurasi database pada file `.env`.
![Cuplikan layar 2023-10-27 142245](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1ee99225-262d-4e97-a09d-8799e8f50c1a)

3. Menghidupkan library dengan melakukan uncomment sintak pada file `app.php`.
![Cuplikan layar 2023-10-27 142822](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/483eb417-b109-4cbf-ba25-0fcdbf445c5c)

4. Menjalankan perintah dibawah pada command line untuk membuat file migration.
![Cuplikan layar 2023-10-27 142927](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9b0b95f0-3561-4910-9ffa-3256ae359b0d)

5. Merubah fungsi `up()` pada file `migrasi create_posts_table`.
![Cuplikan layar 2023-10-27 143348](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/6374939e-4e70-4847-bbec-bdf8c33d0bcb)

6. Merubah fungsi `up()` pada file `create_comments_table`.
![Cuplikan layar 2023-10-27 143605](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/bd902ac5-f3c5-4cf7-8199-8440a4648e03)

7. Merubah fungsi `up()` pada file `create_tags_table`.
![Cuplikan layar 2023-10-27 143842](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/5597f165-abeb-4e80-a237-8a8fe5533b7b)

8. Merubah fungsi `up()` pada file `create_post_tag_table`.
![Cuplikan layar 2023-10-27 144134](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9c46ea06-da5e-4442-b757-20f729091c3e)

9. Menjalankan command `php artisan migrate`.
![Cuplikan layar 2023-10-27 144236](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/be4fde10-97a1-4180-9cce-777a0f43e199)

## Pembuatan Model
1. Membuat file dengan nama `Post.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 144413](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9a1867bc-8b99-48cf-b76d-bbd6c103b4c9)

2. Membuat file dengan nama `Comment.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 144511](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ed6289c7-4a65-4d7b-8079-ad5ead3cd684)

3. Membuat file dengan nama `Tag.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 144549](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/d1f486a5-6756-4734-8d3e-493a8a7a24e9)

## Relasi One-to-Many
1. Menambahkan fungsi `comments()` pada file `Post.php`.
![Cuplikan layar 2023-10-27 145948](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/52eb5e1b-d5dc-4202-8495-ab139fa0ca0a)

2. Menambahkan fungsi `post()` dan atribut postId pada `$fillable` pada file `Comment.php`.
![Cuplikan layar 2023-10-27 150222](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a28b6dc5-c109-459f-883e-4b0dc8777422)

3. Membuat file dengan nama `PostController.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 150712](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3a6b5b01-785a-4572-afb7-f96842dc9554)

4. Membuat file dengan nama `CommentController.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 150816](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/09547aaa-8196-4051-9a98-f6893d4e3edb)

5. Menambahkan sintak dibawah pada `routes/web.php`.
![Cuplikan layar 2023-10-27 151022](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a3e11a89-8100-4b7a-b3db-5962b758110c)

6. Membuat satu post menggunakan postman.
![Cuplikan layar 2023-10-27 151602](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f4714d75-42a0-47ac-abe9-0163accac410)

7. Membuat satu comment menggunakan postman.
![Cuplikan layar 2023-10-27 151848](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/49569d34-5915-4106-9179-1dd7fed3f2d4)

8. Menampilkan post menggunakan postman.
![Cuplikan layar 2023-10-27 152005](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/2341e35a-e7fb-435a-b0ce-b1a981346a29)

## Relasi Many-to-Many
1. Menambahkan fungsi `tags()` pada file `Post.php`.
![Cuplikan layar 2023-10-27 152301](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/56b9bd70-6709-42a1-9fc2-daaf4f45c530)

2. Menambahkan fungsi `posts()` pada file `Tag.php`.
![Cuplikan layar 2023-10-27 152338](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/aaae89b3-17a0-434c-9e94-22133d23b8ee)

3. Membuat file dengan nama `TagController.php` dan isi dengan sintak berikut.
![Cuplikan layar 2023-10-27 152647](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/5424eb63-8d82-4943-bee8-2ac43eca6572)

4. menambahkan fungsi `addTag` dan response `tags` pada `PostController.php`.
![Cuplikan layar 2023-10-27 152948](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/7013fa96-30d1-4952-9bd7-743376edd46d)

5. Menambahkan sintak dibawah pada `routes/web.php`.
![Cuplikan layar 2023-10-27 201851](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/846377b4-32a8-4080-93cd-a3bbafa02fd3)

6. Membuat satu tag menggunakan postman.
![Cuplikan layar 2023-10-27 203629](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/c7b5b277-bba3-4f42-ae85-13fc53fdcc44)

7. Menambahkan tag `jadul` pada post `disana engkau berdua`.
![Cuplikan layar 2023-10-27 205506](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/8358a4e2-3126-49b0-8cbc-4a8dea30873f)

8. Menampilkan post `disana engkau berdua` menggunakan Postman.
![Cuplikan layar 2023-10-27 210439](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/230dc134-cef5-40a4-b6a2-3e04fa4f01f4)

9. Membuat postingan `tanpamu apa artinya` menggunakan postman.
![Cuplikan layar 2023-10-27 210636](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/675b5dd1-3cd7-4efa-8822-e32a01758bdf)

10. Menambahkan tag `jadul` pada postingan `tanpamu apa aritnya`.
![Cuplikan layar 2023-10-27 210817](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/bdf89123-5361-42e9-86c0-cf96603b6514)

11. Membuat tag `lagu` menggunakan postman.
![Cuplikan layar 2023-10-27 211314](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e79e7ba5-02bd-4e74-b280-171c8dd7e535)

12. Menambahkan tag `lagu` pada postingan `tanpamu apa artinya`.
![Cuplikan layar 2023-10-27 211730](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/2ce47ebc-e3ee-4884-889f-054c337482da)

13. Menampilkan post pertama.
![Cuplikan layar 2023-10-27 211845](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/37db7ffe-ceea-4c22-bd6a-271e3df1d6f5)

14. Menampilkan post kedua.
![Cuplikan layar 2023-10-27 211955](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/43eea3a3-96d8-4cc9-a73b-be877e745f0d)
