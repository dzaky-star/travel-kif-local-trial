# Travel KIF — Percobaan Lokal Windows

Paket percobaan untuk Pak Artha. Database berjalan di laptop sendiri, terpisah dari quotation online. Repository ini berisi ZIP source code dan installer lokal, bukan website yang langsung berjalan di GitHub.

## Mulai

1. Instal **Node.js LTS** dari https://nodejs.org/en/download (minimum 22.13).
2. Buka [Travel-KIF-Local-Windows.zip](./Travel-KIF-Local-Windows.zip), lalu klik **Download raw file** (ikon unduh).
3. Klik kanan ZIP di Windows → **Extract All**.
4. Buka folder hasil extract, jalankan **1-INSTALL.cmd**, dan tunggu selesai. Instalasi awal membutuhkan internet.
5. Buka **AKSES-LOKAL.txt** yang dibuat setelah instalasi untuk username/password percobaan.
6. Jalankan **2-JALANKAN.cmd**. Buka http://127.0.0.1:8787 lalu login.

Untuk penggunaan berikutnya cukup jalankan **2-JALANKAN.cmd**. Biarkan jendela server terbuka selama menggunakan aplikasi; tekan Ctrl+C untuk menutup. Data tetap tersimpan di folder `local-data`.

## Isi paket

- Dua quotation contoh, bukan data pelanggan asli.
- Akun percobaan Admin, TC, OPS, Artha (Manager), dan Finance. Login Admin untuk pindah profil.
- Quotation, perhitungan, approval TC → OPS → Manager, diskusi, dan PDF berjalan lokal.
- Tidak memakai kuota D1 produksi dan tidak menyinkronkan perubahan ke tim.
- Email, Google Sheets, dan pembaruan kurs otomatis dinonaktifkan. Kurs awal hanya contoh.
- AI opsional memakai Gemini/Tavily melalui internet; API key tidak disertakan. Lihat `BACA-DULU.txt` untuk pengaturan.

## Catatan

Target **Windows 11 x64**. Runtime lokal dan alur aplikasi sudah diuji di macOS; file `.cmd` belum dijalankan langsung di Windows. AI sungguhan belum diuji karena tidak ada key.

Jangan unggah `local-data`, `.dev.vars`, `AKSES-LOKAL.txt`, atau `node_modules` setelah menjalankan paket. Tidak perlu akun Cloudflare atau pembayaran untuk mencoba paket lokal ini.
