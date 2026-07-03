# WNG Engineering

Dokumen ini menjelaskan gambaran singkat engineering team WNG dan alur deployment yang digunakan.

## 1. Visi Team WNG

Team WNG berfokus untuk membangun aplikasi yang mampu dikembangkan sampai production, memiliki dokumentasi yang terarah, dan mudah di-scale ketika kebutuhan bisnis bertambah.

## 2. Dokumentasi

| Dokumen | Keterangan |
| --- | --- |
| [system-list.md](system-list.md) | List system/aplikasi yang dimiliki atau dikelola oleh WNG. |
| [architecture.md](architecture.md) | Catatan arsitektur, Docker, dan struktur folder server. |

## 3. Deployment Flow

Flow deployment team WNG:

1. developer membuat branch sesuai feature atau perubahan yang dikerjakan;
2. perubahan selesai lalu dibuat request untuk masuk ke staging;
3. SPV melakukan review dan approve perubahan;
4. user melakukan testing di staging;
5. jika hasil testing sudah oke, perubahan dapat masuk ke production;
6. setelah production, team melakukan pengecekan singkat untuk memastikan aplikasi berjalan normal.
