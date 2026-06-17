<!-- Ready-to-use README for qiffym/manage-kost-app. Replace {{...}} placeholders and screenshot URLs. -->

<h1 align="center">Manage Kost App</h1>

<p align="center">A web app to manage a Muslim boarding house (kost) — tenants, rooms, and payments — built for an orphanage (Panti Asuhan Aisyiyah) in Malang.</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-2563EB?style=flat-square" alt="status">
  <img src="https://img.shields.io/badge/license-MIT-2563EB?style=flat-square" alt="license">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL">
</p>

---

## 📸 Screenshot

![Manage Kost App dashboard]({{SCREENSHOT_URL}})

## ✨ Features

- 🏠 Room & tenant management (occupancy, availability)
- 💰 Monthly rent/payment tracking and status
- 👥 Tenant profiles and history
- 📊 Simple admin dashboard for the foundation's staff

## 🧰 Tech Stack

- **Framework:** Laravel (PHP)
- **Database:** MySQL
- **Frontend:** Blade + Tailwind CSS

## ⚡ Quick Start (≤ 5 minutes)

### Prerequisites
- PHP 8.1+ and Composer 2
- MySQL 8 (or MariaDB)
- Node 18+ (for asset build)

### Install & run
```bash
git clone https://github.com/qiffym/manage-kost-app.git
cd manage-kost-app

cp .env.example .env          # then set DB_DATABASE / DB_USERNAME / DB_PASSWORD
composer install
php artisan key:generate
php artisan migrate --seed     # creates tables and demo data
npm install && npm run build
php artisan serve
```

Open http://localhost:8000 and log in with the seeded demo account (see `database/seeders`).

## 🔧 Configuration

| Variable | Description | Example |
|---|---|---|
| `DB_DATABASE` | Database name | `manage_kost` |
| `DB_USERNAME` | DB user | `root` |
| `DB_PASSWORD` | DB password | `secret` |
| `APP_URL` | App base URL | `http://localhost:8000` |

## 🤝 Contributing

Contributions welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 License

MIT — see [LICENSE](LICENSE).

## 👤 Author

**Qiff Ya Muhammad** — [GitHub](https://github.com/qiffym) · [Website](https://qiffym.vercel.app)
