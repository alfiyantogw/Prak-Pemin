## CRUD MongoDB Compass

1. Melakukan koneksi ke database MongoDB menggunakan connection string
![Cuplikan layar 2023-09-19 115801](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/2dd91cf1-c4c3-4985-91cc-ce370b9d6244)

2. Tampilan home database setalh melakukan connection
![Cuplikan layar 2023-09-19 115835](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/771b3997-35b1-447e-b2a2-4f15c283c3e4)
  
3. Membuat database dengan nama database "Bookstore" dan collection name "books"
![Cuplikan layar 2023-09-19 115933](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/bb5f7cb5-d136-480d-a4c4-17c28c8bf6db)

4. Lakukan insert buku pertama dengan melakukan klik “Add Data”, pilih “Insert Document”, isi dengan data yang diinginkan dan klik “Insert”
![Cuplikan layar 2023-09-19 115950](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/feb30bb4-c3e6-417a-b6c6-f969637fa60e)

4. Lakukan insert buku kedua dengan cara yang sama.
![Cuplikan layar 2023-09-19 120007](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/4cda57a8-63ff-4836-a3f7-3449f25c6a32)

5. Tampilan dari data buku yang telah diinput
![Cuplikan layar 2023-09-19 120032](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/e9282754-8a09-45b5-9e49-0b1c73239a3c)

6. Lakukan pencarian buku dengan author “Osamu Dazai” dengan mengisi filter yang diinginkan dan klik “Find”
![Cuplikan layar 2023-09-19 120050](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/52edf790-fc41-49e9-a4ea-85c0f8846c73)

7. Merubah summary pada buku “No Longer Human” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan melakukan klik “Edit Document” (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik “Update”
![Cuplikan layar 2023-09-19 120121](https://github.com/alfiyantogw/Prak-Pemin/assets/99490388/28497b5a-623a-4a7d-8d1c-18bd810eb0e9)

8. Menghapus buku “I Am a Cat” dengan melakukan klik “Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”
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
