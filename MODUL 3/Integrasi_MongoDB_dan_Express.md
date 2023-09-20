## Percobaan instalasi NodeJS
1. Membuka halaman (https://nodejs.org/en) untuk mengunduh node.js
![Cuplikan layar 2023-09-19 202939](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/c37ede29-ecbd-4702-a88c-8d50216e95ca)

2. Mengunduh dan menjalankan node.setup
  ![Cuplikan layar 2023-09-19 204858](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/a7d7f394-7915-4417-8c3a-2b016afae8a6)

3. Menjalankan command `node -v` untuk memastikan node.js sudah terinstal.
![Cuplikan layar 2023-09-20 141457](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/f220afc1-e4b4-43e7-9ca1-4ea85e846691)

## Percobaan instalasi NodeJS
1. Membuat folder dengan nama express-mongodb.

2. menjalankan command `npm init -y` untuk menggenerate file package.json.

3. menjalankan command `npm i express mongoose dotenv` untuk melakukan instalasi express.

## Koneksi Express ke MongoDB
1. Membuat file `index.js` pada root folder dan memasukkan code.

2. Menjalankan command `node index.js`.

3. Membuat file `.env` dan memasukkan code `PORT=5000` pada file tersebut.

4. Mengubah kode pada listening port menjadi berikut dan menjalankan aplikasi kembali.

5. Melakukan copy connection string pada Mongo Compas ke file `.env`.

6. Menambahkan baris kode berikut pada file `index.js`.

## Pembuatan Routing
1. Membuat direktori routes pada tingkat yang sama dengan `index.js` dan membuat file `book.route.js` di dalamnya.

2. Menambahkan sintaks untuk fungsi getAllBooks, getOneBook, createBook, updaateBook, dan deleteBook.

3. Melakukan import `book.route.js` pada file `index.js` dan menambahkan kode seperti tampilan dibawah ini.

4. menguji sebuah endpoint dengan postman.

## Pembuatan Controller
1. Membuat direktori `controllers` di tingkat yang sama dengan `index.js` dan membuat file `book.controller.js` di dalamnya.
2. Menyalin code dari routes untuk fungsi getAllBooks, getOneBook, createBook, updateBook, dan deleteBook.
3. Melakukan import `book.controller.js` pada file `book.route.js`.
4. Merubah fungsi untuk memanggil fungsi dari `book.controller.js`.
5. Melakukan pengujian endpoint dengan postman untuk memastikan response tetap sama.

## Pembuatan Model
1. Membuat direktori `models` di tingkat yang sama dengan `index.js` dan membuat file `book.model.js` di dalamnya.
2. Menambahkan beberapa baris kode pada file `book.model.js`.

## Operasi CRUD
1. Menghapus semua data pada collection books melalui Mongo Compass.
2. Melakukan import `book.models.js` pada file `book.controller.js`.
3. Merubah fungsi createBook.
4. Membuat 2 buah buku dengan data yang disediakan melalui postman.
5. Merubah fungsi getAllBooks.
6. Merubah fungsi getOneBook.
7. Menampilkan semua buku melalui postman.
8. Menampilkan buku Dilan 1990 dengan postman.
9. Merubah fungsi updateBook.
10. Merubah judul buku Dilan 1991 menjadi "<NAMA PANGGILAN> 1991" menggunakan postman.
11. Merubah fungsi deleteBook.
12. Menghapus buku Dilan 1990 menggunakan postman.
