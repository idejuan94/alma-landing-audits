# Breath and Sound — landing page audit
URL: https://almawellness.io/experiencias/breath-and-sound
Audited: 2026-10-23

## Summary
The page is well-structured and mostly on-brand in its own written copy, but it inherits two sitewide issues (emoji icons in the "Lo que te llevas" block, empty `alt` text on all images) and has one real data-integrity problem: the displayed group size contradicts the booking widget's capacity. Host bio has minor typos and an emoji sign-off. Overall: basically solid, with one critical logistics bug and some polish items.

## Brand voice findings
- **Tú, not usted — compliant.** All copy ("vamos a explorar," "Un espacio para soltar, recargar y reconectar contigo mismo") stays in second person informal. No violations found.
- **Sentence case — compliant in Alma's own copy.** Section headers ("Lo que te llevas," "Qué incluye," "Política de cancelación") and body copy are sentence case. The experience title "Breath and Sound" is Title Case, but that reads as the proper name of the session (an English-language product name), not emphasis styling, so it's a judgment call rather than a clear violation.
- **No exclamation marks — compliant.** None found anywhere on the page.
- **Emoji — violation (sitewide, not page-specific).** The "Lo que te llevas" section renders literal emoji as icons: `🌿 Transformación`, `✦ Presencia`, `🌬 Calma`, `🤍 Conexión`. Confirmed in the raw HTML as `<span class="outcome-emoji">🌿</span>`, i.e. real emoji characters in content, not a CSS icon font. This exact block and emoji set also appears unchanged on `casa-sal-x-wellnest`, so it's a template-level violation affecting every listing, not something specific to this host.
- **Emoji in host bio — minor violation.** The bio sign-off reads: *"Gracias por estár aquí, HARI OM 🕉️"* — an emoji, plus a typo ("estár" should be "estar," no accent).
- **No empty superlatives or false urgency — compliant.** "esta sesión única" ("this one-time session") is accurate scheduling language (it only runs once, on Nov 26), not an inflated superlative like "la mejor experiencia." No "¡Reserva YA!," no countdown pressure, no discount-shouting.
- **No overclaimed therapeutic results — compliant.** The copy stays descriptive and process-oriented: *"La respiración es el puente entre el cuerpo y la emoción"* and *"Un espacio para soltar, recargar y reconectar contigo mismo"* — no claims of curing or medically treating anything.
- **Tone — mostly on-brand.** The core description (*"Una experiencia multisensorial que une respiración, música en vivo y vibración sonora"*) is warm and contemplative, in line with Alma's voice. The host bio, by contrast, runs long and reads as a generic host self-introduction ("Cuento con formación en Hatha, Vinyasa, Ashtanga y Vinyasa creativa, así como un diplomado...") rather than curated — this is host-submitted content Alma is publishing as-is, worth a light editorial pass.

## Conversion UX findings
- **Critical data mismatch: group size vs. booking capacity.** The logistics panel states *"Grupo: Grupo de 25 personas,"* but the booking widget's quantity selector only goes from 1 to 10 ("10 lugares," options 1–10). A visitor reading "grupo de 25" has no way to tell whether this is a 25-person group event with only 10 public seats left, or a data-entry error that should say 10. This is confusing enough to cost a booking and should be reconciled or clarified with copy (e.g., "10 lugares disponibles de un grupo de 25").
- **Single clear primary CTA — compliant.** "Reservar" appears at the top near the price, a sticky "Reservar →" persists, and the booking panel's "Reservar mi lugar →" is unambiguous and easy to find without excessive scrolling.
- **Pricing clarity — compliant.** Single tier, $750 MXN per person, clearly displayed in three places; the optional flexible-cancellation add-on (+$120 MXN) is disclosed, not hidden.
- **Logistics upfront — compliant.** Date (Thu, Nov 26, 2026), check-in time, 2h duration, full address with a Maps link, included/not-included items, and a full itinerary are all present before the booking panel.
- **Trust signals — weak.** The only trust/safety signal on the page is "Pago seguro con Stripe." There's no review count, no verification badge, and no testimonial — consistent with the rest of the site's early-stage listings, but worth noting as the catalog grows.
- **Cancellation policy — clear and tiered**, with specific windows (14+ days / 7–14 days / 48h–7 days / <48h) and their refund terms spelled out.
- **Accessibility/UX nit: all images have empty `alt=""`.** Confirmed in the raw HTML for every gallery image (`<img ... alt=""/>`). This is a sitewide pattern across both audited listings, not unique to this page.
- **Mobile viewport — compliant.** `<meta name="viewport" content="width=device-width, initial-scale=1"/>` is present in the page head.
- **Image weight — not assessable.** The image host (`*.supabase.co`) is outside this environment's network allowlist, so file sizes could not be checked this run.

## Recommended changes, prioritized
1. **Critical** — Resolve the 25-person vs. 10-seat mismatch in the group-size field so a visitor can tell whether 25 is the full group or a data error.
2. **Important** — Remove or replace the emoji icons in the "Lo que te llevas" block sitewide (template-level fix, not page-specific) to comply with the no-emoji brand rule.
3. **Important** — Add descriptive `alt` text to listing images sitewide for accessibility.
4. **Nice to have** — Light edit on the host bio: fix "estár" → "estar," tighten the credentials list, and consider trimming or removing the "HARI OM 🕉️" sign-off emoji to stay emoji-free.
