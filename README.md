# 🏠 SiKos — Sistem Manajemen Kos v3

Aplikasi manajemen kos lengkap berbasis web (HTML tunggal), berjalan 100% di browser tanpa server.

---

## 🚀 Cara Pakai

### Buka langsung
1. Ekstrak folder ZIP ini
2. Klik dua kali **`index.html`** → terbuka di browser (Chrome/Edge/Firefox)
3. Semua data otomatis tersimpan di browser (localStorage)

### Install sebagai Aplikasi (PWA) — opsional
Di **Chrome / Edge**:
- Buka `index.html`
- Klik ikon ⬇️ di address bar → "Install SiKos"
- Aplikasi akan muncul di layar utama HP / taskbar komputer

Di **HP Android**:
- Buka file via browser Chrome
- Ketuk menu ⋮ → "Tambahkan ke layar utama"

---

## 📱 Fitur Lengkap

### 🏷️ Profil Kos
- Nama kos, alamat, nomor WA, tipe (putra/putri/campur)
- Upload foto/logo kos (tersimpan lokal)

### 🛏️ Tipe Kamar
- Nama, harga, ukuran, ID meteran listrik
- Stok kamar (bisa lebih dari 1 unit)
- Duplikat kamar dengan 1 klik
- Flag "Ada Request" untuk calon penyewa
- Upload beberapa foto per kamar

### 🌐 Landing Page
- Preview halaman promosi otomatis dari data profil + kamar
- Download sebagai file HTML untuk dibagikan via WA / hosting

### 👥 Data Penyewa
- Nama, WA, kamar, tanggal masuk
- **Durasi sewa** (bulan) → total otomatis dihitung
- **Diskon / potongan** harga
- **Jatuh tempo otomatis** mundur sesuai durasi
- Deposit, kendaraan, status konfirmasi (perpanjang/checkout)
- Board view (kartu penyewa aktif) + Table view lengkap

### 💬 Follow Up WhatsApp
- 5 template pesan siap kirim: 7 hari, 3 hari, hari-H, perpanjang, checkout
- Copy teks 1 klik atau buka WhatsApp langsung

### ⏰ Notifikasi Jatuh Tempo
- Banner otomatis di dashboard & halaman penyewa
- Browser notification (popup sistem) untuk jatuh tempo urgent

### 💰 Keuangan (4 Kas Terpisah)
- **Kas Umum** — operasional harian
- **Kas Listrik** — iuran & tagihan PLN
- **Kas Sampah** — iuran & bayar petugas
- **Kas Sewa** — catatan pembayaran sewa per penyewa
- **Kas Perbaikan** — biaya perbaikan & pemeliharaan

### 📦 Inventaris & 🔧 Sarpras
- Catat barang masuk/keluar, kondisi, lokasi
- Sarpras: status aktif/perbaikan, biaya per item

### 🧹 Bersih-bersih
- Item checklist bisa tambah/hapus/aktifkan-nonaktifkan
- Pilih tanggal bebas, klik kamar → checklist per kamar
- Progress bar per kamar, tandai semua sekaligus

### 📑 Laporan Rekap
- Ringkasan semua kas dalam satu tabel
- Rekap inventaris & penyewa

### 📊 Export Data
- Export **per modul** atau **semua sekaligus** ke Excel (.xlsx)
- Format rapi: header navy, baris zebra, kolom otomatis
- Cetak laporan sebagai PDF via browser

### 💾 Database / Backup
- **Export JSON** → simpan sebagai backup / pindah ke HP lain
- **Import JSON** → pulihkan data dari backup
- Reset semua data

### ↩️ Undo / Redo
- Berlaku di **semua fitur** (kas, penyewa, kamar, inventaris, dll)
- Shortcut keyboard: **Ctrl+Z** (undo) / **Ctrl+Y** atau **Ctrl+Shift+Z** (redo)
- Riwayat hingga 60 langkah

---

## 🔒 Privasi & Data
Semua data tersimpan **hanya di browser kamu** (localStorage).  
Tidak ada data yang dikirim ke server manapun.  
Untuk pindah device: gunakan fitur **Database → Export JSON** lalu import di device baru.

---

## 📂 Struktur File
```
sikos-app/
├── index.html        ← Aplikasi utama (buka ini!)
├── manifest.json     ← Konfigurasi PWA
├── sw.js             ← Service Worker (offline support)
├── icons/
│   ├── icon-192.png  ← Ikon aplikasi
│   └── icon-512.png  ← Ikon aplikasi (besar)
└── README.md         ← Panduan ini
```

---

## 💡 Tips
- **Backup rutin**: Export JSON setiap minggu sebagai cadangan
- **Akses cepat**: Install sebagai PWA agar bisa dibuka dari layar utama HP
- **Offline**: Setelah pernah dibuka online (untuk font & CDN), bisa dipakai offline

---

*Dibuat dengan ❤️ — SiKos v3*
