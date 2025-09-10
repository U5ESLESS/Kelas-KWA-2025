# Soal 7 NoSQL Manipulation

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan

- tujuan soal kali ini adalah mengubah semua komentar produk
- saya memulai dengan melihat salah satu review produk dan melihat ada jim sebagai reviewer
<img width="1079" height="928" alt="Screenshot 2025-09-10 094742" src="https://github.com/user-attachments/assets/89bf3ae2-e994-4ad0-b8a5-5e7da48edd10" />
- saya login sebagai jim dengan cara seperti sebelumnya
- kemudian saya membuka burpsuit untuk mendapatkan request dari product review dengan cara mengedit review saat intercept on
<img width="1079" height="929" alt="Screenshot 2025-09-10 094949" src="https://github.com/user-attachments/assets/5c18879d-e161-4cdf-941b-9ac9451b2e50" />
- saya langung mengirim ke repeater dan melihat isi nya
- kemudian saya membuat payload ({"$ne": null}) dan merubah seluruh komentar dengan payload tsb
<img width="1079" height="923" alt="Screenshot 2025-09-10 095420" src="https://github.com/user-attachments/assets/d1431ab8-e287-4d14-82e9-eb9102a94c6a" />
- setelah saya mematikan intercept dan mengecek website nya, semua komentar berhasil di rubah
<img width="382" height="520" alt="Screenshot 2025-09-10 095531" src="https://github.com/user-attachments/assets/58d79198-13ac-4d45-a6ef-4b3b6b9efaf3" />
