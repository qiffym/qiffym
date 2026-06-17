# Visual Design Spec — @qiffym

Minimalist, high contrast, single accent color. Everything here is achievable for free with web-safe fonts and no paid/copyrighted assets.

## 1. Color Palette (single accent)

| Role | Color | Hex | Usage |
|---|---|---|---|
| Accent (primary) | Blue | `#2563EB` | Badges, links, headings, banner accent, stats cards |
| Accent (hover/dark) | Deep blue | `#1E40AF` | Hover states, secondary emphasis |
| Ink / text | Near-black | `#0F172A` | Body text, banner title |
| Muted text | Slate | `#64748B` | Captions, subtitles |
| Surface | White | `#FFFFFF` | Background (light) |
| Surface alt | Light gray | `#F1F5F9` | Cards, code blocks |
| Border | Gray | `#E2E8F0` | Dividers, borders |

> Keep it to **one accent** (`#2563EB`). All shields.io badges in the profile README already use `2563EB` so the look stays consistent. To rebrand, find/replace `2563EB` everywhere.

**Contrast check:** `#0F172A` on `#FFFFFF` ≈ 17:1, `#FFFFFF` on `#2563EB` ≈ 5.1:1 — both pass WCAG AA.

## 2. Typography (web-safe)

GitHub READMEs render in GitHub's own font stack, so don't fight it. For any custom image/banner you create, use these web-safe / free fonts:

| Use | Font | Fallback stack |
|---|---|---|
| Headings | **Inter** (free) or system UI | `Inter, "Segoe UI", system-ui, Arial, sans-serif` |
| Body | System UI | `system-ui, "Segoe UI", Roboto, Helvetica, Arial, sans-serif` |
| Code / mono | **JetBrains Mono** (free) or system mono | `"JetBrains Mono", "SFMono-Regular", Consolas, monospace` |

Rules: Headings **bold (600–700)**, body **regular (400)**, generous line spacing (1.5), max ~80 chars per line for readability.

## 3. Banner (GitHub profile / repo header)

- **Size:** `1280 × 320 px` (2:0.5 ratio). Safe area: keep text within the centered `1000 × 240 px` zone (sides get cropped on mobile).
- **Format:** PNG or SVG, < 1 MB.
- **Layout (left-aligned):**
  - Left: name + role.
  - Right: 3–4 tech badges/icons (Laravel, React, Next.js, TypeScript) at low opacity.
- **Background:** White `#FFFFFF` with a thin `#2563EB` accent bar/underline. No gradients, no clutter.
- **Suggested text:**
  - Line 1 (bold, ~64px): `Qiff Ya Muhammad`
  - Line 2 (~28px, muted `#64748B`): `Full-stack Web Developer — Laravel + React/Next.js`
  - Line 3 (~20px, accent `#2563EB`): `Malang, Indonesia · qiffym.vercel.app`

ASCII layout reference:
```
┌────────────────────────────────────────────────────────────┐
│  Qiff Ya Muhammad                          [Laravel] [React]│
│  Full-stack Web Developer                  [Next.js] [TS]   │
│  ──────────────────────  (accent #2563EB)                   │
│  Malang, Indonesia · qiffym.vercel.app                      │
└────────────────────────────────────────────────────────────┘
```

Free tools to produce it: Canva (custom 1280×320), Figma, or [capsule-render](https://github.com/kyechan99/capsule-render) for a code-only banner, e.g.:
```
![banner](https://capsule-render.vercel.app/api?type=waving&color=2563EB&height=200&section=header&text=Qiff%20Ya%20Muhammad&fontColor=ffffff&fontSize=48&desc=Full-stack%20Web%20Developer&descSize=20&descAlignY=62)
```

## 4. Avatar

- **Size:** at least `460 × 460 px`, square, displayed as a circle by GitHub.
- **Style:** clean headshot on a plain light/neutral background **or** a simple monogram “Q” in `#2563EB` on white.
- **Consistency:** use the same avatar on GitHub, LinkedIn, and the portfolio so the brand reads as one person.
- Avoid: busy backgrounds, low resolution, group photos, copyrighted characters.

## 5. Consistency Checklist
- [ ] Accent `#2563EB` used everywhere (badges, banner, stats cards).
- [ ] One avatar across GitHub / LinkedIn / portfolio.
- [ ] Same name + role tagline across all surfaces.
- [ ] Banner safe-area respected (readable on mobile).
- [ ] Light background, high-contrast text, no more than one accent color.
