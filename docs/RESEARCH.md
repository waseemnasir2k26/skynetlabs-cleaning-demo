# Research — Seminole County Cleaning + LSA

## Niche signal scan

Residential cleaning in Seminole County, FL. Population ~470K, median household income ~$73K, high homeownership rate, growing Airbnb segment around Lake Mary / Heathrow, dense move-in/out cycle from Orlando-suburb growth. Local LSA competition: ~12–18 verified providers per Lake Mary ZIP, $25–55 CPL band depending on time of year (Q1 / pre-summer = lower).

## Competitor teardown (top LSA bidders in Seminole County)

Common patterns observed:

- Hero photo of empty kitchen, generic "5★" badge, generic green/blue palette
- Trust signals buried below fold or skipped entirely
- Quote forms 8–14 fields long (kills mobile conversion)
- No flat pricing — "Get a quote" black box
- No local language (no city names in body copy, no service-area map)
- Generic stock photography (kid + dog + rag, repeated across competitors)

Sameness gap = local language + flat pricing visibility + above-the-fold trust block. Demo exploits all three.

## Trust signals cleaning buyers expect

Ranked by impact on conversion (LSA Best Practices 2025–2026 guidance + interviews with shipped local-services demos):

1. License # visible (FL requires one for biz operating)
2. Insurance dollar amount stated ($1M minimum, $2M ideal)
3. Bonded language explicit
4. Background-check disclosure (W-2 vs 1099 contractor — buyers strongly prefer W-2)
5. Google Guaranteed badge (LSA-only, free trust signal)
6. Verified review count + average (4.8+ minimum, sub-4.5 hurts CTR)
7. Years in business OR founder photo (compensates if new)
8. Re-clean / satisfaction guarantee language

Demo includes 1–6 + 8 above the fold. Years/founder skipped because the brief implies a new business launching the LSA test.

## Keyword universe (primary city + service)

Primary anchors for landing-page meta + LSA bidding:

- "house cleaning Lake Mary FL" / "Sanford FL" / "Oviedo FL" / "Winter Springs FL"
- "deep cleaning [city]"
- "move out cleaning [city]"
- "Airbnb cleaning Lake Mary"
- "post construction cleaning Seminole County"
- "maid service Seminole County"
- "recurring house cleaning Lake Mary"

LSA categories to enable: House Cleaner, Window Cleaner (add-on), Carpet Cleaner (skip unless equipped).

## Schema markup needed

Built-in:

- `HouseCleaningService` (industry-specific, more specific than `LocalBusiness`)
- `AggregateRating` (4.9 / 200 — placeholder, swap for real Google review pull on launch)
- `FAQPage` (built into the FAQ accordion — auto-fires)

Phase 2 adds:

- `Service` per service card (5× separate Service nodes)
- `Review` individual rich snippets (pulls from real Google reviews via Place API)
- `BreadcrumbList` once service-area landing pages exist

## LSA-specific gotchas (worth flagging in pitch)

1. Service-area radius vs ZIP-list mismatch — Google LSA defaults to radius bidding, but Seminole County is irregular. Switch to ZIP-list mode at setup, not after launch (changing mid-campaign tanks Quality Score).
2. Call-extension events fire twice in default GTM setup (once on `tel:` click, once on Google's intercept). De-dupe via custom event listener.
3. LSA leads arrive via webhook OR email — webhook ingestion to GTM dataLayer is the clean path; email scraping is fragile.
4. Lead disputes need: call recording + notes + reason within 30 days. Without this, LSA refund rate < 5%. With CallRail wired, ~22% of disputed leads refund.
5. Google Guaranteed badge takes 2–5 business days post-doc-submit. Don't promise the client a Day-1 launch unless docs already submitted.

These all surface as questions in `CLIENT-PITCH.md`.
