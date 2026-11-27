# Lybraria

### Aplikasi Pengelolaan Perpustakaan Kampus Berbasis Android

## 1. Deskripsi Project

**Lybraria** merupakan aplikasi mobile berbasis Android yang dirancang untuk membantu pengelolaan operasional dan sirkulasi perpustakaan kampus secara digital.

Aplikasi ini memiliki dua jenis pengguna, yaitu **Admin** dan **Anggota**. Admin berperan sebagai petugas perpustakaan yang mengelola data buku, kategori, anggota, peminjaman, pengembalian, serta denda keterlambatan. Sementara itu, Anggota merupakan mahasiswa terdaftar yang dapat melihat katalog buku, mencari buku, mengajukan peminjaman, dan memantau status serta riwayat peminjaman.

Lybraria dikembangkan untuk lingkup satu perpustakaan kampus dengan NIM sebagai identitas keanggotaan mahasiswa. Pengajuan peminjaman dilakukan melalui aplikasi, sedangkan pengambilan dan pengembalian buku dilaksanakan secara langsung di perpustakaan.

Project ini dikembangkan menggunakan **Kotlin, Jetpack Compose, REST API, dan PostgreSQL** untuk memenuhi kebutuhan Project Akhir mata kuliah Pengembangan Aplikasi Mobile (PAM) 2026.

## 2. Informasi Project

| Keterangan | Informasi |
|---|---|
| Nama Project | Lybraria |
| Tema | Pendidikan |
| Lingkup | Perpustakaan Kampus |
| Platform | Android |
| Bahasa Pemrograman | Kotlin |
| UI Framework | Jetpack Compose |
| Navigasi | Navigation Compose |
| Arsitektur Mobile | MVVM |
| Backend | REST API |
| Database | PostgreSQL |
| Autentikasi | JWT & Refresh Token |
| Status | Dalam Pengembangan |

## 3. Identitas Mahasiswa

| Keterangan | Informasi |
|---|---|
| Nama | Sukma Hawa Iza Ghazali |
| NIM | 20240140148 |
| Mata Kuliah | Pengembangan Aplikasi Mobile (PAM) |

## 4. Repository Project

Pengembangan Lybraria dipisahkan menjadi dua repository agar pengelolaan aplikasi mobile dan layanan backend lebih terstruktur.

