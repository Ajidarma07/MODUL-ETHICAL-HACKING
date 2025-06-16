# Bab 4: Proxy Tools

## 🔍 Apa Itu Proxy Tool?

Proxy tool adalah alat yang menjadi perantara antara browser dan server web. Proxy bisa mencegat, memodifikasi, dan mencatat semua data yang dikirim dan diterima.

---

## 🎯 Fungsi Proxy Tools dalam Pentesting:

1. **Intercept Request & Response**  
   Melihat & menyimpan semua data HTTP

2. **Modify on the Fly**  
   Mengubah parameter sebelum dikirim (contoh: ubah `role=guest` jadi `role=admin`)

3. **Bypass Validasi Client-Side**  
   Skip validasi browser dan kirim data mentah

4. **Repeater / Fuzzer**  
   Uji payload berulang (XSS, SQLi, dll)

5. **Logging**  
   Dokumentasi semua request/respons

---

## ⚒️ Contoh Proxy Tools:

- **Burp Suite**
- **OWASP ZAP**
- **Fiddler**
- **Charles Proxy**

---

> Proxy tools sangat penting dalam proses eksploitasi dan analisis aplikasi web.
