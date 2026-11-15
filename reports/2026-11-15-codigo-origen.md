# Código origen — landing page audit
URL: https://almawellness.io/experiencias/codigo-origen
Audited: 2026-11-15

## Summary
Structurally the page is solid — pricing, dates, cancellation policy, and included/not-included lists are all present and clear. The main problems are brand-voice violations (emoji throughout, several typos undermining the "curado" tone) and a couple of small conversion-UX gaps (ambiguous secondary CTA label, no social proof, no safety note for intensive practices).

## Brand voice findings
- **Emoji used throughout, which the brand book bans outright:** the page uses 📍 (location), 🌿 (Transformación), ✦ (Presencia), 🌬 (Calma), and 🤍 (Conexión) as section/value markers. None of these are decorative accidents — they're used as structural icons, so this is a page-wide pattern, not a one-off.
- **Typos undermine the "curado" (every word deliberate) tone:** "expericia" (Día 1 copy), "reprogramacion" (missing accent, appears twice), "proprio" and "afore" in the room description (almost certainly meant "propio" and "aire"), and "Trasporte al lugar" in the not-included list. For a brand that positions itself as curated and deliberate, these read as careless.
- **Borderline generic/salesy phrasing:** each day of the itinerary is described as "única y mágica." It's not a banned superlative outright, but "mágica" repeated as a stock intensifier reads closer to generic retreat marketing copy than the "contemplativo" voice the brand book asks for.
- **No exclamation marks and no ALL CAPS/Title-Case headlines** — confirmed directly against the raw HTML's rendered text (only "!" occurrences are inside markup/scripts, none in visible copy). This part is clean.
- **No overclaimed medical/therapeutic results.** The host's "psicóloga, terapeuta y canalizadora" framing and language like "trabajo del inconsciente" and "reconocer patrones" stay in curation/facilitation territory rather than claiming to cure anything.

## Conversion UX findings
- **Ambiguous secondary CTA:** the booking-panel button reads "Elige un paquete" ("choose a package") rather than an action like "Reservar," so it reads as an instruction, not a call to act. The header CTA ("Reservar") is fine and sits above the fold.
- **No social proof anywhere on the page** — no reviews, testimonials, or past-attendee signals, despite the retreat being positioned as a significant time/money commitment ($33,000 MXN, 4 days).
- **No safety/screening note for physically intensive practices.** The itinerary includes temazcal, breathwork, and "trabajo del inconsciente" sessions with no visible contraindication note (e.g., pregnancy, cardiac conditions, claustrophobia) — a trust gap for anyone evaluating whether this is right for them.
- **Pricing, dates, location, group size, and cancellation policy are all clearly stated** — this part of the page does its job well, including a real refund table (100% >14 days, 50%/credit 7–14 days, credit-only 48h–7 days, no refund <48h) and a clearly priced flexible-cancellation add-on.
- **Gallery images appear duplicated in the markup** (each of 8 images renders twice) — worth a developer check, though it's not confirmable from rendered text alone whether this doubles actual page weight or is just redundant DOM.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji (📍🌿✦🌬🤍) and replace with plain text labels or sentence-case headers; this is a hard brand-voice rule.
2. **Important** — Fix the typos ("expericia," "reprogramacion," "proprio," "afore," "Trasporte") — quick copy pass, meaningful credibility fix.
3. **Important** — Rename "Elige un paquete" to an action-oriented CTA consistent with "Reservar."
4. **Nice to have** — Add a brief safety/screening note near the itinerary for temazcal/breathwork sessions.
5. **Nice to have** — Replace "única y mágica" with more specific, concrete language per day rather than a repeated stock intensifier.
6. **Nice to have** — Have engineering confirm/fix the duplicated gallery image elements.