| Repository | Fungsi | Link |
|---|---|---|
| Lybraria Mobile | Aplikasi Android berbasis Kotlin dan Jetpack Compose | [0148_Lybraria](https://github.com/iizaghz/0148_Lybraria) |
| Lybraria API | Backend REST API, autentikasi, pengelolaan data, dan PostgreSQL | [0148_API_Lybraria](https://github.com/iizaghz/0148_API_Lybraria) |

**Catatan:** Repository ini (`0148_Lybraria`) digunakan untuk pengembangan aplikasi mobile dan dokumentasi progress project. Riwayat pengembangan backend dicatat pada repository API yang terpisah.

## 5. Teknologi Project

- **Kotlin** — Bahasa pemrograman aplikasi Android.
- **Jetpack Compose** — Pengembangan antarmuka aplikasi mobile.
- **Navigation Compose** — Navigasi antarlayar aplikasi.
- **MVVM & StateFlow** — Pengelolaan state dan pemisahan logika aplikasi.
- **REST API & JSON** — Komunikasi antara aplikasi dan backend.
- **PostgreSQL** — Penyimpanan data relasional pada server.
- **JWT & Refresh Token** — Autentikasi dan pengelolaan sesi pengguna.
- **Local File Storage** — Penyimpanan dan pembacaan berkas lokal Android.

Implementasi dilakukan secara bertahap. Pengembangan backend telah dimulai, sedangkan aplikasi mobile masih mengikuti tahapan pengembangan project.

## 6. Fitur Utama

### Admin

- Login dan logout.
- Mengelola data buku (CRUDS).
- Mengelola kategori buku (CRUDS).
- Mengelola data anggota (CRUDS).
- Mengelola peminjaman dan pengembalian buku (CRUDS).
- Mengelola denda keterlambatan (CRUDS).
- Melihat ringkasan informasi pada dashboard.
- Menyimpan dan membaca laporan lokal.

### Anggota

- Login dan logout.
- Melihat katalog dan detail buku.
- Mencari buku dan memfilter berdasarkan kategori.
- Mengajukan dan membatalkan pengajuan peminjaman.
- Melihat status serta riwayat peminjaman.
- Melihat informasi denda pribadi.
- Melihat profil keanggotaan.
- Menyimpan dan membaca arsip lokal.

## 7. Progress Mingguan (Weekly Progress)

Berikut merupakan dokumentasi perkembangan project Lybraria berdasarkan kegiatan penyusunan SRS serta riwayat commit pengembangan backend pada GitHub.

### 📅 Minggu 1 (12–19 November 2026)

**Fokus: Analisis Kebutuhan dan Penyusunan SRS Lybraria**

- **Penentuan Konsep Project:** Menetapkan nama Lybraria, tema pendidikan, lingkup perpustakaan kampus, tujuan aplikasi, serta dua peran pengguna, yaitu Admin dan Anggota.
- **Identifikasi Kebutuhan Sistem:** Menentukan fitur pengelolaan buku, kategori, anggota, peminjaman, pengembalian, denda keterlambatan, serta layanan katalog bagi Anggota.
- **Perancangan Teknologi:** Menentukan Kotlin, Jetpack Compose, Navigation Compose, MVVM, REST API, PostgreSQL, serta JWT dan Refresh Token.
- **Penyusunan Dokumen SRS:** Menyusun Introduction, Overall Description, System Features, External Interface Requirements, Other Nonfunctional Requirements, dan Other Requirements.
- **Analisis Entitas Data:** Mengidentifikasi lima entitas utama, yaitu `kategori`, `buku`, `anggota`, `peminjaman`, dan `denda`.

**Hasil:** Draf awal Software Requirements Specification (SRS) Lybraria.

**Status: Completed**

### 📅 Minggu 2 (19–26 November 2026)

**Fokus: Penyempurnaan SRS dan Pemodelan Sistem**

- **Penyusunan Use Case Diagram:** Menggambarkan interaksi Admin dan Anggota dengan fitur utama aplikasi Lybraria.
- **Penyusunan Activity Diagram:** Melengkapi alur login, logout, pengelolaan buku, kategori, anggota, peminjaman, pengembalian, serta pengelolaan denda.
- **Pemodelan Alur CRUDS:** Menggambarkan operasi Create, Read, Update, Delete, dan Search beserta validasi dan respons kegagalan.
- **Penyusunan ERD:** Merancang hubungan lima entitas utama dengan Primary Key, Foreign Key, Unique Constraint, dan kardinalitas relasi.
- **Penyusunan RAT:** Mendefinisikan atribut, tipe data PostgreSQL, batasan nilai, dan integritas referensial.
- **Sinkronisasi Dokumen:** Menyesuaikan kebutuhan fungsional, diagram, aturan soft-delete, serta rancangan PostgreSQL agar konsisten.
- **Finalisasi SRS:** Melengkapi spesifikasi sebagai acuan implementasi backend dan aplikasi mobile.

**Hasil:** Dokumen SRS Lybraria beserta Use Case Diagram, Activity Diagram, ERD, dan RAT.

**Status: Completed**

### 📅 Minggu 3 (27 November 2026)

**Fokus: Pengembangan Backend REST API Lybraria**

Pengembangan pada minggu ini dilakukan melalui repository **[0148_API_Lybraria](https://github.com/iizaghz/0148_API_Lybraria)**. Rincian berikut mengacu pada riwayat commit backend.

- **Fondasi Backend dan PostgreSQL** (`ee0624d`): Penambahan domain enum, response helper, dan penanganan kesalahan PostgreSQL untuk membangun struktur dasar layanan API.

- **Keamanan dan Autentikasi JWT** (`b1bb48f`, `85ad264`, `12a0f99`): Implementasi hashing kata sandi menggunakan bcrypt, utilitas JWT, middleware autentikasi dan otorisasi berbasis peran, serta endpoint login, refresh token, profil pengguna, dan logout.

- **Data Awal dan Pengujian Autentikasi** (`3ac6089`, `346e7f3`): Penambahan script seeder akun Admin dan contoh Anggota serta integration test untuk autentikasi dan Role-Based Access Control (RBAC).

- **Category Management CRUDS** (`23d19f6`, `bf31912`, `32a970d`): Implementasi repository, validasi input, service, controller, route berbasis RBAC, dan integration test pengelolaan kategori.

- **Book Management CRUDS** (`59a9420`, `906e0e8`, `4e88d8d`): Pengembangan pengelolaan buku, validasi data, stok, soft-delete, endpoint API, dan integration test.

- **Member Management CRUDS** (`a51816`, `518a76a`, `44806f2`): Implementasi pengelolaan anggota, validasi input, otorisasi Admin, pemeriksaan tanggungan, soft-delete, dan pengujian integrasi.

- **Borrowing & Return Management** (`7b8d905`, `128248c`, `8222f7d`): Implementasi repository, service transaksi, controller, route RBAC, peminjaman dan pengembalian buku, serta pengujian transaksi.

- **Late Fine Management CRUDS** (`02dbd75`, `a5838e0`, `d4ed210`): Implementasi pengelolaan denda, validasi input, service, controller, endpoint API, serta pengujian integrasi dengan dashboard Admin.

- **Admin Dashboard** (`a809cc4`): Penambahan endpoint ringkasan statistik dashboard untuk mendukung tampilan informasi operasional perpustakaan.

- **Dokumentasi REST API** (`e3bf8f9`, `3272195`, `646fd45`): Penyusunan README backend, dokumentasi endpoint dan konfigurasi lokal, spesifikasi OpenAPI 3.0, serta antarmuka Swagger UI pada `/api/docs`.

- **Penyempurnaan Keamanan dan Validasi** (`321f819`, `44e6252`, `494141d`, `d913ff9`): Penguatan revokasi sesi logout, validasi JSON, pencegahan duplikasi denda otomatis, validasi tipe angka PostgreSQL, serta pengamanan perubahan akun anggota.

- **Perbaikan Transaksi dan Konsistensi Data** (`2f8ed30`, `5f0c8f5`, `150960d`): Penambahan transaksi ACID dan row locking pada pembaruan/penghapusan buku, perbaikan pencarian menggunakan ILIKE, normalisasi nilai NUMERIC JSON, serta penguatan konsistensi transaksi peminjaman dan denda.

- **Pengujian Regresi Keamanan** (`01a726c`, `f889e6a`, `f5878d8`): Penambahan pengujian keamanan lanjutan, penguatan validasi JWT HS256, pembaruan Refresh Token secara atomik, pembatasan panjang password, dan pengujian regresi terhadap kasus ekstrem.


**Riwayat commit:** [Lihat seluruh commit API Lybraria](https://github.com/iizaghz/0148_API_Lybraria/commits/main/)
