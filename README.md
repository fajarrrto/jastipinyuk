# Jastipinyuk Bandung - Jasa Titip Oleh-Oleh Bandung

Aplikasi web modern berbasis **PWA (Progressive Web App)** untuk pemesanan, pencatatan transaksi, pelacakan pesanan, dan manajemen logistik jastip oleh-oleh khas Bandung (Tiramisusu by Chocomory, Bolu Susu Lembang, Kartika Sari, Goela Semoet, Roti Segar).

🌐 **Domain Resmi:** [https://jastipinyuk.my.id](https://jastipinyuk.my.id)

---

## 🚀 Fitur Utama

1. **Formulir Pemesanan Customer Interaktif**:
   - Pilihan toko oleh-oleh populer dengan varian dan harga otomatis.
   - Perhitungan jadwal estimasi *ready* (otomatis sinkron ke hari Sabtu).
   - Generate unik **Order ID** (misal: `JB-202610-XXXX`).
   - Integrasi tombol langsung ke WhatsApp Admin setelah simpan pesanan.

2. **Lacak Pesanan Mandiri (Customer Tracking)**:
   - Customer dapat melacak status belanja & pengiriman (*Order Placed -> Purchased -> In Transit -> Delivered*) hanya dengan nomor WhatsApp atau Kode Order.

3. **Dashboard Monitoring & Finansial (Superadmin & Admin)**:
   - **Financial Analytics**: Total Full Payment, Payment Order Only, Total Fee Lunas, Fee Belum Lunas, Modal Asli Terkumpul, Total Target Omzet.
   - **Quick Update Status**: Ubah status pembayaran (*Full Payment, Order Only, Fee Only, Unpaid, Refunded*) dan tracking pengiriman (*Order Placed, Purchased, In Transit, Delivered, Cancelled*) langsung di tabel.
   - **Kirim Tagihan ke WhatsApp Customer**: Tombol 1-klik untuk mengirim pesan invoice lengkap ke nomor WA pemesan.
   - **Cetak Invoice PDF**: Otomatis generate struk/invoice berformat PDF via `html2pdf.js`.
   - **Ekspor Data CSV & Buka Google Sheets**.
   - **Manajemen Akun Admin**: Tambah, edit sandi, ubah role, dan hapus akun admin.

---

## 📲 Cara Install Aplikasi di HP Android (.APK / WebAPK)

Aplikasi ini sudah berstandar **PWA Standalone**, sehingga dapat dipasang langsung menjadi aplikasi Android native:

### Metode 1: Pasang Langsung dari Browser HP (Direkomendasikan - Tanpa Download File)
1. Buka link **[https://jastipinyuk.my.id](https://jastipinyuk.my.id)** melalui **Google Chrome** di HP Android.
2. Banner **"Install Sekarang"** atau tombol **"📲 Install App"** di pojok kanan atas akan muncul secara otomatis.
3. Klik tombol tersebut, lalu pilih **"Install" / "Tambahkan ke Layar Utama"**.
4. Sistem Android akan otomatis mengemas aplikasi menjadi **WebAPK** resmi yang memiliki ikon sendiri di daftar aplikasi HP, dapat dibuka layar penuh (tanpa bilah browser), dan terasa seperti aplikasi native Play Store.

### Metode 2: Download / Generate File Standalone `.apk`
Jika Anda memerlukan file mentah `.apk` yang bisa dikirim via WhatsApp atau dibagikan:
1. Buka [https://www.pwabuilder.com](https://www.pwabuilder.com).
2. Masukkan URL: `https://jastipinyuk.my.id` lalu klik **Start**.
3. PWABuilder akan mendeteksi `manifest.json`, icon, dan service worker (skor 100% PWA compliant).
4. Klik **Package for Stores** -> Pilih **Android** -> Klik **Generate Package**.
5. Unduh file `.apk` / `.aab` yang telah ditandatangani (signed APK) siap install di HP Android mana saja!

---

## 🛠️ Stack Teknologi

- **Frontend**: HTML5, Vanilla JavaScript ES6+, Bootstrap 5.3.3, Google Fonts (Plus Jakarta Sans)
- **PWA**: Service Worker (`sw.js`), Web App Manifest (`manifest.json`), Maskable App Icons (192x192 & 512x512)
- **PDF Engine**: `html2pdf.js`
- **Backend & Database**: Google Apps Script Web App & Google Sheets (Zero Hosting Cost)
