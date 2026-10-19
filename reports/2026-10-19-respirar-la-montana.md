# Respirar la montaña — landing page audit
URL: https://almawellness.io/experiencias/respirar-la-montana
Audited: 2026-10-19

## Summary
The page is well-written and structurally solid — logistics, pricing, host credentials, and cancellation terms are all upfront and honest, and the CTA is easy to find. It is pulled down by one hard brand-voice violation (emoji used throughout a feature list) and one real conversion bug: the directory card marks this listing "Agotado" (sold out) while the detail page itself shows three open dates with available spots.

## Brand voice findings
- **Emoji violation (hard rule break).** The "Lo que te llevas" section pairs every item with an emoji: "🌿 Silencio interior", "🌬 Respiración consciente", "🌄 Conexión con la naturaleza", "🤍 Descanso real", "✦ Claridad mental", "🌙 Presencia plena". Alma's brand book says no emoji anywhere — this is six separate instances on one page.
- **Tone lands correctly where it counts.** The intro copy — "Las montañas de Tepoztlán llevan siglos siendo lugar de encuentro entre lo humano y lo sagrado... entrar en otro tiempo: el tiempo de la respiración, del silencio y de la escucha interna" — and the pull-quote "El descanso profundo no es un lujo. Es la condición de todo lo demás." read as genuinely contemplativo and curado, not generic wellness marketing. No exclamation marks, no superlatives ("la mejor"), no fake urgency language, no overclaimed therapeutic results.
- **Person and case are correct.** Consistent tú throughout ("te invitamos", "Lo que te llevas"), and the one first-person CTA, "Reservar mi lugar →", is exactly the allowed exception. Headings ("Qué incluye", "No incluye", "Elige una fecha") are sentence case, not Title Case or caps.

## Conversion UX findings
- **Sold-out/available mismatch (real friction).** The directory listing shows this card with a "Agotado" badge and `soldOut: true` in the page data, making the card non-clickable from `/experiencias`. But the detail page itself (reachable directly, e.g. because a user bookmarked or was linked to it) lists three bookable dates with open spots: "Sáb 22 – Dom 23 nov: 4 lugares", "Sáb 6 – Dom 7 dic: 8 lugares", "Sáb 20 – Dom 21 dic: 12 lugares", plus a live "Reservar mi lugar →" CTA. A user arriving directly at the page would reasonably try to book; a user browsing the directory is told it's unavailable and never clicks through. This looks like a data sync bug between the listing feed and the detail page, not an intentional state.
- **CTA is clear and persistent.** "Reservar mi lugar →" sits with the date picker, and a sticky "Reservar →" bar with the price repeats at the bottom — single, unambiguous primary action, no scrolling hunt required.
- **Pricing and logistics are fully transparent.** Price ($2,400 MXN/persona) is shown twice, add-ons are itemized ("Habitación privada (disponible con cargo adicional)", "Masaje terapéutico (reserva aparte)", flexible-cancellation add-on at "+$120 MXN"), and "No incluye" explicitly calls out what's excluded (transporte). Date, duration, group size cap (14), language, and location (with a Google Maps link) are all stated before any scrolling is needed.
- **Trust signals present but thin.** Host bio ("María López... 12 años facilitando retiros... yoga terapéutico, meditación vipassana y trabajo somático") and a tiered, specific cancellation policy (100% / 50% / 0% refund by days-before) are both present and build real confidence. No reviews, ratings, or past-guest social proof appear anywhere on the page — a gap, though not unusual for a first-time or new host listing.
- **No technical red flags.** Mobile viewport meta tag is present, images are lazy-loaded and reasonably sized (600px-wide Unsplash sources), and no broken links or walls of unbroken text were observed.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji from the "Lo que te llevas" section; replace with plain sentence-case labels or a simple icon system that doesn't rely on emoji glyphs. This is a flat brand-book violation, not a style preference.
2. **Critical** — Fix the sold-out/availability data mismatch between the directory card and the detail page. Either the directory's `soldOut` flag is stale or the detail page is serving cached/incorrect date availability — a user should never see contradictory inventory state between the two.
3. **Nice to have** — Add at least a placeholder for reviews/social proof (even "primera experiencia en Alma" framing) once the host has guest history, to strengthen trust signals on an otherwise trust-light but well-reasoned page.
