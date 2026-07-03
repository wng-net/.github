# WNG Architecture

Dokumen ini berisi catatan arsitektur, Docker, dan struktur folder server yang digunakan oleh system WNG.

## 1. Deployment Architecture

Secara umum, system WNG diarahkan menggunakan arsitektur container-based dengan Docker. Setiap aplikasi berjalan sebagai service/container terpisah dan dihubungkan melalui reverse proxy.

## 2. Standard Server Folder

Struktur folder server yang direkomendasikan:

```txt
/opt
|-- apps
|   |-- yoitrans
|   |   |-- app
|   |   |-- docker-compose.yml
|   |   |-- .env
|   |   `-- README.md
|   `-- example-system
|       |-- app
|       |-- docker-compose.yml
|       |-- .env
|       `-- README.md
|-- proxy
|   |-- docker-compose.yml
|   |-- nginx
|   |   `-- conf.d
|   `-- certs
`-- other
    |-- backup
    |-- scripts
    `-- monitoring
```

## 3. Folder Responsibility

| Folder | Fungsi |
| --- | --- |
| `/opt/apps` | Tempat semua aplikasi utama WNG disimpan dan dijalankan. |
| `/opt/apps/<system-name>` | Folder khusus per system, berisi source/app, env, compose file, dan dokumentasi lokal. |
| `/opt/proxy` | Reverse proxy untuk mengatur akses domain/subdomain ke container aplikasi. |
| `/opt/proxy/nginx/conf.d` | Konfigurasi routing Nginx atau reverse proxy lain. |
| `/opt/proxy/certs` | Sertifikat SSL/TLS jika dikelola manual. |
| `/opt/other/backup` | Lokasi script atau hasil backup database/file penting. |
| `/opt/other/scripts` | Script operasional seperti deploy, restart, backup, atau cleanup. |
| `/opt/other/monitoring` | Konfigurasi monitoring/logging jika digunakan. |

## 4. Docker Service

Setiap aplikasi minimal memiliki:

- `docker-compose.yml` untuk menjalankan service aplikasi;
- `.env` untuk konfigurasi environment;
- container aplikasi, contoh: `app`, `web`, `queue`, atau `scheduler`;
- database container jika database berada di server yang sama;
- volume untuk data persistent seperti database, storage, dan upload file;
- network Docker yang terhubung dengan proxy.

Contoh service yang umum dipakai:

- `app`: service utama aplikasi;
- `web`: Nginx atau web server aplikasi;
- `db`: MySQL/MariaDB/PostgreSQL;
- `queue`: worker untuk job asynchronous;
- `scheduler`: scheduler/cron;
- `redis`: cache/session/queue broker jika dibutuhkan.
