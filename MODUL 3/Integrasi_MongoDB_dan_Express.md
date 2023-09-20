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
2. Menambahkan beberapa baris kode pada file `book.model.js`
3. 


8. Lakukan insert buku kedua dengan cara yang sama.
![Cuplikan layar 2023-09-19 120007](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/4cda57a8-63ff-4836-a3f7-3449f25c6a32)

9. Tampilan dari data buku yang telah diinput
![Cuplikan layar 2023-09-19 120032](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e9282754-8a09-45b5-9e49-0b1c73239a3c)

10. Lakukan pencarian buku dengan author “Osamu Dazai” dengan mengisi filter yang diinginkan dan klik “Find”
![Cuplikan layar 2023-09-19 120050](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/52edf790-fc41-49e9-a4ea-85c0f8846c73)

11. Merubah summary pada buku “No Longer Human” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan melakukan klik “Edit Document” (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik “Update”
![Cuplikan layar 2023-09-19 120121](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/28497b5a-623a-4a7d-8d1c-18bd810eb0e9)

12. Menghapus buku “I Am a Cat” dengan melakukan klik “Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”
![Cuplikan layar 2023-09-19 120141](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/5e4f6f80-5d69-491a-b5e2-dddf05c019bd)



## CRUD Mongo DB Shell

1. Lakukan koneksi ke MongoDB Server dengan menjalankan command `mongosh` bagi yang menggunakan terminal build in OS seperti tampilan dibawwah ini
![Cuplikan layar 2023-09-19 120157](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3e090684-3e8a-400d-9494-9cb72a226ce0)

2. Melihat list database yang ada di server dengan menjalankan command `show dbs`
![Cuplikan layar 2023-09-19 120224](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/6cbc40d1-e9fd-4c02-9920-75be5c747c2d)

2. Berpindah ke database “bookstore” dengan menggunakan command `use bookstore` , memastikan terdapat tanda `>` untuk berpindahnya database
![Cuplikan layar 2023-09-19 120243](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/c36089f7-32f9-4f3d-956e-9a14c0b7f2d3)

3. Gunakan command `show collections` untuk melihat collection yang tersedia pada database
![Cuplikan layar 2023-09-19 120258](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/ede19988-1af0-490d-8f50-147e2c2a1358)


4. Melakukan insert buku “Overlord I” dengan menggunakan command `db.books.insertOne(<data kalian>)` , setelah insert buku berhasil maka MongoDB akan muncul tampilan seperti berikut.
![Cuplikan layar 2023-09-19 120315](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/fe651577-cbc9-488c-9deb-7f4df449778d)


5. Lakukan insert buku “The Setting Sun” dan “Hujan” dengan insert many dengan menggunakan command `db.books.insertMany(<data kalian>)` , dan akan mengembalikan pesan sebagai berikut.
![Cuplikan layar 2023-09-19 120330](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/4eddef81-6872-4b76-9c8c-54852807a33d)

5. Lakukan pencarian buku dengan menggunakan command `db.books.find()` untuk melakukan pencarian semua buku.
![insert banyak buku](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3a3a552e-e340-45d8-86d1-f49f7cfa3713)

6. Tampilkan seluruh buku dengan author “Osamu Dazai” dengan mengisi argument pada find() dengan menggunakan command `db.books.find({author: "Osamu Dazai"})` dimana filter yang saya gunakan disini adalah filter author
![Cuplikan layar 2023-09-19 120601](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/3b764dd5-62cb-4499-b9cb-e8d5b229465a)

7. Lakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan mengunakan `command db.books.updateOne({<filter>}, {$set: {<data yang akan di update>}})` sehingga output yang dihasilkan oleh MongoDB akan menjadi seperti berikut
![Cuplikan layar 2023-09-19 120625](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/46c21773-4ce4-4318-a98e-4f6e4a2a9e1e)

8. Lakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu
Dazai” dengan menggunakan command `db.books.updateMany({<filter>}, {$set: {<data
yang akan di update>}})`
![Cuplikan layar 2023-09-19 120643](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/39ce53ed-43bc-4c0a-ac69-5a91a46126bc)

9. Lakukan penghapusan pada buku “Overlord I” dengan menggunakan command `db.books.deleteOne({title: "Overlord I"})`
![Cuplikan layar 2023-09-19 120625](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/2309e746-1033-47a4-ae0c-74af1af25699)

10.Lakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan command `db.books.deleteMany({author: "Osamu Dazai"})`
![Cuplikan layar 2023-09-19 120739](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/6e4ad280-63d1-4d3c-b3d6-7ad9629ef1e0)
