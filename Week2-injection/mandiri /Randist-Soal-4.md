# Soal 4 picoctf: Irish-Name-Repo 3

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan
- tujuan kita adalah masuk sebagai admin
<img width="1079" height="922" alt="Screenshot 2025-09-10 084419" src="https://github.com/user-attachments/assets/0223d56b-76d1-4ded-a012-cc248ef0ea96" />

- setelah masuk kedalam login admin, kita hanya di berikan opsi pass
<img width="1079" height="929" alt="Screenshot 2025-09-10 084426" src="https://github.com/user-attachments/assets/5fbff4f1-79af-437d-9d79-4a637eb8bbf3" />

- saat saya mencoba menggunakan payload yang biasa saya pakai yaitu ' OR '1'='1'-- hasil nya tidak terjadi apa-apa, namun ada kejanggalan pada kalimat debug.
- maka saya coba untuk mengganti debug dari 0 menjadi 1
<img width="1075" height="929" alt="Screenshot 2025-09-10 090022" src="https://github.com/user-attachments/assets/1c0bda24-d5c9-4ef7-b644-6bb817f6a1e9" />
- setelah saya coba bereksperimen saya menemukan bahwa hasil dari pass adalah rot13
<img width="1079" height="928" alt="Screenshot 2025-09-10 090040" src="https://github.com/user-attachments/assets/f0f4a51a-c60f-484d-b6e6-08f12a240196" />
<img width="1079" height="927" alt="Screenshot 2025-09-10 090201" src="https://github.com/user-attachments/assets/4d9c3ed3-369c-4d88-8b4a-92cfeec201ac" />
<img width="1079" height="564" alt="Screenshot 2025-09-10 090344" src="https://github.com/user-attachments/assets/b1fc8535-7a88-4ff9-ac4e-0ea6a8ef83a6" />
- maka saya coba memasukan payload dengan cara sebaliknya dan saya mendapatkan hasil seperti gambar berikut
<img width="1079" height="599" alt="Screenshot 2025-09-10 090431" src="https://github.com/user-attachments/assets/28d8ef3c-da45-4673-923a-a02b2441f212" />
- setelah saya coba login ternyata berhasil
<img width="1079" height="924" alt="Screenshot 2025-09-10 090451" src="https://github.com/user-attachments/assets/13eef703-90df-4213-92dd-e3fae9299b59" />
flag sudah di dapatkan
