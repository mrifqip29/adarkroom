# A Dark Room
![Logo](https://upload.wikimedia.org/wikipedia/commons/9/9a/A_dark_room_logo.jpg "A Dark Room")
## About
A Dark Room merupakan sebuah game berbasis text adventure yang dapat dimainkan di web browser. Terdapat pula versi mobile game ini pada paltform Android maupun iOS yang dapat diunduh pada marketplace masing-masing platform
[Github](https://github.com/doublespeakgames/adarkroom)
# Instalasi
## Requirement
1. HTML5
2. Perangkat Non-mobile
## Instalasi Virtual Machine Ubuntu
1. Membuat VM Ubuntu Server, disini kami menggunakan virtual machine yang tersedia di [Github Pak Auriza](https://github.com/auriza/komdat-lab/blob/master/p01.md).
2. Setting Port, yang berutujuan untuk agar VM bisa diakses dari luar melalui alamat IP host (localhost). Masuk ke 'Settings -> Network -> Advanced -> Port Forwarding' dan tambahkan dua aturan berikut.
![Port Forwarding](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/1583252089290.png)
3. Login dengan kredensial
```bash
Username: student
Password: student
```
4. Instalasi LAMP
  ```bash
# akses vm dari host
ssh student@localhost -p 2222
  ```
![ssh](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/1583252080896.png)
  ```
# install apache, mysql, php
sudo apt update
sudo apt upgrade
sudo apt install apache2 php mysql-server
sudo apt install php-mysql php-gd php-mbstring php-xml php-curl
sudo service apache2 restart
  ```
![Install1](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/1583252033334.png)  

5. Buka http://localhost:8000/ untuk memeriksa apakah LAMP sudah benar terinstall.

*Tidak perlu menginstall HTML5 karena sudah terdapat dari VM nya sendiri.*

## Menghubungkan VM dengan terminal/cmd
```bash
ssh student@localhost -p 2200
```
## Instalasi Game A Dark Room
1. Ganti directory ke `/var/www/html`
2. Git clone repository A Dark Room.
```bash
sudo git clone https://github.com/doublespeakgames/adarkroom.git
  ```
![Install2](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/1583252016914.png) 
 
3. Buka http://localhost:8000/adarkroom untuk memainkan game.
## Gameplay
Pemain hanya perlu menekan button yang berisi pilihan untuk memainkannya, seiring waktu pemain perlu mengumpulkan resource berupa kayu, bulu, dan daging untuk membangun sebuah alat atau bangunan.
## Main Page : A Firelit Room
Pada page ini berisi halaman utama dimana terdapat menu build, craft, dan buy. 
![Main Page](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%201%20main%20page.png)
## The Village
Pada page ini berisi halaman dimana terdapat button _gather wood_ untuk mengumpulkan kayu, _check traps_ untuk mengumpulkan resource (jika sudah membangun _trap_), dan jasa-jasa yang ter-_unlock_ ketika sudah membangun bangunan tertentu. 
![Page Village](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%202%20page%20village.png)
## A Dusty Path
Page ini berisi persiapan-persiapan peralatan yang bisa dibawa sebelum menuju ke Adventure Map.
![A Dusty Path](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%203%20a%20dusty%20path.png)
## Adventure
Berisi map untuk dieksplorasi, dengan berbagai bangunan yang bisa dikunjungi, dan musuh-musuh yang bisa dilawan.
![Adventure Map](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%203b%20a%20dusty%20path%20map.png)
## Attack Enemy 
Ketika bertemu dengan musuh, Anda bisa melawan musuh dengan senjata yang Anda punya dan menyembuhkan diri dengan barang yang Anda punya.
![Attack Enemy](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%203c%20attack%20enemy.png)
## Enemy Loot
Ketika musuh sudah berhasil dimatikan, akan muncul _loot_ yang dimiliki oleh musuh tersebut.
![Enemy Loot](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%203d%20enemy%20dead.png)
## Arrive Location
Ketika sampai di lokasi manapun, akan muncul popup berikut, bervariasi dengan lokasi yang didatangi.
![Arrive Location](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%203e%20arrived%20checkpoint.png)
## And Old Starship
Menu ini muncul ketika sudah mendatangi lokasi _An Wrecked Starship_ di _Adventure Map_. Terdapat button _Reinforce Hull_, _Upgrade Engine_, dan _Lift off_.
![An Old Starship](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/gameplay%204%20an%20old%20starship.png)

Ketika Anda mengklik button _lift off_, akan menuju minigame dimana kita harus menghindari _obstacle-obstacle_ yang berjatuhan.

![Starship Game](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/space%20game.png)
## Saving Games
Jika ingin menyimpan data permainan, klik save games di menu sebelah bawah kanan. Akan muncul menu _import_ dan _export_.
![Saving Games](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/save%20gameplay.png)

Klik _export_ jika ingin menyimpan permainan. Akan muncul kode enkripsi yang bisa kalian _copy_ dan import jika ingin kalian load gameplay nya.

![Export Gameplay](https://github.com/mrifqip29/adarkroom/blob/master/Screenshot/export%20gameplay.png)


# Referensi
- <https://github.com/auriza>
- <https://github.com/awesome-selfhosted/awesome-selfhosted>
- <https://github.com/doublespeakgames/adarkroom>
- Nabil Ahmad
