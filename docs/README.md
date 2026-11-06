# SisaBaik API - Chapter 8: Autentikasi dan Otorisasi

Modul pengembangan web untuk penerapan autentikasi, otorisasi berbasis peran (RBAC), keamanan dasar aplikasi web, serta pengelolaan rahasia melalui environment variables.

## Fitur Utama
- **Autentikasi & Hashing:** Pendaftaran mandiri dengan hashing kata sandi menggunakan `bcryptjs` dan token berbasis `JWT` (JSON Web Token).
- **Otorisasi Berbasis Peran (RBAC):** Pembatasan hak akses antara *Pengunjung*, *Pembeli*, dan *Penyedia* (dengan status verifikasi usaha).
- **Kepemilikan Data:** Pengamanan mutasi penawaran dan akses pesanan agar hanya dapat diakses oleh pemilik yang sah.
- **Manajemen Sesi:** Mekanisme *logout* universal dengan pencabutan versi token (`versi_token`).

## Migrasi Database
Chapter 8 menambahkan migrasi baru pada tabel `pengguna`:
- `database/07_auth.sql` (menambahkan kolom `kata_sandi_hash` dan `versi_token`).

## Konfigurasi Environment (`.env`)
Salin file `.env.example` menjadi `.env` dan sesuaikan konfigurasi berikut:
- Konfigurasi database PostgreSQL (`PGHOST`, `PGPORT`, `PGDATABASE`, `PGUSER`, `PGPASSWORD`)
- `JWT_SECRET` (wajib 64 digit hex acak yang dihasilkan melalui `crypto.randomBytes`)

## Cara Menjalankan Proyek
1. Install dependencies:
   ```bash
   npm install