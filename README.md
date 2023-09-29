# ScriptVPS

Ini adalah [Marzban](https://github.com/Gozargah/Marzban) yang sudah saya tambahkan nginx untuk konfigurasi WebSocket single port. </br>
WebSocket sudah support untuk 443 TLS, 80 HTTP dan Wildcard path, contoh /enter-your-custom-path/trojan </br>

Disclaimer: Proyek ini hanya untuk pembelajaran dan komunikasi pribadi, mohon jangan menggunakannya untuk tujuan ilegal. </br>
Credit full to [Gozargah Marzban](https://github.com/Gozargah), saya hanya edit sedikit untuk instalasi sederhana bagi pemula . </br>

# List Protocol yang support
- VLess
- VMess
- Trojan
- ShadowSocks (To Be added)

# Yang harus dipersiapkan
- VPS dengan minimal spek 1 Core 1 GB ram
- Domain yang sudah di pointing ke CloudFlare
- Pemahaman dasar perintah Linux

# Sistem VM yang dapat digunakan
- Debian 10 </br>
- Debian 11 </br>
- Ubuntu 18.04 </br>
- Ubuntu 20.04 </br>
- Ubuntu 22.04 </br>



# Instalasi
  ```html
 apt-get update && apt-get upgrade -y && apt dist-upgrade -y && update-grub && reboot
 ```
Pastikan anda sudah login sebagai root sebelum menjalankan perintah dibawah
 ```html
 wget https://raw.githubusercontent.com/cerdasbarus/ScriptVPS/main/mar.sh && chmod +x mar.sh && ./mar.sh
 ```
 
Setelah instalasi berhasil, Panel login / Admin bisa ditambahkan dengan command
```html
marzban cli admin create --sudo
 ```
Buka panel Marzban dengan mengunjungi https://domainmu/dashboard <br>
Username dan Password default panel adalah :
- Username : admin
- Password : admin

Jika ingin mengubah konfigurasi env variable 
```html
nano /opt/marzban/.env
 ```
Perintah Restart service Marzban 
```html
marzban restart
 ```
Perintah Cek Logs service Marzban 
```html
marzban logs
 ```
Perintah Cek update service Marzban
```html
marzban update
 ```
# Cloudflare Sett

Pastikan SSL/TLS Setting pada cloudflare sudah di set menjadi full
![image](assets/268485705-3aeedf09-308e-41b0-9640-50e4abb77aa0.png) </br>

Lalu pada tab **Network** pastikan gRPC dan WebSocket sudah ON 
![image](assets/268485759-65d9b413-fda4-478a-99a5-b33d8e5fec3d.png)



# Setting Host Marzban
 
 Saat masuk ke panel, setting host di menu kanan atas <br>
 ![image](assets/268485795-6b96bce7-39c7-4b5c-b01e-8dfdea91cb47.png) </br>

Lalu ubah variabel {SERVER_IP} dibawah menjadi domain yang sudah di pointing tadi <br>
# TROJAN WS
![image](assets/268486958-191a485c-07a7-4a28-88d3-b66fa403abc7.png)
# VMESS WS
![image](assets/268486998-7e8b8622-5b55-4d03-aaf3-6a30eabb62e8.png)
# VLESS WS
![image](assets/268487033-ed50c2e1-6060-4773-a8bb-067e3fc5b7e4.png)
</br>

Jika ada typo atau saran bisa PM ke saya di :<a href="https://t.me/cerdascharo" target=”_blank”><img src="https://img.shields.io/static/v1?style=for-the-badge&logo=Telegram&label=Telegram&message=Click%20Here&color=blue"></a><br>
<br>
Jika anda berminat bisa join ke Telegram channel saya di :<a href="https://t.me/cerdascharo" target=”_blank”><img src="https://img.shields.io/static/v1?style=for-the-badge&logo=Telegram&label=Telegram&message=Click%20Here&color=blue"></a><br>
<br>

Ready VPN Xray-Core, <br>

- Paket Reguler : https://t.me/cerdascharo

</br>
