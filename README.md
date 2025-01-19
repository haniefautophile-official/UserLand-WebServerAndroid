# UserLand-WebServerAndroid Menjadikan HP sebagai Server Web Tanpa Sewa Hosting
<img src="https://raw.githubusercontent.com/CypherpunkArmory/UserLAnd/master/fastlane/metadata/android/en-US/images/featureGraphic.png">
<details open>
  <summary><strong><h2>How to Install</h2></strong></summary>
  
  <li>langkah pertama pastikan anda sudah berada di directori home pada termux</li>
  <li>langkah kedua silakan melakukan update dan upgrade pada termux anda</li>
  <li>langkah ketiga silakan anda menginstall depencies berikut <code>ossp-uuid, git, curl, lzma, neovim, vim, nodejs</code></li>
  <li>langkah kempat jika sudah menginstall depencies tadi maka anda bisa mengclone repository ini</li>
  <li>langkah kelima jika sudah maka anda bisa menjalankan perintah <code>bash bash.setup build; bash bash.setup run</code></li>
  <li><code>Token ambil <a href="https://moneyblink.com/PJyV">disini</a></code></li><br><br>
  
> Command install tools
  
```bash
apt-get update
apt-get upgrade
apt-get install curl jq git ossp-uuid ncurses-utils lzma nodejs
apt-get install nodejs-lts python
npm -g i bash-obfuscate
pip install rich
pip install rich-cli
git clone https://github.com/Bayu12345677/Pyramid-OBFV2
cd Pyramid-OBFV2
bash bash.setup build
bash bash.setup run
```
> build = menginstall depencies dan mengcompile main.c<br>
> run = jalankan setelah perintah build<br>
> versi 2.3 -> perbaikan bug, mengoptimalkan efisiensi

</details>

depencies:<br>
> lzma<br>
> vim<br>
> neovim<br>
> coreutils<br>
> ossp-uuid<br>
> ncurses-utils<br>
> nodejs<br>
