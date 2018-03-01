---
layout: post
title: Mekanisme Chatbot Bahasa Indonesia
date: 2018-2-27
---
Ada sebuah sistem yang dapat berbicara dengan Anda. Terutama via teks.



Ketik saja sebuah kalimat, sampaikan, maka akan muncul tanggapan dari sistem.

Di era yang gelegak digital, chatbot: [kombinasi](http://www.ijcaonline.org/archives/volume173/number7/mehta-2017-ijca-915367.pdf) antara _messaging_ dan kecerdasan buatan.
>An important component in developing chatbots is the way the chatbot analyses the input, and finds the best match from the stored knowledge (Shawar, 2005: 20).
Bilang saja bahwa komponen utama pada chatbot tentu mesin chat yang dituntut agar mampu mengartikan kalimat masukan (_input_) lalu menyerahkan jawaban (_output_) pada pengguna. Sebuah [NLP](https://connect.aricent.com/2017/10/10-questions-answers-about-chatbots).

Atau itu sama dengan sistem mengenali setiap kalimat pengguna berdasar pada pengetahuan yang sudah disusun. [1]

Selagi konstruksi berasas kerumitan keluaran tanggapan atau NLG, bukan NLU yang lebih tinggi.
Maka, kelola pengetahuan chatbot telah menjadi keseluruhan terhadap sistem.

Tiwari dan kawan-kawan membawa istilah [BASAAP](http://oaji.net/pdf.html?n=2017/786-1493219906.pdf) pada prinsip chatbot. [Be As Smart As A Puppy](http://medium.com/p/how-design-can-help-bridge-the-ai-gap-87526ca31dd4#d579) yang hanya mahir dilatih sebagaimana seperti seekor anak anjing.

Tapi tidak akan setiap bentuk atau contoh kalimat dilatih kepada chatbot dalam arti menyimpan semua 
bentuk pertanyaan ke pengetahuan chatbot.

_more manageable machine_. kata [George Kassabgi](https://medium.com/p/how-chat-bots-work-dfff656a35e2).

### Lalu Chatbot Bekerja ?

Dari sebagian besar tiga arsitektur saat membangun sistem bersifat percakapan (_conversational system_). [2]

Akan termasuk ke yang _rule-oriented_.

Seperti di kanal [chatbots.org](https://www.chatbots.org/ai_zone/viewthread/3009).

Ambil sebuah contoh kalimat: Kenapa kamu sendiri saja?

Contoh klasik dari chatbot _rule-based_ mencakup Eliza dan Parry. Eliza juga mencabut beberapa kata-kata dari kalimat dan lalu membuat kalimat lain dengan kata-kata ini. [2]

Kalimat lain atau sebagai kata kunci yang akan mewakili maksud contoh kalimat.

Hasil ekstraksi berupa kata kunci (_keyword_) ini akan disimpan atau menjadi pengetahuan chatbot. Bentuk jawaban mengiringi setiap dari mereka.

Ketika sebuah kalimat masukan diberikan oleh pengguna.

Kalimat ini akan dicari atau dibanding dengan semua kandidat berupa kata kunci tadi, mana yang paling sebanding terhadap teks kalimat sebagai dalih chatbot menampilkan jawaban.

Menunjuk proses yang sebanding, maka jawaban atau tanggapan yang mengiringi _keyword_ tadi yang akan tampil.



Proses perbandingan ini punya macam variasi.

Salah satu dengan metode _exact string matching_ seperti yang ada di [sini](http://repository.uin-suska.ac.id/3571/5/BAB%20IV.pdf), [ini](http://repository.uin-suska.ac.id/3654) dan [ini](http://repository.uin-suska.ac.id/3818).

Yang termasuk [exact string matching](http://www.jcomputers.us/vol12/jcp1202-10.pdf): brute force, Knuth Morris Pratt dan Boyer-Moore.

Awali dengan kalimat yang tadi: Kenapa kamu sendiri saja?

Chatbot lebih dulu menyimpan kata yang punya arti signifikan dari contoh kalimat: kamu sendiri

Saat kalimat yang harus persis seperti itu diberikan kepada sistem, maka sistem sudah mengerti lalu akan menjawab kalimat dengan membawa tanggapan sesuai kata kunci yang sebanding.



Ini masih kalimat dengan bentuk kata dan maksud sama: kamu kenapa sendiri ?



Tidak sebanding dengan kata kunci tadi. Mau berapa kali mesin chatbot dilatih?

Dalam hal kalimat, punya bentuk kata dan maksud yang sama, hanya berbeda susunan atau urutan.

Pathak menyadari,
> 1,000 ways of asking the same thing

Jelas saja, tidak perlu umpama menyimpan seribu kalimat yang masih menanyakan hal yang sama.

Tapi ini perihal membangun chatbot dari nol from scratch tidak dengan perantara asosiasi seperti Microsoft LUIS atau Facebook Messager. Tidak pula dibangun menggunakan AIML.

[1] 

[2] M. Gatti de Bayser, et al. [_A Hybrid Architecture for Multi-Party Conversational Systems_](https://arxiv.org/pdf/1705.01214). (2017). arXiv:1705.01214v2
