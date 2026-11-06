# SisaBaik Frontend - Chapter 9: Membangun Antarmuka dengan Vue

Modul pengembangan web untuk membangun antarmuka berbasis komponen menggunakan Vue 3, Composition API, pengelolaan *state*, *props*, *emits*, serta integrasi design system[cite: 54, 55].

## Fitur Utama
- **Single File Components (SFC):** Penyusunan antarmuka modular dengan blok `<script setup>`, `<template>`, dan `<style scoped>`[cite: 57].
- **Reaktivitas & State:** Penggunaan `ref` untuk reaktivitas data dan `computed` untuk data turunan (seperti filter katalog dan perhitungan unit tersedia)[cite: 57, 58].
- **Komponen Berkelanjutan:** Penggunaan komponen kartu penawaran (`KartuPenawaran.vue`), filter, dan formulir dengan validasi lokal[cite: 55, 59].
- **Aset Visual Lokal:** Pemanfaatan logo dan ilustrasi kategori berbasis SVG lokal tanpa ketergantungan CDN eksternal[cite: 56, 63].

## Persyaratan Perangkat
- Menggunakan **Node.js** versi 22.18.0 (atau yang lebih baru pada seri 22) / 24.12.0 ke atas[cite: 62].

## Cara Menjalankan Proyek Frontend
Masuk ke direktori frontend, lalu jalankan perintah berikut:
1. Install dependencies:
   ```bash
   npm install