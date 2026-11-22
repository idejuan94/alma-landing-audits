# Moon's Ocean Retreat — landing page audit
URL: https://almawellness.io/experiencias/moons-ocean-retreat
Audited: 2026-11-22

## Summary
This is the highest-priced listing audited so far ($35,000 MXN/person) and reads noticeably more like luxury-travel marketing than Alma's contemplative voice ("lujo," "premium," "universo"), without crossing into the hard-rule violations (no exclamation marks, no overclaimed medical results, no ALL CAPS). The bigger issue is a booking-widget bug: the people-selector changes but the total price doesn't, which is a real risk of under-charging or confusing a buyer at this price point.

## Brand voice findings
- **Emoji (hard rule, site-wide template issue):** 🌿 🌬 🤍 📍 ✦ from the same shared template components flagged on other listings today.
- **Tone drifts toward generic luxury-travel marketing:** "exclusivo," "lujo," "premium," and describing Pilates as a "universo" read as aspirational travel-brand copy rather than Alma's warm-but-plain voice. None of these are empty superlatives about outcomes ("la mejor," "#1") so they don't trip the hard rule, but they're the clearest example today of copy that "reads generic/corporate/salesy instead" of curated.
- No exclamation marks, no ALL CAPS, no overclaimed therapeutic/medical results — the wellness language stays soft and non-clinical ("volver al cuerpo," "prácticas somáticas").

## Conversion UX findings
- **Booking widget bug:** the quantity selector shows "5 lugares" but the total stays fixed at $35,000, which is the per-person price. If this is meant to scale with group size, it's broken; if it's intentionally per-person-only, the selector is misleading as presented. Worth a human checking the live checkout flow directly, since this is the kind of bug that causes either lost revenue or an angry customer at checkout.
- CTA is clear ("Reservar mi lugar →," sticky bar).
- Logistics are thorough and honest: exact dates, 4-day/3-night structure, detailed day-by-day itinerary, what's included (transport from meeting point, all meals, certified staff) vs. explicitly not included (flights, own return booking) — this is a good example of the "honesto" pillar in practice.
- No reviews, ratings, or verification badge visible — the most significant trust gap of today's four listings given this is also the highest price point.
- Images carry empty `alt=""` attributes — same site-wide gap as other listings.

## Recommended changes, prioritized
1. **Critical** — Verify/fix the group-size selector vs. total-price behavior in the booking widget before more bookings go through at this price point.
2. **Important** — Add reviews, ratings, or host/biologist-team credentials — the page mentions "certified local staff" and "the team's biologist" but doesn't substantiate either; a line of credentials would help at this price.
3. **Nice to have** — Tone down "lujo"/"premium"/"universo" language toward Alma's plainer, more contemplative register; add alt text to images.
