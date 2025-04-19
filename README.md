# Aplikasi Desktop Audit Barang

Aplikasi desktop berbasis **Tauri** yang digunakan untuk melakukan auditisasi barang. Aplikasi ini menggunakan **Next.js** untuk frontend dan **SQLite** untuk penyimpanan data lokal. Dengan aplikasi ini, pengguna dapat mengelola data audit barang dengan mudah melalui antarmuka grafis yang sederhana namun efektif.

## Fitur

- **Input Data Barang**: Menambah data barang yang diaudit.
- **Daftar Barang**: Melihat dan mengelola daftar barang yang telah diaudit.
- **Penyimpanan Lokal**: Menggunakan SQLite untuk menyimpan data secara lokal pada perangkat.

## Teknologi yang Digunakan

- **Tauri**: Untuk membuat aplikasi desktop menggunakan teknologi web.
- **Next.js**: Framework React untuk membangun antarmuka pengguna (UI).
- **SQLite**: Database lokal untuk menyimpan data audit barang.
- **Rust**: Digunakan pada backend untuk memanipulasi data dan menjalankan aplikasi Tauri.

## Persyaratan

Sebelum memulai, pastikan bahwa Anda memiliki alat berikut:

- **Node.js** (Versi 16.x atau lebih baru)
- **Rust** (Versi 1.58 atau lebih baru)
- **SQLite** (SQLite database sudah disertakan di dalam aplikasi)

## Instalasi

### 1. Clone Repositori
Clone repositori ini ke mesin lokal Anda:

```bash
git clone https://github.com/username/audit-app.git
cd demsare-audit
```

### 2. Instal Dependensi Frontend (Next.js)
Masuk ke direktori frontend dan instal dependensinya:

```bash
cd frontend
npm install
```

### 3. Instal Dependensi Backend (Tauri)
Instal dependensi untuk backend Tauri:

```bash
cd src-tauri
cargo install
```

### 4. Menjalankan Aplikasi
Setelah semua dependensi terinstal, Anda dapat menjalankan aplikasi dengan perintah berikut:

```bash
npm run tauri dev
```

### Cara Kerja Aplikasi
Aplikasi ini mengelola data audit barang dengan frontend menggunakan Next.js dan backend menggunakan Rust/Tauri. Proses yang terjadi adalah:

1. Frontend: Menggunakan React dan Next.js untuk memberikan UI yang interaktif. Pengguna dapat memasukkan data barang dan melihat daftar barang yang telah diaudit.
2. Backend: Menggunakan Tauri dengan Rust untuk mengelola logika backend dan komunikasi dengan SQLite untuk menyimpan data barang secara lokal.
3. SQLite: Semua data barang disimpan di database SQLite lokal yang terintegrasi dengan aplikasi.
