---
layout: post
title:  "Aplikasi 'Titip Aku'"
date:   2021-06-16 13:00:00 +0700
date_creation: "2019"
tags: Firebase Android_Java Assignment
desc: "Proyek ini merupakan tugas akhir semester dari mata kuliah <i>Software Development Project</i> (SDP) yang mengangkat topik jasa penitipan barang dengan nama <b>'Titip Aku'</b>, yang berbasis Android Java."
---

Aplikasi *Titip-Aku* merupakan tugas akhir semester dari mata kuliah *Software Development Project* yang menghasilkan sebuah aplikasi Android. Aplikasi ini memanfaatkan *database* NoSQL Firebase untuk menyimpan data.  Aplikasi ini bertujuan untuk memfasilitasi pengguna untuk melakukan kegiatan titip barang dari suatu tempat menuju tempat lainnya.

<!-- SS Home -->
<img alt="Halaman login" src="{{site.url}}/assets/titipaku-sdp/home.jpg" class="img-fluid"> 

<!-- fitur utama -->
## Fitur Utama

Sesuai dengan namanya, aplikasi "Titip Aku" adalah sebuah marketplace yang memfasilitasi dua belah pihak yang berupa penjual dan pembeli. Seorang user yang terdaftar pada apliklasi ini dapat berperan sebagai penjual dan pembeli. Selain melakukan transaksi jual beli seperti marketplace lainnya, aplikasi ini dapat melakukan negosiasi. Fitur negosiasi ini dilakukan oleh pembeli terhadap produk yang telah disediakan oleh penjual. Pengguna juga dapat menggunakan fitur note untuk menyimpan nama dan harga barang pada aplikasi untuk mempermudah mengingat barang yang diincar. 

<!-- SS Nego -->
<img alt="Halaman login" src="{{site.url}}/assets/titipaku-sdp/dinego.jpg" class="img-fluid"> 

<!-- fitur penjual -->
## Fitur Penjual

Seperti pada marketplace umumnya, fitur-fitur yang diberikan oleh aplikasi kepada penjual adalah melakukan post barang yang ingin dijual, chat dengan pembeli, mendapatkan rating dari transaksi yang sukses, dan sebagainya. Pada aplikasi ini penjual juga dapat melakukan post barang preorder dan berjadwal. Post berjadwal merupakan post penjualan yang dilakukan oleh penjual ketika pada suatu lokasi pada waktu tertentu, dimana hal ini sangat bermanfaat sebagai live shopping dan tidak perlu melakukan post secara individual. Penjual yang menggunakan fitur nego juga mendapatkan perlindungan dari sistem dengan melakukan pembatasan perubahan biaya sebesar 20% dari harga awal. Hal ini digunakan agar penjual tidak mudah tertipu oleh permainan angka yang dilakukan oleh pembeli. 

<!-- SS post penjual -->
<img alt="Halaman login" src="{{site.url}}/assets/titipaku-sdp/onsale.jpg" class="img-fluid"> 

<!-- fitur pembeli -->
## Fitur Pembeli
Pembeli berperan sebagai pihak yang melakukan pembelian terhadap barang yang dijual oleh penjual. Pembeli dapat melakukan chat, nego, dan memasukkan barang pada cart yang dimilikinya. Pembeli dapat melakukan nego kepada penjual terhadap barang yang diminta, dengan treshold harga nego sebesar 20% dari harga awal. Pembeli juga dapat melakukan chat terhadap penjual untuk mendapatkan informasi lebih lanjut terhadap transaksi yang dilakukan. 

<!-- SS post pembeli -->
<img alt="Halaman login" src="{{site.url}}/assets/titipaku-sdp/pembelian.jpg" class="img-fluid"> 