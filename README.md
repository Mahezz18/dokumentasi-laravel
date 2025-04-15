# Panduan Instalasi Laravel di Windows

## 📚 Daftar Isi
- [Pengenalan Laravel](#-apa-itu-laravel)
- [Persyaratan Sistem](#-persyaratan-sistem)
- [Langkah Instalasi](#-langkah-instalasi)
  - [1. Instal Visual Studio Code](#-1-instal-visual-studio-code)
  - [2. Instal Laragon](#-2-instal-laragon)
  - [3. Verifikasi Instalasi PHP](#-3-verifikasi-instalasi-php)
  - [4. Instal Composer](#-4-instal-composer)
  - [5. Konfigurasi PATH PHP (Opsional)](#-5-konfigurasi-path-php-opsional)
  - [6. Membuat Proyek Laravel](#-6-membuat-proyek-laravel)
  - [7. Menjalankan Server Development](#-7-menjalankan-server-development)
- [Konfigurasi Tambahan](#-konfigurasi-tambahan)
- [Troubleshooting](#-troubleshooting)

---

## 🚀 Apa itu Laravel?
Laravel adalah framework PHP open-source yang menggunakan arsitektur MVC (Model-View-Controller). Fitur utamanya meliputi:
- **Eloquent ORM** untuk manajemen database
- **Blade Templating Engine**
- **Artisan CLI** untuk otomatisasi tugas
- Sistem autentikasi bawaan
- Dukungan komunitas yang besar

---

## 🔧 Persyaratan Sistem
| Komponen         | Deskripsi                                                                 | Unduhan                                    |
|------------------|---------------------------------------------------------------------------|--------------------------------------------|
| **PHP**          | Versi 8.0.2 atau lebih baru                                              | Termasuk dalam Laragon                    |
| **Composer**     | Dependency Manager untuk PHP                                             | [Download Composer](https://getcomposer.org) |
| **Laragon**      | Server lokal (Termasuk Apache, MySQL, PHP)                               | [Download Laragon](https://laragon.org)   |
| **VSCode**       | Editor kode yang direkomendasikan                                        | [Download VSCode](https://code.visualstudio.com) |
| **Git**          | Opsional, untuk version control                                          | [Download Git](https://git-scm.com)       |

---

## 🛠 Langkah Instalasi

### 📥 1. Instal Visual Studio Code
1. Kunjungi [situs resmi VSCode](https://code.visualstudio.com).
2. Pilih versi **Windows** dan unduh installer.
3. Jalankan file `.exe` yang telah diunduh.
4. Ikuti panduan instalasi dengan pengaturan default.
5. Buka VSCode setelah instalasi selesai.

---

### 🖥 2. Instal Laragon
1. Unduh Laragon versi terbaru dari [laragon.org](https://laragon.org).
2. Jalankan file `laragon-wamp.exe`.
3. Pilih bahasa **English** dan ikuti langkah instalasi:
   - Pilih direktori instalasi (default: `C:\laragon`).
   - Centang opsi **Create Desktop Shortcut**.
4. Setelah instalasi, buka Laragon dan klik **Start All** untuk mengaktifkan server.

---

### 🔍 3. Verifikasi Instalasi PHP
Buka Command Prompt/PowerShell dan jalankan:
```bash
php -v
