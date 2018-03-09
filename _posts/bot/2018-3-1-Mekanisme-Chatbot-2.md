---
layout: post
title: Mekanisme Chatbot Bahasa Indonesia | Seksi Kedua
date: 2018-3-1
---
Suatu kesenangan sendiri dalam menciptakan perangkat lunak yang mengadakan percakapan antara seorang pengguna dengan sebuah sistem atau dikenal chatbot. Tanpa asosiasi atau menggunakan _platform_ luar.

Di komponen utama chatbot yang mengolah: mengartikan masukan kalimat pengguna lalu menampilkan tanggapan kepada mereka. Ini berarti [NLP]({% post_url 2018-2-27-Mekanisme-Chatbot %}).
Salah satu dengan menerapkan _exact string matching_.

Bahwa masalah dengan exact matching yang jadi komponen utama ini:
Ada _incapacity_ pada menangani maksud kalimat serupa masih dalam bentuk kata dan maksud yang sama hanya berbeda susunan kata.

Dan bahaya bila harus _exact_ atau [_precise_](http://www.iamwire.com/2017/08/chatbots-customer-intent/156451). Malah kebalikan.
Chatbot harus mampu memperkirakan maksud kalimat pengguna tanpa perlu mengenalkan secara tegas kalimat tersebut ke pengetahuan chatbot.

Salah satu contoh exact matching ialah _brute force_.
Lihatlah sedikit perbandingan antara brute force dengan sebuah pendekatan lain yang disebut sebagai _bag-of-words_.
Halaman dari [datatonic](http://blog.datatonic.com/2016/09/make-bots-great-again.html) membahas hal tersebut.

> One application for conversational interfaces is in question answering, where the bag-of-words approach can be used to identify documents in which the answer to a user's question can be found (McTear _et al_., 2016).

Dalam hal ini, _document_ yang dimaksud yaitu pengetahuan chatbot.

Bagaimana [bag-of-words](https://machinelearningmastery.com/gentle-introduction-bag-words-model/) di komponen utama chatbot?

[Contoh penerapan](https://gist.github.com/guspan-tanadi/07310883a20745849f28da67316eb68f) bag-of-words chatbot bahasa Indonesia.

Terhadap kalimat: Kenapa kamu sendiri saja? atau kalimat serupa: Kamu kenapa sendiri?

Hanya perlu mengadakan satu kata kunci (_keyword_).

Memang seperti berdampak pada chatbot menjadi tidak mampu membedakan konteks kalimat antara
Anjing mengejar seorang
dengan
Seorang mengejar anjing.

Tapi kembali lagi, tidak ada pemakaian kelas atau jenis kata seperti pada _Part of Speech_ karena [_error prone_](https://arxiv.org/pdf/1707.02919).

Perihal menangani kata-kata umum dengan kata-kata yang jarang yakni sebuah _tf-idf_.

Beginilah NLG yang memerhatikan struktur keruwetan keluaran (_output_) atau tanggapan dari chatbot.

Bag-of-words pada chatbot sebab,
> [Language modeling](https://en.wikipedia.org/wiki/Category:Language_modeling) is regarded as a strong baseline for most NLP applications (Hashemi _et al_., 2016).

Hashemi _et al._ (2016). [_Query Intent Detection using Convolutional Neural Networks_](http://people.cs.pitt.edu/~hashemi/papers/QRUMS2016_HBHashemi.pdf).

McTear, Michael.; Callejas, Zoraida.; Griol, David. (2016). _The Conversational Interface: Talking to Smart Devices_. hlm. 167