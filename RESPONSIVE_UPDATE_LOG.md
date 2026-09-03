# Responsive Redesign — Update Log

**Date**: September 3, 2026  
**Commit**: `8553308`

---

## Changes Made

### 1. Responsive CSS (Mobile-First)
- Removed fixed `max-width: 480px` on `.cv` — now scales from 480px → 600px → 900px → 1400px
- All font sizes converted from `px` to `clamp()` for smooth scaling
- Avatar scales: 90px (mobile) → 110px (tablet) → 140px (desktop) → 180px (TV)
- Skills grid: 2 cols → 3 cols → 4 cols → 5 cols
- Language tags have `min-height: 44px` for touch targets on tablet+
- Body padding scales with `clamp(8px, 2vw, 24px)`

### 2. Breakpoints
| Screen | Width | Card Max | Avatar | Skills Cols |
|--------|-------|----------|--------|-------------|
| Mobile | 0-600px | 480px | 90px | 2 |
| Tablet | 601-1024px | 600px | 110px | 3 |
| Desktop | 1025-1440px | 900px | 140px | 4 |
| TV/4K | 1441px+ | 1400px | 180px | 5 |

### 3. Arabic Subtitle Fix
- Added `data-i18n="subtitle"` to `.subtitle` element
- Added `subtitle` key to all 4 language translations:
  - FR: "Designer Graphique & Développeur Web"
  - EN: "Graphic Designer & Web Developer"
  - ES: "Diseñador Gráfico y Desarrollador Web"
  - AR: "مصمم جرافيك ومطور ويب"

### 4. Viewport Meta
- Removed `maximum-scale=1.0, user-scalable=no` (accessibility improvement)

---

## Live Links

| Platform | URL |
|----------|-----|
| GitHub Pages | https://ucfzem.github.io/ucf-cv/ |
| Vercel | https://ucf-n5r7vizbg-ucfzem-s-projects.vercel.app |
| Cloudflare Pages | https://ucf-cv.pages.dev |
