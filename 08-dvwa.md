# Bab 8: Studi Kasus – DVWA

## 💡 Apa Itu DVWA?

DVWA = Damn Vulnerable Web Application  
Aplikasi web lokal untuk latihan ethical hacking dengan kerentanan nyata.

---

## 📋 Cara Pakai:
1. Clone DVWA dari GitHub
2. Install di VM (misal Metasploitable 2)
3. Akses dari browser

---

## 🧪 Contoh Kerentanan:

### 1. **Command Injection**
- Coba payload: `127.0.0.1; whoami`

### 2. **Brute Force**
- Gunakan wordlist (rockyou.txt)
- Tools: Hydra, Burp Intruder

### 3. **CSRF**
- Cek form yang tidak punya token
- Buat HTML jahat meniru request

### 4. **XSS**
- Masukkan script JS ke input
- Contoh: `<script>alert(1)</script>`

### 5. **SQL Injection**
- Masukkan `' OR 1=1 --`
- Curi data, bypass login

### 6. **File Upload**
- Upload file `.php` lalu akses URL
- Coba reverse shell

### 7. **File Inclusion**
- Coba `?page=../../etc/passwd`

---

> DVWA adalah tempat terbaik untuk latihan eksploitasi kerentanan web secara legal.
