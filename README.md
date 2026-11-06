# Laravel

[Laravel](https://laravel.com/) adalah sebuah *framework* aplikasi web berbasis PHP yang dirancang untuk membuat proses pengembangan web menjadi lebih cepat dan terstruktur. Alih-alih membangun semuanya dari nol (seperti *routing*, pengaturan *file*, dan keamanan), Laravel telah menyediakan fondasi tersebut sehingga pengembang dapat langsung fokus pada kebutuhan aplikasi.

---

Pola arsitektur **MVC (Model-View-Controller)**:
*   **Model:** Bagian yang merepresentasikan struktur data dan aturan aplikasi (pada tahap ini kita belum menggunakan *database*, melainkan menggunakan *array*).
*   **View:** Bagian yang mengatur *User Interface* yang dilihat oleh pengguna, menggunakan *template engine* bawaan Laravel yaitu **Blade**.
*   **Controller:** Bagian yang bertindak sebagai jembatan pengatur alur; menerima permintaan dari pengguna (*request* lewat *Route*), mengolah data, dan mengirimkannya ke *View*.

---

# System Requirements

1.  **PHP** (Minimal versi 8.3, disarankan 8.5) 
    *   *Disarankan menggunakan XAMPP versi terbaru:* [Unduh XAMPP](https://www.apachefriends.org/download.html)
2.  **Composer** (Minimal versi 2.x) - Manajer dependensi untuk PHP.
    *   [Unduh Composer](https://getcomposer.org/download/)
3.  **Visual Studio Code (VS Code)** - *Code editor* pilihan.
    *   [Unduh VS Code](https://code.visualstudio.com/)
4.  **Git** - Untuk sistem kontrol versi (*version control*).
    *   [Unduh Git](https://git-scm.com/downloads)

---

Tambahan seblum dijalankan 

**XAMPP**

Agar komputermu kenal perintah php : 

- tekan tombol Windows di keyboard
- ketik Environment Variables
- lalu pilih Edit the system environment variables
- Klik tombol Environment Variables... di kanan bawah
- Di kotak bagian bawah (System variables), cari tulisan Path, lalu klik dua kali (double click)
- Klik tombol New, lalu ketik: C:\xampp\php
- Klik OK di semua kotak sampai tertutup.

**Composer**

- Akan ada halaman yang meminta lokasi file PHP. 
- Pastikan lokasinya mengarah ke C:\xampp\php\php.exe.
- Klik Next terus sampai Install, lalu Finish.

---

# Praktek
1. Buka terminal (atau Git Bash/CMD) dan jalankan perintah berikut:
```bash
cd composer create-project laravel/laravel pbo-laravel
```

2. Arahkan terminal ke dalam folder proyek
```bash
cd pbo-laravel
```

3. Gunakan Composer untuk mengunduh semua inti *framework* Laravel dan *library* pendukungnya
```bash
composer install
```

4. Salin file konfigurasi bawaan agar proyek memiliki file `.env` sendiri:
```bash
cp .env.example .env
```

5. Ketik perintah berikut untuk memproduksi kunci keamanan baru
```bash
php artisan key:generate
```

6. Nyalakan mesin server *development* bawaan Laravel:
```bash
php artisan serve
```

Buka *browser* (Chrome/Edge/Firefox) dan ketikkan alamat berikut di kolom URL:
[http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

