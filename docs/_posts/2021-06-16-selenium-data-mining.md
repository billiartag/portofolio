---
layout: post
title:  "Selenium Scraping"
date:   2021-06-16 14:00:00 +0700
date_creation: "2020"
tags: Web_Scraping Selenium Python Assignment
desc: "Aplikasi ini merupakan penunjang proyek tugas akhir semester dari mata kuliah <i>Data Mining</i> untuk menghasilkan file HTML beserta atribut-atribut lainnya untuk diproses pada aplikasi TF-IDF."
toc: true
---

## Apa itu Selenium..

Selenium adalah salah satu *tool* yang digunakan untuk melakukan scraping. Pada project ini digunakan bahasa pemrograman Python untuk melaksanakan proses scraping dengan Selenium. 
## Tujuan dari Project ini

Project ini bertujuan untuk mendapatkan data menggunakan Selenium sebagai alat scrapingnya. Data didapatkan dari situs-situs yang sudah ditentukan sebelumnya dan disimpan kedalam file dalam bentuk yang seragam dan sudah ditentukan sebelummnya. Project ini sendiri merupakan tugas akhir dari mata kuliah Web Mining, yang kemudian datanya digunakan untuk me-feed program lainnya.

## Proses

### Contoh Sumber Data

Salah satu contoh dari situs yang di-scrap adalah situs [hijauku.com](hijauku.com), situs ini memiliki salah satu [artikel](https://hijauku.com/2016/08/21/kophi-kampanyekan-wisata-alam-bertanggung-jawab/) yang di-scrap pada project ini. 

<img  alt="Artikel situs Hijauku"  src="{{site.url}}/assets/selenium-data-mining/site-ss.png"  class="img-fluid mx-auto">

### Contoh Hasil Ekstraksi Data

Seperti yang terlihat pada tangkapan layar, terdapat judul, isi, waktu upload, author, dan gambar pada artikel. Pada project ini data yang diambil adalah waktu upload, judul, dan isi dari artikel. Data yang berhasil didapatkan tersebut kemudian disimpan ke dalam file XML. File XML dipilih karena kelebihannya yang memiliki tatanan yang konsisten pada setiap filenya. 

<img  alt="Hasil scraping dalam format XML"  src="{{site.url}}/assets/selenium-data-mining/xml-ss.png"  class="img-fluid mx-auto">

Proses ini dilakukan berulang kali hingga mencapai jumlah data yang diinginkan. Pada project ini data yang diinginkan berjumlah ribuan dan selesai dalam hitungan jam. Data ini kemudian digunakan sebagai dataset pada proses TF-IDF yang juga merupakan tugas mata kuliah Web Mining. 

## Kesimpulan

Dengan menggunakan project ini, situs berbasis HTML statis maupun interaktif dapat diekstrak dan disimpan ke dalam sebuah file. File tersebut dapat digunakan pada program lainnya secara mudah dengan membaca format yang digunakan oleh file-file hasil ekstraksi. 