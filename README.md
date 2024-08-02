## Aplikasi-Website-e-Rental
##### _Aplikasi Website e-Rental Menyediakan layanan sewa kendaraan termasuk mobil angkutan barang dan truk, dengan berbagai pilihan untuk kebutuhan pribadi dan bisnis._
## 
[![N|Solid](https://laravel.com/img/logotype.min.svg)]()
Framework Laravel version 10

[![Figma](https://img.shields.io/badge/--F24E1E?logo=figma&logoColor=ffffff)](https://www.figma.com/design/ysErny15fLPBMwO2KzXJZz/Rent-Car?node-id=0-1&t=7RgSd1SvjbpSFRBj-1)
User Interface
## Features

- Terdapat 2 user (admin dan pihak yang menyetujui
- Admin dapat menginputkan pemesanan kendaraan dan menentukan driver serta pihak yang menyetujui pemesanan
- Pihak yang menyetujui dapat melakukan persetujuan melalui aplikasi
- Terdapat dashboard yang menampilkan grafik pemakaian kendaraan
- Terdapat laporan periodik pemesanan kendaraan yang dapat di export (Excel)



## Getting Started

PHP versi 8.1.
Assuming you've already installed on your machine: PHP version 8.1, Laravel, Composer.

install dependencies
```sh
composer install
npm install
```

create .env file and generate the application key
```sh
cp .env.example .env
php artisan key:generate
```

create database
```sh
php artisan db
```

migration and seeder
```sh
php artisan migrate --seed
```

Then launch the server:
```sh
php artisan serve
```
The Laravel sample project is now up and running! Access it at http://localhost:8000.
## Data User

- username : admin@gmail.com
	password : 123456
	level    : admin

-	username : users@gmail.com
	password : 12345678
	level    : users


## Development
- Sales mencari order , setelah mendapat order sales membuat data customer miliknya sendiri, sehingga setiap customer dan order akan melekat dengan nama salesnya yang berguna untuk melihat kinerja sales.
- Admin menginput data-data orderan seperti nama inventory yang dirental oleh customer, jumlah inventory yang dirental, tanggal mulai rental, durasi rental, nama dan telp customer.
- Kemudian sales bisa memberikan approval data orderan.
- Pada contoh ini setiap customer diberi limit jumlah inventory yang boleh dirental dalam satu order adalah sebanyak 5 unit.
- Setiap data orderan diberi status untuk membantu admin dan sales dalam memantau inventory yang dirental customer. Secara default ada 2 status yaitu status Open untuk barang yang masih dirental dan status Kembali untuk barang yang sudah dikembalikan oleh customer.
- Orderan yang telah kembali inventorynya akan diinput ke tabel pengembalian inventory. Pengembalian ini juga diberi status yaitu status Tepat Waktu untuk barang yang dikembalikan tepat waktu oleh customer dan status Terlambat jika ada kelebihan waktu dari durasi yang sudah dicatat saat pembuatan order.
- Setelah pengemblian inventory oleh customer dan sudah diinputkan ke tabel penerimaan maka bisa dibuatkan Invoice oleh sales atau admin dimana invoice ini sudah lengkap dengan perhitungan jika ada perpanjangan waktu atau keterlambatan rental oleh customer.
- Invoice yang sudah dibuatkan bisa dicetak atau dibuat ke dalam file PDF.


## License

The Laravel framework is open-sourced software licensed under the MIT license.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
