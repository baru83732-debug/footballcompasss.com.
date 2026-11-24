# FootBall Compasss — Frontend

Konfigurasi final:
- Desain premium navy/cyan/hijau
- Bahasa Indonesia
- Akses menggunakan akun
- Tampilan responsif untuk HP Android

## Isi paket
- `index.html`: frontend awal dengan halaman masuk/daftar, dashboard, detail analisis, 11 pasar, pencarian, dan navigasi.

## Penting: status saat ini
Halaman analisis masih memakai DATA CONTOH yang diberi label simulasi. Belum ada data pertandingan live, statistik aktual, odds, maupun prediksi aktual. Backend, database, dan API-Football belum dipasang.

## Pasang di GitHub dari HP Android
1. Buka repository GitHub milikmu.
2. Buka `index.html` lalu pilih Edit, atau unggah file ini jika belum ada.
3. Ganti isi file dengan `index.html` dari paket ini, lalu Commit changes.
4. Untuk membuat website publik, aktifkan GitHub Pages dari Settings > Pages > Deploy from a branch > `main` > `/ (root)`.

## Mengaktifkan akun sungguhan (Supabase)
Mode demo lokal bukan autentikasi sungguhan. Untuk akun aman yang tersimpan di server:
1. Buat project di https://supabase.com
2. Buka Project Settings > API.
3. Salin Project URL dan anon/public key.
4. Di `index.html`, isi `SUPABASE_URL` dan `SUPABASE_ANON_KEY`.
5. Jangan pernah memasukkan `service_role` key atau API-Football key ke frontend.
6. Atur Authentication > URL Configuration dengan URL website GitHub Pages milikmu sebagai Site URL dan Redirect URL.

## Tahap berikutnya
Backend terpisah perlu dibuat untuk menyimpan API-Football key secara rahasia, mengambil data fixture/statistik, menjalankan model Poisson, serta menyimpan riwayat ke database. Jangan menampilkan angka contoh sebagai data aktual.
