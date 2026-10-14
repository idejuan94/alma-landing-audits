# Mantra Afro Move — landing page audit
URL: https://almawellness.io/experiencias/mantra-afro-move
Audited: 2026-10-14

## Summary
Structurally the page is solid — clear single CTA, cancellation terms, logistics all upfront, no walls of text. The brand-voice violations are what drag it down: emoji used as section icons, an ALL CAPS brand name in the opening line, and zero trust signals (no host credentials, no reviews). Fixable without a redesign.

## Brand voice findings
- "MANTRA ORIGEN son sesiones de entrenamiento físico basadas en movimientos de danzas africanas y afrolatinas." — ALL CAPS used for the brand name as the lead-in to body copy. Sentence case should hold even for brand mentions; if emphasis is wanted, use styling (bold/italic), not caps.
- "Lo que te llevas" icons: 🌿 Transformación, ✦ Presencia, 🌬 Calma, 🤍 Conexión, plus a 📍 on the address line — emoji appear four+ times. Hard rule is no emoji anywhere; these read as generic wellness-app decoration, not curated Alma voice.
- "Una hora para sumergirnos en una experiencia física y energética salvaje, conectando con nuestras raíces africanas." — tú/nosotros voice is correctly used, and the line reads warm and specific rather than generic. This is a good example of "contemplativo" tone to preserve when fixing the rest.
- No exclamation marks and no false urgency/discount language found — compliant there. "30 lugares" reads as plain capacity info, not manufactured scarcity, so it's fine as-is.
- Host line "Origen La Inmaculada / Ani Somali" gives no indication which is the person and which is the studio, and no bio — this isn't a tone violation but it undercuts the "honesto" and "curado" principles: a curated marketplace should tell you who is actually leading the session.

## Conversion UX findings
- Single clear CTA ("Reservar mi lugar →"), appears in header, booking panel, and sticky bar — easy to find, not excessive. Good.
- No trust signals at all: no host credentials, no reviews/testimonials, no verification badge. For a session described as "física y energética salvaje" led by someone with no stated training background, this is a real gap — visitors have nothing to vet the instructor against.
- Pricing is a single clear tier ($300 MXN) plus one named add-on (flexible cancellation, +$120 MXN) — no hidden-cost ambiguity, but currency label is inconsistent ("$300" in the header vs. "$300MXN" in the booking panel).
- Logistics (dates, time, duration, location with map link, group size, language, what's included/excluded, what to bring) are all present and upfront. Solid.
- Minor copy bug: "Ropa comoda" is missing its accent (should be "cómoda").
- Naming inconsistency: the experience is titled "Mantra Afro Move" but the included-session line calls it "African Move" — same thing, different name, reads unpolished.
- Navigation has redundant/confusing links: "Inspirarme" (described elsewhere as host videos) routes to the same `/experiencias` page as the plain "Experiencias" link, and "Entrar" appears twice in the nav. Minor friction, not blocking.
- Five unique images each appear duplicated in the markup — not necessarily a weight problem, but worth a dev check for redundant DOM/requests.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji (🌿 ✦ 🌬 🤍 📍) and replace the ALL CAPS "MANTRA ORIGEN" opening line with sentence case. Both are explicit, non-negotiable brand-voice violations.
2. **Important** — Add a short host bio with actual credentials/training background for Ani Somali / Origen La Inmaculada, and add at least one trust signal (review, past-attendee note, or verification mention) — right now there's nothing for a first-time visitor to vet the instructor or studio against.
3. **Nice to have** — Fix the "Ropa comoda" accent, align the experience name between the title and the "included" line, standardize the $300 vs. $300MXN currency display, and de-duplicate the "Inspirarme"/"Experiencias" nav links and repeated image tags.
