# Retiro de 1 día EL LATIDO DEL BOSQUE — landing page audit
URL: https://almawellness.io/experiencias/retiro-de-1-dia-el-latido-del-bosque
Audited: 2026-11-24

## Summary
This page has more brand-voice problems than most new listings: an ALL CAPS title, two empty superlatives, and the same emoji violation seen across the site. Conversion UX is functional but has a few logistics inconsistencies (duration math, group-size mismatch) that should be cleaned up before this goes live-quality.

## Brand voice findings
- **ALL CAPS headline — hard rule violation.** The title itself reads "Retiro de 1 día EL LATIDO DEL BOSQUE" — the experience name is in full caps mid-headline, which the brand book explicitly flags regardless of surrounding sentence-case text.
- **Empty superlatives — hard rule violation.** The subheadline promises you'll "proyectar el mejor año nuevo," and the host bio adds "buscas la mejor versión de ti." Both are the kind of generic superlative claim the brand book calls out by name.
- **Emoji present — hard rule violation.** 🌿, 🌬, 🤍, 📍, and ✦ appear as inline icons, same pattern as other recently-audited pages.
- **Borderline overclaimed therapeutic language.** The host bio's "tecnologías sagradas de sanación y espiritualidad" frames the offering as a healing technology rather than a curated experience — it doesn't claim to cure anything specific, but it reads closer to a therapeutic promise than Alma's "curates, doesn't replace treatment" stance intends.
- **Tú used consistently, no exclamation marks.** "te abrazará," "date una pausa," and the rest of the hero copy stay correctly second-person informal with no exclamation marks.
- **Tone drifts toward generic wellness-marketing copy** in the hero paragraph ("los árboles guardianes, las abuelas rocas... te darán las respuestas") — poetic, but closer to stock retreat-ad language than the contemplative, deliberate voice the brand book asks for.

## Conversion UX findings
- **Single primary CTA, reasonably easy to find.** "Reservar mi lugar →" in the booking panel plus a sticky "Reservar →" bar at the bottom.
- **Pricing is clear and low-friction:** $600 MXN per person, quantity selector (1–10), optional +$120 MXN flexible-cancellation add-on, inclusions (yoga, Breath Walk, meditation, brunch, closing ceremony, park entry) and the one exclusion (parking) are both stated.
- **Logistics inconsistency: duration doesn't match the itinerary.** The page states an 8-hour duration, but the itinerary runs 8:00 a.m.–3:00 p.m., which is 7 hours — a small but checkable discrepancy that undermines trust in the other logistics details.
- **Logistics inconsistency: group size vs. booking cap.** The stated group size is "20 people," but the booking widget's quantity selector only allows up to 10 spots per booking — not necessarily a bug (could be per-booking vs. total-event capacity), but worth confirming it's intentional rather than a stale limit.
- **Trust signals are thin.** The host is named only as "Jardín del Yoga" with "Desde hace 20 años comparto el yoga..." — no named individual, no credentials, no reviews, no verification badge. The cancellation table (100% at 14+ days down to no refund under 48h) and "Pago seguro con Stripe" are the only real trust signals.
- **Formatting risk in the cancellation table.** The cancellation policy's header row appears separated from its body by a blank line in the source, which may cause it to render as plain text instead of a table — worth a visual check.
- **Itinerary is a single unbroken line of times and activities**, making it harder to scan than a simple list would be.
- **Possible image duplication**, same pattern as other recently-audited pages — each image block appears to repeat.

## Recommended changes, prioritized
1. **Critical** — Fix the ALL CAPS experience name in the title/headline ("EL LATIDO DEL BOSQUE" → sentence case).
2. **Critical** — Remove the empty superlatives ("el mejor año nuevo," "la mejor versión de ti") and replace with concrete, honest language about what the day actually offers.
3. **Critical** — Remove emoji (🌿, 🌬, 🤍, 📍, ✦) from the page.
4. **Important** — Reconcile the duration (stated 8h vs. itinerary's actual 7h window) and clarify whether "20 people" group size vs. the 10-spot booking cap is intentional.
5. **Important** — Soften "tecnologías sagradas de sanación y espiritualidad" to avoid reading as a therapeutic/medical claim.
6. **Nice to have** — Break the itinerary into a scannable list instead of one unbroken line; verify the cancellation table actually renders as a table; spot-check for duplicated images.
