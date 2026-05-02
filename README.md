# Sparkline — Seminole County Cleaning Demo

Speculative landing page for residential cleaning + Google LSA test campaign. Three design variants in a single HTML file with a sticky variant switcher (top-right). Client picks → polish → ship.

## Variants

| | Axis | Vibe |
|---|---|---|
| **V1 · Editorial** | Cream + sage + claret accents · Fraunces serif · magazine grid | Premium, warm, residential |
| **V2 · Cinematic** | Navy + electric mint · Space Grotesk · gradient orbs + Ken Burns | Modern, tech-forward, conversion-tuned |
| **V3 · Minimal** | White + sky blue · brutalist grid · monospace + extrabold sans | Bold, confident, performance-marketing native |

## What's wired

- Google LSA-ready trust block (license #, $2M insured, Google Guaranteed badge)
- Service-area band (Lake Mary, Sanford, Oviedo, Winter Springs, Altamonte, Casselberry, Longwood, Heathrow)
- Six service cards with flat pricing
- 3-step process timeline
- Verified-review carousel (6 unique testimonials per niche, no copy-paste)
- 6-question FAQ accordion
- Mobile sticky call bar
- LocalBusiness + AggregateRating JSON-LD schema
- `noindex,nofollow` (vercel.json header + meta + robots.txt)
- All CTAs emit dataLayer events ready for GTM (`lead-form-submit`, `phone-click`, `quote-cta`) with `source` + `variant` attribution

## GTM wire-up (Phase 2)

1. Drop GTM container snippet in `<head>`
2. Trigger: Custom Event = `lead-form-submit` → GA4 conversion + LSA offline-conversion upload
3. Trigger: Custom Event = `phone-click` → GA4 conversion + Google Ads call event
4. Trigger: Custom Event = `quote-cta` → micro-conversion (engagement)
5. Server-side container optional ($35/mo Stape) for clean iOS attribution

## Stack

Pure HTML + Tailwind CDN + vanilla JS. No build step. ~30 KB gzipped.

## Local

Open `index.html` in any browser. URL hashes (`#v1` `#v2` `#v3`) deep-link to a specific variant — share with the client to focus a review round.

## Demo by

[SkynetLabs](https://skynetjoe.com) · MIT
