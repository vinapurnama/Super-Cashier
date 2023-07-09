# Super-Cashier
Sistem kasir sederhana dengan menggunakan bahasa Python

### Latar Belakang Masalah
Klien yang bernama Adi membutuhkan sistem kasir _self-service_ di Supermarket miliknya. Sehingga _costumer_ yang tidak berada di kota tersebut bisa membeli barang dari supermarket ini. Program ini dibuat menggunakan bahasa pemrograman Python. 

### Feature Requirement 
Sistem kasir _self-service_, yaitu Costumer dapat melakukan hal-hal sebagai berikut:
1.	Membuat ID transaksi
2.	Memasukkan nama item, jumlah item dan harga barang
3.	Melakukan update item jika terdapat kesalahan input
4.	Menghapus item belanjaan jika batal membeli item belanjaan
5.	Memeriksa kembali item belanjaan apakah udah benar
6.	Melihat total belanjaan yang sudah dibeli dan mendapatkan diskon jika total belanjaan memenuhi syarat minimum belanja. 

### Flowchart 
![Flowchart Template (1)](https://github.com/vinapurnama/Super-Cashier/assets/138844375/628cbe21-ebc6-4cc3-82ac-661d6e27d42b)

### Penjelasan Function
Function untuk menambahkan item pesanan
![Screenshot 2023-07-09 200553](https://github.com/vinapurnama/Super-Cashier/assets/138844375/b848181b-f0d4-4c6b-8d5d-aa4432319342)

Function untuk mengubah item yang sudah dipesan
![Screenshot 2023-07-09 200949](https://github.com/vinapurnama/Super-Cashier/assets/138844375/2826d878-2fc3-4633-aa53-ab1b445d99df)

Function untuk menghapus salah satu item dari daftar pesanan
![Screenshot 2023-07-09 201219](https://github.com/vinapurnama/Super-Cashier/assets/138844375/1fc2580c-c5b6-42c3-9360-30dc42fd4afd)

Function untuk membatalkan pesanan atau menghapus semua item dari daftar pesanan 
![Screenshot 2023-07-09 201353](https://github.com/vinapurnama/Super-Cashier/assets/138844375/8d0558b8-8de1-48c0-934a-1d986ceca8a8)

Function untuk memastikan pesanan yang diinput sudah benar
![Screenshot 2023-07-09 201534](https://github.com/vinapurnama/Super-Cashier/assets/138844375/09566e19-abff-469d-bf97-36906220fb1c)

Function untuk menghitung total belanja dan diskon yang diperoleh (jika memenuhi ketentuan yang berlaku)
![Screenshot 2023-07-09 201740](https://github.com/vinapurnama/Super-Cashier/assets/138844375/aaa893ee-613b-4321-9edf-d35ea3641611)

### Test Case
Test 1:
Costumer ingin menambahkan dua item baru menggunakan method `add_item()`. Item yang ditambahkan adalah sebagai berikut:
-  Nama item: Ayam Goreng, Qty: 2, Harga: 20000
- Nama item: Pasta Gigi, Qty: 3, Harga: 15000

![Screenshot 2023-07-09 202456](https://github.com/vinapurnama/Super-Cashier/assets/138844375/54fc9cd3-291d-428b-a913-e649b854ee41)
![Screenshot 2023-07-09 202710](https://github.com/vinapurnama/Super-Cashier/assets/138844375/e7cf1e79-96c9-4b83-8268-84f09ad2bda4)

Test 2:
Ternyata Costumer salah membeli salah satu item dari belanjaan yang sudah ditambahkan, maka Costumer menggunakan method `delete_item()` untuk menghapus item. Item yang ingin dihapus adalah **Pasta Gigi.**
![Screenshot 2023-07-09 203126](https://github.com/vinapurnama/Super-Cashier/assets/138844375/cb471727-6d56-411a-8b44-5f0ae47f3aba)

Test 3:
Ternyata setelah dipikir-pikir Costumer salah memasukkan item yang ingin dibelanjakan! Daripada menghapusnya satu-satu, maka Costumer cukup menggunakan method `reset_transaction() `untuk menghapus semua item yang sudah ditambahkan
![Screenshot 2023-07-09 203415](https://github.com/vinapurnama/Super-Cashier/assets/138844375/b7bc4c90-b4f9-4b97-9c3d-8d2f45ad3526)

Test 4:
Setelah Costumer selesai berbelanja, sistem akan menghitung total belanja yang harus dibayarkan menggunakan method `total_price()`. Sebelum mengeluarkan output total belanja akan menampilkan item-item yang dibeli
![Screenshot 2023-07-09 203415](https://github.com/vinapurnama/Super-Cashier/assets/138844375/dc1f3d79-db1c-4768-b6b1-a5a7b18a4a44)

### Saran Perbaikan
1.  Membuat menu login user dan sistem member supermarket, sehingga costumer dapat mengumpulkan poin dan mendapatkan promo
2.  Menghubungkan riwayat belanja costumer ke database, sehingga pihak supermarket bisa men-_track_ barang apa saja yang paling sering dibeli
