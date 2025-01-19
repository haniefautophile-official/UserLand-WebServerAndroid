# UserLand-WebServerAndroid Menjadikan HP sebagai Server Web Tanpa Sewa Hosting
<img src="https://raw.githubusercontent.com/CypherpunkArmory/UserLAnd/master/fastlane/metadata/android/en-US/images/featureGraphic.png">
<details open>
  <summary><strong><h2>How to Install Part 1</h2></strong></summary>
  
  <li>langkah pertama download aplikasi userland di playstore, lalu buka dan pilih ubuntu</li>
  
> Install di ubuntu userland, copy semua kode ini dan paste di ubuntu
  
```bash
=> su lalu enter
=> passwd lalu enter (Buat password dan konfirmasi password) Password tidak akan terlihat
=> apt update ; apt upgrade -y ; apt install neofetch -y ; apt install nano -y ; apt install nginx -y ; service nginx status
=> nano /etc/nginx/sites-available/default
```
> Cari tulisan listen, kemudian ganti angka 80 menjadi 8080c<br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-17-29-45-892_tech.ula.jpg">
> Setelah itu, simpan dengan menekan tombol ctrl + x + y lalu enter<br>
> Lanjut installasi
```
=> service nginx restart
=> cd /var/www/html
=> ls
=> rm -f index.nginx-debian.html
=> nano index.html
```
> Tulis seperti sevagai contoh atau anda bisa mengarangnya sendiri
> Example: <h1>Welcome to Web Server Android</h1>
> Lalu simpan dengan menekan tombol ctrl + x + y lalu enter
> Next installasi paert 2
> Buka termux dan ketik atau copy semua kode ini:
```bash
=> apt update ; apt upgrade -y ; pkg install openssh nmap
=> ssh root@192.168.xxx (Ip hp anda)
=> ssh root@192.168.xxx -p 2022
```
> (Ketik yes, lalu masukan password yang sudah anda buat di userland)
```
=> hostname
=> su usrland
```
> (Untuk pindah ke userland dari termux)
```
=> service nginx status
```
> Jika anda melihat nginx status running itu berarti server anda sedang berjalan.
```
=> neofetch
```
> untuk memastikan telah terhubung ke userland bila muncul tampilan ubuntu dan spesifikasi android anda.
```
=> sudo adduser redminote6pro
```
> Untuk menambahkan userbaru  (Bebas mau namai apa terserah anda dan user harus harus huruf kecil semua)
> Setelah itu anda di perintah buat password di user baru dan konfirmasi password, isi identitas anda atau bisa anda isi hanya di pertama dan kosongkan sisanya, lalu enter, kemudian ketik y dan enter.

```

</details>

depencies:<br>
> lzma<br>
> vim<br>
> neovim<br>
> coreutils<br>
> ossp-uuid<br>
> ncurses-utils<br>
> nodejs<br>
