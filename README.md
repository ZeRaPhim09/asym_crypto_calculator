<h1 align="center">🔐 Asymmetric Cryptography Suite</h1>

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Font__Awesome-528DD7?style=for-the-badge&logo=font-awesome&logoColor=white" alt="Font Awesome" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License" />
</p>

<p align="center">
  <strong>Sistem Terintegrasi Kalkulator Kriptografi Asimetris Interaktif — 100% Client-Side & Offline-First</strong>
</p>

---

## 📖 Tentang Proyek

**Asymmetric Cryptography Suite** adalah sebuah platform web terpadu yang menyatukan enam modul kalkulator kriptografi asimetris ke dalam satu ruang kerja (*workspace*) terpusat. Menggunakan pendekatan arsitektur mirip *Single Page Application* (SPA) dengan injeksi `iframe`, aplikasi ini membundel berbagai alat kalkulasi algoritma rumit tanpa menimbulkan konflik penamaan fungsi pada JavaScript induk.

Antarmuka dirancang dengan gaya **Modern SaaS Dark Mode** yang bersih, dilengkapi dengan *collapsible sidebar* yang interaktif, serta implementasi sistem persistensi data berbasis *state-retention* yang tangguh.

---

## ✨ Fitur Unggulan

* 🗂️ **Dasbor Terintegrasi:** Menyatukan 6 modul kalkulator kriptografi independen dalam satu halaman navigasi yang mulus.
* 🔄 **State Retention (Anti-Loss):** Berkat integrasi `localStorage`, aplikasi akan secara otomatis mengingat dan memuat kembali modul kalkulator terakhir yang Anda buka, bahkan setelah halaman di-*refresh*.
* 🎛️ **Collapsible Sidebar:** Menu navigasi samping dapat dibuka-tutup melalui tombol *toggle* mengambang di pojok kiri atas untuk memberikan ruang kalkulasi yang lebih luas.
* ⚡ **BigInt Engine Processing:** Mampu memproses perhitungan bilangan bulat raksasa secara akurat langsung di memori *browser* tanpa ketergantungan pada server pihak ketiga.
* 📱 **Desain Responsif:** Layout dasbor adaptif dan fleksibel saat diakses melalui perangkat komputer maupun layar ponsel cerdas.

---

## 🧩 Modul & Algoritma yang Tersedia

Sistem ini terbagi ke dalam tiga kelompok arsitektur utama:

### 1. Modul Rivest-Shamir-Adleman (RSA)
* **RSA Keygen (`rsa_keygen.html`):** Demonstrasi proses pencarian nilai parameter kunci dari faktorisasi bilangan modulus $n$ menjadi faktor prima $p$ dan $q$, visualisasi fungsi Totient Euler $\phi(n)$, uji relatif prima eksponen publik $e$, hingga penemuan invers modular eksponen privat $d$ menggunakan *Extended Euclidean Algorithm*.
* **RSA Calculator (`rsa_main_cal.html`):** Eksekusi proses enkripsi pesan teks/angka menjadi *ciphertext* ($c = m^e \pmod n$) serta fungsi dekripsi dengan fitur pembagian ukuran blok (*block-sizing computation*).

### 2. Modul Rabin Cryptosystem
* **Rabin Crypto (`rabin_main.html`):** Implementasi algoritma enkripsi asimetris berbasis kuadratik ($c = m^2 \pmod n$) dan proses dekripsi sisa sisa tiongkok (*Chinese Remainder Theorem* - CRT) untuk mengekstrak 4 kandidat akar kuadrat akar murni disertai sistem penyaringan redundansi bit (*tail replication filter*).

### 3. Modul ElGamal & Diffie-Hellman Exchange
* **Diffie-Hellman (`diffie_hellman.html`):** Simulasi interaktif kesepakatan kunci rahasia bersama (*Shared Secret Key*) antara dua pihak melalui saluran tidak aman, dilengkapi visualisasi kalkulasi logaritma diskrit.
* **ElGamal Toolkit (`el_gamal_main.html`):** Pembangkitan pasang kunci, kalkulasi parameter enkripsi komponen sepasang $\gamma$ dan $\delta$, serta pemulihan pesan teks menggunakan pembuktian teorema Fermat kecil.
* **Z\*p Generator (`zp_el_gamal.html`):** Pencari elemen pembangun grup (*primitive root/generator*) menggunakan metode faktorisasi eksponen pengujian berulang.

---

## 📂 Struktur Direktori Repositori

Untuk memastikan fungsionalitas tautan navigasi dasbor bekerja dengan sempurna, seluruh file modul harus berada dalam satu direktori tingkat yang sama sebagai berikut:

```text
📁 crypto-suite
├── 📄 index.html             # Dasbor Utama (Sistem Navigasi & Sidebar Toggle)
├── 📄 rsa_keygen.html        # Modul Pembangkitan Kunci RSA
├── 📄 rsa_main_cal.html      # Modul Kalkulator Enkripsi/Dekripsi RSA
├── 📄 rabin_main.html        # Modul Sistem Kriptografi Rabin & CRT
├── 📄 diffie_hellman.html    # Modul Simulasi Pertukaran Kunci Diffie-Hellman
├── 📄 el_gamal_main.html     # Modul Toolkit Pemrosesan ElGamal
└── 📄 zp_el_gamal.html       # Modul Pencari Akar Primitif Grup Z*p
```

🚀 Panduan Instalasi & Penggunaan
Proyek ini dibangun murni menggunakan teknologi web native/vanilla tanpa memerlukan backend server (Node.js, PHP, dsb) atau instalasi package manager tambahan.

1. Kloning Repositori:

Bash
git clone [https://github.com/ZeRaPhim09/MyBread-Website.git](https://github.com/ZeRaPhim09/MyBread-Website.git)

2. Jalankan Aplikasi:

Cukup masuk ke folder hasil kloning, lalu klik ganda (double-click) pada file index.html untuk membukanya langsung di browser pilihan Anda.

Atau bagi pengguna VS Code, klik kanan pada file index.html lalu pilih "Open with Live Server" untuk mendapatkan pengalaman pengerjaan berkala yang lebih responsif.

👨‍💻 Pengembang
Dikembangkan oleh Zefanya Raditya Pratama.

"Terus mengoptimalkan kapasitas diri: merangkul perubahan, mengeksekusi ide, dan beradaptasi dengan setiap tantangan baru."

🔗 LinkedIn

📝 Medium

Dibuat untuk keperluan riset, eksperimen akademis, dan portofolio implementasi logika Rekayasa Perangkat Lunak Kripto.
