# Sonoterapia individual — landing page audit
URL: https://almawellness.io/experiencias/sonoterapia-individual
Audited: 2026-10-13

## Summary
The page's structure, pricing, and logistics are solid and conversion-friendly, but it has two hard brand-guideline violations: an overclaimed therapeutic/medical benefit sentence and six emoji used as UI decoration throughout the page. These are easy, contained fixes rather than structural problems — the rest of the page (CTA placement, cancellation terms, host bio) is in good shape.

## Brand voice findings
- **Overclaimed therapeutic/medical results (critical).** The practice description states: *"Su vibración permite que regresemos a un estado original de armonía, salud y relajación facilitando **la sanación del cuerpo**, **mejorando la calidad del sueño** y liberando el estrés acumulado del día a día."* This asserts the session heals the body and improves sleep quality as settled fact, not a curated, subjective offering. This is exactly the overclaiming the brand book prohibits — Alma curates experiences, it doesn't promise medical outcomes.
- **Emoji used throughout (critical).** Found in the page markup: the location line is literally `📍 A domicilio`; the "Lo que te llevas" section pairs each word with an emoji — `🌿 Transformación`, `✦ Presencia`, `🌬 Calma`, `🤍 Conexión` (the code even classes these `outcome-emoji`); and the host bio sign-off ends with `HARI OM 🕉️`. "No emoji, anywhere" is a non-negotiable rule, and this page has six distinct instances.
- **Tú voice, correctly used.** Copy consistently uses tú ("te acompaño," "Tú eliges el día y la hora," "Cada sesión se adapta a ti") and the CTA "Reservar mi lugar →" is the allowed first-person-claim exception. No usted anywhere.
- **No exclamation marks** found in any body copy, labels, or CTAs — compliant.
- **Generic/templated tone in one section.** The "Lo que te llevas" block (Transformación / Presencia / Calma / Conexión) reads like a stock wellness-marketing checklist rather than the specific, deliberate language used elsewhere on the page (e.g., the host bio is warm and particular — "Mi búsqueda por aprender y comprender mejor el yoga me llevó a Varkala, India"). Worth rewriting to sound as curated as the rest of the page.
- **Minor note:** "HARI OM" appears in full caps as a sign-off/mantra rather than stylistic emphasis — likely fine as a cultural convention, but flagging since it's the one piece of copy that isn't sentence case.

## Conversion UX findings
- **Clear, persistent CTA.** "Reservar" is available via a sticky bar, and "Reservar mi lugar →" / "Reservar →" repeat near the date picker and at the page bottom — no scrolling hunt required.
- **Logistics are upfront and complete.** Duration (1.5h), group size ("Grupo de 1 personas"), languages (Español, Inglés), location ("A domicilio · MX"), and flexible date selection are all shown before any CTA.
- **Pricing is transparent.** Single price ($2,300 MXN per person) shown consistently, with the only add-on (flexible cancellation, +$120 MXN) clearly itemized rather than hidden.
- **Cancellation policy is clear and tiered** (100% refund >15 days, 50% at 8–14 days, no refund ≤7 days), plus "Sin cargo hasta confirmar · Pago seguro" as a payment trust signal.
- **Missing alt text.** Every carousel `<img>` tag ships `alt=""` (empty) — e.g. `<img src=".../1791495013140-fxjdyij96m.JPG" alt="" class="gc-bg" .../>`. This is a real accessibility and SEO gap, not a guess — confirmed in the page's own markup.
- **No reviews, ratings, or host-verification badge** appear anywhere on the page. For a solo practitioner session like this, some form of social proof (reviews, a verified badge, or a completed-sessions count) would meaningfully reduce booking friction.
- **Viewport meta tag is present** (`width=device-width, initial-scale=1`) — mobile rendering is not a concern.
- **Image weight not assessable** — the carousel images are hosted on Supabase storage but could not be fetched directly from this audit environment to check file size, so no claim is made either way.

## Recommended changes, prioritized
1. **Critical** — Rewrite the sentence claiming the session facilitates bodily healing and improved sleep quality into subjective, non-medical language (e.g., describe what people tend to feel, not what the session delivers). Remove all six emoji instances (📍, 🌿, ✦, 🌬, 🤍, 🕉️) and replace with text-only equivalents consistent with the rest of the site.
2. **Important** — Add descriptive alt text to the three carousel images. Add at least one trust/social-proof signal (reviews, verified-host badge, or number of sessions held) since none currently exists on the page.
3. **Nice to have** — Rewrite the "Lo que te llevas" outcomes section to match the specific, curated tone of the host bio rather than reading as a generic wellness checklist.
