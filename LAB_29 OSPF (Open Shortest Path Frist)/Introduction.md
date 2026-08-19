## OSPF (Open Shortest Path Frist) ##

OSPF adalah protokol routing dinamis yang secara otomatis mencari dan mengatur jalur terpendek (tercepat) menggunakan algoritma Dikjstra SPF
(Shortest Path Frist)
Berbeda dengan *Routing Statis* yang mengharuskan memasukan rute manual rute setu persatu.
OSPF Sangat efisien dalam mendeteksi perubahan topologi jaringan secara real-time.

**Cara Kerja OSPF**
1. Neighbor Discovery: Router mengirimkan paket Hello untuk menemukan router tetangga yang terhubung langsung di jaringan yang sama.
2. Link-State Database (LSDB): Router bertukar informasi status link (LSA) untuk menyamakan pandangan topologi jaringan di seluruh area.
3. Route Calculation: Setiap router menjalankan algoritma Dijkstra secara independen untuk menentukan rute optimal di dalam tabel routing.

---

Konfigurasi OSPF dari Mikrotik v6

<img width="900" height="572" alt="ospf topolgi" src="https://github.com/user-attachments/assets/be3bb37f-0720-4f3f-91f5-ddc769162cd7" />

## R1, R2 dan R3 kita setting terlebih dahulu

**R1**

a. buat ip address terlebih dahulu pada tab ip lalu addresses lalu masukan ip dan ethernet sesuai dengan topologi yang diberikan

<img width="629" height="379" alt="image" src="https://github.com/user-attachments/assets/cbe4155b-f50f-400f-8308-95f0ec51afc3" />


b. Pilih menu Routing, klik OSPF

<img width="257" height="145" alt="1" src="https://github.com/user-attachments/assets/31ae3e09-fa9e-4661-a379-056e553a0a39" />

c. Pada tab intances ganti konfigurasi instance biarkan jadi default dan masukan router id 1.1.1.1

<img width="1084" height="387" alt="2" src="https://github.com/user-attachments/assets/07fabbec-7232-4e6f-a7b6-6e36761d90be" />

d. Lalu pada tab Areas pastikan nama area dan area ID sudah aktif secara default

<img width="658" height="355" alt="3" src="https://github.com/user-attachments/assets/42a4dce8-154a-4df8-9d36-78d241b85edf" />

e. Pada tab Networks masukan alamat network yang terdapat pada router dengan Area backbone

<img width="662" height="354" alt="net" src="https://github.com/user-attachments/assets/b21755fa-cdf0-4eee-a0aa-b449ed27ecec" />

