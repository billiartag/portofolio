---
layout: post
title:  "TF-IDF"
date:   2021-06-16 14:30:00 +0700
date_creation: "2020"
tags: TF-IDF Python Assignment
desc: "Aplikasi ini merupakan tugas akhir semester dari mata kuliah <i>Data Mining</i> yang mengimplementasikan algoritma TF-IDF dengan dataset berbasis teks."
toc: true
---

## Apa Project Ini dan TF IDF?
Project ini merupakan implementasi algoritma **TF IDF** yang didasarkan pada data yang dimiliki. Project ini merupakan tugas akhir dari mata kuliah Web Mining yang juga project lanjutan dari project Selenium sebelumnya.  
Project ini mengimplementasikan TF-IDF (Inverted Document Frequency dan Term Frequency) dan Cosine Similiarty pada teks yang diterima untuk mendapatkan hasil yang paling dekat dengan query yang diminta. Hasil dari proses tersebut akan mengembalikan top-5 dari artikel yang dianggap paling mendekati dari *query* yang diminta oleh *user* kedalam bentuk **file HTML**. 

## Data
Data diambil dari project sebelumnya. Pada project sebelumnya hasil data yang berupa XML dikumpulkan menjadi satu dan dijadikan menjadi sebuah file utuh berformat JSON. Setiap datum yang terdapat pada JSON memiliki struktur sebagai berikut:
-   title
-   content
-   published_at
-   fetched_at
-   url
-   topic

Data yang akan diproses adalah data pada bagian **content** atau isi dari artikel-artikel yang dimiliki. 

## Proses

Preparasi yang diperlukan adalah membuat folder HTML dan menaruh dataset yang digunakan, se-level dengan file python yang dieksekusi. File dataset yang digunakan harus dapat diparse dan sesuai dengan format JSON yang dapat diolah oleh library JSON di python.

Prepocessing data dilakukan setelah melakukan parsing JSON terhadap data awal. Data yang dibaca dari JSON satu persatu diproses dengan stemming, stopword removal, dan menghilangkan angka. 

Proses tersebut dilakukan dengan **memanfaatkan Library Sastrawi** yang dapat melakukan stemming dan stopword removal pada Bahasa Indonesia, dan regex, agar program dapat dibuat dengan simpel. 

Setelah preprocessing tersebut selesai, dilakukan **perhitungan Document Frequency dan Term Frequency** yang menghasilkan angka dan dimasukkan ke dalam array. Dilakukan perhitungan cosinus similiarity yang didasarkan dari query user yang telah di-tokenisasi. Indeks data dari perhitungan tersebut disimpan kemudian dilakukan generate file HTML pada data tersebut.

## Hasil
Saat pertama membuka program, user akan diminta query yang diminta dan jumlah dari artikel yang nantinya akan di-*export* menjadi file HTML

<img  alt="User Input"  src="{{site.url}}/assets/tfidf-data-mining/user-input.jpg"  class="img-fluid">

Setelah user melakukan entry yang diminta, maka program akan membaca dataset yang dimiliki pada komputer lokal. Seperti pada gambar di bawah ini, komputer menemukan 3 (tiga) buah file sebagai dataset.

<img  alt="Dataset Processing"  src="{{site.url}}/assets/tfidf-data-mining/dataset-process.jpg"  class="img-fluid">

Program akan melakukan perhitungan cosine similiarity dan TF-IDF untuk menentukan artikel-artikel yang dianggap mendekati. Program akan menghasilkan output berupa title dari artikel dan topik dari artikel yang didapatkan, seperti gambar di bawah ini.

<img  alt="Process"  src="{{site.url}}/assets/tfidf-data-mining/result-process.jpg"  class="img-fluid">

Hasil akhir dari program ini adalah sejumlah file HTML sesuai dengan jumlah yang diminta berdasarkan hasil perhitungan sebelumnya. 

<img  alt="HTML Results"  src="{{site.url}}/assets/tfidf-data-mining/result.jpg"  class="img-fluid">

## Kesimpulan
Program ini berfugnsi untuk mendapatkan artikel-artikel yang dianggap mirip dengan keyword (-keyword) yang di-*input* oleh user kepada program, lalu program akan menghasilkan beberapa file HTML yang didasarkan pada artikel-artikel yang dianggap cocok. 