# Soal 3 picoctf: No SQL Injection

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan
- seperti biasa kita coba payload di login page untuk mendapatkan request http pada burpsuite
- kemudian kita download file yang di beri dari pico dan cek semua isi file nya
<img width="1079" height="1874" alt="Screenshot 2025-09-10 083026" src="https://github.com/user-attachments/assets/47ecd274-f036-4cc0-821b-1e5b7b49038b" />

- kita bisa dapati ada hal yang janggal pada server.js dan mari kita coba tempelkan payload yang bisa kita buat
({
  "email": "{\"$ne\": null}",
  "password": "{\"$ne\": null}"
}) ke dalam burpsuite

<img width="1079" height="920" alt="Screenshot 2025-09-10 082945" src="https://github.com/user-attachments/assets/9f21c595-71c1-4576-ad4c-60de3eba048f" />
- setelah kita send request, kita bisa dapati ada sebuah token yang bisa di decode
<img width="506" height="373" alt="Screenshot 2025-09-10 083121" src="https://github.com/user-attachments/assets/5cf273e5-c6d6-4d99-afe2-e2d6eb65004c" />

- langsung saja kita decode
<img width="747" height="578" alt="Screenshot 2025-09-10 083155" src="https://github.com/user-attachments/assets/7f37d0e3-959f-48be-b6a4-09ca3af360e5" />
flag sudah di dapatkan
