# WNG System List

Dokumen ini khusus berisi list system/aplikasi yang dimiliki atau dikelola oleh WNG.

Untuk dokumentasi umum engineering, lihat [README.md](README.md).

## 1. Sistem POS

| Item | Detail |
| --- | --- |
| Nama System | Sistem POS |
| Description | Aplikasi Point of Sales untuk manajemen transaksi dan inventaris produk secara efisien. |
| Tujuan | Membantu proses kasir dan penyusunan laporan penjualan agar operasional bisnis lebih terorganisir. |
| Feature | Input transaksi produk masuk dan keluar, sistem kasir yang scalable dan real-time, manajemen stok barang yang terintegrasi dengan laporan keuangan dan transaksi. |
| Tech Stack | Laravel, Inertia JS, MySQL |
| Database Connect | MySQL - `admin_posku` |
| Repository Link | https://github.com/wng-net/pos-systems |
| Link Staging | - |
| Link Production | https://posku.visioner.systems/login |
| Third Party Connect | - |
| Deployment | CPanel |
| Status | Active / Development |

## 2. Sistem Warehouse

| Item | Detail |
| --- | --- |
| Nama System | Sistem Warehouse |
| Description | Sistem manajemen inventaris dan transaksi yang dirancang untuk mendukung alur kerja gudang. |
| Tujuan | Membantu proses manajemen gudang dan menyajikan laporan inventaris yang akurat agar operasional gudang lebih terorganisir. |
| Feature | Input transaksi barang masuk dan keluar, dashboard/admin panel, autentikasi user, manajemen stok barang real-time, pelaporan gudang, dan stok opname yang komprehensif. |
| Tech Stack | Laravel, Bootstrap, MySQL |
| Database Connect | MySQL - `gudang_barang` |
| Repository Link | https://github.com/wng-net/warehouse-systems |
| Link Staging | - |
| Link Production | https://warehouse-bali.wng.co.id/ |
| Third Party Connect | - |
| Deployment | CPanel |
| Status | Active / Development |

## 3. E-Absensi

| Item | Detail |
| --- | --- |
| Nama System | E-Absensi |
| Description | Sistem kehadiran karyawan berbasis GPS. |
| Tujuan | Mempermudah pencatatan kehadiran karyawan secara real-time dan otomatis untuk mendukung administrasi yang efisien dan akurat. |
| Feature | Pencatatan kehadiran berbasis lokasi/geotagging, manajemen data karyawan, dan rekapitulasi data absensi yang terintegrasi. |
| Tech Stack | Laravel, Bootstrap, MySQL |
| Database Connect | MySQL - `absensi_db` |
| Repository Link | https://github.com/wng-net/e-absensi |
| Link Staging | https://e-absensi-stg.yoicorp.co.id/ |
| Link Production | https://eabsensi.visioner.systems/ |
| Third Party Connect | Leaflet js |
| Deployment | Docker, CPanel |
| Status | Active / Development |

## 4. ICRM

| Item | Detail |
| --- | --- |
| Nama System | ICRM |
| Description | Platform manajemen hubungan pelanggan internet berbasis website. |
| Tujuan | Mempermudah pencatatan dan pengelolaan calon pelanggan yang melakukan registrasi. |
| Feature | Approval calon pelanggan sesuai aturan yang berlaku, manajemen data calon pelanggan, dan pengelolaan chat yang terintegrasi secara real-time. |
| Tech Stack | Laravel, Next js, MySQL |
| Database Connect | MySQL - `icrm_db` |
| Repository Link | https://github.com/wng-net/icrm-fe, https://github.com/wng-net/icrm-be |
| Link Staging | https://icrm-stg.yoicorp.co.id/ |
| Link API Staging | https://api-stg-icrm.yoicorp.co.id/ |
| Link Production | https://icrmplus.visioner.systems/ |
| Link API Production | https://api-icrmplus.visioner.systems/ |
| Third Party Connect | - |
| Deployment | Docker, CPanel |
| Status | Active / Development |

## 5. E-Billing

