1. Internet dan Koneksi Antar Router
Internet terhubung ke jaringan melalui tiga router yang berfungsi sebagai penghubung antara jaringan lokal (LAN) dan jaringan eksternal (internet).
Tiga router yang digunakan adalah R1 KHI, R2 KJ, dan R3 CR. Mereka masing-masing memiliki antarmuka dengan alamat IP yang berbeda:
R1 KHI: 192.168.20.1/24 dan 11.11.11.1/24.
R2 KJ: 192.168.10.1/24 dan 11.11.11.2/24.
R3 CR: 192.168.30.1/24 dan 12.12.12.1/24 serta 12.12.12.2/24.
2. Koneksi Antar Router
R1 KHI terhubung ke R2 KJ dan R3 CR menggunakan koneksi WAN atau jalur antar-router dengan alamat IP masing-masing di subnet yang berbeda.
R1 KHI memiliki koneksi ke R2 KJ di alamat IP 11.11.11.1/24 (R1) dan 11.11.11.2/24 (R2).
R1 KHI juga terhubung ke R3 CR melalui alamat IP 12.12.12.1/24 (R1) dan 12.12.12.2/24 (R3).
3. Koneksi Router ke Switch
Setiap router (R1 KHI, R2 KJ, dan R3 CR) terhubung ke switch yang mendistribusikan koneksi ke perangkat komputer yang ada di jaringan lokal (LAN).
Misalnya, R1 KHI terhubung ke Switch di subnet 192.168.11.1/24, R2 KJ terhubung ke Switch di subnet 192.168.21.1/24, dan R3 CR terhubung ke Switch di subnet 192.168.26.1/24.
4. Distribusi IP ke Komputer
Dari setiap switch, terdapat beberapa komputer yang diberikan alamat IP statis atau dinamis di masing-masing subnet:
Switch 1 (terhubung dengan R1 KHI) menghubungkan komputer-komputer dengan IP seperti 192.168.11.1/24, 192.168.13.1/24, dan 192.168.12.1/24.
Switch 2 (terhubung dengan R2 KJ) menghubungkan komputer-komputer dengan IP seperti 192.168.21.1/24, 192.168.22.1/24, dan 192.168.23.1/24.
Switch 3 (terhubung dengan R3 CR) menghubungkan komputer-komputer dengan IP seperti 192.168.31.1/24, 192.168.32.1/24, dan 192.168.33.1/24.
5. Pengaturan Subnet
Setiap segmen jaringan LAN memiliki subnet yang berbeda, yaitu:
R1 KHI di subnet 192.168.11.0/24.
R2 KJ di subnet 192.168.21.0/24.
R3 CR di subnet 192.168.26.0/24.
Subnet ini digunakan untuk memisahkan trafik jaringan dan mengelompokkan perangkat yang memiliki tujuan komunikasi yang sama.
6. Alur Data dalam Jaringan
Ketika sebuah perangkat (misalnya, komputer) ingin berkomunikasi dengan perangkat lain di jaringan yang berbeda, paket data akan melewati switch, router, dan antar-router, serta keluar menuju Internet jika diperlukan.
Routing pada setiap router memastikan paket data dikirimkan ke subnet yang tepat menggunakan protokol routing yang sesuai, seperti RIP atau OSPF.
7. Deskripsi IP dan Koneksi
Di gambar ini, setiap koneksi antar perangkat dan alamat IP ditunjukkan untuk memudahkan pemahaman mengenai alur komunikasi data dalam jaringan. Setiap router dan switch memiliki alamat IP yang berbeda pada interface yang terhubung ke subnet LAN dan WAN.
8. Kesimpulan
Gambar ini menunjukkan topologi jaringan berbasis router dan switch yang menyediakan akses ke internet untuk beberapa perangkat yang terhubung di beberapa subnet berbeda.
Koneksi antar router memungkinkan komunikasi antar jaringan lokal yang terpisah, serta distribusi data ke perangkat komputer melalui switch.