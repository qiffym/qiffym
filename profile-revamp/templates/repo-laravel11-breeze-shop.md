<!-- Ready-to-use README for qiffym/laravel11-breeze-shop. Replace {{...}} and screenshots. -->

<h1 align="center">Laravel 11 Breeze Shop</h1>

<p align="center">A full e-commerce store built on Laravel 11 with Breeze authentication — catalog, cart, and checkout.</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-2563EB?style=flat-square" alt="status">
  <img src="https://img.shields.io/badge/license-MIT-2563EB?style=flat-square" alt="license">
  <img src="https://img.shields.io/badge/Laravel%2011-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel 11">
  <img src="https://img.shields.io/badge/Breeze-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Breeze">
  <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind">
</p>

---

## 📸 Screenshot

![Breeze Shop storefront]({{SCREENSHOT_URL}})

## ✨ Features

- 🛍️ Product catalog with categories
- 🛒 Shopping cart (add / update / remove)
- 🔐 Authentication via Laravel Breeze
- 💳 Checkout flow and order summary
- 📱 Responsive UI with Tailwind CSS

## 🧰 Tech Stack

- **Framework:** Laravel 11 (PHP)
- **Auth:** Laravel Breeze
- **Frontend:** Blade + Tailwind CSS
- **Database:** MySQL

## ⚡ Quick Start (≤ 5 minutes)

### Prerequisites
- PHP 8.2+ and Composer 2
- MySQL 8
- Node 18+

### Install & run
```bash
git clone https://github.com/qiffym/laravel11-breeze-shop.git
cd laravel11-breeze-shop

cp .env.example .env           # set DB credentials
composer install
php artisan key:generate
php artisan migrate --seed     # seeds demo products
npm install && npm run build
php artisan serve
```

Open http://localhost:8000 and browse the seeded products.

## 🔧 Configuration

| Variable | Description | Example |
|---|---|---|
| `DB_DATABASE` | Database name | `breeze_shop` |
| `DB_USERNAME` | DB user | `root` |
| `DB_PASSWORD` | DB password | `secret` |

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 License

MIT — see [LICENSE](LICENSE).

## 👤 Author

**Qiff Ya Muhammad** — [GitHub](https://github.com/qiffym) · [Website](https://qiffym.vercel.app)
