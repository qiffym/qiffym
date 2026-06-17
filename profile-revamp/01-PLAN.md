# GitHub Profile Revamp — Master Plan (@qiffym)

This document is the implementation playbook. It is written so a cheaper/smaller AI model (or a human) can execute each step with minimal extra reasoning. Every section has concrete, copy-pasteable outputs in the linked files.

**Deliverables in this folder**
- `00-AUDIT.md` — 1-page audit (problems + opportunities + priority list)
- `01-PLAN.md` — this file (strategy, structure, visual, implementation steps)
- `02-PROFILE-README.md` — final profile README, EN + ID, ready to paste
- `03-VISUAL-DESIGN.md` — palette, typography, banner/avatar specs
- `templates/REPO-README-TEMPLATE.md` — reusable repo README skeleton
- `templates/CONTRIBUTING-TEMPLATE.md` — short CONTRIBUTING template
- `templates/repo-*.md` — filled READMEs for the recommended pinned repos

---

## 1. Content Strategy

**Positioning (one line):** *Full-stack web developer building production apps with Laravel and React/Next.js.*

**Audience priority:** (1) recruiters/clients scanning quickly, (2) fellow developers, (3) collaborators.

**Principles**
- Lead with proof (real projects, demos), not adjectives.
- Keep everything scannable: short lines, tables, badges.
- Bilingual but not duplicated everywhere — full summary in EN + ID, the rest in EN with ID where it adds value.
- One accent color, high contrast, minimal decoration (per brief).
- Every project links to either a live demo or a clear README that runs in ≤ 5 minutes.

**Content pillars to show repeatedly:** Laravel/PHP · React/Next.js/TypeScript · Payments & real-world business apps · Clean documentation.

---

## 2. Profile README Structure (outline)

The full ready-to-paste content lives in `02-PROFILE-README.md`. Outline:

1. **Banner** (optional image) + **Header**: name, role, location, contact badges.
2. **Professional summary — English** (2–4 sentences).
3. **Ringkasan profesional — Bahasa Indonesia** (2–4 kalimat).
4. **Tech stack / core skills** with level + tag badges.
5. **Featured projects (3–5)**: name, 1-line description, tech stack, demo/CTA link.
6. **GitHub stats & top languages** (badges/cards).
7. **Footer**: contact, LinkedIn, website, availability.

Mobile note: GitHub collapses tables and shrinks images on mobile. Keep tables ≤ 3 columns, keep badge rows short, and avoid side-by-side HTML `<img>` blocks wider than ~860px.

---

## 3. Pinned Repos Recommendation (4–6)

Pin these, in this order. Rationale and a documentation checklist are included. Filled README templates are in `templates/`.

| # | Repo | 1-sentence description | Why pin it |
|---|---|---|---|
| 1 | `manage-kost-app` | Web app to manage a Muslim boarding house (kost) for an orphanage in Malang. | Real client/social-impact project — strongest "this solves a real problem" signal. |
| 2 | `laravel11-midtrans-payment-gateway` | Laravel 11 integration with the Midtrans payment gateway. | High-value, locally relevant skill; payments are a strong hiring signal. |
| 3 | `laravel-filament-cashier` | Subscription billing with Laravel Cashier inside a Filament admin panel. | Already has a star; shows admin panels + billing depth. |
| 4 | `laravel11-breeze-shop` | Full e-commerce store built on Laravel 11 + Breeze. | End-to-end product flow (catalog, cart, checkout). |
| 5 | `portfolio` | Personal portfolio site (live at qiffym.vercel.app). | Live demo + shows front-end/Next.js + design taste. |
| 6 | `eling-react-ts` (+ `api.eling`) | React + TypeScript front-end with a Laravel API backend. | Demonstrates decoupled full-stack architecture. |

**Per-repo documentation checklist (apply to each pinned repo):**
- [ ] One-line GitHub description set (Settings → top of repo).
- [ ] Topics/tags added (e.g. `laravel`, `php`, `react`, `typescript`, `midtrans`).
- [ ] README with: title, badges, screenshot/demo, features, tech stack, quick start (≤ 5 min), usage, license.
- [ ] Live demo or screenshots/GIF included.
- [ ] `.env.example` present and referenced in quick start.
- [ ] `LICENSE` file (MIT recommended).
- [ ] `CONTRIBUTING.md` (use template) if open to contributions.

---

## 4. Repo README Templates

- `templates/REPO-README-TEMPLATE.md` — generic skeleton (badges, install, screenshot, demo blocks).
- `templates/CONTRIBUTING-TEMPLATE.md` — short contribution guide.
- Filled, project-specific versions:
  - `templates/repo-manage-kost-app.md`
  - `templates/repo-laravel11-midtrans-payment-gateway.md`
  - `templates/repo-laravel-filament-cashier.md`
  - `templates/repo-laravel11-breeze-shop.md`
  - `templates/repo-portfolio.md`

Each filled README is written to meet the "runnable demo in ≤ 5 minutes" criterion.

---

## 5. Visual Design

See `03-VISUAL-DESIGN.md` for the palette, typography, banner size/text, and avatar guidance. Summary: single accent color, dark-on-light high contrast, web-safe fonts, 1280×320 banner.

---

## 6. Step-by-Step Implementation (for a cheaper AI model / human)

> The profile README repo is `qiffym/qiffym`. Its root `README.md` is what shows on the profile.

**Phase A — Profile README (highest impact, lowest effort)**
1. Open `02-PROFILE-README.md` in this folder.
2. Replace every `REPLACE_*` placeholder (LinkedIn URL, email, etc.) with real values.
3. Copy the entire content into `qiffym/qiffym` root `README.md`.
4. Commit: `docs: revamp profile README (EN + ID)`.

**Phase B — Profile settings (manual, GitHub UI)**
1. Set **Bio**: `Full-stack web dev · Laravel + React/Next.js · Malang, ID`.
2. Add **Social links**: LinkedIn, website (qiffym.vercel.app), email.
3. Upload a clean **avatar** per `03-VISUAL-DESIGN.md`.

**Phase C — Pin repos**
1. Profile → "Customize your pins" → select the 4–6 repos from §3 in the listed order.

**Phase D — Repo descriptions & topics (per pinned repo)**
1. Add the 1-sentence description from §3 to each repo.
2. Add topics/tags.

**Phase E — Repo READMEs (per pinned repo)**
1. For each pinned repo, copy the matching `templates/repo-*.md` into that repo's `README.md`.
2. Fill placeholders (screenshots, demo URL, env vars).
3. Add `.env.example`, `LICENSE`, and `CONTRIBUTING.md` (from template) as needed.
4. Commit each repo separately.

**Phase F — Verify success criteria**
1. View profile on desktop + mobile (GitHub mobile app or narrow browser).
2. Confirm EN + ID summaries render.
3. Time yourself running one pinned demo from a clean clone — must be ≤ 5 min.

---

## 7. Constraints & Assumptions (from brief)
- Do **not** modify code in any repo without the owner's approval — this plan only touches docs/README/profile assets.
- Owner provides access/screenshots/env values where placeholders exist.
- No paid assets or copyrighted logos are created here.
