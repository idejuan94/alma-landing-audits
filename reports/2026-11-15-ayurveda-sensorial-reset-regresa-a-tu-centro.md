# Ayurveda Sensorial Reset: Regresa a tu centro — landing page audit
URL: https://almawellness.io/experiencias/ayurveda-sensorial-reset-regresa-a-tu-centro
Audited: 2026-11-15

## Summary
This page has the most e-commerce-flavored pricing presentation seen in this audit series — a struck-through "before" price next to a "Preventa" label — which sits uneasily against the brand's no-discount-shouting rule, on top of the same emoji pattern seen elsewhere on the site. The logistics, inclusions, and cancellation terms are otherwise clear, and notably this page does include an explicit medical disclaimer, which is good practice worth preserving.

## Brand voice findings
- **Emoji used as structural markers, same pattern as other listings:** 📍 (ubicación), 🌿 (Transformación), ✦ (Presencia), 🌬 (Calma), 🤍 (Conexión), 🎟 (Preventa) — six distinct emoji on one page, violating the no-emoji rule.
- **"Preventa" + strikethrough pricing reads as discount-shouting:** the page shows a crossed-out "$14,500" next to a presale price of "$13,000," plus a group discount text that says "Ahorran $1,000 cada uno" — a figure that doesn't actually match the $1,500 difference between the struck-through and presale prices. This combination (markdown framing + math that doesn't add up) is exactly the kind of e-commerce pressure language the brand book asks Alma to avoid, and it also undermines trust through the inconsistency.
- **No exclamation marks** in visible copy — confirmed against raw HTML. Clean.
- **Headline capitalization is inconsistent with the rest of the page:** the H1 ("Ayurveda Sensorial Reset: Regresa a tu centro") is rendered in Title Case while every other heading on the page ("Itinerario," "Qué incluye," "Qué llevar," "Política de cancelación") uses sentence case. Likely just how the host entered the title, but it stands out against the brand's sentence-case standard.
- **Good: explicit, honest medical disclaimer present.** "No constituye un tratamiento médico ni sustituye la atención de profesionales de la salud" appears in the "No incluye" section — this is exactly the honest, non-overclaiming language the brand book calls for, and other experience pages on the site (e.g. código origen) are missing an equivalent note. The only issue is placement: it's in small print at the bottom of a list rather than near the price or booking CTA where someone evaluating the experience would see it.

## Conversion UX findings
- **Pricing math inconsistency is a real friction point**, not just a tone issue: a buyer comparing the struck-through price, the presale price, and the "ahorran $1,000" claim will notice the numbers don't reconcile, which undercuts trust right at the decision point.
- **Three separate "Reservar" buttons** (header, booking-panel "Reservar mi lugar →", and a sticky "Reservar →" at the bottom of the price panel) — redundant, but not harmful; the primary CTA is easy to find without scrolling.
- **Cancellation table has a gap:** tiers are ">15 days: 100%", "8–14 days: 50%", "7 days or less: no refund" — day 15 itself isn't covered by any row.
- **No social proof** — no reviews, testimonials, or past-cohort signals for either host.
- **Host credentials stated but not independently verifiable** (no license numbers, certification links) — consistent with the rest of the site, but worth flagging since this page leans more heavily on clinical-adjacent language (Ayurveda, somatic therapy, Shirodhara/Abhyanga) than most listings.
- **Gallery images (~14) appear duplicated in the markup**, same pattern as other listings on the site — likely a shared template issue, not specific to this page.

## Recommended changes, prioritized
1. **Critical** — Fix the pricing math so the "ahorran" figure matches the actual discount shown; an incorrect savings claim is both a trust problem and arguably misleading.
2. **Critical** — Remove the emoji (📍🌿✦🌬🤍🎟); same hard brand-voice rule as elsewhere on the site.
3. **Important** — Reconsider the "Preventa" + strikethrough-price framing — it reads as e-commerce urgency language rather than Alma's curated tone, even without an exclamation mark or countdown.
4. **Important** — Move the medical disclaimer closer to the price/CTA so it's seen at the decision point, not buried at the bottom of the inclusions list.
5. **Nice to have** — Collapse the three "Reservar" buttons' redundancy isn't harmful, but consider whether the sticky bottom CTA is actually needed given the header CTA is already persistent.
6. **Nice to have** — Fix the cancellation table's day-15 gap.
