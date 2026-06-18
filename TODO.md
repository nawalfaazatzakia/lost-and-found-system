# TODO - Dockerfile & docker-compose

- [x] Tambah `Dockerfile` untuk Laravel (PHP-FPM 8.3) + Composer + deps PHP + Node untuk Vite build.
- [x] Tambah `docker-compose.yml` berisi service: `nginx`, `app`, `db`.
- [x] Tambah konfigurasi Nginx `nginx/default.conf` (proxy ke PHP-FPM via `app:9000`).
- [ ] Verifikasi dengan build: `docker compose build`
- [ ] Jalankan: `docker compose up -d`
- [ ] Setelah container siap, jalankan migrasi (opsional): `docker compose exec app php artisan migrate --force`
- [ ] Pastikan file `.env` di project benar (atau set env via container sebagaimana sudah di `docker-compose.yml`).

