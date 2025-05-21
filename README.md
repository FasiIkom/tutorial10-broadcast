## 1.1 How to run it and what happens when you type some text in the clients

Cara menjalankan:<br>
Buka terminal dan jalankan `cargo run --bin server` untuk menjalankan server. Lalu, untuk menjalankan client, buka terminal baru (bisa lebih dari 1 tergantung banyak client yang diinginkan), lalu di tiap terminal, jalankan `cargo run --bin client`

Apa yang terjadi jika saya memasukkan text di client?<br>
Saat saya mengetik pesan di salah satu client, pesan tersebut dikirim ke server dan kemudian disiarkan ke semua client yang terhubung, sehingga semua client bisa menerima dan menampilkan pesan secara real-time.

### Screnshot client 1 (pengirim pesan)
![Image](https://github.com/user-attachments/assets/1d9a6441-013e-48ec-9d7a-41beb1648980)

### Screenshot client 2
![Image](https://github.com/user-attachments/assets/fcfc3c66-e43f-43fa-879a-7df90cd4c6bb)

### Screenshot server
![Image](https://github.com/user-attachments/assets/c7c7142e-bb38-4492-be54-679501a45e9d)