| Item | Detail |
| --- | --- |
| Nama System | E-Billing |
| Description | Platform pengelolaan tagihan digital yang dirancang untuk mengotomatisasi proses pembuatan invoice. |
| Tujuan | Mempermudah pencatatan dan pengelolaan tagihan pelanggan, serta memantau pembayaran pelanggan agar operasional keuangan lebih efisien dan tertib. |
| Feature | Pembuatan invoice otomatis, reminder real-time yang terintegrasi dengan WhatsApp dan email, pembayaran yang terintegrasi dengan Mikrotik dan VA, serta laporan data keuangan real-time. |
| Tech Stack | Laravel, Next js, MySQL |
| Database Connect | MySQL - `billings_db` |
| Repository Link | https://github.com/wng-net/billing-be, https://github.com/wng-net/billing-fe |
| Link Staging | https://billing-stg.yoicorp.co.id/ |
| Link API Staging | https://api-stg-billing.yoicorp.co.id/ |
| Link Production | https://ebilling.visioner.systems/ |
| Link API Production | https://api-billing.visioner.systems/ |
| Third Party Connect | DOKU, Leaflet js, WA Blast, RouterOS, Laravolt (Library Data Geo Indonesia) |
| Deployment | Docker, CPanel |
| Status | Active / Development |

## 6. Ticketing

| Item | Detail |
| --- | --- |
| Nama System | Ticketing |
| Description | Platform manajemen tiket untuk mengelola laporan gangguan internet secara terpusat dan sistematis. |
| Tujuan | Mempercepat respons tim teknis dalam menyelesaikan kendala pelanggan internet. |
| Feature | Pembuatan tiket otomatis untuk setiap laporan gangguan dan pelacakan status penanganan yang terintegrasi untuk menjaga transparansi komunikasi dengan pelanggan. |
| Tech Stack | Laravel, Next js, MySQL |
| Database Connect | MySQL - `ticketing_db` |
| Repository Link | https://github.com/wng-net/ticketing-be, https://github.com/wng-net/ticketing-fe |
| Link Staging | https://ticketing-stg.yoicorp.co.id/ |
| Link API Staging | https://api-stg-ticketing.yoicorp.co.id/ |
| Link Production | - |
| Link API Production | - |
| Third Party Connect | Leaflet js |
| Deployment | Docker |
| Status | Active / Development |

## 7. OLT Monitoring

| Item | Detail |
| --- | --- |
| Nama System | OLT Monitoring |
| Description | Dashboard pemantauan infrastruktur OLT (Optical Line Terminal) untuk mengawasi status perangkat jaringan secara real-time. |
| Tujuan | Memastikan stabilitas koneksi perangkat OLT dan mempercepat deteksi dini gangguan pada sisi pelanggan. |
| Feature | Visualisasi status link dan traffic perangkat secara real-time, integrasi dengan RouterOS dan Mikrotik, serta manajemen data OLT yang lebih efisien. |
| Tech Stack | Laravel, Next js, MySQL |
| Database Connect | MySQL - `olt_db` |
| Repository Link | https://github.com/wng-net/olt-monitoring |
| Link Staging | https://olt-monitoring-stg.yoicorp.co.id/login |
| Link Production | - |
| Third Party Connect | RouterOS |
| Deployment | Docker |
| Status | Active / Development |

## 8. Yoitrans

| Item | Detail |
| --- | --- |
| Nama System | Yoitrans |
| Description | Aplikasi manajemen operasional untuk mengelola alur layanan transportasi travel secara digital dan efisien. |
| Tujuan | Mengotomatisasi proses reservasi dan manajemen transportasi untuk meningkatkan efisiensi operasional penyedia jasa serta memberikan pengalaman booking yang praktis bagi pengguna. |
| Feature | Pemesanan unit kendaraan, manajemen jadwal perjalanan, dan laporan pendapatan harian yang terintegrasi. |
| Tech Stack | Laravel, Bootstrap |
| Database Connect | MySQL - `yoitrans_db` |
| Repository Link | - |
| Link Staging | - |
| Link Production | https://yoitrans.com/ |
| Third Party Connect | - |
| Deployment | Docker |
| Status | Active / Development |

## 9. IWAR

| Item | Detail |
| --- | --- |
| Nama System | IWAR |
| Description | Platform digital untuk mengelola proses pendaftaran dan aktivasi layanan internet pelanggan di lingkungan warga secara terpusat. |
| Tujuan | Mempercepat alur registrasi pelanggan baru dan mempermudah pendataan administratif untuk meningkatkan efisiensi pengelolaan layanan internet rumahan. |
| Feature | Form registrasi online, verifikasi data pelanggan yang terintegrasi dengan database layanan internet, dan pengecekan lokasi pemasangan berdasarkan lokasi ODP yang tersedia. |
| Tech Stack | Next js |
| Database Connect | MySQL - `billings_db`, `icrm_db` |
| Repository Link | https://github.com/wng-net/iwar-fe |
| Link Staging | - |
| Link Production | - |
| Third Party Connect | Leaflet js, Laravolt (Library Data Geo Indonesia) |
| Deployment | Docker |
| Status | Active / Development |
