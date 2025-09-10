# Soal 1 Login Admin

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan

## 1. Menangkap Permintaan Login
- gunakan **Burp Suite**, untuk "menyadap" permintaan login yang dikirim dari browser.  
- request nya berupa **HTTP POST** dan berisi data login email dan password dalam format JSON.  


---

## 2. Mengubah Query SQL
- ubah Data email menjadi: **admin@juice-sh.op ' OR '1'='1' --** 
- fungsi dari hal tersebut adalah untuk membuat perintah SQL agar selalu **benar**, sehingga password tidak lagi dicek.  


---



