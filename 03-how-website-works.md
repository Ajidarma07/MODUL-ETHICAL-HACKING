---
description: Bagaimana Website Berkerja?
---

# How Websites Work?

## 🌐 Bagaimana Website Berfungsi?

Bayangin kamu lagi buka browser bisa Chrome, Firefox, atau Safari terus kamu ngetik alamat kayak youtube.com. Nah, pas kamu tekan\
Enter, sebenarnya kamu lagi ngirimin permintaan ke komputer lain (yang disebut server) buat minta halaman web itu ditampilin.\
Browser kamu = kayak tukang ojek online. Dia nganter permintaan kamu ke server,terus balik lagi bawa “pesanan” berupa tampilan website.

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 201028.png" alt=""><figcaption></figcaption></figure>

***

## ⚙️ Dua Bagian Website:

<div align="left"><figure><img src=".gitbook/assets/image (3) (1).png" alt="" width="140"><figcaption></figcaption></figure></div>

**Front End (Client-Side)**

Ini bagian yang kamu liat di layar: gambar,tombol,tulisan,form login, dsb. Dibuat\
pake HTML, CSS, dan JavaScript. Browser kamu yang ngerender ini semua.

Kayak bagian depan rumah tempat tamu datang dan liat-liat

<div align="left"><figure><img src=".gitbook/assets/image (4) (1).png" alt="" width="149"><figcaption></figcaption></figure></div>

**Back End (Server-Side)**

Ini bagian di belakang layar,tempat semua proses terjadi: ambil data dari database,&#x20;hitung logika aplikasi, dll..

Anggap aja kayak dapur restoran customer gak ngeliat,tapi semua proses\
masaknya di situ.



## 🔐 Kenapa Harus Peduli Sama Ini?:

**Karena kalau kamu tau cara kerja website, kamu juga bisa tau celah keamanannya.**

* **Man-in-the-Middle**: intercept data

Kalau data dari browser ke server tidak dienkripsi (Tidak HTTPS), bisa disadap orang. Seperti lagi chat tapi dibaca\
orang di tengah.

* **SQL Injection / XSS**

Kalau server gak filter input user dengan baik, penyerang bisa masukin kode jahat buat ngerusak atau ambil\
data.

* **Session Hacking**

Kalau cookie tidak aman, orang lain bisa bajak sesi login kamu. Bisa aja mereka jadi "kamu" di mata website.







***

## 🔣 HTML

HTML itu singkatan dari HyperText Markup Language.\


HTML itu bukan bahasa pemrograman, tapi bahasa markup yang fungsinya buat ngebentuk struktur dasar\
halaman web.\
Bayangin kamu bangun rumah. Nah, HTML itu kayak kerangka atau fondasi rumahnya. Dinding, atap, jendela,\
pintu semuanya disusun pake HTML

**Kalau kamu ngerti HTML, kamu bisa:**

* Mengerti struktur halaman saat ingin eksploitasi XSS (Cross Site Scripting)
* Analisa form login untuk uji coba Brute Force / SQL
* Cek source code halaman untuk melihat celah
* Modifikasi halaman lokal menggunakan DevTools (buat pentest atau fun)

<figure><img src=".gitbook/assets/image (4).png" alt="" width="375"><figcaption><p>Contoh HTML</p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 205327.png" alt="" width="411"><figcaption><p><strong>Fungsi-fungsi</strong></p></figcaption></figure>



***

## 🧠 Apa Itu JavaScript?

JavaScript adalah bahasa pemrograman yang membuat website jadi hidup dan interaktif.\
Kalau HTML itu kerangkanya, CSS itu bajunya, maka JavaScript itu otaknya&#x20;Dia yang ngatur interaksi, respon user, logika, dan segala hal dinamis di web.

Contoh gampang: Pas kamu klik tombol terus muncul pop-up, atau pas ngetik di form terus muncul notifikasi&#x20;"email nggak valid" itu kerjaannya JavaScript!

JavaScript itu serbaguna banget, terutama di sisi front-end (client-side), tapi juga bisa dipakai di back-end (pakai Node.js). Berikut&#x20;beberapa hal keren yang bisa dia lakuin.

* Manipulasi Halaman (DOM)
* Ubah isi halaman tanpa reload. Misalnya sembunyiin/ munculin elemen, ubah teks, dll.
* Validasi Form
* Mengecek input user sebelum dikirim ke server (contoh: email harus ada @,password minimal 8 karakter).
* Membuat Animasi
* Ngerender animasi, transisi, efek-efek kece.
* Interaksi Real-Time
* Mengambil data tanpa harus reload halaman. Contohnya scroll Instagram terus konten munculterus itu JavaScript yang kerja.

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 210410.png" alt="" width="563"><figcaption><p><strong>JavaScript</strong></p></figcaption></figure>

## Apa Itu IP Address ?🤔

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 210837.png" alt=""><figcaption><p><strong>Analogi IP Address</strong></p></figcaption></figure>

Setiap perangkat(komputer, HP, server, dll) yang nyambung ke&#x20;internet punya alamat unik—itulah IP (Internet Protocol) Address.

IP Itu Bisa Apa Aja?

* Menentukan lokasifisik (kira-kira)
* Menjadi identitas perangkat di jaringan
* Dipakai buat routing data dari satu titik ke titik lain

***

## Ada 2 Versi ✌

1. IPv4 → Contoh: 192.168.1.1

* Format angka, dipisah titik, total 4 blok
* Udah hampir habis stok alamat

&#x20; 2\.  IPv6 → Contoh: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

* Format lebih panjang, pake heksadesimal
* Solusi untuk jumlah device internet yang makin banyak

## Apa Itu DNS?

DNS (Domain Name System) itu seperti kontak di HP kamu

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 212509.png" alt=""><figcaption></figcaption></figure>

Proses simpelnya:

1. Kamu ketik youtube.com
2. Browser tanya ke DNS:"Eh, IP address buat youtube.com berapa ya?"
3. DNS jawab:"Oh itu di 172.217.194.206"
4. Browser langsung nyambung ke IP itu buat ambil halaman website-nya

## Proses DNS Lookup:

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 212852.png" alt="" width="563"><figcaption><p><strong>Proses DNS Lookup</strong></p></figcaption></figure>

## Port & Service:&#x20;

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 213215.png" alt="" width="422"><figcaption><p><strong>PORT</strong></p></figcaption></figure>

***

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 213357.png" alt="" width="434"><figcaption><p><strong>SERVICE</strong></p></figcaption></figure>

Port diwakili sama angka dari 0 sampai 65535:

1. 0-1023 = Well-known ports (buatlayanan standar, kayak HTTP, FTP, SSH)
2. 1024-49151 = Registered ports (buat aplikasitertentu, semi-standar)
3. 49152–65535 = Dynamic/private ports (biasanya dipakai secara acak

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 213708.png" alt="" width="538"><figcaption><p><strong>Port &#x26; Servis Populer</strong></p></figcaption></figure>

### Apa Itu HTTP Response Code?

HTTP Response Code (kadang disebut status code) adalah angka 3 digit yang dikirim server sebagai balasan ke browser&#x20;setelah kamu minta sesuatu (misal akses halaman, kirim form, login, dsb).

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 214032.png" alt="" width="563"><figcaption><p><strong>Kode HTTP</strong></p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 214208.png" alt=""><figcaption><p><strong>Kode HTTP yang Paling Sering Ketemu</strong></p></figcaption></figure>

> Penting bagi pentester memahami struktur website agar bisa mengenali celah keamanan secara akurat.
