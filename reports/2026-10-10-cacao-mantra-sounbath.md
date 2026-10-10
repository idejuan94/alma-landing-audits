# Cacao * Mantra * Sounbath — landing page audit
URL: https://almawellness.io/experiencias/cacao-mantra-sounbath
Audited: 2026-10-10

## Summary
This page is basically solid. The Spanish copy is warm, specific, and reads as genuinely curated rather than templated, and logistics/pricing/cancellation terms are all clear and upfront. The one real brand issue is emoji use sprinkled through the body copy and the benefit-icon row, which breaks the hard "no emoji" rule; everything else is minor polish.

## Brand voice findings
- **Emoji in body copy:** "🤍Este mes dedicaremos nuestro encuentro a la Devi, la Madre Divina..." — a heart emoji opens the paragraph inline with the text. Hard-rule violation (no emoji, anywhere).
- **Emoji as benefit icons:** the "Lo que te llevas" row uses 🌿 Transformación · ✦ Presencia · 🌬 Calma · 🤍 Conexión — four emoji used as decorative markers. Same violation, and likely shared across other listing templates (worth a sitewide fix, not just this page).
- **Emoji in host sign-off:** the bio closes "Gracias por estár aquí, HARI OM 🕉️" — emoji again. ("HARI OM" itself is a genuine ceremonial phrase, not emphasis-caps abuse, so that part is fine on its own.)
- **tú voice:** correct and consistent — "Lo que te llevas," "Reservar mi lugar →." No *usted* anywhere.
- **No exclamation marks:** the raw HTML contains literal `!` characters, but all of them are React hydration comments (`<!-- -->`), not visible copy — the actual text has none. Compliant.
- **No superlatives, false urgency, or overclaimed medical results found.** The tone itself is a good example of the brand's contemplative register: "Juntamos la medicina del cacao, la vibración de los cuencos y la práctica del mantra para crear una experiencia profunda que nos invita a descansar el cuerpo y renovar el alma."

## Conversion UX findings
- **Primary CTA:** clear and singular — "Reservar mi lugar →," reinforced by a sticky header/mobile bar CTA. No excess scrolling needed.
- **Trust signals:** strong host bio (15+ years of yoga practice, named training lineage including time in Varkala, India) and a clearly tiered cancellation policy (100% refund 15+ days out, 50% at 8–14 days, none inside 7 days). No reviews or testimonials, and the directory page's claim "Cada experiencia verificada por el equipo de Alma" is not repeated on the listing itself — a missed trust-reinforcement opportunity.
- **Pricing:** fully clear — $450 MXN/person, $800 MXN for a group of 2, optional flexible-cancellation add-on for +$120 MXN. No hidden costs implied.
- **Logistics upfront:** date (Fri Oct 23, 2026), check-in time, 2h duration, group cap (22, with "10 lugares" remaining), language (Español), full address with a Google Maps link, minute-by-minute itinerary, and explicit included/not-included lists.
- **Friction:** all three gallery images have `alt=""` — no accessibility/SEO text. Nothing else looks broken; no walls of unbroken text (the long-form description is a single reasonably short paragraph); mobile viewport meta tag is present.

## Recommended changes, prioritized
1. **Critical** — Remove emoji from the body paragraph, the "Lo que te llevas" icon row (🤍🌿✦🌬), and the host bio sign-off (🕉️), per the brand's hard no-emoji rule. If this icon row is a shared template component, fix it once at the template level.
2. **Important** — Add descriptive alt text to the three experience images.
3. **Nice to have** — Surface the "verificado por el equipo de Alma" trust signal directly on the individual listing page, not only the directory.
