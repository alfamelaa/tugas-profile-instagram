# Readme Bootstrap
- penjelasan desain
- tampilan profil IG sederhana dengan Bootstrap 5 (CDN), tanpa JS & tanpa CSS tambahan
- header mobile di tengah, mulai sm jadi dua kolom rata kiri
- feed foto pakai grid 1 → 2 → 3 kolom (col-12, col-sm-6, col-lg-4)
- foto persegi pakai ratio-1x1, gambar dari assets/img

- struktur file
 - index.html (halaman utama)
 - assets/img/ (semua gambar: pp.jpg, 1.jpeg … 12.jpeg)

- build/run
- cukup buka index.html di browser
- butuh internet untuk CDN Bootstrap

- dependensi
- Bootstrap 5 via CDN
- tidak ada npm / build tools

- jawaban pertanyaan
- Konfigurasi col per breakpoint
 - col-12 (mobile 1 kolom, gampang di-tap) → col-sm-6 (tablet 2 kolom, pas dibaca) → col-lg-4 (desktop 3 kolom, padat seperti IG).

- Tombol tetap mudah dijangkau di mobile
 - Header pakai d-flex flex-wrap gap-2 + justify-content-center (mobile) → justify-content-sm-start (lebih lebar). Kalau mau lebih nyaman, pakai .btn biasa (tanpa -sm) atau tambah py-2 px-3.

- Kalau postingan jadi 50
 - Grid tetap rapi karena sistem row/col otomatis membungkus. Potensi masalah: loading jadi berat. Solusi cepat: tambahkan loading="lazy" di <img>; kalau sangat banyak, pakai pagination/infinite scroll (di luar scope tugas).