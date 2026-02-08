🌐 **Bahasa:** [English](README.md) | Bahasa Indonesia

# Rotasi V3 - Smart URL Shortener dengan Auto-Mirror

**URL shortener tingkat enterprise dengan monitoring domain otomatis, penggantian mirror otomatis, dan caching performa tinggi.**

---

## 🎯 Fitur Utama

### URL Shortening
- ✅ Kode custom atau auto-generate
- ✅ Multi tipe rotasi: Sequential, Random, Weighted
- ✅ Passthrough parameter URL
- ✅ Bulk shortlink creation

### Smart Rotation
- ✅ Multi-destinasi per shortlink
- ✅ Distribusi weighted untuk A/B testing
- ✅ Rotasi destinasi otomatis
- ✅ Tracking klik real-time

### Domain Monitoring
- ✅ Pengecekan status domain otomatis (interval 5 menit)
- ✅ Deteksi pemblokiran Nawala
- ✅ Notifikasi alert via Telegram
- ✅ Auto-nonaktifkan destinasi yang terblokir

### Sistem Auto-Mirror
- ✅ Generate URL mirror otomatis
- ✅ Integrasi DNS Cloudflare
- ✅ Auto-config reverse proxy Nginx
- ✅ Auto-replace mirror yang terblokir
- ✅ Infrastruktur self-healing

### Manajemen Campaign
- ✅ Grupkan shortlink berdasarkan campaign
- ✅ Manajemen bulk target URL
- ✅ Analitik level campaign
- ✅ Tracking penggunaan per campaign

### Performa
- ✅ Redis caching (TTL 60 detik)
- ✅ Batch click counter (kurangi DB writes)
- ✅ Support PM2 cluster mode
- ✅ Handle 500K+ redirect/hari

### Dashboard Admin
- ✅ UI React modern dengan dark theme
- ✅ Statistik real-time
- ✅ Logging aktivitas admin
- ✅ Multi-admin dengan roles

---

## 📋 Kebutuhan Sistem

### Server
| Komponen | Minimum | Rekomendasi |
|----------|---------|-------------|
| OS | Ubuntu 22.04+ | Ubuntu 24.04 LTS |
| CPU | 2 core | 4+ core |
| RAM | 2 GB | 4+ GB |
| Storage | 20 GB SSD | 50+ GB SSD |

### Software Stack
- **Node.js** 20.x LTS
- **PostgreSQL** 15+
- **Redis** 7+
- **Nginx** (terbaru)
- **PM2** (process manager)
- **Certbot** (sertifikat SSL)

### Layanan External
- Akun **Cloudflare** (untuk DNS API - tier gratis cukup)
- **Telegram Bot** (opsional, untuk alert)

---

## 📁 Struktur Project

```
RotasiV3P/
├── SERVER/                 # Backend API
│   ├── src/
│   │   ├── controllers/    # Route handlers
│   │   ├── services/       # Business logic
│   │   ├── db/             # Database schema
│   │   └── views/          # Halaman error
│   └── .env
├── WEB/                    # Frontend Dashboard
│   ├── src/
│   │   ├── components/     # Komponen React
│   │   └── hooks/          # Custom hooks
│   └── dist/               # Build production
└── DEPLOY_GUIDE.md         # Panduan deploy
```

---

## 💰 Harga (Pembelian Sekali Bayar)

### Opsi Lisensi

| Paket | Harga |
|-------|-------|
| **Basic** | Rp 3.500.000 |
| **Standard** | Rp 5.000.000 |
| **Enterprise** | Rp 8.000.000 |

### Yang Termasuk

| Fitur | Basic | Standard | Enterprise |
|-------|:-----:|:--------:|:----------:|
| Source Code Lengkap | ✅ | ✅ | ✅ |
| Panduan Deployment | ✅ | ✅ | ✅ |
| 1x Bantuan Instalasi | ❌ | ✅ | ✅ |
| Video Tutorial | ❌ | ✅ | ✅ |
| White-label (hapus branding) | ❌ | ❌ | ✅ |
| Support Prioritas (30 hari) | ❌ | ❌ | ✅ |

### Ketentuan
- ⚠️ **Tidak ada update** setelah pembelian
- ⚠️ **Tidak ada maintenance** termasuk
- ⚠️ **Tidak ada SLA** atau garansi support
- ✅ **Domain unlimited** di server sendiri
- ✅ **Kepemilikan penuh** source code
- ✅ **Modifikasi bebas** untuk personal/komersial
- ❌ **Dilarang dijual kembali** source code-nya

---

## 📞 Kontak

- Telegram: @kitaoverdose

---

## 📜 Lisensi

Lisensi Proprietary - Source code disediakan hanya untuk penggunaan pembeli. Redistribusi atau penjualan kembali dilarang.

© 2024 Rotasi V3. Hak cipta dilindungi.

