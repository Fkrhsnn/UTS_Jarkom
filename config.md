# Topologi Jaringan

Topologi ini merupakan bagian dari tugas jaringan komunikasi lanjut (UTS) di Universitas Esa Unggul. Topologi ini terdiri dari beberapa router dan perangkat laptop yang terhubung dalam jaringan menggunakan protokol routing **RIP**.

## Struktur Topologi

Diagram jaringan terdiri dari beberapa komponen utama:

### 1. Router
Topologi ini menggunakan tiga router utama:
   - **Router R1 (KJ)**
   - **Router R2 (CR)**
   - **Router R3 (KHI)**

Setiap router memiliki beberapa antarmuka Ethernet dengan konfigurasi alamat IP yang berbeda untuk menghubungkan berbagai segmen jaringan.

### 2. Antarmuka dan Alamat IP
Berikut adalah konfigurasi IP pada setiap router:
   - **Router R1**:
     - **Eth 2**: 192.167.2.1/24
   - **Router R2**:
     - **Eth 4**: 22.22.22.1
     - **Eth 3**: 11.11.11.2
   - **Router R3**:
     - **Eth 3**: 33.33.33.2
     - **Eth 4**: 12.12.12.1

Setiap antarmuka terhubung ke subnet berbeda, memungkinkan komunikasi antar perangkat dalam jaringan secara terpisah.

### 3. Protokol Routing - RIP
Protokol **RIP (Routing Information Protocol)** digunakan untuk mengelola rute di dalam jaringan ini. RIP membantu setiap router untuk mengetahui rute terbaik berdasarkan jumlah "hop" atau lompatan antara jaringan.

### 4. Koneksi Perangkat Laptop
Diagram menunjukkan beberapa perangkat laptop yang terhubung ke router melalui alamat IP **192.167.2.1/24**. Ini menunjukkan adanya segmentasi jaringan yang memastikan perangkat laptop dapat saling terhubung melalui subnet yang ditentukan.

## Tujuan Topologi
Topologi ini dirancang untuk:
- Mengelola lalu lintas antar-segmen jaringan menggunakan protokol RIP.
- Menghubungkan perangkat pada subnet berbeda, sehingga komunikasi dalam jaringan tetap efisien.

---

**Disusun oleh:**
- **Nama**: Muhamas Fikri
- **NIM**: 20210801098
- **Mata Kuliah**: Jaringan Komunikasi Lanjut
