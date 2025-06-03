# Info Sistem Web Lengkap

Website sederhana untuk menampilkan informasi lengkap mengenai browser, perangkat keras, jaringan, kondisi, dan sensor (seperti orientasi perangkat) dari sisi klien secara *real-time*. Dibangun dengan HTML, Tailwind CSS, dan JavaScript murni.

![Pratinjau Aplikasi (Ganti dengan screenshot aplikasi Anda jika ada)](https://i.imgur.com/yMtnjve.png)
*(Saran: Ambil screenshot halaman web Anda dan unggah ke repositori atau layanan hosting gambar, lalu ganti URL_SCREENSHOT_ANDA_DI_SINI dengan URL gambar tersebut)*

## ✨ Fitur Utama

Halaman web ini dapat mendeteksi dan menampilkan:

* **Informasi Browser:**
    * User Agent
    * Nama Kode Aplikasi, Nama Aplikasi, Versi Aplikasi
    * Platform Sistem Operasi
    * Bahasa Browser
    * Status Cookies & Java (legacy)
    * Status Online/Offline
* **Informasi Perangkat:**
    * Resolusi Layar (lebar, tinggi, lebar & tinggi tersedia)
    * Kedalaman Warna & Pixel
    * Orientasi Layar (potret/lanskap)
    * Dukungan Sentuh & Jumlah Maksimum Titik Sentuh
    * Estimasi Jumlah Inti CPU (Logis)
    * Estimasi Memori Perangkat (RAM)
* **Informasi Jaringan (dari sisi klien):**
    * URL Saat Ini, Hostname, Pathname, Protokol
    * Alamat IP Publik Pengguna (menggunakan layanan eksternal `api.ipify.org`)
    * Tipe Koneksi Efektif (jika didukung API)
    * Estimasi Kecepatan Download & RTT (jika didukung API)
    * Status Mode Hemat Data
* **Informasi Kondisi:**
    * Status Baterai (level, status pengisian, estimasi waktu)
    * Preferensi Mode Gelap Sistem Pengguna
    * Zona Waktu Pengguna
* **Informasi Sensor "Sudut" (Orientasi Perangkat):**
    * Dukungan `DeviceOrientationEvent`
    * Nilai Alpha (rotasi sumbu Z)
    * Nilai Beta (rotasi sumbu X)
    * Nilai Gamma (rotasi sumbu Y)
    * Status Orientasi Absolut
    *(Membutuhkan izin pengguna dan dukungan sensor dari perangkat)*

## 🛠️ Teknologi yang Digunakan

* **HTML5:** Struktur dasar halaman web.
* **Tailwind CSS:** Framework CSS utility-first untuk styling cepat dan responsif.
* **JavaScript (ES6+):** Untuk mengambil data, memanipulasi DOM, dan interaktivitas.
* **Font:** Google Fonts (Inter).
* **API Browser:** `navigator`, `screen`, `window.location`, `navigator.connection`, `navigator.getBattery()`, `window.matchMedia`, `DeviceOrientationEvent`, `Intl.DateTimeFormat`.
* **Layanan Eksternal:** `https://api.ipify.org` untuk mendapatkan alamat IP publik.

## 🚀 Cara Menggunakan

1.  **Clone repositori ini:**
    ```bash
    git clone [https://github.com/xr-wahyuu/Info-Sistem-Web.git](https://github.com/xr-wahyuu/Info-Sistem-Web.git)
    ```
2.  **Masuk ke direktori proyek:**
    ```bash
    cd info-sistem-web
    ```
3.  **Buka file HTML utama** (misalnya `index.html` atau nama file HTML yang Anda gunakan) di browser web favorit Anda.

Tidak ada langkah build atau dependensi server yang diperlukan, karena ini adalah proyek frontend murni.

## 🔧 Kustomisasi & Pengembangan Lanjutan

* **Mengubah Tampilan:** Anda dapat dengan mudah mengubah gaya dengan memodifikasi kelas Tailwind CSS langsung di HTML atau menambahkan CSS kustom di dalam tag `<style>` atau file CSS terpisah.
* **Menambah Fitur:** Eksplorasi lebih banyak Browser API untuk menambahkan informasi lain yang mungkin berguna.
* **Izin Sensor:** Perhatikan bahwa beberapa fitur seperti orientasi perangkat dan status baterai mungkin memerlukan izin eksplisit dari pengguna atau hanya berfungsi pada koneksi HTTPS di beberapa browser.

## 🤝 Berkontribusi

Kontribusi selalu diterima! Jika Anda memiliki ide untuk perbaikan atau fitur baru, silakan:
1.  Fork repositori ini.
2.  Buat branch fitur baru (`git checkout -b fitur/NamaFiturBaru`).
3.  Commit perubahan Anda (`git commit -m 'Menambahkan fitur X'`).
4.  Push ke branch (`git push origin fitur/NamaFiturBaru`).
5.  Buat Pull Request baru.

## 📄 Lisensi

Proyek ini dilisensikan di bawah [Lisensi MIT](LICENSE.md).

---

Dibuat dengan ❤️ dan secangkir kopi.
