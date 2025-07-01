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

<figure><img src=".gitbook/assets/image (5) (1).png" alt="" width="228"><figcaption></figcaption></figure>

Mirip kayak detektif yang sedang&#x20;mengumpulkan informasi tentang&#x20;suatu kasus sebelum bertindak lebih lanjut.

***

## 🔍 Jenis Recon:

### 🧘 Passive Recon:

**Mengumpulkan informasi tanpa&#x20;berinteraksi langsung dengan target:**

* Whois lookup
* DNS Enum
* Google Dorking
* Shodan, Wayback Machine

### 🔨 Active Recon:

**Mengumpulkan informasi dengan&#x20;berinteraksi langsung dengan target:**

* Nmap, Nikto
* Dirsearch, WhatWeb
* Wappalyzer, Subfinder

<h2 align="center">Tools For Recon:</h2>

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 101717.png" alt=""><figcaption></figcaption></figure>

## 🧠Web Technologies & CMS

**Kenapa Perlu Tahu Teknologi Web?**

🔍 “Tidak bisa menebak celah kalau tidak tahu&#x20;temboknya dari apa.”

Beda teknologi, beda potensi kerentanannya. Bantu kita nentuin pendekatan pentest. Bisa pakai exploit yang spesifik.

**Contoh:**

WordPress ➝ target plugin vulnerable\
Node.js ➝ rentan RCE (Remote Code Execution).



**CMS = Content Management System**

🛠 Platform siap pakai untuk bangun website tanpa coding dari nol.

**Contoh CMS:**

* WordPress (paling umum, plugin banyak)
* Joomla
* Drupal
* Ghost (khusus blog

**Banyak serangan muncul dari plugin/theme pihak ketiga!**



**Kenapa CMS mudah Rentan:**

🔨Banyak plugin eksternal → risiko tinggi\
❌User jarang update → lubang keamanan tetap terbuka\
⚙️Default config & exposed admin page



🛑 **Contoh umum:**

* wp-admin terbuka
* Plugin bajakan yang inject malware
* Brute force ke halaman login WordPress

## 📝 Steps to Recon:

**Langkah 1: Menentukan Target**\
Gunakan situs legal yang umum diakses publik, seperti:

* Website Universitas
* Website Pemerintah lokal
* Situs berita nasional

(jangan targetkan web perbankan, militer, dan rumah sakit).



**Langkah 2: Passive Reconnaissance**\
Gunakan metode passive reconnaissance terlebih dahulu:

* Whois
* WhatWeb
* Wappalyzer
* Shodan



**Langkah 3: Active Reconnaissance**

* Nmap
* Dirsearch
* Subfinder
* Shortscan
* Wpscan

**Langkah 4: Working Paper/Checklist Filling**

* Word/Googledocs
* Excel
* Notes

Contoh Working Paper



📋 **Tugas Dokumentasi:**

Setiap peserta diminta untuk&#x20;mencatat hasil berikut:

* IP address dan nameserver
* Teknologi website (CMS, server,  \
  dll)
* Port dan services terbuka
* Direktori sensitif yang  \
  ditemukan
* Potensi entry point untuk  \
  eksploitasi



***

> Semakin banyak data saat recon, semakin tajam eksploitasi yang bisa dilakukan.
