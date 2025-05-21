## 2.1 How to run it and what happens when you type some text in the clients

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

## 2.2 Modifying the websocket port

Ketika saya memodifikasi port pada client dari 2000 menjadi 8080, maka server tidak akan bisa berjalan karena server sendiri berjalan di server 2000, yang mana server dan client harus berada di port yang sama. Jadi, agar aplikasi tetap berjalan, jika ingin mengubah port ke 8080, server dan client keduanya harus berjalan di port tersebut.

### Tampilan sebelum mengubah port server ke 8080
Server:
![Image](https://github.com/user-attachments/assets/9cecc507-d20e-4e7f-bbf6-9ea8966c5eee)

Client:
![Image](https://github.com/user-attachments/assets/39b4bae5-15aa-4331-93a1-7bad0a730283)

### Tampilan setelah mengubah port server ke 8080
Server:
![Image](https://github.com/user-attachments/assets/c54a05a0-f063-401b-a9a6-a93a292c0981)

Client:
![Image](https://github.com/user-attachments/assets/78ced868-e207-4da4-9af0-040487ace28c)


## 2.3 Menambahkan informasi IP
Pada eksperimen ini, saya menambahkan info IP untuk menampilkan client mana yang mengirimkan pesan tersebut.

### Tampilan server setelah modifikasi
![Image](https://github.com/user-attachments/assets/7c60edc0-173c-4dbc-9fcf-c1828ed501fb)

### Tampilan client 1
![Image](https://github.com/user-attachments/assets/21c58c53-1536-4b93-83b2-054a26c5a2b7)

### Tampilan client 2
![Image](https://github.com/user-attachments/assets/d4c5597b-d62e-4222-bd3f-072d6c46d6d6)

### Tampilan client 3
![Image](https://github.com/user-attachments/assets/3feee4aa-bc72-4c45-b473-74ecf886b7b1)

Dari 3 gambar di atas, dapat dilihat ketiga client memiliki nama yang sama, sehingga untuk membedakannya kita menggunakan port.