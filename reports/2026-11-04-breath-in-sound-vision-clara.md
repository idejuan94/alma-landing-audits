# BREATH IN SOUND: VISIÓN CLARA — landing page audit
URL: https://almawellness.io/experiencias/breath-in-sound-vision-clara
Audited: 2026-11-04

## Summary
The body copy is some of the most on-brand writing seen in this audit series so far — short, contemplative sentences that genuinely earn the "curado" tone. But the page's template-level defects recur here too: ALL-CAPS section headers break the sentence-case rule throughout, and the same recurring emoji outcome tags flagged on `bano-de-gong` (2026-11-03) show up again, confirming this is a component-level bug, not a one-off copy mistake. Conversion UX is otherwise solid.

## Brand voice findings
- **ALL CAPS section headers, hard rule violation.** The hero headline itself is rendered `BREATH IN SOUND: VISIÓN CLARA` (and the `<title>` tag matches: "BREATH IN SOUND: VISIÓN CLARA · BREATH IN SOUND · Alma"), and four section headers follow the same pattern: `LA EXPERIENCIA`, `¿QUÉ ES LA VISIÓN CLARA?`, `ESTO ES PARA TI, SI:`, `LO QUE TE LLEVAS`. Sentence case is a hard rule here — these should read "La experiencia," "¿Qué es la visión clara?," etc.
- **Emoji present, same recurring template bug as `bano-de-gong`.** The "Lo que te llevas" outcome tags use: 🌿 "Transformación", ✦ "Presencia", 🌬 "Calma", 🤍 "Conexión" — identical set to the previous audit. The location line also carries a 📍 pin emoji ("📍 131, Avenida Oaxaca, Roma Norte"). This confirms the emoji aren't copy errors on individual listings — they're baked into a shared component (outcome tags + location line) and will keep appearing on every new experience until fixed at that level.
- **Tú voice is consistent and well-executed.** No "usted" anywhere. Address is consistently second-person: "No necesitas experiencia previa," "Tu cuerpo lo sabe antes que tu cabeza," "Sientes que llevas tiempo dando vueltas." The CTA "Reservar mi lugar →" correctly uses first person for the self-claimed booking action.
- **No exclamation marks, no empty superlatives, no false urgency.** Nothing like "¡Reserva YA!" or "la mejor experiencia" appears. No countdown pressure or discount-shouting.
- **No overclaimed therapeutic/medical results — this is a clear improvement over `bano-de-gong`.** The closest the copy gets to a benefits claim is "Una mente más tranquila — no por control, sino por soltar," which is experiential and hedged, not a medical claim. Compare to `bano-de-gong`'s "regulación del sistema nervioso" language — this page avoids that trap entirely.
- **Genuinely strong "curado" tone in the body copy.** Example, quoted in full: *"No es un insight. No es una revelación. Es cuando el ruido baja — y lo que siempre estuvo ahí se vuelve obvio. Tu cuerpo lo sabe antes que tu cabeza. La respiración solo despeja el camino."* Short sentences, room to breathe, nothing generic or salesy — this is exactly the voice the brand book describes, and it's worth holding up as a reference example for other hosts' copy.

## Conversion UX findings
- **Single clear CTA, no scrolling needed.** "Reservar" is visible in the sticky header immediately, with "Reservar mi lugar →" in the booking widget and "Reservar →" repeated at the bottom.
- **Credible trust signals via host bio.** Ana Korff (breathwork facilitator) and Julia Klykova (DJ, somatic practitioner, sound healer) are named with specific roles and "más de 10 años de experiencia combinada." No reviews or ratings exist on the page — consistent with every other listing audited so far, so this looks like a platform-wide gap rather than this listing's problem.
- **Pricing is transparent.** $888 MXN per person, flexible-cancellation add-on disclosed at +$120 MXN, no hidden costs implied.
- **Cancellation policy is a clear, tiered table**: 100% refund past 14 days, 50%/credit at 7–14 days, credit-only inside 7 days, no refund inside 48 hours.
- **Logistics are upfront and complete**: exact date/time (Sun, Nov 8, 2026, 11:00–13:00), venue with a Google Maps link, language (Spanish), what's included, and a packing note ("Ropa comoda, aqua" — note the missing accent on "cómoda" and "agua," a minor typo).
- **Minor ambiguity — group size vs. booking cap.** The page states "Grupo de 13 personas" but the quantity selector only allows booking up to "5 lugares." It's unclear whether 13 is the full group size with 5 seats remaining, or whether this is a leftover template figure — the same ambiguity flagged on `bano-de-gong`'s 25-vs-15 mismatch. Likely intentional (remaining availability) but worth confirming since it reads as inconsistent on first glance.
- **Missing alt text on all images**, confirmed in the raw HTML: all three `<img>` tags on the page have `alt=""`. This is an accessibility and SEO gap, and like the emoji, looks like a template-level default rather than a per-listing choice.
- **Mobile-responsive viewport tag is present** (`<meta name="viewport" content="width=device-width, initial-scale=1"/>`), confirmed in raw HTML.
- **Image weight not assessed** — the three images are hosted on Supabase storage and this run couldn't verify file size or dimensions; no obvious red flag from the HTML alone.

## Recommended changes, prioritized
1. **Critical** — Fix sentence case across the hero headline, `<title>` tag, and all section headers (`LA EXPERIENCIA`, `¿QUÉ ES LA VISIÓN CLARA?`, `ESTO ES PARA TI, SI:`, `LO QUE TE LLEVAS`). This is a hard brand rule and currently breaks on every header on the page.
2. **Critical** — Remove the emoji from the outcome tags (🌿 ✦ 🌬 🤍) and the location pin (📍). This is the same component already flagged on `bano-de-gong` — fixing it there should fix it here and on every future listing at once.
3. **Important** — Add alt text to the three listing images; currently all are empty.
4. **Nice to have** — Clarify the "13 personas" vs. "5 lugares" relationship so it reads as remaining availability rather than a data mismatch. Also fix the missing accents in "Ropa comoda, aqua" → "Ropa cómoda, agua."
