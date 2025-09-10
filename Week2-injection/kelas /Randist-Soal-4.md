# Soal 4 Database Schena

## Randist Prawandha Putera 5027231059

# Langkah-langkah pengerjaan

## 1. Intercept Request
- Gunakan *Burp Suite* untuk menangkap HTTP request, misalnya pada fitur pencarian produk.
<img width="1079" height="953" alt="image" src="https://github.com/user-attachments/assets/4758b9f2-0487-415c-bc42-b2961de4858c" />

- klik bagian product search
<img width="1078" height="901" alt="image" src="https://github.com/user-attachments/assets/30b9f101-5094-47c0-930b-40d403cd8243" />

- kirim ke repeater lalu send
<img width="1077" height="619" alt="image" src="https://github.com/user-attachments/assets/a52127c5-9246-4b8d-b8c4-5c80a61a997a" />

- cek Database yang Dipakai menggunakan cara Masukkan payload **a'))UNION+Select+1+from+sqlite_master--**
<img width="1079" height="895" alt="image" src="https://github.com/user-attachments/assets/f64d5765-094f-468c-8c2b-9ca9a4105665" />
dari hasil diatas kita dapatkan bahwa database tsb adalah SQLITE

## 2. Cari Jumlah Kolom
- gunakan teknik error-based injection dengan mencoba query:
(' UNION SELECT NULL--)
- tambahkan NULL secara bertahap sampai tidak muncul error.
(' UNION SELECT NULL, NULL, NULL--)
<img width="1079" height="899" alt="image" src="https://github.com/user-attachments/assets/664862f3-77d9-4b06-b444-a7a782d90f62" />
Dari sini kita tahu ada sejumlah kolom tertentu yang bisa di-union.

## 3. Ambil Informasi Schema
- gunakan query untuk membaca tabel sistem SQLite:
(' UNION SELECT sql, NULL, NULL FROM sqlite_master--)
<img width="1079" height="898" alt="image" src="https://github.com/user-attachments/assets/b54bd8b4-f638-4ebf-9dd8-94e0ef4c0361" />

Hasilnya akan menampilkan struktur tabel (schema) dari database Juice Shop.
