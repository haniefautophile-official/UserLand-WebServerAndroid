# UserLand-WebServerAndroid Menjadikan HP sebagai Server Web Tanpa Sewa Hosting
<img src="https://raw.githubusercontent.com/CypherpunkArmory/UserLAnd/master/fastlane/metadata/android/en-US/images/featureGraphic.png">
<details open>
  <summary><strong><h2>How to Install Part 1</h2></strong></summary>
  
  <li>langkah pertama download aplikasi userland di playstore dan termux di frdoid, lalu buka dan pilih ubuntu</li>
 
> Install di ubuntu userland, copy semua kode ini dan paste di ubuntu
  
```bash
=> sudo su lalu enter
=> passwd lalu enter (Buat password dan konfirmasi password) Password tidak akan terlihat
=> apt update ; apt upgrade -y ; apt install neofetch -y ; apt install nano -y ; apt install nginx -y ; service nginx status
=> nano /etc/nginx/sites-available/default
```
<li>Cari tulisan listen, kemudian ganti angka 80 menjadi 8080</li><br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-17-29-45-892_tech.ula.jpg"><br>
<li>Setelah itu, simpan dengan menekan tombol ctrl + x + y lalu enter</li><br>
<li>Lanjut installasi</li><br>
```
=> service nginx restart
=> cd /var/www/html
=> ls
=> rm -f index.nginx-debian.html
=> nano index.html
```
> Tulis sebagai contoh atau anda bisa mengarangnya sendiri<br>
> Example:<br>
> Welcome to Web Server Android<br>
> Lalu simpan dengan menekan tombol ctrl + x + y lalu enter<br>
> Next installasi part 2<br>
> Buka termux dan ketik atau copy semua kode ini:<br>
```
=> apt update ; apt upgrade -y ; pkg install openssh nmap
=> ssh root@192.168.xxx (Ip hp anda)
```
> Untuk mengetahui alamat ip anda buka ponsel, cari tentang ponsel, lihat keseleuruhan spesifikasi. Ada di alamat address.
```
=> ssh root@192.168.xxx -p 2022
```
> (Ketik yes, lalu masukan password yang sudah anda buat di userland)
```
=> hostname
=> su userland
```
> (Untuk pindah ke userland dari termux)
```
=> service nginx status
```
> Jika anda melihat nginx status running itu berarti server anda sedang berjalan.<br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-14-56-220_com.termux.jpg"><br>
```
=> neofetch
```
> untuk memastikan telah terhubung ke userland bila muncul tampilan ubuntu dan spesifikasi android anda.
```
=> sudo adduser redminote6pro
```
> Untuk menambahkan userbaru  (Bebas mau namai apa terserah anda dan user harus harus huruf kecil semua)<br>
> Setelah itu anda di perintah buat password di user baru dan konfirmasi password, isi identitas anda atau bisa anda isi hanya di pertama dan kosongkan sisanya, lalu enter, kemudian ketik y dan enter.<br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-17-32-017_com.termux.jpg"><br>
> Cek user apakah user anda telah aktif atau tidak dengan mengetik:<br>
```
=> su redminote6pro
=> nano /var/www/html/index.html
```
Kemudian ketik kode sederhana ini untuk uji coba:
```
<h1>Test Web Server Android Redmi Note 6 Pro</h1>
```
> Setelah itu klik ctrl + x + y dan enter untuk menyimpan.<br>
> Setelah itu cek di browser dengan memasukan ip kita dengan port 8080.<br>
> Contoh: 192.168.xxx:8080<br>
> Maka lihat hasilnya.<br>
> Kemudian onlinenkan server anda agar bisa di gunakan banyak orang dengan masuk ke situs ngrox, pilih bagian logo pingwin, lalu copy semua kode di apt<br>
> <img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-09-07-946_com.android.chrome.jpg"><br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-20-46-920_com.termux.jpg"><br>
> Tunggu installasi sampai selesai. Dan jika sudah selesai maka lanjut ke kode selanjutnya dari ngrok:<br>
```
=> ngrok config add-authtoken xxxxxxx
```
> Jalankan web yang sudah anda buat dengan mengetik:
```
=> ngrok http 8080
```
> Maka akan berjalan seperti ini:<br>
> <img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-34-35-171_com.termux.jpg">
> Lalu copy https sampai seperti gambar di atas<br>
> Lalu copy di browser.<br>
<img src="https://github.com/haniefautophile-official/UserLand-WebServerAndroid/blob/main/ss/Screenshot_2025-01-18-18-34-24-555_com.android.chrome.jpg"><br>

</details>

Selamat anda sudah mempunyai server web pribadi tanpa beli hosting<br>

