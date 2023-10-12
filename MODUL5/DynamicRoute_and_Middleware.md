# Dynamic Route dan Middleware

### Dynamic Route
1. Menambahkan dynamic routes pada aplikasi lumen dengan menggunakan sintaks dibawah ini pada file `routes\web.php`.
   ![Cuplikan layar 2023-10-04 145546](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/994f1ccb-0279-400c-80a3-50b144097fcb)

2. Selanjutnya adalah menambahkan parameter pada routes.
   ![Cuplikan layar 2023-10-04 145657](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/0c3fbdaf-6947-42c5-af79-75a8d8dbde53)

3. Menambahkan optional routes pada aplikasi lumen kita, saat memanggil endpoint tidak harus menggunakan parameter variable.
  ![Cuplikan layar 2023-10-04 145751](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3b22cdcc-d009-4db7-9827-edd797b5821a)

### Aliases Route
1. Menggunakan aliases route untuk memberikan naman pada route yang telah dibuat.
  ![Cuplikan layar 2023-10-04 155022](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/4ac07331-07a8-4973-a0e3-827b6ae5925d)

### Group Route
1. Melakukan grouping terhadap routes agar lebih mudah pada saat penulisan route pada `web.php`.
   ![Cuplikan layar 2023-10-04 155154](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3f56dd5e-7c66-4234-9742-b3b93f406b08)

### Middleware
1. Membuat middleware baru dengan nama `AgeMiddleware` pada path `app/Http/Middleware` dengan isi sebagai berikut.
  ![Cuplikan layar 2023-10-04 155437](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/7ea287bf-1358-4265-be26-ae2b15c77dd9)

2. Selanjutnya adalah dengan menambahkan `AgeMiddleware` pada aplikasi yang dibuat dengan menambahkan sintaks berikut pada file `bootstrap/app.php`.
  ![Cuplikan layar 2023-10-04 155611](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3b3fab9d-8a08-4759-bb75-16e091dd88f0)

3. Terakhir adalah menambahkan middleware pada routes dengan sintaks berikut.
   ![Cuplikan layar 2023-10-04 155745](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ba6bc9ed-7c43-47a2-b202-f2e913fb7acb)
