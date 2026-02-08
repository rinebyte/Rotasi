# Rotasi V3 - Smart URL Shortener with Auto-Mirror

**Enterprise-grade URL shortener with intelligent domain monitoring, auto-mirror replacement, and high-performance caching.**

---

## 🎯 Core Features

### URL Shortening
- ✅ Custom short codes or auto-generated
- ✅ Multiple rotation types: Sequential, Random, Weighted
- ✅ URL parameter passthrough
- ✅ Bulk shortlink creation

### Smart Rotation
- ✅ Multi-destination support per shortlink
- ✅ Weighted distribution for A/B testing
- ✅ Automatic destination rotation
- ✅ Real-time click tracking

### Domain Monitoring
- ✅ Automatic domain status checking (5-minute interval)
- ✅ Nawala/ISP blocking detection
- ✅ Telegram alert notifications
- ✅ Auto-deactivate blocked destinations

### Auto-Mirror System
- ✅ Automatic mirror URL generation
- ✅ Cloudflare DNS integration
- ✅ Nginx reverse proxy auto-config
- ✅ Auto-replace blocked mirrors
- ✅ Self-healing infrastructure

### Campaign Management
- ✅ Group shortlinks by campaign
- ✅ Bulk target URL management
- ✅ Campaign-level analytics
- ✅ Usage tracking per campaign

### Performance
- ✅ Redis caching (60s TTL)
- ✅ Batch click counter (reduce DB writes)
- ✅ PM2 cluster mode support
- ✅ Handles 500K+ redirects/day

### Admin Dashboard
- ✅ Modern React UI with dark theme
- ✅ Real-time statistics
- ✅ Admin activity logging
- ✅ Multi-admin support with roles

---

## 📋 Requirements

### Server
| Component | Minimum | Recommended |
|-----------|---------|-------------|
| OS | Ubuntu 22.04+ | Ubuntu 24.04 LTS |
| CPU | 2 cores | 4+ cores |
| RAM | 2 GB | 4+ GB |
| Storage | 20 GB SSD | 50+ GB SSD |

### Software Stack
- **Node.js** 20.x LTS
- **PostgreSQL** 15+
- **Redis** 7+
- **Nginx** (latest)
- **PM2** (process manager)
- **Certbot** (SSL certificates)

### External Services
- **Cloudflare** account (for DNS API - free tier works)
- **Telegram Bot** (optional, for alerts)

---

## 📁 Project Structure

```
RotasiV3P/
├── SERVER/                 # Backend API
│   ├── src/
│   │   ├── controllers/    # Route handlers
│   │   ├── services/       # Business logic
│   │   ├── db/             # Database schema
│   │   └── views/          # Error pages
│   └── .env
├── WEB/                    # Frontend Dashboard
│   ├── src/
│   │   ├── components/     # React components
│   │   └── hooks/          # Custom hooks
│   └── dist/               # Production build
└── DEPLOY_GUIDE.md         # Deployment guide
```

---

## 💰 Pricing (One-Time Purchase)

### License Options

| Package | Price (IDR) | Price (USD) |
|---------|-------------|-------------|
| **Basic** | Rp 3.500.000 | $220 |
| **Standard** | Rp 5.000.000 | $310 |
| **Enterprise** | Rp 8.000.000 | $500 |

### What's Included

| Feature | Basic | Standard | Enterprise |
|---------|:-----:|:--------:|:----------:|
| Full Source Code | ✅ | ✅ | ✅ |
| Deployment Guide | ✅ | ✅ | ✅ |
| 1x Installation Assist | ❌ | ✅ | ✅ |
| Video Tutorial | ❌ | ✅ | ✅ |
| White-label (remove branding) | ❌ | ❌ | ✅ |
| Priority Support (30 days) | ❌ | ❌ | ✅ |

### Terms
- ⚠️ **No updates** after purchase
- ⚠️ **No maintenance** included
- ⚠️ **No SLA** or guaranteed support
- ✅ **Unlimited domains** on your own server
- ✅ **Full ownership** of source code
- ✅ **Modify freely** for personal/commercial use
- ❌ **No reselling** of source code

---

## 📞 Contact

- Telegram: @kitaoverdose

---

## 📜 License

Proprietary License - Source code is provided for buyer's use only. Redistribution or resale is prohibited.

© 2024 Rotasi V3. All rights reserved.