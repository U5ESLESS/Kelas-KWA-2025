# Soal 1 Login Admin

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan

## 1. Menangkap Permintaan Login
- buka login page
- gunakan console pada browser, ketik **(') atau (")** pada kolom username/email, untuk "menyadap" permintaan login yang dikirim dari browser.
- pass di isi bebas  
- buka network pada console dan amati data login email dan password dalam response.  
<img width="1919" height="981" alt="image" src="https://github.com/user-attachments/assets/7c465c94-d2f1-4d3e-b484-e76e2a4467c2" />


---

## 2. Mengubah Query SQL
- ubah Data email menjadi: **(' OR '1'='1' --) atau (' OR true--)** 
- fungsi dari hal tersebut adalah untuk membuat perintah SQL agar selalu **benar**, sehingga password tidak lagi dicek.
- dalam kasus saya, saya menggunakan (' OR true--)  


---

## 3. berhasil login sebagai admin

