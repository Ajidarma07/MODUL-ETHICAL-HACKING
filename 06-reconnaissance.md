# Reconnaissance

## 🕵️ Apa Itu Reconnaissance?

Reconnaissance adalah proses awal dalam penetration testing untuk mengumpulkan informasitentang target.&#x20;informasi yang didapat menentukan efektivitas tahap berikutnya dalam Penetration Testing.

***

## 📖 Metode Pentest:

* Reconnaissance
* Planning
* Exploitation
* Post Exploit
* Reporting

<figure><img src=".gitbook/assets/image (5).png" alt="" width="228"><figcaption></figcaption></figure>

Mirip kayak detektif yang sedang&#x20;mengumpulkan informasi tentang&#x20;suatu kasus sebelum bertindak lebih lanjut.

***

## 🔍 Jenis Recon:

### 🧘 Passive Recon:

Mengumpulkan informasi tanpa&#x20;berinteraksi langsung dengan target

* Whois lookup
* DNS Enum
* Google Dorking
* Shodan, Wayback Machine

### 🔨 Active Recon:

Mengumpulkan informasi dengan&#x20;berinteraksi langsung dengan target

* Nmap, Nikto
* Dirsearch, WhatWeb
* Wappalyzer, Subfinder

<h2 align="center">Tools For Recon:</h2>

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 101717.png" alt=""><figcaption></figcaption></figure>

## 🧠Web Technologies & CMS

Kenapa Perlu Tahu Teknologi Web?

🔍 “Tidak bisa menebak celah kalau tidak tahu&#x20;temboknya dari apa.”

Beda teknologi, beda potensi kerentanannya. Bantu kita nentuin pendekatan pentest. Bisa pakai exploit yang spesifik.

Contoh:

WordPress ➝ target plugin vulnerable\
Node.js ➝ rentan RCE (Remote Code Execution).



CMS = Content Management System

🛠 Platform siap pakai untuk bangun website tanpa coding dari nol.

Contoh CMS:

* WordPress (paling umum, plugin banyak)
* Joomla
* Drupal
* Ghost (khusus blog

**Banyak serangan muncul dari plugin/theme pihak ketiga!**

Kenapa CMS mudah Rentan

🔨Banyak plugin eksternal → risiko tinggi\
❌User jarang update → lubang keamanan tetap terbuka\
⚙️Default config & exposed admin page



🛑 Contoh umum:

* wp-admin terbuka
* Plugin bajakan yang inject malware
* Brute force ke halaman login WordPress

## 📝 Checklist Hasil Recon:

* IP & nameserver
* Teknologi web (CMS/server)
* Port terbuka
* Direktori sensitif
* Entry point eksploitasi

***

> Semakin banyak data saat recon, semakin tajam eksploitasi yang bisa dilakukan.
