# Bab 5: Authentication & Session Management

## 🔐 Authentication & Session

- **Authentication**: proses login (username + password)
- **Session**: menjaga identitas pengguna setelah login

---

## 🍪 Cookies dan Session ID

- Cookie: file kecil dari server
- Session ID: penanda unik sesi
- JWT: token modern berbasis digital signature

---

## 🔎 Cara Lihat Session:

1. Login ke website
2. Buka proxy > HTTP history
3. Cari `Set-Cookie`
4. Lihat apakah cookie dikirim saat refresh

---

## ⚠️ Masalah Umum

- **Session Hijacking**: session ID dicuri
- **Brute Force**: coba banyak kombinasi login
- **Poor Logout Handling**
- **Insecure Cookie**: tanpa `HttpOnly` atau `Secure`

---

> Authentication yang lemah adalah celah besar dalam sistem keamanan web.
