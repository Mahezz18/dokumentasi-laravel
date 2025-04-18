# Panduan Instalasi Laravel di Windows

----

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

Contoh output: PHP 8.1.10 (cli) (built: Aug  1 2022 20:17:19)

```

### ✅ 4. Instal Composer

- Unduh Composer dari [https://getcomposer.org](https://getcomposer.org)
  
- Instal seperti biasa (pastikan memilih path PHP dari Laragon saat instalasi)

Contoh path PHP jika menggunakan laragon:

```
C:\laragon\bin\php\php-8.1.10-Win32-vs16-x64\php.exe
```

- Cek instalasi Composer, buka terminal lalu jalankan perintah :

```bash
composer -V
```

Contoh output:

```
Composer version 2.x.x
```



### ✅ 5. Atur PATH PHP (Jika Diperlukan)

Jika `php -v` tidak berfungsi atau menunjukkan versi yang salah:

- klik **windows + s**
- Ketik **environment variabel** buka lalu buka **environment variabel**



- Klik **Path** terlebih dahulu lalu klik **edit**


- Klik **new**

- Tambahkan path PHP dari Laragon ke variabel lingkungan (menyesuaikan dengan path dan versi php yang kalian miliki):

  ```
  C:\laragon\bin\php\php-8.1.10-Win32-vs16-x64\
  ```


- Klik **ok** pada semua jendela environment variabel sampai semuanya terutup kembali

- Restart Command Prompt lalu jalankan

  ```
  php -v
  ```

### ✅ 6. Buat Proyek Laravel Baru

```bash
composer create-project laravel/laravel nama-proyek
```

Contoh:

```bash
composer create-project laravel/laravel kuliah-framework
```


- Klik **Enter** lalu tunggu sampai selesai

### ✅ 7. Jalankan Server Laravel

- Buka folder laravel yang kita download tadi menggunakan code editor
- klik **"ctrl" + " ` "** untuk membuka terminal di vscode

Jalankan perintah ini di terminal

```bash
php artisan serve
```



Buka browser dan akses:

```
http://127.0.0.1:8000
```



Jika halaman welcome Laravel muncul, maka instalasi berhasil ✅

---

## 🔍 Catatan Tambahan

- Pastikan ekstensi berikut aktif di file `php.ini`:
  ```ini
  extension=openssl
  extension=curl
  extension=zip
  ```
- Caranya buka file **php.ini**

contoh lokasi file **php.ini**

```
C:\laragon\bin\php\php-8.1.10-Win32-vs16-x64\php.ini
```

- Atau lebih mudah bisa mencari file **php.ini** dengan membuka laragon klik menu, klik php, dan klik php.ini


```
;extension=openssl
;extension=curl
;extension=zip
```

- klik **"ctrl" + "f"** untuk mencari ketiga ekstensi terbut
- hapus **";"** pada 3 ekstensi tersebut lalu save dan close


- `php artisan` adalah antarmuka command line Laravel
- Folder `vendor/` berisi semua paket yang diinstal melalui Composer

---

## ✅ Selesai!

Sekarang Laravel sudah berhasil diinstal dan siap digunakan di komputer lokal menggunakan Laragon.
