# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [2026.10] - 2026-10-12

- skynetlabs-cleaning-demo ('Sparkline') is a public speculative landing-page demo for a residential cleaning business in Seminole County, FL, with three design variants in one static `index.html`.
- State: single static page plus `docs/` (research, design tokens, client pitch); last build commit 2026-05-02; no markup or config changes this month.
- Reviewed October 2026: README, tree and history read; the only README link (skynetjoe.com) returns 200. A MIT LICENSE file was added because the README states MIT.
- Known gaps: the page is deliberately noindex,nofollow (speculative demo); the GTM container is documented as a later phase and not wired; no tests or live URL in the README.

## [2026.09] - 2026-09-16

- Maintenance review of skynetlabs-cleaning-demo ("Sparkline") — a speculative landing-page demo by SkynetLabs for a residential cleaning business in Seminole County, FL, built around a Google LSA test campaign.
- Status: single static `index.html` (~30 KB gzipped) with three design variants (V1 Editorial, V2 Cinematic, V3 Minimal) behind a sticky switcher and `#v1`/`#v2`/`#v3` deep links. Pure HTML + Tailwind CDN + vanilla JS, no build step. Includes an LSA trust block, service-area band, flat-price service cards, FAQ accordion, mobile sticky call bar, LocalBusiness + AggregateRating JSON-LD, and dataLayer events (`lead-form-submit`, `phone-click`, `quote-cta`) with source/variant attribution.
- Supporting docs are versioned in `docs/`: RESEARCH.md, DESIGN-TOKENS.md, CLIENT-PITCH.md. Last commit was 2026-05-02, the original three-variant build.
- Reviewed September 2026: docs refreshed, versioned as v2026.09. No markup, asset or config changes in this release.
- Known gaps, all pre-existing: the page is deliberately `noindex,nofollow` (meta, robots.txt and a `vercel.json` header) because it is speculative; the GTM container is documented as Phase 2 and is not wired; README says MIT but there is no LICENSE file; no CHANGELOG.md before this release; no live URL is stated in the README.
