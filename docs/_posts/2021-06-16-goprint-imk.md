---
layout: post
title:  "Situs Go-Print"
date:   2021-06-16 12:00:00 +0700
date_creation: "2018"
tags: Bootstrap HCI PHP Web_Development Assignment
desc: "Proyek ini merupakan tugas akhir semester dari mata kuliah Interaksi Manusia dan Komputer (IMK) atau disebut dengan <i>Human Computer Interaction</i> (HCI) yang mengangkat topik jasa printing online dengan nama <b>'Go-Print'</b> berbasis web."
---

Situs **Go-Print** adalah situs yang dibuat sebagai hasil dari pembelajaran mata kuliah Interaksi Manusia dan Komputer (IMK) yang diselenggarakan pada semester ke-3\. Situs ini berfungsi sebagai wadah bagi pelaku usaha printing yang ingin me-modernkan usahanya, secara teoritis. User dari situs ini adalah pelanggan / customer dan admin / pelaku usaha. Untuk bagian customer dibagi menjadi halaman home, order, dan pembayaran, sedangkan untuk bagian admin terdapat halaman home. Ketika situs ini dibuka akan menampilkan halaman login dan halaman register untuk menambah customer baru. Situs ini berbasis bahasa PHP dan menggunakan _database_ PostgerSQL agar dapat di\-_host_ di Heroku(awalnya menggunakan MySQL).

Situs Go-Print dapat diakses [disini](https://goprint-imk.herokuapp.com/)

Halaman Login             |  Halaman Register
:-------------------------:|:-------------------------:
<img alt="Halaman login" src="{{site.url}}/assets/goprint-imk/regist_done.PNG" class="img-fluid">  |  <img alt="Halaman register" src="{{site.url}}/assets/goprint-imk/regist_error.PNG" class="img-fluid">

Seperti yang terlihat pada gambar, halaman login berisikan _field_ username dan password, yang kemudian disusul dengan tombol login dan register. Tombol login akan menyalurkan user ke halaman home sesuai dengan role masing-masing. Tombol register akan membawa user ke halaman register untuk mendaftar ke dalam sistem. Gambar dibawah ini merupakan hasil dari proses registrasi, dimana akna menghasilkan pesan sesuai dengan apa yang diproses oleh sistem. Pesan ini ditampilkan pada bagian atas dari _form_. Pada gambar di kiri ditampilkan pesan berhasil setelah user berhasil mendaftarkan diri dan tidak menggunakan username yang telah ada sebelumnnya. Sedangkan pada gambar di kanan menampilkan pesan error yang menandakan user menggunakan username yang sama dengan user yang lain.

Message Berhasil             |  Message Gagal
:-------------------------:|:-------------------------:
<img alt="Message berhasil" src="{{site.url}}/assets/goprint-imk/login.PNG"  class="img-fluid">  |  <img alt="Message gagal" src="{{site.url}}/assets/goprint-imk/regist.PNG"  class="img-fluid">

Setelah user customer berhasil mendaftarkan diri ke dalam sistem dan melakukan login maka user dihadapkan dengan halaman _home_ yang menampilkan sebuah tabel yang berisikan _order_\-an yang telah dibuat sebelummnya. Untuk melakukan order, user dapat menekan tombol "order" di sebelah tombol "logout" yang terdapat pada _navigation bar_. Sesuai dengan namanya, navgation bar ini terletak pada bagian atas yang berisikan menu-menu utama yang dapat diakses oleh user. Pada user customer navbar berisikan: link menuju home, tombol menuju halaman order, dan tombol logout untuk memutuskan _session_ pada sistem. Tombol logout diberi warna aksen merah untuk membedakan fungsi dari tombol yang berdampingan. Gambar di bawah adalah perbandingan dari customer yang belum pernah melakukan order dengan customer yang sudah pernah melakukan order dan menyelesaikan order-nya.

Halaman Home Customer             |  Halaman Home Customer Setelah Meng-order
:-------------------------:|:-------------------------:
<img alt="Halaman home customer" src="{{site.url}}/assets/goprint-imk/index_cust.PNG"  class="img-fluid">  |  <img alt="Halaman home customer setelah order" src="{{site.url}}/assets/goprint-imk/index_cust_selesai.PNG"  class="img-fluid">

Untuk melakukan order, maka customer harus mengisikan beberapa detail yang kemudian disimpan ke dalam sistem. Detail dari order tersebut adalah: tanggal pengiriman atau tanggal pengambilan, alamat jika dikirim, jenis kertas yang digunakan, jumlah halaman, jumlah salinan, dan _file_ yang akan diprint. Setelah customer mengisi semua field tersebut, maka total biaya yang dikeluarkan akan ditampilkan pada bagian bawah form. Pada bagian kiri bawah terdapat 2 (dua) tombol, yaitu tombol "cancel" untuk membatalkan rencana order yang mengembalikan customer ke halaman home dan tombol "checkout" untuk menyimpan order ke dalam sistem dan menampilkan rincian pembayaran.  

Halaman Order             |  Halaman Home Customer Setelah Meng-order
:-------------------------:|:-------------------------:
<img alt="Halaman order" src="{{site.url}}/assets/goprint-imk/order_isi.PNG"  class="img-fluid">  |  <img alt="Halaman setelah order" src="{{site.url}}/assets/goprint-imk/order_checkout.PNG"  class="img-fluid">

Bagian terakhir adalah halaman home dari user admin, halaman ini berisikan order yang belum terselesaikan pada sistem. Admin dapat memilih untuk menyelesaikan order atau membatalkan order. Ketika admin menekan salah satu tombol ini, maka sistem akan memroses dan menghilangkannya dari halaman home admin. User dari admin ini dapat diakses dengan "admin" dalam kedua field. Gambar di bawah adalah gambaran dari halaman admin. 

<img alt="Halaman home admin" src="{{site.url}}/assets/goprint-imk/index_admin.PNG"  class="img-fluid">

Memang sistem ini sangat sederhana dan memiliki banyak _plot-hole_, hal ini disebabkan karna sistem ini hanya digunakan untuk _showcase_ tampilan dan bukan showcase dari kemampuan yang dimiliki sistem.
