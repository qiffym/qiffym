<!-- Ready-to-use README for qiffym/laravel-filament-cashier. Replace {{...}} and screenshots. -->

<h1 align="center">Laravel Filament Cashier</h1>

<p align="center">Subscription billing with Laravel Cashier, managed through a Filament admin panel.</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-2563EB?style=flat-square" alt="status">
  <img src="https://img.shields.io/badge/license-MIT-2563EB?style=flat-square" alt="license">
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel">
  <img src="https://img.shields.io/badge/Filament-FDAE4B?style=flat-square" alt="Filament">
  <img src="https://img.shields.io/badge/Cashier-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Cashier">
</p>

---

## 📸 Screenshot

![Filament billing panel]({{SCREENSHOT_URL}})

## ✨ Features

- 🔐 Filament admin panel for managing users and subscriptions
- 💳 Laravel Cashier subscription lifecycle (subscribe, swap, cancel, resume)
- 🧾 Invoices and billing status
- 🪝 Stripe webhook handling

## 🧰 Tech Stack

- **Framework:** Laravel (PHP)
- **Admin:** Filament
- **Billing:** Laravel Cashier (Stripe)
- **Database:** MySQL

## ⚡ Quick Start (≤ 5 minutes)

### Prerequisites
- PHP 8.1+ and Composer 2
- MySQL 8
- A [Stripe test](https://dashboard.stripe.com/test/apikeys) account (publishable + secret keys)

### Install & run
```bash
git clone https://github.com/qiffym/laravel-filament-cashier.git
cd laravel-filament-cashier

cp .env.example .env           # add Stripe keys (see below)
composer install
php artisan key:generate
php artisan migrate
php artisan make:filament-user  # create an admin login
php artisan serve
```

Open http://localhost:8000/admin and log in. Use [Stripe test cards](https://docs.stripe.com/testing) (e.g. `4242 4242 4242 4242`).

## 🔧 Configuration

| Variable | Description | Example |
|---|---|---|
| `STRIPE_KEY` | Stripe publishable key | `pk_test_xxx` |
| `STRIPE_SECRET` | Stripe secret key | `sk_test_xxx` |
| `STRIPE_WEBHOOK_SECRET` | Webhook signing secret | `whsec_xxx` |

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 License

MIT — see [LICENSE](LICENSE).

## 👤 Author

**Qiff Ya Muhammad** — [GitHub](https://github.com/qiffym) · [Website](https://qiffym.vercel.app)
