# How Websites Work?

## 🌐 Bagaimana Website Berfungsi?

Bayangin kamu lagi buka browser bisa Chrome, Firefox, atau Safari terus kamu ngetik alamat kayak youtube.com. Nah, pas kamu tekan\
Enter, sebenarnya kamu lagi ngirimin permintaan ke komputer lain (yang disebut server) buat minta halaman web itu ditampilin.\
Browser kamu = kayak tukang ojek online. Dia nganter permintaan kamu ke server,terus balik lagi bawa “pesanan” berupa tampilan website.

<figure><img src=".gitbook/assets/Screenshot 2025-06-30 201028.png" alt=""><figcaption></figcaption></figure>

***

## ⚙️ Dua Bagian Website:

<div align="left"><figure><img src=".gitbook/assets/image (3).png" alt="" width="140"><figcaption></figcaption></figure></div>

**Front End (Client-Side)**

Ini bagian yang kamu liat di layar: gambar,tombol,tulisan,form login, dsb. Dibuat\
pake HTML, CSS, dan JavaScript. Browser kamu yang ngerender ini semua.

Kayak bagian depan rumah tempat tamu datang dan liat-liat

<div align="left"><figure><img src=".gitbook/assets/image (4).png" alt="" width="149"><figcaption></figcaption></figure></div>

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

* Session Hacking

Kalau cookie tidak aman, orang lain bisa bajak sesi login kamu. Bisa aja mereka jadi "kamu" di mata website.







***

## 🔣 HTML

HTML itu singkatan dari HyperText Markup Language.\


HTML itu bukan bahasa pemrograman, tapi bahasa markup yang fungsinya buat ngebentuk struktur dasar\
halaman web.\
Bayangin kamu bangun rumah. Nah, HTML itu kayak kerangka atau fondasi rumahnya. Dinding, atap, jendela,\
pintu semuanya disusun pake HTML

**Kalau kamu ngerti HTML, kamu bisa:**

*

***

## 🧠 IP Address dan DNS

* **IP Address** = alamat server
* **DNS** = sistem yang mengubah nama domain jadi IP

***

## 🔌 Port dan Service

Port = pintu masuk layanan di server

* Port 80 = HTTP
* Port 443 = HTTPS
* Port 22 = SSH

***

## 📶 HTTP Status Code

* 200 = OK
* 404 = Not Found
* 500 = Server Error

***

> Penting bagi pentester memahami struktur website agar bisa mengenali celah keamanan secara akurat.
