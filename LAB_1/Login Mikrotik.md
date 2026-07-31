# Login MikroTik Menggunakan WinBox

Assalamualaikum wr wb, disini saya akan membuat langkah-langkah untuk melakukan *login* atau meremote perangkat router MikroTik menggunakan aplikasi WinBox, Webfig, SSH Telnet 

---

1. Login Mikrotik menggunakan aplikasi **Winbox**:


Aplikasi ini sering digunakan dengan **Port 8291 TCP**

<img width="95" height="96" alt="Screenshot 2026-07-31 141808" src="https://github.com/user-attachments/assets/241cf402-524c-4c0d-9c03-902bbcdbbf93" />


a. download aplikasi winbox di https://mikrotik.com/download/winbox

b. Setelah download buka aplikasi winbox, klik bagian **Neighbors** dan **Refresh**

c. Sesudah muncul tampilan tersbut, klik Mac address=6C:3B:6B:E2:09:5D lalu **connect** (untuk password kosongkan saja)

<img width="1366" height="516" alt="Screenshot 2026-07-31 153107" src="https://github.com/user-attachments/assets/729c5e4e-ece8-46f8-b159-a6d0b68f1575" />


---

## Langkah-Langkah Login ke MikroTik

Ikuti langkah-langkah di bawah ini untuk terhubung ke router MikroTik Anda:

### 1. Hubungkan Perangkat
* Colokkan kabel LAN dari port **Ether2** (atau port selain Ether1 yang biasanya dipakai untuk internet/WAN) di router MikroTik ke port LAN di Laptop/PC Anda.
* (Opsional) Jika menggunakan konfigurasi *default* pabrik, pastikan pengaturan IP Address di laptop Anda diset ke **Obtain an IP address automatically (DHCP)**.

### 2. Buka Aplikasi WinBox
* Double-click pada file aplikasi `winbox.exe` yang sudah Anda download.

### 3. Pilih Tab "Neighbors" (Tetangga Jaringan)
* Di jendela utama WinBox, klik tab **Neighbors** di bagian bawah/samping untuk mendeteksi perangkat MikroTik yang terhubung secara fisik dalam satu jaringan lokal.
* WinBox akan memindai dan menampilkan informasi router berupa:
  * **MAC Address** (Disarankan digunakan untuk login pertama kali jika IP belum diset).
  * **IP Address** (Biasanya default `192.168.88.1`).
  * **Identity** (Nama router, default: `MikroTik`).
  * **Board hingga Version**.

### 4. Masukkan Kredensial Login (Default)
Klik pada **MAC Address** atau **IP Address** yang muncul pada daftar *Neighbors* tersebut, lalu isi kolom login:
* **Connect To:** *(Terisi otomatis saat Anda klik MAC/IP di tab Neighbors)*
* **Login:** `admin` *(Default pabrik MikroTik)*
* **Password:** *(Kosongkan saja untuk router baru/default pabrik, atau masukkan password Anda jika sudah pernah diubah)*

> 💡 **Catatan Penting:** Jika Anda terhubung menggunakan IP Address, pastikan IP laptop Anda satu segmen dengan router (Contoh: IP Router `192.168.88.1`, maka IP Laptop bisa `192.168.88.2`). Jika bingung, gunakan **MAC Address** untuk koneksi yang lebih aman tanpa pusing memikirkan IP.

### 5. Tombol Connect
* Klik tombol **Connect** di bagian kanan bawah.
* Jika berhasil, jendela baru dashboard **RouterOS** (WinBox GUI) akan terbuka, dan Anda siap melakukan konfigurasi jaringan!

---

## ⚠️ Troubleshooting (Kendala Umum)
* **MikroTik tidak muncul di Neighbors?** 
  * Cek kembali fisik kabel LAN (pastikan lampu indikator port menyala).
  * Matikan sementara (Disable) *Windows Defender Firewall* atau antivirus pihak ketiga yang terkadang memblokir *discovery broadcast* WinBox.
* **Muncul Error "RouterOS version mismatch"?**
  * Versi WinBox Anda terlalu lama atau terlalu baru dibandingkan versi sistem operasi router. Gunakan versi WinBox yang sesuai.
