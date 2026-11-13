# Autopilot Off: Tu vida como jardín — landing page audit
URL: https://almawellness.io/experiencias/autopilot-off-tu-vida-como-jardin
Audited: 2026-11-13

## Summary
Structurally this page is solid: logistics, pricing, inclusions and cancellation terms are all clear and upfront, and the single "Reservar" CTA is easy to find (including a sticky bottom bar). The copy itself is mostly on-voice (tú, sentence case, no exclamation marks, no overclaimed results), but the page breaks the no-emoji rule outright and leans on a presale strikethrough-price pattern that reads as e-commerce discount-shouting rather than Alma's curated tone.

## Brand voice findings
- **Emoji violation (hard rule):** the "Lo que te llevas" section uses emoji as bullet markers — `🌿 Transformación ✦ Presencia 🌬 Calma 🤍 Conexión` — and the address line uses `📍 3 Camino a los Azulejos...`, and the price box uses `🎟 Preventa`. That's 6 emoji instances on one page against a hard "no emoji, anywhere" rule.
- **Discount-shouting / e-commerce pricing pattern:** `🎟 Preventa $ 1,500 $ 1,200 MXN · por persona` shows a crossed-out "original" price next to a lower "presale" price, plus a quantity selector capped at "20 lugares." This is a standard e-commerce urgency/discount pattern the brand book calls out to avoid, even without an exclamation mark attached.
- **tú/usted and sentence case:** clean. Copy consistently uses tú register (e.g. "¿Quién diseñó tu jardín?", "Reservar mi lugar"), and all headings/labels ("Qué incluye," "Sobre House of Hoomans," "Política de cancelación") are sentence case, not Title Case or ALL CAPS.
- **No exclamation marks, no overclaimed therapeutic results:** clean. The host-description copy ("buscamos generar espacios de conexión auténtica, exploración y crecimiento personal y colectivo") stays descriptive rather than claiming medical/therapeutic outcomes.
- **Minor tone inconsistency:** the itinerary mixes English into otherwise Spanish copy — "Healthy break" and "Healthy snack break" — which reads as an un-curated, slightly generic word choice rather than "curado" (every word deliberate).

## Conversion UX findings
- **Primary CTA:** clear and prominent — "Reservar mi lugar →" in the booking widget plus a persistent sticky footer bar ("$1,200 · antes $1,500 · Reservar →"). No excessive scrolling needed.
- **Pricing:** fully transparent — base price, presale discount, per-person total, and an optional flexible-cancellation add-on (+$120 MXN) are all shown before checkout, with no hidden costs implied.
- **Logistics:** complete and upfront — date (sáb, 28 de nov de 2026), check-in time, 4h duration, group size (30 people), language, full venue address with a Google Maps link, what's included/excluded, and what to bring.
- **Trust signals — gap:** there's a short "Sobre House of Hoomans" blurb (host community description) and a "Pago seguro con Stripe" note, but no individual facilitator bio/credentials and no reviews or testimonials anywhere on the page — a social-proof gap for a first-time visitor deciding whether to trust this host.
- **Cancellation terms:** clear and graduated (100% refund >15 days out, 50% at 8–14 days, no refund ≤7 days), which is good-faith and transparent.
- **Technical:** the page does include a mobile viewport meta tag (`width=device-width, initial-scale=1`), so no mobile-responsiveness issue. No broken links observed. Roughly a dozen images are pulled from a Supabase storage bucket; file sizes weren't visible in the HTML so page weight can't be assessed from this audit.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji (🌿 ✦ 🌬 🤍 📍 🎟) and replace with plain text or a non-emoji icon/typographic marker; this is a flat violation of the hard "no emoji" rule.
2. **Important** — Rework the "Preventa $1,500 → $1,200" strikethrough-price presentation into Alma's own voice (e.g. state the current price plainly, or explain the presale window in a sentence) instead of the discount-shouting pattern.
3. **Important** — Add a short facilitator/host bio with credentials, and surface any reviews or past-attendee social proof if they exist, to close the trust-signal gap.
4. **Nice to have** — Replace "Healthy break" / "Healthy snack break" with Spanish equivalents for voice consistency.
