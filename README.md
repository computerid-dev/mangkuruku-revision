# MANGKURUKU v1.2.0
Aplikasi PWA manajemen bimbel. Data tersimpan LOKAL di perangkat (localStorage), tanpa server.
## Menjalankan
- Lokal: `npx serve .` atau `python3 -m http.server 8080`, buka http://localhost:8080
- Deploy: unggah isi ZIP ke Vercel/Netlify/GitHub Pages (hosting statis, HTTPS). Buka di HP > menu browser > "Pasang aplikasi".
- ZIP2APK: `index.html` sudah di root ZIP.
## Catatan
- Login lokal: password dibuat saat pertama dibuka. Ini pengaman tampilan di perangkat, bukan keamanan server.
- Backup: Pengaturan > Ekspor data (ZIP). Pindah perangkat: Impor data (ZIP). Password tidak ikut backup.
- Link laporan orang tua berisi data laporan di dalam link (berlaku 30 hari); tanpa server, link tidak bisa dicabut.
- Tombol WhatsApp membuka WhatsApp dengan pesan terisi; pengiriman tetap ditekan manual.
## Struktur data (v1.2.0)
- Kelas = kelompok (Kelompok 1, 2, 3) untuk absensi dan jadwal.
- Program = paket berbayar dengan SPP sendiri (Paket Lengkap, Paket TKA B.Indonesia + Matematika, Program TKA Matematika); mapel per program bisa diatur di menu Kelas & Program.
- Mapel: Matematika Umum, TKA Bahasa Indonesia, TKA Matematika. Nilai dan laporan dipisah per mapel.
- Mengganti ZIP di hosting tidak menghapus data di HP, karena data tersimpan di browser. Data versi lama otomatis dimigrasi.
