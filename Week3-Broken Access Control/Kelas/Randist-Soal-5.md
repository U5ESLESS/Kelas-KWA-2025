# Soal 5 Forged Feedback
## Randist Prawandha Putera 5027231059
## Langkah-langkah pengerjaan
## 1. login akun dan masuk ke customer feedback
- setelah login masuk ke page customer feedbak
<img width="1093" height="1014" alt="image" src="https://github.com/user-attachments/assets/b2ceb94c-ff8a-4bf1-909e-9318ba717606" />

---

## 2. Interception
- isi feedback asal dan captcha (jangan submit terlebih dahulu)
- nyalakan intercept pada burpsuite
- submit untuk mendapatkan request di burpsuite
<img width="1918" height="1024" alt="image" src="https://github.com/user-attachments/assets/59212ae1-446c-4c1d-ac3a-28325210e61e" />

---

## 3. Forged Feedback
- perhatikan request dari post API/Feedbacks/ HTTP/1.1
- kita dapatkan ada sebuah **UserId":2**
<img width="893" height="435" alt="image" src="https://github.com/user-attachments/assets/f93e1b85-9a04-4cb0-b3fe-454fe4aa20ad" />
- ubah value dari userId nya contoh (UserId":2 menjadi UserId":4)
- setelah value nya sudah di ubah, langkah terakhir adalah memforward request tsb.
<img width="890" height="1023" alt="image" src="https://github.com/user-attachments/assets/696fcbcb-1030-4c0d-a9fa-a3330b94ab64" />
<img width="1022" height="1023" alt="image" src="https://github.com/user-attachments/assets/7f1b0d70-3089-40f6-b3ec-aa62b920ea48" />
Soal berhasil kita selesaikan
