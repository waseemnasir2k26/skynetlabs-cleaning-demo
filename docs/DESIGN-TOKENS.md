# Design Tokens — Seminole Cleaning Demo

## Niche logic

Residential cleaning in central FL. Buyers are 35–55 homeowners + landlords + Airbnb hosts. Cleaning category = trust > beauty. Three variants test three taste poles so the client can self-select instead of guessing taste in a survey.

## V1 · Editorial (cream + sage)

| Token | Value | Use |
|---|---|---|
| `cream` | `#F5F1EA` | Page bg |
| `sage` | `#5C7A6B` | Primary accent · CTA hover · italic em |
| `sageDark` | `#3F5A4D` | Active states |
| `ink` | `#1F2A2A` | Body text · primary CTA bg |
| `claret` | `#8B3A3A` | Star ratings · ✦ separators |

Type: Fraunces (display, italic-friendly) + Inter (body). Dropcap, asymmetric image stack, marquee service-area band, giant background numerals 01/02/03 at 4% opacity.

Why this works: cleaning brands skew either ugly utility (Maids.com tier) or sterile clinical (Molly Maid blue). Editorial cream+sage signals premium-residential-but-warm — closer to a boutique hotel housekeeping department than a franchise.

## V2 · Cinematic (navy + mint)

| Token | Value | Use |
|---|---|---|
| `navy` | `#0A1628` | Section bg |
| `navyDeep` | `#050D18` | Page bg |
| `mint` | `#00E5A0` | Primary accent · CTA · gradient stops |
| `frost` | `#E8F4F0` | Body text |
| `sky` | `#0EA5E9` | Secondary gradient stop |

Type: Space Grotesk (display, geometric) + Inter (body). Gradient orbs (blur 80px, 50% opacity) drifting behind hero. Ken Burns hero image. Pulsing status dot ("Booking now").

Why this works: appeals to data-driven founders. The demo's analytical pitch — "measurably better" — frames the brand as a ScottsCleaning/MaidThis category-disruptor, not a mom-and-pop. Pairs naturally with LSA performance-marketing mindset.

## V3 · Minimal (white + sky)

| Token | Value | Use |
|---|---|---|
| `white` | `#FFFFFF` | Page bg |
| `black` | `#000000` | Borders · type · primary CTA |
| `sky` | `#0EA5E9` | Single accent — links · highlights · key sections |

Type: Inter Extrabold (display, brutalist) + JetBrains Mono (UI labels, "[ Seminole County / FL / 2026 ]"). Hard 2px black borders, grid-paper bg overlay, square corners (no border-radius).

Why this works: brutalism + monospace = trust through performance signaling. Reads as "we know what we're doing" without warmth — the V3 picker is the LSA-pure-conversion buyer. Aggressive CTAs ("→ GET QUOTE"), all-caps service tags, every claim datafied.

## Shared

- All variants `noindex,nofollow` until launch
- All CTAs emit `dataLayer.push({event, source, variant})` for GTM attribution
- Mobile sticky call bar shared across variants (ink/sage)
- Same JSON-LD schema across all
