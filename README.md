# A Dark Room
![Logo](https://upload.wikimedia.org/wikipedia/commons/9/9a/A_dark_room_logo.jpg "A Dark Room")
## About
A Dark Room merupakan sebuah game berbasis text adventure yang dapat dimainkan di web browser atau mobile. 
[Github](https://github.com/doublespeakgames/adarkroom)
## Gameplay
Pemain hanya perlu menekan button yang berisi pilihan untuk memainkannya, seiring waktu pemain perlu mengumpulkan resource berupa kayu, bulu, dan daging untuk membangun sebuah alat atau bangunan.
![Gameplay](https://www.mobygames.com/images/shots/l/760808-a-dark-room-browser-screenshot-moving-the-cursor-over-a-letter.png)
# Instalasi
## Requirement
1. HTML5
## Instalasi Virtual Machine Ubuntu
1. Membuat VM Ubuntu Server, disini kami menggunakan virtual machine yang tersedia di [Github Pak Auriza](https://github.com/auriza/komdat-lab/blob/master/p01.md).
2. Setting Port, yang berutujuan untuk agar VM bisa diakses dari luar melalui alamat IP host (localhost). Masuk ke 'Settings -> Network -> Advanced -> Port Forwarding' dan tambahkan dua aturan berikut.
---insert image here---
3. Login dengan kredensial
```bash
Username: student
Password: student
```
4. Instalasi LAMP
  ```bash
# akses vm dari host
ssh student@localhost -p 2222

# install apache, mysql, php
sudo apt update
sudo apt upgrade
sudo apt install apache2 php mysql-server
sudo apt install php-mysql php-gd php-mbstring php-xml php-curl
sudo service apache2 restart
  ```
5. Buka http://localhost:8000/ untuk memeriksa apakah LAMP sudah benar terinstall.

*Tidak perlu menginstall HTML5 karena sudah terdapat dari VM nya sendiri.*


## Instalasi Game A Dark Room
1. Ganti directory ke `/var/www/html`
--insert image here---
2. Git clone repository A Dark Room.
```bash
sudo git clone https://github.com/doublespeakgames/adarkroom.git
  ```
3. Buka http://localhost:8000/adarkroom untuk memainkan game.
# Penggunaan
--insert image here---
# Referensi
- <https://github.com/auriza>
- <https://github.com/awesome-selfhosted/awesome-selfhosted>
- <https://github.com/doublespeakgames/adarkroom>
- Nabil Ahmad
