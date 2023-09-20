## Percobaan instalasi NodeJS
1. Membuka halaman (https://nodejs.org/en) untuk mengunduh node.js
![Cuplikan layar 2023-09-19 202939](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/c37ede29-ecbd-4702-a88c-8d50216e95ca)

2. Mengunduh dan menjalankan node.setup
  ![Cuplikan layar 2023-09-19 204858](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a7d7f394-7915-4417-8c3a-2b016afae8a6)

3. Menjalankan command `node -v` untuk memastikan node.js sudah terinstal.
![Cuplikan layar 2023-09-20 141457](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f220afc1-e4b4-43e7-9ca1-4ea85e846691)

## Percobaan instalasi NodeJS
1. Membuat folder dengan nama express-mongodb.
![Cuplikan layar 2023-09-20 202127](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9173f421-26cc-46c2-a72b-4bb680751b21)

2. menjalankan command `npm init -y` untuk menggenerate file package.json.
![Cuplikan layar 2023-09-19 215035](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/21ef3daf-e30c-46c1-994f-9f61379d8b7b)

3. menjalankan command `npm i express mongoose dotenv` untuk melakukan instalasi express.
![Cuplikan layar 2023-09-19 215330](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/55fae6fc-71be-487c-9203-b404390e58b3)

## Koneksi Express ke MongoDB
1. Membuat file `index.js` pada root folder dan memasukkan code.
![Cuplikan layar 2023-09-19 215610](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/01694d3a-a0d7-40f7-b845-8cfed1e53d9f)

2. Menjalankan command `node index.js`.
![Cuplikan layar 2023-09-19 215858](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a3867d68-2967-426c-9ca6-9c453a4a9b34)

3. Membuat file `.env` dan memasukkan code `PORT=5000` pada file tersebut.
![Cuplikan layar 2023-09-19 220327](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/7b23e120-e5ea-4fda-ba26-845fc8574c88)

4. Mengubah kode pada listening port menjadi berikut dan menjalankan aplikasi kembali.
![Cuplikan layar 2023-09-19 220407](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/38641ba4-5e5b-4656-b15c-03322491dafd)
![Cuplikan layar 2023-09-19 220445](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3d24cca4-0fea-4858-aa13-8bad350b87de)

5. Melakukan copy connection string pada Mongo Compas ke file `.env`.
![Cuplikan layar 2023-09-19 220837](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/58a28588-38a2-46ef-bb8c-c4f13eb7fd15)

6. Menambahkan baris kode berikut pada file `index.js`.
![Cuplikan layar 2023-09-19 221424](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/cbafa0a6-9bef-4913-862d-54e1f1f87b5d)

## Pembuatan Routing
1. Membuat direktori routes pada tingkat yang sama dengan `index.js` dan membuat file `book.route.js` di dalamnya.
![Cuplikan layar 2023-09-19 221758](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/7bb4b017-44d7-4e80-a36f-e128eebc5ca0)

2. Menambahkan sintaks untuk fungsi getAllBooks, getOneBook, createBook, updaateBook, dan deleteBook.
![Cuplikan layar 2023-09-19 221948](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b2ed32df-5c22-4128-87e5-ff72d2932aaa)
![Cuplikan layar 2023-09-19 223547](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/fa524d78-2699-4258-b4a6-bbfab07f1728)

3. Melakukan import `book.route.js` pada file `index.js` dan menambahkan kode seperti tampilan dibawah ini.
![Cuplikan layar 2023-09-20 064944](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/dc3ca8fd-7190-4c19-918c-f2c6ae36be2b)

4. menguji sebuah endpoint dengan postman.
![Cuplikan layar 2023-09-20 104051](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/0dd8c0ae-e2c7-4775-9601-f7b890a32120)

## Pembuatan Controller
1. Membuat direktori `controllers` di tingkat yang sama dengan `index.js` dan membuat file `book.controller.js` di dalamnya.
![Cuplikan layar 2023-09-20 111825](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e7c9a77b-4a61-475d-a487-64178af695e9)

2. Menyalin code dari routes untuk fungsi getAllBooks, getOneBook, createBook, updateBook, dan deleteBook.
![Cuplikan layar 2023-09-20 112119](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/96869278-175a-4bb3-bb28-0d72ba4ba5df)
![Cuplikan layar 2023-09-20 112230](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ca49ad72-4d12-498c-a3fb-59d877ec5ffb)

3. Melakukan import `book.controller.js` pada file `book.route.js`.
![Cuplikan layar 2023-09-20 112351](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/084a714f-cb46-4b2c-a1a0-25450839a4b8)

4. Merubah fungsi untuk memanggil fungsi dari `book.controller.js`.
![Cuplikan layar 2023-09-20 112705](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/d3b8d0d4-beb6-4ca0-80f0-1908a5cac1d4)
5. Melakukan pengujian endpoint dengan postman untuk memastikan response tetap sama.
![Cuplikan layar 2023-09-20 113258](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/db71012d-9104-4a53-b92a-3a45d7518335)

## Pembuatan Model
1. Membuat direktori `models` di tingkat yang sama dengan `index.js` dan membuat file `book.model.js` di dalamnya.
![Cuplikan layar 2023-09-20 113428](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/21a8085f-ce1d-4f2a-a3dc-b9886059de9b)

2. Menambahkan beberapa baris kode pada file `book.model.js`.
![Cuplikan layar 2023-09-20 113539](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/8fdc243c-8605-4de9-ac22-b1320410706b)

## Operasi CRUD
1. Menghapus semua data pada collection books melalui Mongo Compass.
![Cuplikan layar 2023-09-20 114056](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ab14803d-cd25-4f6a-8055-dc2c3f5f55f8)

2. Melakukan import `book.models.js` pada file `book.controller.js`.
![Cuplikan layar 2023-09-20 114323](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/1b28210c-8c19-4655-88d8-d7157e94b9ec)

3. Merubah fungsi createBook.
![Cuplikan layar 2023-09-20 114432](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/27efc8b8-b836-4677-b088-f6b34e3a903c)

4. Membuat 2 buah buku dengan data yang disediakan melalui postman.
![Cuplikan layar 2023-09-20 115103](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/793ed7fd-85fd-46bd-bf40-979753883994)
![Cuplikan layar 2023-09-20 115231](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/72659355-f221-4b12-9e36-2e4b7edfd1f5)

5. Merubah fungsi getAllBooks.
![Cuplikan layar 2023-09-20 115518](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e00df04f-b15d-40b4-b66c-73d9d025cfc8)

6. Merubah fungsi getOneBook.
![Cuplikan layar 2023-09-20 115557](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/aca11393-cd4b-41fd-ba28-77d0f6ee1924)

7. Menampilkan semua buku melalui postman.
![Cuplikan layar 2023-09-20 120423](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/15c63321-e494-4ae4-951f-cfcb2996bb2e)

8. Menampilkan buku Dilan 1990 dengan postman.
![Cuplikan layar 2023-09-20 120739](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a25deba2-75a8-439d-bd8c-ab4ccd38f9fa)

9. Merubah fungsi updateBook.
![Cuplikan layar 2023-09-20 120856](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/b692f51c-4603-4e6e-87f0-1f3c565c1401)

10. Merubah judul buku Dilan 1991 menjadi "<NAMA PANGGILAN> 1991" menggunakan postman.
![Cuplikan layar 2023-09-20 122652](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9b2316d7-32ca-41f2-820e-3aee3756e1c1)

11. Merubah fungsi deleteBook.
![Cuplikan layar 2023-09-20 123533](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3c35b06e-46ee-4a12-a4b3-fa503f061335)

12. Menghapus buku Dilan 1990 menggunakan postman.
![Cuplikan layar 2023-09-20 123806](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/9128c003-5c1c-40db-a2bc-e2f04dbfacaf)
