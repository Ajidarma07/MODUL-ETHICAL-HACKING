---
description: Tools Keamanan
---

# Proxy Tools

## 🔍 Apa Itu Proxy Tool?

Proxy tool itu adalah alat yang jadi "perantara"&#x20;antara browser kamu dan server web.\


Ibarat kamu mau ngobrol sama seseorang,&#x20;tapi ada orang ketiga yang menerjemahkan, mencatat,&#x20;bahkan kadang mengedit omongan kamu dulu\
sebelum dikirim.\


Nah, proxy tool ini si "orang ketiga" itu.

***

## 🎯 Fungsi Proxy Tools dalam Pentesting:

1. **Intercept Request & Response**\
   Bisa melihat, ubah, simpan semua data yang dikirim browser ke server (dan sebaliknya).   \
   Cocok buat analisa form login, cookie, header, dan payload.
2. **Modify on the Fly**\
   Mengubah parameter sebelum dikirim (contoh: ubah `role=guest` jadi `role=admin`)
3. **Bypass Validasi Client-Side**\
   Validasi di sisi browser bisa di-skip, dan kamu bisa kirim data mentah langsung ke server.
4. **Repeater / Fuzzer**\
   Kirim permintaan yang sama berulang-ulang, cocok buat testing XSS, SQLi, Auth Bypass, dsb
5. **Logging**\
   Cocok buat audit atau debugging web application, atau ngelacak celah yang sulit ditemukan.

***

## ⚒️ Contoh Proxy Tools:

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 092248.png" alt=""><figcaption><p><strong>BurpSuite, OWASP, CAIDO</strong></p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2025-07-01 092423.png" alt=""><figcaption><p><strong>Inilah contoh ilustrasi BurpSuite bekerja</strong></p></figcaption></figure>

> Proxy tools sangat penting dalam proses eksploitasi dan analisis aplikasi web.
