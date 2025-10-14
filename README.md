# 🍽️ Restaurant Booking Manager - Multi-Location

WordPress plugin quản lý đặt bàn nhà hàng đa địa điểm với email confirmation và multi-language support.

## ✨ Features

### Multi-Location Support
- ✅ Quản lý 3+ locations độc lập (HCM, HN, JP)
- ✅ Settings riêng cho mỗi location
- ✅ Timezone support
- ✅ Phone validation theo location

### Smart Booking Flow
- ✅ 2-step booking process
- ✅ Real-time availability check
- ✅ Alternative time suggestions
- ✅ Email confirmation với token (2h expire)

### Multi-Language
- ✅ Tiếng Việt 🇻🇳
- ✅ English 🇺🇸
- ✅ 日本語 🇯🇵

### Role-Based Access
- ✅ Super Admin (all locations)
- ✅ Location Manager (specific location)
- ✅ Permission system

### Email System
- ✅ Confirmation email với link
- ✅ Auto-confirm qua email
- ✅ Multi-language templates
- ✅ Token expiration (2 hours)

---

## 📋 Requirements

- WordPress 5.8+
- PHP 7.4+
- MySQL 5.7+
- HTTPS (recommended for email confirmation)

---

## 🚀 Installation

### Quick Start
1. Download plugin
2. Upload to `/wp-content/plugins/`
3. Activate trong WP Admin
4. Go to **Đặt bàn > Locations** để setup

### Detailed Setup
See [INSTALLATION.md](docs/INSTALLATION.md)

---

## 📖 Documentation

- [User Guide](docs/USER_GUIDE.md) - Hướng dẫn khách hàng
- [Admin Guide](docs/ADMIN_GUIDE.md) - Hướng dẫn quản trị
- [Developer Guide](docs/DEVELOPER.md) - Tài liệu lập trình
- [API Documentation](docs/API.md) - REST API docs
- [Migration Guide](docs/MIGRATION.md) - Nâng cấp từ phiên bản cũ

---

## 🗺️ Roadmap

See [ROADMAP.md](ROADMAP.md) for detailed implementation plan.

### Current Status: Phase 1 ⚠️ IN PROGRESS
- [x] Requirements & Architecture
- [ ] Database Migration
- [ ] Location Management Core
- [ ] Authentication & Roles
- [ ] Frontend Multi-step Flow
- [ ] Email Confirmation System
- [ ] Backend per Location
- [ ] Integration & Testing

---

## 🛠️ Tech Stack

- **Backend:** PHP 7.4+ (WordPress)
- **Frontend:** Vanilla JS (jQuery)
- **Database:** MySQL/MariaDB
- **Email:** WordPress wp_mail()
- **Architecture:** Plugin → API Ready → Standalone Ready

---

## 🔐 Security

- ✅ CSRF protection (nonce)
- ✅ SQL injection prevention (prepared statements)
- ✅ XSS protection (sanitization)
- ✅ Email token hashing (SHA-256)
- ✅ Rate limiting (confirmation endpoint)
- ✅ Role-based access control

---

## 🌐 Multi-Location Architecture
```
┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│   HCM       │    │     HN      │    │     JP      │
│  Location   │    │  Location   │    │  Location   │
└──────┬──────┘    └──────┬──────┘    └──────┬──────┘
       │                  │                  │
       └──────────────────┴──────────────────┘
                          │
              ┌───────────▼───────────┐
              │   Shared Database     │
              │   - Bookings          │
              │   - Tables            │
              │   - Customers         │
              └───────────────────────┘
```

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 📄 License

GPL v2 or later

---

## 👨‍💻 Author

**NewIT5S**
- GitHub: [@newit5s](https://github.com/newit5s)
- Email: your@email.com

---

## 📞 Support

- 📖 [Documentation](docs/)
- 🐛 [Issue Tracker](https://github.com/newit5s/wp_booking-table/issues)
- 💬 [Discussions](https://github.com/newit5s/wp_booking-table/discussions)

---

## 🎯 Version

**Current:** v2.0.0-alpha (Multi-location)  
**Previous:** v1.0.0 (Single location)

See [CHANGELOG.md](CHANGELOG.md) for history.
