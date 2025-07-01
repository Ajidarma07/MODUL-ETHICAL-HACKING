# Authentication & Session Management

## 🔐 Authentication & Session

* **Authentication**: Proses  &#x20;identifikasi pengguna  &#x20;Misal: login pakai username  &#x20;dan password
* **Session**: Kondisi  &#x20;setelah user berhasil  &#x20;login  &#x20;Supaya website tahu “kita  &#x20;masih orang yang sama”  &#x20;meski buka banyak halaman

“Auth itu seperti menunjukkan KTP, session itu seperti stempel\
tangan waktu masuk konser supaya bisa bolak-balik venue.”

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 093248.png" alt=""><figcaption></figcaption></figure>

***

## 🍪 SessionID, Cookies, danJSON Web Token(JWT)

**Cookies adalah file kecil yang disimpan browser, biasanya isinya:**

* Session ID
* Info user (kadang)
* Token login

Session ID → penanda unik sesi user. Kalau ini bocor, bisa dipakai orang lain buat nyamar jadi kita.

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

Alternatif modern selain session ID:

JWT = token yang sudah berisi info user dan tanda tangan digital&#x20;

Format: header.payload.signature (dipisah titik).

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 094333.png" alt=""><figcaption></figcaption></figure>

✔️**Kelebihan:**

Stateless (tidak perlu disimpan di server)&#x20;Bisa di-verify langsung.

❗**Tapi hati-hati kalau payload terlalu banyak data sensitif.**

***

## 🔎Cara Lihat Session ID, Cookies atau JWT:

🛠**Praktek:**&#x20;

1. Login ke Website
2. Lihat HTTP request pakai Proxy > HTTP history
3. Perhatikan response dari server:  Apakah ada Set-Cookie? dan Nilai sessionnya apa?
4. Coba refresh halaman, lihat cookie tetap dikirim atau enggak

<figure><img src=".gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

***

## ⚠️ Masalah Umum di Authentication & Session:

* **Session Hijacking**: kalau session ID bocor, hacker bisa ambil alih sesi
* **Brute Force**: mencoba ribuan kombinasi username/password
* **Poor Logout Handling:** user sudah logout, tapi session masih aktif
* **Insecure Cookie**: cookie tidak di-encrypt atau tanpa HttpOnly, Secure flag

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 095959.png" alt=""><figcaption></figcaption></figure>

***

> Authentication yang lemah adalah celah besar dalam sistem keamanan web.
