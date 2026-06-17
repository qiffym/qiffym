<!-- Ready-to-use README for qiffym/laravel11-midtrans-payment-gateway. Replace {{...}} and screenshots. -->

<h1 align="center">Laravel 11 × Midtrans Payment Gateway</h1>

<p align="center">A clean Laravel 11 example that accepts online payments through the Midtrans payment gateway (Snap + webhook handling).</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-active-2563EB?style=flat-square" alt="status">
  <img src="https://img.shields.io/badge/license-MIT-2563EB?style=flat-square" alt="license">
  <img src="https://img.shields.io/badge/Laravel%2011-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel 11">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Midtrans-1A88D8?style=flat-square" alt="Midtrans">
</p>

---

## 📸 Demo

![Midtrans Snap checkout]({{SCREENSHOT_URL}})

> Use a short GIF showing: create order → Snap popup → success callback.

## ✨ Features

- 💳 Midtrans **Snap** checkout integration
- 🔔 Server-side **notification/webhook** handling to confirm payment status
- 🧾 Order creation and status tracking (pending → paid → failed)
- 🧪 Works in Midtrans **Sandbox** out of the box

## 🧰 Tech Stack

- **Framework:** Laravel 11 (PHP)
- **Payments:** Midtrans PHP SDK
- **Database:** MySQL

## ⚡ Quick Start (≤ 5 minutes)

### Prerequisites
- PHP 8.2+ and Composer 2
- MySQL 8
- A free [Midtrans Sandbox](https://dashboard.sandbox.midtrans.com/) account (for Server & Client keys)

### Install & run
```bash
git clone https://github.com/qiffym/laravel11-midtrans-payment-gateway.git
cd laravel11-midtrans-payment-gateway

cp .env.example .env           # add your Midtrans keys (see below)
composer install
php artisan key:generate
php artisan migrate
php artisan serve
```

Open http://localhost:8000, create an order, and pay with a [Midtrans test card](https://docs.midtrans.com/docs/testing-payment-on-sandbox).

## 🔧 Configuration

| Variable | Description | Example |
|---|---|---|
| `MIDTRANS_SERVER_KEY` | Server key from Midtrans dashboard | `SB-Mid-server-xxxx` |
| `MIDTRANS_CLIENT_KEY` | Client key from Midtrans dashboard | `SB-Mid-client-xxxx` |
| `MIDTRANS_IS_PRODUCTION` | Sandbox vs production | `false` |

> For local webhook testing, expose your app with `ngrok` and set the notification URL in the Midtrans dashboard.

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## 📄 License

MIT — see [LICENSE](LICENSE).

## 👤 Author

**Qiff Ya Muhammad** — [GitHub](https://github.com/qiffym) · [Website](https://qiffym.vercel.app)
