# Laporan Kegiatan BPS (Kabupaten Bone)

Aplikasi Android berbasis Jetpack Compose yang dirancang untuk memudahkan pegawai BPS dalam melaporkan kegiatan harian, melakukan perencanaan kegiatan mendatang, dan memantau poin kedisiplinan secara real-time. Aplikasi ini terintegrasi langsung dengan **Google Sheets** dan **Google Drive** sebagai backend.

## 🚀 Fitur Unggulan

### 1. Dashboard & Kalender Kustom (`BpsCustomCalendar`)
Sistem kalender cerdas dengan indikator status berbasis titik warna:
*   🟢 **Hijau (#8DC63F)**: Laporan Selesai (Tepat Waktu/Poin Maksimal).
*   🔵 **Biru (#00AEEF)**: Rencana Kegiatan (Terjadwal).
*   🟠 **Oranye (#F7941D)**: Laporan Lampau (Diselesaikan lewat dari hari-H).

### 2. Sistem Perencanaan (Planning)
*   Membuat rencana kegiatan untuk tanggal di masa depan.
*   Logika proteksi: Rencana hanya bisa diubah menjadi laporan final saat hari-H atau sesudahnya.
*   Otomatis menghapus entri di sheet `Plans` saat laporan berhasil dikonversi.

### 3. Pelaporan Lengkap
*   Input data kegiatan berbasis tim kerja.
*   Lampiran bukti dukung (Foto Dokumentasi, Tangkapan Layar, Link, atau Catatan).
*   **Fitur Lokasi (GPS)**: Khusus untuk kegiatan "Izin", aplikasi mencatat koordinat lokasi (DMS) secara akurat.
*   **Export PDF**: Laporan otomatis dikonversi menjadi file PDF menggunakan template Google Docs.

### 4. Fitur Admin
*   **Manajemen User**: Menambah, mengaktifkan/menonaktifkan akun, dan reset password.
*   **Pemantauan Real-time**: Melihat siapa saja yang belum melapor pada hari tertentu.
*   **Ranking Bulanan**: Perhitungan otomatis peringkat pegawai berdasarkan akumulasi poin kedisiplinan.

