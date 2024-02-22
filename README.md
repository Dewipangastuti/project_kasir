KELOMPOK  2
-	Dewi Pangastuti
-	Robi Ardiansyah
________________________________________
PROJECT CASHIER________________________________________
A.	Latar Belakang Masalah
Andi adalah pemilik supermarket yang ingin membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item, dan harga item yang dibeli dan fitur lain.
B.	Tools
a.	Language
-	Phython
b.	Libraries
-	tabulate
C.	Requirement / Objectives yang dibutuhkan program
1.	Membuat id customer
Trnsct_123 = Transaction ( )
2.	Customer menambahkan (input) nama item, jumlah item, dan harga barang.
add_item([<nama item>, <jumlah item>, <harga per item>])
3.	Jika terjadi kesalahan dalam memasukkan nama item atau jumlah item atau harga item tetapi tidak ingin menghapus itemnya, customer dapat melakukan hal berikut: 

a.	Update nama item dengan method : 
update_item_name(<nama item>, <update nama item>)
b.	Update jumlah item dengan method : 
update_item_qty(<nama_item>, <update jumlah item>)
c.	Update harga item dengan menggunakan method :
update_item_price (<nama_item> , <update harga item>)
4.	Jika batal membeli item belanjaan, customer bisa melakukan
a.	Menghapus salah satu item dari nama item dengan method
delete_item (<nama_item>)
Ketika menghapus salah satu nama item, maka jumlah item dan harga per item pada baris atau list tersebut akan terhapus.
b.	Langsung menghapus semua transaksi atau reset transaksi dengan method : 
reset_transaction ( )
5.	Customer mengecek apabila ada kesalahan dalam input 
check_order ( )
Dengan ketentuan : 
-	Mengeluaran pesan “Pemesanan sudah benar” jika tidak ada kesalahan input
-	Mengeluarkan pesan “Terdapat kesalahan input data” jika terjadi kesalahan input.
-	Menampilkan output transaksi atau pemesanan apa yang telah dibeli
6.	Customer menghitung total belanja dengan method : 
total_price ( )

Dengan ketentuan : 
-	Jika total belanja diatas Rp. 200.000 maka akan dapat diskon 5%
-	Jika total belanja diatas Rp. 300.000 maka akan dapat diskon 8%
-	Jika total belanja diatas Rp. 500.000 maka akan dapat diskon 10%
D.	Flowchart program
 
link flowchart



E.	Function atau atribut yang dibuat

No	Function	Deskripsi
1	generate_transaction_id	Process :
generate id transaksi

2	add_item ( )	Input : 
-	Nama item
-	Jumlah item
-	Harga per item
3	update_item	Input :
-	Pilih menu update
4	update_item_name ( )	Input : 
-	Update nama item
5	update_item_qty ( )	Input : 
-	Update jumlah item
6	update_item_price ( )	Input : 
-	Update harga item
7	delete_item ( )	menghapus item
8	reset_transaction ( )	reset transaction
9	check_order ( )	Display : 
Menampilkan item, jumlah item dan harga per item
10	total_price ( )	Display : 
Menampilkan keseluruhan item beserta total harganya


F.	Script Code
 
link code

G.	Test Case
1.	Test 1 
User ingin menambahkan dua item baru dengan mmenggunakan method 
add_item ( ) . Item yang ditambahkan adalah berikut :
-	Nama item : Pasta Gigi, Qty : 2, Harga : 5000
-	Nama item : Body Lotion, Qty : 3, Harga : 12000
Output :
 	 





2.	Test 2
Setelah dilihat lagi ternyata nama item yang dimasukkan salah, sehingga user menggunakan method update_item( ) dan update_item_name( ). Item yang salah dalam penulisan nama adalah pasta gigi.
Output :
 









3.	Test 3
Setelah memasukkan item belanja, ternyata user salah memasukkan jumlah item, sehingga user dapat menggunakan method update_item( ) dan update_item_qty ( ) untuk mengubahnya.
Output :
 













4.	Test 4
Setelah di cek lagi ternyata user salah memasukkan harga, sehingga user menggunakan method update_item ( ) dan update_item_price ( ). Dan item yang salah harga adalah Body Lotion.
Output :
 













5.	Test 5
Ternyata user salah memasukkan item belanjaan yang sudah di tambahkan, maka user menggunakan method delete_item ( ) untuk menghapus item. Item yang dihapus adalah pasta gigi mint.
Output :
  

6.	Test 6
Setelah dipikir-pikir, ternyata user salah memasukan item yang ingin di belanjakan, dariada menghapusnya satu-satu user menggunakan method reset_transaction ( ) untuk menghapus semua item yang sudah ditambahkan.
Output :
 
7.	Test 7
Karena tidak ingin terjadi kesalahan lagi user ingin mengecek item yang telah diinputkan lagi setelah di reset menggunakan method check_order(  ).
Output :
 
8.	Test 8
Setelah user berbelanja, akan menghitung total belanja yang harus dibayarkan menggunakan method total_price ( ) . 
Output :
 

Kesimpulan 
1.	Berikut beberapa method dalam kode:
•	add_item(): Menambahkan item baru ke dictionary.
•	update_item(): Membuka menu update item dan memungkinkan perubahan nama, jumlah, atau harga item.
•	delete_item(): Menghapus item dari dictionary.
•	reset_transaction(): Menghapus semua item dan transaction ID.
•	check_order(): Menampilkan daftar item dan total harga.
•	total_price(): Menghitung total harga, menerapkan diskon, dan menampilkan struk pembayaran.
2.	Berikut beberapa menu yang ada di dalam kode :
•	Tambah Item: Menambahkan item baru ke transaksi.
•	Update Item: Memperbarui nama, jumlah, atau harga item.
•	Hapus Item: Menghapus item dari daftar belanja.
•	Reset Transaksi: Memulai transaksi baru.
•	Check Order: Menampilkan daftar item dan total harga.
•	Bayar: Melakukan pembayaran dan mencetak struk.
•	Keluar: Mengakhiri program.
Catatan : 
Ketika daftar belanja masih kosong, hanya opsi "1. Tambah Item" dan "7. Keluar" yang tersedia. Setelah ada item dalam daftar belanja, semua menu utama (1-6) beserta "7. Keluar" akan muncul.
