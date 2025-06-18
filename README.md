# 📚 Sistem Perwalian

Proyek ini merupakan aplikasi berbasis Laravel yang menyediakan fitur **CRUD (Create, Read, Update, Delete)** untuk entitas **Mahasiswa** dan **Dosen Wali**. Data mahasiswa diambil dari **API eksternal**, dan pengguna aplikasi dibatasi hanya untuk dua peran: **Mahasiswa** dan **Dosen Wali**.

---
## Link Backend ##
🔗 **Repositori Backend:** (https://github.com/abdau88/uas_pbf_soal_A.git)

---


## ⚙️ Teknologi yang Digunakan

- [Laravel](https://laravel.com/) - Framework PHP yang digunakan untuk membangun aplikasi web secara lebih cepat, rapi, dan terstruktur.
  - Mengatur Struktur Kode (MVC):
    - Model: Mengelola data dan database  
    - View: Tampilan antarmuka pengguna (HTML, Blade)  
    - Controller: Mengatur alur logika aplikasi  
- RESTful API - Untuk sumber data eksternal
- MySQL - Sebagai database lokal

---

## 🗃️ Database
query database :

```bash
CREATE DATABASE db_rumahsakit_23102043;
USE db_rumahsakit_230102043;

CREATE TABLE pasien (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nama VARCHAR(100),
  alamat TEXT,
  tanggal_lahir DATE,
  jenis_kelamin ENUM('L', 'P')
);

CREATE TABLE obat (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nama_obat VARCHAR(100),
  kategori VARCHAR(50),
  stok INT,
  harga DECIMAL(10,2)
);
```

---

## 🖥️ Setup Backend (CodeIgniter)

### 1. Clone Repo Backend
```bash
git clone https://github.com/abdau88/uas_pbf_soal_A.git
```

### 2. Install Dependency CodeIgniter
```bash
composer install
```

### 3. Menjalankan CodeIgniter
```bash
php spark serve
```
### 4. Cek Endpoint


## 🖥️ Setup Frontend (Laravel)

### 1. Melalui terminal/cmd
```bash
composer create-project laravel/laravel FRONTEND-UAS-23010243 ^10
```

### 2. Melalui Laragon
- Buka Laragon
- Klik kanan Quick app
- Laravel

### 3. Install Dependency Laravel
```bash
Composer install
```

### 4. Menjalankan Laravel
```bash
php artisan serve
```

# 📅 Tahapan Pembuatan Frontend

## Controller
```bash
php artisan make:controller PasienController / php artisan make:model Pasien -mcr
```

