## 📖 Deskripsi Proyek

**Crypto Suite** adalah sebuah perkakas (*toolkit*) kriptografi asimetris yang dirancang khusus untuk kebutuhan edukasi, eksperimen, dan rekayasa kriptografi. Aplikasi ini mengintegrasikan berbagai algoritma enkripsi publik ke dalam satu *dashboard* antarmuka (*Modern Dark Mode*) yang intuitif.

Dibangun dengan arsitektur menyerupai *Single Page Application* (SPA) menggunakan metode injeksi `iframe`, seluruh modul berjalan secara independen namun tetap terpusat dalam satu ruang kerja (*workspace*).

**Modul yang Tersedia:**
* **RSA System:** Pembangkitan kunci (Faktorisasi prima, Euclidean) & Kalkulator Enkripsi/Dekripsi.
* **Rabin Cryptography:** Enkripsi kunci publik dengan ekstraksi akar kuadrat modulo menggunakan Teorema Sisa Tiongkok (CRT).
* **Diffie-Hellman:** Simulasi pertukaran kunci rahasia (*Key Exchange*) dan pencarian Logaritma Diskrit.
* **ElGamal Toolkit:** Kalkulasi lengkap mulai dari enkripsi, dekripsi, hingga Pembangkitan Generator $Z^*_p$ (Akar Primitif).

Keunggulan utama dari *suite* ini adalah **100% Client-Side Processing**. Semua kalkulasi matematis raksasa (menggunakan *BigInt Engine* bawaan JavaScript) dieksekusi langsung di memori *browser* pengguna, sehingga dijamin aman, cepat, dan sepenuhnya *offline*.

---

## ⚙️ Konfigurasi & Instalasi

Karena proyek ini dibangun murni menggunakan **Vanilla HTML, CSS, dan JavaScript**, tidak ada dependensi eksternal, *package manager* (seperti npm), atau *server backend* yang perlu dikonfigurasi.

### Persyaratan Sistem
* *Web Browser* modern (Chrome, Firefox, Safari, atau Edge) yang mendukung fitur `BigInt` JavaScript.
* (Opsional) Ekstensi *Live Server* di VS Code untuk pengalaman pengembangan yang lebih baik.

### Langkah-langkah Menjalankan Aplikasi
1. **Kloning Repositori:**
   Buka terminal Anda dan jalankan perintah berikut:
   ```bash
   git clone [https://github.com/ZeRaPhim09/crypto-suite.git](https://github.com/ZeRaPhim09/crypto-suite.git)

   Buka Direktori:
Masuk ke dalam folder hasil kloning:

Bash
cd crypto-suite
Jalankan Aplikasi:
Tidak perlu kompilasi. Anda cukup membuka file index.html langsung ke dalam browser Anda:

Windows/Linux: Klik ganda (double-click) pada file index.html.

Mac: Ketik open index.html di terminal.

VS Code: Klik kanan pada index.html dan pilih "Open with Live Server".

⚠️ Catatan Struktur Direktori
Agar navigasi sidebar berfungsi dengan benar, pastikan file induk (index.html) berada di dalam folder (direktori) yang persis sama dengan file-file modul kalkulatornya:

rsa_keygen.html

rsa_main_cal.html

rabin_main.html

diffie_hellman.html

el_gamal_main.html

zp_el_gamal.html


Dengan format di atas, siapa pun yang mengunjungi repositori Anda akan langsung mengerti bahwa proyek ini sangat kompleks secara matematis, namun sangat mudah dan ringan untuk di- *deploy*.
