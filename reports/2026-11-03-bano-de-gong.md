# Baño de Gong — landing page audit
URL: https://almawellness.io/experiencias/bano-de-gong
Audited: 2026-11-03

## Summary
Structurally the page is solid — clear single CTA, detailed itinerary, transparent cancellation table, and a well-credentialed host bio. But it breaks the "no emoji, anywhere" brand rule in multiple places, makes unqualified therapeutic-outcome claims, and has two internal data inconsistencies (group size vs. ticket cap, and session duration vs. stated itinerary) that will read as sloppy to a careful buyer.

## Brand voice findings
- **Emoji present, hard rule violation.** The outcome tags use emoji explicitly marked by the site's own `outcome-emoji` CSS class: 🌿 "Transformación", ✦ "Presencia", 🌬 "Calma", 🤍 "Conexión". The pricing badge also reads `🎟 Preventa`, and the location line reads `📍 Jalapa esquina con Coahuila...`. None of this is incidental — it's styled as a repeating design pattern, so it'll likely recur on every new listing until the template is fixed.
- **Overclaimed therapeutic results.** The meta description and body copy state: *"Algunos de los múltiples beneficios que te trae esta experiencia son: una mejora considerable en la calidad del sueño, la regulación del sistema nervioso, así como la restauración de tu energía de manera integral."* This reads as a medical/therapeutic outcome claim ("mejora considerable," "regulación del sistema nervioso") stated as fact rather than Alma curating an experience that *may* support wellbeing — closer to the "esto cura tu ansiedad" pattern the brand book explicitly rules out than to honest, hedged language.
- **Tú voice is consistent.** No "usted" found anywhere; copy consistently addresses the reader as "tú" ("para conectarte contigo," "para que puedas soltar la tensión"). CTA "Reservar mi lugar →" correctly uses first person for the self-claimed action.
- **No exclamation marks, no ALL CAPS, no empty superlatives or fake urgency found in the visible copy.** "Preventa" and the struck-through "antes $500 / $350" are presale pricing, not discount-shouting or countdown pressure — this is a defensible use of pricing contrast and reads as honest rather than salesy.
- **Tone otherwise lands close to brand:** short, contemplative sentences ("para que puedas soltar la tensión y entrar en las profundidades de tu ser"), no generic corporate filler.

## Conversion UX findings
- **Single clear CTA, easy to find.** "Reservar" in the header, "Reservar mi lugar →" in the booking widget, and a sticky "Reservar →" footer button — no scrolling required to act.
- **Strong trust signals.** Host Verónica María's bio is specific and credible: "más de 10 años de experiencia," "6 certificaciones en Gong," has interpreted for international Gong trainings in Mexico, and her session has been part of the Morelos state government's "Cartelera Bienestar" program since 2024. This is exactly the kind of concrete, verifiable credential the brand book wants in place of empty superlatives.
- **No reviews or testimonials** — not a blocker on its own (this looks like a newer/first-run listing), but worth flagging since there's otherwise no peer social proof.
- **Pricing is clear**, with the add-on (flexible cancellation, +$120 MXN) disclosed rather than hidden, and a transparent tiered refund table (100% / 50% / none by days-before).
- **Logistics are thorough**: exact date, address, minute-by-minute itinerary, what's included/not included, and a packing list.
- **Data inconsistency — group size vs. capacity.** The page states "Grupo de 25 personas" in the logistics block, but the date/ticket selector caps bookings at "15 lugares." A buyer comparing these will either think spots are scarcer than claimed or that the group-size figure is wrong — this needs reconciling.
- **Data inconsistency — duration vs. itinerary.** The summary lists session duration as "2h," but the stated itinerary (10:00 puerta → 11:45 cierre) runs 1h45. Separately, the session itself is described as "45 a 50 minutos sin interrupciones" while the itinerary's Gong block (10:30–11:45) runs 75 minutes. These numbers should match.
- **No egregious page-weight issues**: viewport meta tag is present (mobile-responsive), and the 6 images on the page are a normal count for a listing page — not visibly oversized from the HTML alone.

## Recommended changes, prioritized
1. **Critical** — Remove the emoji from the outcome tags, pricing badge, and location line (🌿 ✦ 🌬 🤍 🎟 📍). This is a hard, non-negotiable brand rule and appears to be a repeating template pattern, so fixing it at the component level (not just this page) will prevent it recurring on future listings.
2. **Critical** — Rewrite the benefits sentence to drop the therapeutic-outcome framing ("mejora considerable en la calidad del sueño," "regulación del sistema nervioso") in favor of honest, hedged, non-medical language consistent with curation rather than treatment.
3. **Important** — Reconcile "Grupo de 25 personas" against the 15-spot ticket cap, and reconcile the "2h" / "45–50 min" duration claims against the stated 10:00–11:45 itinerary.
4. **Nice to have** — Consider adding at least a placeholder for reviews/social proof once available, since the host credentials currently carry all the trust-building weight alone.
