# Networking wellness - Sauna, Cold plunge & Connections — landing page audit
URL: https://almawellness.io/experiencias/networking-wellness-sauna-cold-plunge-connections
Audited: 2026-11-22

## Summary
The page is logistically complete (dates, price, host, cancellation terms, included/not included) but reads as the most e-commerce/salesy listing audited so far: it stacks a struck-through "was $400 / now $350" discount, a "Preventa" urgency badge, and several unsubstantiated physiological claims (dopamine, inflammation, nervous-system regulation) on top of a site-wide emoji icon set that violates the no-emoji rule on every listing. Structurally solid, but brand voice needs real cleanup here.

## Brand voice findings
- **Emoji (hard rule, site-wide template issue):** Confirmed in the raw HTML: `📍 <!-- --> 56, Calle Valladolid, Roma Norte...` before the address, and a `🎟 <!-- --> Preventa` badge marked up with class `"...color:var(--accent)">🎟"`. These come from a shared template component (the booking-badge and address-line markup), not hand-written copy for this listing — the same icon set appears on every other listing audited today, so this is a platform-level fix, not a per-page one.
- **False urgency / e-commerce language (hard rule):** Struck-through original price "$400" next to "$350" marked "Preventa," plus "cupo limitado" / "solo 8 personas." This is textbook discount-shouting — exactly what the brand book prohibits.
- **Overclaimed therapeutic/medical results (hard rule):** The copy claims cold immersion "disparar dopamina" (triggers dopamine) and reduces inflammation, that heat "activar la circulación" and relaxes muscle, that breathwork "regulan el sistema nervioso," and that the drinks "desinflamar." Alma curates wellness experiences; it shouldn't be the one making these physiological claims on a host's behalf.
- **Tone:** "exclusiva," "high-value conversations" read as corporate networking-event copy rather than Alma's warm/contemplative voice — closer to a LinkedIn mixer than a wellness curation.
- No exclamation marks and no usted found — those hard rules are respected here.

## Conversion UX findings
- Primary CTA is clear and repeated ("Reservar mi lugar →," sticky "Reservar →") — easy to find.
- Logistics are upfront and specific: two concrete dates, address with map link, 8-person cap, included/not included, what to bring.
- Cancellation policy and Stripe payment notice are present — reasonable trust signals, but there are **no reviews, ratings, or host verification** anywhere on the page, which is a gap for a new-to-the-platform-sounding host running a paid group session.
- Internal inconsistency: duration is labeled "2h" at the top but the itinerary runs 7:00–10:00 PM (3 hours) and the inclusions list says "3 horas." Pick one number.
- All images on the page carry empty `alt=""` attributes (confirmed in raw HTML) — site-wide accessibility gap, not specific to this listing.
- Viewport meta tag is present and correct (`width=device-width, initial-scale=1`).

## Recommended changes, prioritized
1. **Critical** — Remove the emoji icon set from the shared template (location pin, ticket badge, and the outcomes-row icons used across the site) — this is a one-time platform fix that resolves the no-emoji violation everywhere, not just here.
2. **Critical** — Drop the struck-through discount price and "Preventa" scarcity badge, or reframe without e-commerce pressure tactics; soften or remove the dopamine/inflammation/nervous-system claims to avoid implying medical benefit.
3. **Important** — Fix the 2h vs. 3h duration inconsistency.
4. **Important** — Add at least a host bio/credentials line or early reviews once available; this format (recurring paid social event) especially benefits from social proof.
5. **Nice to have** — Add descriptive alt text to listing images site-wide.
