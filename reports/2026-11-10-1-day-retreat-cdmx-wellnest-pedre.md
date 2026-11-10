# 1 Day Retreat CDMX Wellnest * Pedre — landing page audit
URL: https://almawellness.io/experiencias/1-day-retreat-cdmx-wellnest-pedre
Audited: 2026-11-10

## Summary
The page covers the logistics well (dates, pricing, cancellation policy, itinerary) and avoids exclamation marks and overclaiming, but it breaks two hard brand rules (all-caps title, emoji) and has enough internal inconsistencies (duration, naming, a booking-total bug) that it reads unpolished rather than "curado."

## Brand voice findings
- **ALL CAPS headline** — the page title is "1 DAY RETREAT CDMX WELLNEST * _PEDRE_". Sentence case is a hard rule; this should read something like "1 day retreat CDMX Wellnest · Pedre."
- **Emoji present** — 📍 (location), 🌿 (Transformación), 🌬 (Calma), 🤍 (Conexión) appear as pillar/section icons. Alma's rule is no emoji anywhere, so these need to go even in a decorative/iconographic role.
- **Naming inconsistency reads as unpolished, not "curado"** — the title calls it "1 DAY RETREAT," the body calls it "WELLNEST Morning Retreat." Minor, but it's exactly the kind of inconsistency the "every word deliberate" standard is meant to catch.
- Tone otherwise lands fine: no exclamation marks, no superlatives ("la mejor..."), no medical overclaiming. The closing line — "Porque en WELLNEST creemos que el bienestar se disfruta más cuando lo comparte mos" — is warm without being salesy, and tú form is used consistently ("reconectar contigo," "Reservar mi lugar →").

## Conversion UX findings
- **Booking total looks broken** — the widget shows 6 places selected with a total of "$777," but the stated per-person price is $777 MXN, so 6 places should total $4,662. This is either a real pricing bug or a confusing default-state display; either way it will make a buyer stop and distrust the checkout right before paying.
- **Duration mismatch** — the page states the retreat is 4h, but the itinerary runs 9:00 a.m.–12:00 p.m. (3 hours). Small, but it undercuts trust in the other logistics details.
- Trust signals are thin: no host bio/credentials, no reviews or testimonials for Wellnest, only "Pago seguro con Stripe" as a trust marker.
- What's working: a single clear CTA ("Reservar mi lugar →," also sticky in the footer), clear included/not-included list, clear cancellation tiers (100% / 50% / 0% refund by days-out), and a Google Maps link for the venue.

## Recommended changes, prioritized
1. **Critical** — Fix the booking-total calculation (or the default-selection display) so the price shown always matches places × per-person price before checkout.
2. **Critical** — Remove sentence-case and emoji violations: rewrite the title in sentence case and drop 📍🌿🌬🤍 in favor of text labels or non-emoji icons.
3. **Important** — Reconcile the 4h stated duration with the 9 a.m.–12 p.m. itinerary, and settle on one name for the experience ("1 day retreat" vs. "WELLNEST Morning Retreat") used consistently across the page.
4. **Nice to have** — Add even a short host bio/credentials line for Wellnest, since there's currently no trust signal beyond the payment processor.
