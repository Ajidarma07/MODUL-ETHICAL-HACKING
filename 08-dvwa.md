# Damn Vulnerable Web App

## 💡 Apa Itu Damn Vulnerable Web App (DVWA)?

Aplikasi web lokal berisi kerentanan nyata untuk latihan ethical hacking.

**Cara Pakai Damn Vulnerable Web App (DVWA):**

1. 1.Clone dari Github lalu install
2. Install VM Metasploitable 2

<div align="center"><figure><img src=".gitbook/assets/image (1).png" alt="" width="413"><figcaption><p><strong>Damn Vulnerable Web App</strong></p></figcaption></figure></div>

<figure><img src=".gitbook/assets/image (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

## Command Injection:

**Deskripsi:**

Command Injection adalah jenis kerentanan yang terjadi saat aplikasi web menyisipkan input pengguna langsung ke perintah sistem&#x20;operasi (OS). Jika input ini tidak disaring dengan baik, penyerang bisa menyisipkan perintah tambahan, yang akan dieksekusi oleh sistem.

<figure><img src=".gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>

**Cara Berpikir Seorang Ethical Hacker:**

* Identifikasi Titik Injeksi  &#x20;Cari form atau URL yang menerima input dan memicu interaksi dengan sistem  &#x20;Contoh: form input alamat IP, domain, atau path file
* Lakukan Tes dengan Payload Aman  &#x20;Masukkan IP biasa: 127.0.0.1  &#x20;Lalu coba payload ringan seperti:

1. 127.0.0.1; whoami
2. 127.0.0.1 && whoami
3. 127.0.0.1 || whoami



🧠 **Mindset:**

“Bagaimana caranya input saya bisa ‘memecah’ atau ‘menambahkan’ perintah\
ke command line server?”

***

## Brute Force:

**Deskripsi:**

Brute Force adalah teknik serangan di mana attacker mencoba berbagai kombinasi username dan password secara berulang-ulang hingga menemukan\
yang benar.

**Jenis brute force umum:**

* Credential stuffing: menggunakan combo username/password yang pernah bocor
* Dictionary attack: pakai daftar password umum (admin, 123456, dll)
* Pure brute force: semua kemungkinan karakter

**Proses:**

1. **Identifikasi Form Login**   \
   Cari form login atau halaman authentication di web target
2. **Uji Manual Terlebih Dulu**   \
   Coba kombinasi admin:admin, admin:password   \
   Perhatikan respon jika login berhasil → redirect? flag? tulisan?
3. **Otomatisasi Brute Force**   \
   Gunakan tools seperti: Hydra, Burp Intruder, FFUF (untuk parameter brute)
4. **Gunakan Wordlist**   \
   Contoh file: rockyou.txt, custom wordlist

## Cross Site Request Forgery

CSRF adalah serangan di mana penyerang memanfaatkan status login korban untuk menjalankan aksi tanpa izin, dengan mengelabui browser korban&#x20;agar mengirim request ke situs yang sudah dia login sebelumnya.&#x20;

📌 Ibarat kamu disuruh klik link iseng, tapi ternyata link itu bikin kamu ngirim uang ke orang lain padahal kamu sudah login ke internet banking.

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption><p><strong>Cara kerja CFRSs</strong></p></figcaption></figure>

📦 **Ciri-Ciri Umum Aplikasi Rentan CSRF:**

* Tidak ada token CSRF di form  &#x20;
* Tidak ada validasi ulang terhadap aksi penting
* Aplikasi hanya bergantung pada cookie/session untuk autentikasi



**Cara Berpikir Ethical Hacker (dan Attacker)**

1. **Pahami Sesi & Konteks Korban**   \
   Korban sudah login di aplikasi target   \
   Browser korban menyimpan session/cookie aktif
2. 🎯 **Cari Form Tanpa Perlindungan CSRF**   \
   Contoh: form ubah password, transfer, atau update profile   \
   Cek apakah form punya CSRF token   \
   Jika tidak → bisa jadi target
3. 🎯 **Buat HTML Jahat yang Meniru Request**



## Cross Site Scripting

**Deskripsi:**

XSS (Cross-Site Scripting) adalah kerentanan web yang memungkinkan penyerang menyisipkan kode JavaScript berbahaya ke halaman web yang dilihat oleh\
pengguna lain.

📌 Dengan XSS, attacker bisa membuat browser korban menjalankan script yang tidak diinginkan.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (5).png" alt="" width="450"><figcaption></figcaption></figure>

🧠 **Mindset:**

“Apakah input saya dimasukkan ke HTML tanpa disanitasi?”\
“Apakah HTML, attribute, atau JS bisa disusupi kode saya?”

## SQL Injection

**Deskripsi:**

SQL Injection adalah kerentanan yang memungkinkan penyerang menyisipkan perintah SQL berbahaya ke dalam input yang dikirimkan ke server, untuk\
memanipulasi database.

📌 Misalnya: attacker bisa login tanpa password, mencuri data, bahkan mengubah isi database.

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

💣 Dampak Umum dari SQLi:

* Bypass login (akses tanpa password)
* Dump data (usernames, passwords, email, dsb)
* Modifikasi/menghapus data)

## File Uploads Vulnerability

**Deskripsi:**

File Upload Vulnerability adalah celah keamanan yang memungkinkan penyerang mengunggah file berbahaya (biasanya file dengan kode server-side seperti\
.php, .jsp, .asp) ke server target, dan menjalankannya.

📌 Tujuan utama: mendapatkan Remote Code Execution (RCE), akses shell, atau deface website.

<figure><img src=".gitbook/assets/image (7).png" alt="" width="563"><figcaption></figcaption></figure>

⚠️ **Masalah Umum:**

* Tidak membatasi ekstensi file
* Tidak mengecek MIME type
* File disimpan di folder yang bisa diakses publik
* Tidak ada validasi isi file

## File Inclusion

**Deskripsi**:&#x20;

File Inclusion adalah kerentanan yang memungkinkan attacker untuk memuat dan mengeksekusi file lain dalam aplikasi web, baik dari lokal maupun remote.

📌 Umumnya terjadi karena aplikasi menerima input user untuk menentukan file mana yang akan dimuat, lalu menyisipkan input tersebut dalam fungsi include, require, include\_once, atau require\_once tanpa validasi.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (10).png" alt="" width="510"><figcaption></figcaption></figure>

***

> DVWA adalah tempat terbaik untuk latihan eksploitasi kerentanan web secara legal.
