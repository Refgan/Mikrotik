# Login MikroTik Menggunakan WinBox

Assalamualaikum wr wb, disini saya akan membuat langkah-langkah untuk melakukan *login* atau meremote perangkat router MikroTik menggunakan aplikasi WinBox, Webfig, SSH Telnet dan FTP

---

1. Login Mikrotik menggunakan aplikasi **Winbox**:


Aplikasi ini sering digunakan dengan **Port 8291 TCP**

<img width="95" height="96" alt="Screenshot 2026-07-31 141808" src="https://github.com/user-attachments/assets/241cf402-524c-4c0d-9c03-902bbcdbbf93" />


a. download aplikasi winbox di https://mikrotik.com/download/winbox

b. Setelah download buka aplikasi winbox, klik bagian **Neighbors** dan **Refresh**

c. Sesudah muncul tampilan tersbut, klik Mac address=6C:3B:6B:E2:09:5D lalu **connect** (untuk password kosongkan saja)

<img width="1366" height="516" alt="Screenshot 2026-07-31 153107" src="https://github.com/user-attachments/assets/729c5e4e-ece8-46f8-b159-a6d0b68f1575" />

d. nanti akan masuk ke dalam halaman berikut

<img width="1365" height="767" alt="Screenshot 2026-08-07 132856" src="https://github.com/user-attachments/assets/c1e99c7a-144f-461c-aadf-14cfb74118ba" />


---

## 2. login Dengan Webfig

<img width="82" height="105" alt="Screenshot 2026-08-07 133226" src="https://github.com/user-attachments/assets/a8bbcb4b-0013-4c30-a366-909f3bac5d6d" />


a. kalian masuk ke web chrome

b. Pada tab Pencarian ketik ip default mikrotik **192.168.88.1**

<img width="344" height="122" alt="ss" src="https://github.com/user-attachments/assets/5fb99104-c5f2-4005-a79e-17fba33bcc5e" />

c. Login dengan admin untuk password kosongkan saja

<img width="1365" height="767" alt="Screenshot 2026-08-07 133652" src="https://github.com/user-attachments/assets/002f0c16-449e-47bd-beec-db069b0b915b" />

berikut adalah tampilan MikroTik di dalam Website chrome :

<img width="1362" height="736" alt="Screenshot 2026-08-07 134807" src="https://github.com/user-attachments/assets/3a6f16ca-e8ad-49aa-b980-e411c8a29349" />


### 3.Login Mikrotik dengan SSH dan Telnet

 **1. Telnet**


*Pastikan aplikasi PuTTY sudah terinstal di komputer/laptop*, (https://putty.org/index.html)

<img width="138" height="145" alt="puiy" src="https://github.com/user-attachments/assets/42b89c68-57bc-4c25-bce2-2c76a84484cf" />


a. Buka aplikasi PuTTY di komputer Anda.

b. Pada bagian Connection type, pilih opsi SSH. 

c. Masukkan alamat IP MikroTik pada kolom Host Name (or IP address). (Contoh: 192.168.88.1).

d. Pastikan kolom Port terisi angka 22 (port default SSH).

e. Klik tombol Open di bagian bawah.

<img width="447" height="443" alt="Screenshot 2026-08-07 141255" src="https://github.com/user-attachments/assets/98227929-5dfb-4532-91d5-6ba33336f399" />


Jika muncul jendela peringatan keamanan (*PuTTY Security Alert*), klik saja Accept atau Yes.
Akan muncul jendela hitam (*command prompt*). 
Ketik login MikroTik Anda dengan admin, lalu tekan Enter.
Anda akan masuk ke command line MikroTik yang ditandai dengan munculnya prompt nama router Anda.
<img width="658" height="418" alt="Screenshot 2026-08-07 142939" src="https://github.com/user-attachments/assets/c71e3d75-e20c-4b40-b5ca-6f4c64575370" />

**2. SSH**

Dan yang kedua menggunakan SSH dalam aplikasi PuTTY
