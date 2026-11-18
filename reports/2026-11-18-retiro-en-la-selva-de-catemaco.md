# Retiro en la selva de Catemaco — landing page audit
URL: https://almawellness.io/experiencias/retiro-en-la-selva-de-catemaco
Audited: 2026-11-18

## Summary
Structurally this page is in good shape — single clear CTA, full pricing, a real cancellation-policy table, and complete logistics (dates, location, group size, language). The recurring brand-voice problem seen on other listings (template emoji used as section icons) is present here too, and there are a couple of small content inconsistencies in the inclusions copy plus missing image alt text.

## Brand voice findings
- **Emoji used as structural icons, which the brand book bans outright:** "Lo que te llevas 🌿 Transformación ✦ Presencia 🌬 Calma 🤍 Conexión" and "📍 Cabañas Ixaya, Dos Amates" near the location link. This is the same template pattern flagged on other audited listings (e.g. `codigo-origen`) — it looks like a shared component, so a single fix would likely clear it site-wide.
- **No exclamation marks, no ALL CAPS, no Title-Case-for-emphasis headlines** — confirmed against the raw HTML's rendered text; headings like "Qué incluye," "Política de cancelación," and "Elige una fecha" are properly sentence case, and the title "Retiro en la selva de *Catemaco*" only capitalizes the proper noun.
- **Tú voice used correctly and warmly:** "Lo que te llevas," and the primary CTA "Reservar mi lugar →" is the first-person self-claiming phrasing the brand book explicitly allows.
- **No overclaimed medical/therapeutic results.** "Limpias energéticas con especialistas locales" and "barroterapia tradicional" are named as practices/activities, not framed as cures — this stays on the right side of the line.
- **Minor stylistic note, not a hard violation:** "paz absoluta" ("absolute peace") in the host description leans toward the kind of blanket superlative the brand book warns about, though it's not a "la mejor de México" / "#1" claim. Worth a look if tightening the contemplativo voice further.
- **Host/venue description reads warm and specific, not corporate:** "Son construcciones ecológicas en bambú y piedra integradas al entorno natural, con interiores de bambú, ambiente ceremonial, jardines exuberantes, comedores y hamacas, en un entorno de selva y niebla" — concrete, sensory language that matches the intended tone.

## Conversion UX findings
- **Single clear primary CTA, easy to find:** "Reservar mi lugar →" sits in the booking widget alongside the price, with a secondary sticky "Reservar →" bar for mobile — no excessive scrolling needed.
- **Pricing is mostly clear but one phrase introduces ambiguity:** the page states "Paquete base de ejemplo: 4 días / 3 noches por $3,000 MXN por persona, personalizable" — calling the shown package "de ejemplo" ("as an example") next to a real checkout widget with a "Total $3,000" summary could make a buyer unsure whether $3,000 is the actual price or just an illustrative placeholder.
- **Inclusions list doesn't fully match the body copy:** "Qué incluye" lists "3 noches de hospedaje, 2 tours, 1 temazcal tradicional guiado, 3 desayunos y 2 cenas," but the longer description separately mentions "comidas" (lunches) and "pizzas caseras" that aren't reflected in the formal inclusions list — minor but creates room for a buyer to wonder what's actually covered. There's also no "no incluye" (not included) section at all.
- **No trust signals beyond the venue description:** no reviews, ratings, or past-attendee testimonials; the "especialistas locales" running the limpias energéticas aren't named or credentialed (only the logistics contact, Andrés Barboza, is named). For a 4-day/3-night commitment this is a credibility gap.
- **Date shown without a year:** "3 dic → 6 dic" — presumably 2026, but the page never states it, which is a small but avoidable ambiguity.
- **Missing alt text:** all four gallery images (each rendered twice as background/foreground layers) have `alt=""` — an accessibility and SEO gap, not just a nitpick.
- **Mobile viewport meta tag is present** (`width=device-width, initial-scale=1`), so no responsiveness red flag there.

## Recommended changes, prioritized
1. **Critical** — Remove the emoji (📍🌿🌬🤍) from the shared "what you'll take away" / location components; this is a hard brand-voice rule and the same component appears to be reused across other listings.
2. **Important** — Drop "de ejemplo" from the pricing description, or make clear what parts of the package are customizable vs. fixed, so the $3,000 total reads as a firm price.
3. **Important** — Reconcile the inclusions list with the body copy (lunches, "pizzas caseras") and add a "no incluye" section so buyers know exactly what's covered.
4. **Nice to have** — Name/credential the "especialistas locales" leading the limpias energéticas, or at least note their background, to close the trust-signal gap.
5. **Nice to have** — Add the year to the displayed dates, and fill in real `alt` text on the gallery images.
