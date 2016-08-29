# ujian_khusus


                      Penjelasan

Instalasi Node.js dan MongoDB


 

NodeJS sudah terinstall dengan versi 4.2.3

 
Gambar di atas mengaktifkan  server mongodb yang sudah terinstall  dan mongodb telah aktif pada port 2017

Membuat File Package.json


 

File ini merupakan file yang menyimpan informasi penting tentang project yang sedang dibuat seperti nama, versi, dll.

Instalasi Modul

Pastikan sudah masuk dalam folder dimana package.json yang dibuat tadi disimpan. Modul-modul ini digunakan mempermudah pembangunan aplikasi

1.	Pemasangan modul package Express
 
2.	Pemasangan body-parser

3.	Pemasangan modul Jade

4.	Pemasangan Modul MongoDB

Setelah semua modul sukses terinstall maka akhirnya file package.json tampilan seperti di bawah ini. Pada package terdapat nama modul yang terinstall dan versinya


Menghubungkan aplikasi dengan MongoDB / koneksi ke mongoDB

Buat file index.js yang berisi setting server dan koneksi ke mongoDB

Menginisialisasi variable aplikasi adalah express dan mengatur aplikasi pada port 3000,
Variable app = express() berfungsi untuk memuat atau me-load dependencies express agar aplikasi dapat menggunakan methods yang ada pada module tersebut.
Sedangkan app.use(express.static(path.join)(_dirname, ‘public’)) ini berfungsi sebagai pengaturan Express.
Variable mongohost adalah nama host yang digunakan mongoDB
Variable mongoport adalah port yang digunakan server mongoDB
Membuat vaiable untuk collectionDriver.js yang nanti digunakan sebagai controller aplikasi. Dan variable url untuk akses aplikasi.
Membuat render halaman view di index.js 

Pada index.js menambahkan script untuk render halaman view seperti halaman utama, tambah, edit, dan hapus.

1.	Render ke halaman utama atau index

2.	Render ke halaman form tambah / new pegawai 

3.	Render ke halaman form edit pegawai

4.	Render ke halaman daftar Pegawai

5.	Membuat render untuk fungsi tambah, update menggunakan method post  dan delete menggunakan method get

Membuat Controller disimpan dengan file CollectionDrive.js  

CollectionDrive.js  ini untuk membuat fungsi mengambil semua data / obyek atau megambil obyek berdasarkan id  pada database,   
Variable objekid = require(‘mongodb’).objekID berfungsi untuk memuat atau me-load dependencies data /obyek id pada mongodb 


Membuat Frontend view

Membuat halaman untuk index, form tambah, edit, daftar dan detail pegawai dengan memanfaatkan tempelate jade  dan menggunakan jquery mobile mebuat tampilan menarik.

1.	New.jade untuk halaman form tambah pegawai

2.	edit.jade untuk halaman form edit pegawai

3.	List.jade untuk tampilan daftar Pegawai
 
4.	Detail.jade untuk halaman tampilan detail pegawai
 
Menjalankan Aplikasi

1.	Koneksi antara server mongoDB dengan nodeJs melalui express

2.	Akses Aplikasi pada localhost:3000
