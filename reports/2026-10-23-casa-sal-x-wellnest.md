# Casa Sal x Wellnest — landing page audit
URL: https://almawellness.io/experiencias/casa-sal-x-wellnest
Audited: 2026-10-23

## Summary
This is the strongest-written listing audited so far: clean tú-voice copy, no exclamation marks, no overclaimed results, and thorough logistics (included/not-included, cancellation tiers, arrival-transport edge case). The main issues are the same sitewide template problems (emoji icons, empty image alt text) plus one soft UX ambiguity around the booking quantity cap. Structurally solid; no critical brand violations found in the host-written copy itself.

## Brand voice findings
- **Tú, not usted — compliant.** *"Cuatro días frente al mar para reconectar contigo"* and *"para que puedas moverte, descansar, conocer personas nuevas y simplemente volver a ti"* stay consistently informal second person.
- **Sentence case — compliant.** All section headers ("Lo que te llevas," "Qué incluye," "No incluye," "Qué llevar," "Sobre Casa Sal x Wellnest," "Política de cancelación") are sentence case. Item labels like "Welcome Kit," "Pilates Mat," "Sound Healing," and "Ice Bath" are Title Case, but these read as proper names of specific classes/products rather than emphasis styling — a minor stylistic inconsistency, not an ALL-CAPS or shouting violation.
- **No exclamation marks — compliant.** None found.
- **Emoji — violation (sitewide template, not this host's copy).** Same "Lo que te llevas" block as `breath-and-sound`: `🌿 Transformación`, `✦ Presencia`, `🌬 Calma`, `🤍 Conexión`, confirmed as literal emoji in the markup. Since this exact block is identical across listings, it's a template fix, not something to raise with this specific host.
- **No empty superlatives or false urgency — compliant.** No "mejor," no "#1," no "¡Reserva YA!," no countdown or discount-shouting language anywhere on the page.
- **No overclaimed therapeutic results — compliant.** The copy is careful to describe mechanism, not cure: *"Cada actividad trabaja una capa distinta —cuerpo, respiración y sistema nervioso— mientras dejamos espacio para descansar"* — this is honest and specific without medical overreach.
- **Tone — on-brand and arguably the best example audited so far.** *"No buscamos que el retiro se sienta rígido ni excesivamente espiritual: creemos en un wellness que también puede ser divertido, social y aspiracional"* is warm, honest about what the experience is (and isn't), and avoids generic corporate wellness-speak. "lujo relajado" ("relaxed luxury") and "aspiracional" lean slightly toward marketing language, but stay short of empty superlatives and fit the brand's honesty principle by being specific about what kind of experience this is.

## Conversion UX findings
- **Single clear primary CTA — compliant.** "Reservar" at top, sticky "Reservar →," and "Reservar mi lugar →" in the booking panel — consistent with the other listing and easy to find.
- **Pricing clarity — compliant.** $26,000 MXN per person, single tier, clearly shown in three places; the optional flexible-cancellation add-on (+$120 MXN) is disclosed up front.
- **Logistics upfront — strong.** Dates (Jan 29 → Feb 1, 4 days/3 nights), check-in time, full address, language options, and unusually thorough included/not-included lists — down to a specific edge case (*"Si tu vuelo de llegada es en un horario diferente al establecido para el grupo, podemos coordinar una van... Costo adicional: $400 MXN"*). This is a good example of the "honesto" (honest) brand value in action.
- **Minor ambiguity: group size vs. booking cap.** The page states "Grupo de 10 personas" while the booking widget caps at 4 ("4 lugares," selector 1–4). Unlike the `breath-and-sound` listing (25 vs. 10, unexplained), this gap is small enough to plausibly mean "6 of 10 spots already taken" — but the page never says so explicitly, so a visitor can't tell the difference between "almost full" and "data inconsistency." Worth a one-line clarification (e.g., "4 lugares disponibles de 10").
- **Trust signals — weak, same as the rest of the site.** Only "Pago seguro con Stripe" is present; no reviews, ratings, or verification badge.
- **Cancellation policy — clear**, with three plain tiers (15+ days / 8–14 days / 7 days or less).
- **Accessibility/UX nit: all images have empty `alt=""`.** Same sitewide pattern as `breath-and-sound` — confirmed in the raw HTML for all 5 gallery images.
- **Mobile viewport — compliant.** `<meta name="viewport" content="width=device-width, initial-scale=1"/>` present.
- **Navigation nit:** the top-nav "Inspirarme" link appears to point to the same route as "Experiencias" (`/experiencias`) rather than a distinct inspiration/video feed — likely a sitewide nav issue worth a human double-check, not specific to this listing.
- **Image weight — not assessable** this run; the asset host (`*.supabase.co`) is outside this environment's network allowlist.

## Recommended changes, prioritized
1. **Important** — Clarify the gap between "Grupo de 10 personas" and the 4-seat booking cap with a one-line explanation, so it doesn't read as a data error.
2. **Important** — Remove or replace the emoji icons in the "Lo que te llevas" block sitewide (same template issue flagged on `breath-and-sound`).
3. **Nice to have** — Add descriptive `alt` text to listing images sitewide.
4. **Nice to have** — Double-check whether "Inspirarme" in the top nav is meant to link somewhere other than `/experiencias`.
