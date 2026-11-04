# Laravel

[Laravel](https://laravel.com/) adalah kerangka kerja (*framework*) aplikasi web berbasis PHP yang dirancang untuk membuat proses pengembangan web menjadi lebih cepat, elegan, dan terstruktur. Alih-alih membangun semuanya dari nol (seperti *routing*, pengaturan *file*, dan keamanan), Laravel telah menyediakan fondasi tersebut sehingga pengembang dapat langsung fokus pada logika bisnis (kebutuhan aplikasi).

---

Pola arsitektur **MVC (Model-View-Controller)**:
*   **Model:** Bagian yang merepresentasikan struktur data dan aturan bisnis (pada tahap ini kita belum menggunakan *database*, melainkan menggunakan *array* statis).
*   **View:** Bagian yang mengatur tampilan antarmuka (UI) yang dilihat pengguna, menggunakan *template engine* bawaan Laravel yaitu **Blade**.
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

Akan ada halaman yang meminta lokasi file PHP. 

Pastikan lokasinya mengarah ke C:\xampp\php\php.exe.

Klik Next terus sampai Install, lalu Finish.

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
