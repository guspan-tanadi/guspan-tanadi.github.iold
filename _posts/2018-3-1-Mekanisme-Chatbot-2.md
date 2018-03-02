---
layout: post
title: Mekanisme Chatbot Bahasa Indonesia | Seksi Kedua
date: 2018-3-1
---
Suatu kesenangan sendiri dalam menciptakan perangkat lunak yang mengadakan percakapan antara seorang pengguna dengan sebuah sistem atau dikenal chatbot. Tanpa asosiasi atau menggunakan _platform_ luar.

Di komponen utama chatbot yang mengolah: mengartikan masukan kalimat pengguna lalu menampilkan tanggapan kepada mereka. Ini berarti [NLP]({% post_url 2018-2-27-Mekanisme-Chatbot %}).
Salah satu dengan menerapkan _exact string matching_.

Bahwa masalah dengan exact matching yang jadi komponen utama ini:
Ada _incapacity_ dalam menangani maksud kalimat serupa masih dalam bentuk kata dan maksud yang sama hanya berbeda susunan kata.

Dan bahaya bila harus _exact_. Malah kebalikan.
Chatbot harus mampu memperkirakan maksud kalimat pengguna tanpa perlu mengenalkan secara tegas kalimat tersebut ke pengetahuan chatbot.

Salah satu contoh exact matching ialah _brute force_.
Lihatlah sedikit perbandingan antara brute force dengan sebuah pendekatan lain yang disebut sebagai _bag of words_. Halaman dari [datatonic](http://blog.datatonic.com/2016/09/make-bots-great-again.html) membahas hal tersebut.

Bag-of-words can be used to retrieve relevant document within an user query. (McTear _et al_., 2016).

Bagaimana bag of words di komponen utama chatbot?



Terhadap kalimat: Kenapa kamu sendiri saja? atau kalimat serupa: Kamu kenapa sendiri?

Hanya perlu mengadakan satu kata kunci.

Memang seperti berdampak pada chatbot menjadi tidak mampu membedakan konteks kalimat antara
Anjing mengejar orang
dengan
Orang mengejar anjing

Tapi kembali lagi, tidak ada pemakaian kelas atau jenis kata seperti pada _Part of Speech_ karena [_error prone_](https://arxiv.org/pdf/1707.02919).

Perihal menangani kata-kata umum dengan kata-kata yang jarang sebuah bentuk tf-idf.

Ini masih tetap NLG yang memerhatikan struktur keruwetan keluaran (_output_) atau tanggapan dari sistem.

Bag of words pada chatbot ini sebab,
> Language modeling is regarded as a strong baseline for most NLP applications. (Hashemi _et al_., 2016).
