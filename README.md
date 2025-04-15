# 📘 Panduan Instalasi Laravel (Windows)

## 📌 Apa itu Laravel?

Laravel adalah salah satu framework PHP paling populer dan powerful yang digunakan untuk membangun aplikasi web modern secara cepat, elegan, dan efisien. Dibangun dengan prinsip MVC (Model-View-Controller), Laravel menyediakan berbagai fitur bawaan seperti routing, sistem autentikasi, manajemen database dengan Eloquent ORM, templating dengan Blade, sistem migrasi, serta Artisan CLI yang mempermudah pengembangan.

Laravel juga didukung oleh ekosistem yang luas seperti Laravel Mix, Sanctum, dan Jetstream, serta komunitas yang aktif, sehingga sangat ideal untuk proyek skala kecil hingga besar.

---

## 🔧 Kebutuhan Instalasi

| Alat                   | Kegunaan                                                                      |
| ---------------------- | ----------------------------------------------------------------------------- |
| **Visual Studio Code** | Code editor yang digunakan untuk menjalankan Laravel                          |
| **PHP**                | Bahasa pemrograman utama yang digunakan Laravel                               |
| **Composer**           | Manajer dependensi untuk PHP, digunakan untuk menginstal Laravel dan paketnya |
| **Laragon**            | Lingkungan server lokal ringan yang sudah termasuk PHP, MySQL, dll            |
| **Git** _(opsional)_   | Sistem kontrol versi, sering dibutuhkan oleh Composer saat mengunduh paket    |

---

## 🧱 Langkah-langkah Instalasi

### ✅ 1. Instal VSCode

- Unduh VSCode dari [https://code.visualstudio.com/download](https://code.visualstudio.com/download)
- Ikuti proses instalasi, jalankan aplikasi

### ✅ 2. Instal Laragon

- Unduh dari [https://laragon.org/download/](https://laragon.org/download/)
- Jalankan installer, pilih pengaturan default, klik **Install**
- Setelah selesai, klik **Start All** di aplikasi Laragon

### ✅ 3. Cek Instalasi PHP

Buka **Command Prompt** lalu ketik:

```bash
php -v
