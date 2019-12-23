# qrlogin
## QR Code scanner for login hotspot MikroTik

### Cara pakai

1. Tambahkan code button di login.html
```
<button onclick="window.location='https://starwifi88.github.io/qr/?hotspot=Nama Hotspot Anda';">QR Login</button>
```
2. Tambahkan script berikut di MikroTik via terminal.
```
/ip hotspot walled-garden ip
add action=accept comment="HMS QR Code Scanner" disabled=no dst-host=ztarwifi88.github.io
```
