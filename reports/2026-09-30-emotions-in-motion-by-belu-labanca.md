# EMOTIONS IN MOTION® by Belu Labanca — landing page audit
URL: https://almawellness.io/experiencias/emotions-in-motion-by-belu-labanca
Audited: 2026-09-30

## Summary
Structurally solid — clear single CTA, transparent pricing, a detailed cancellation table, and a legible host bio. But the page breaks two of Alma's non-negotiable brand-voice rules (emoji, and an all-caps proper-name headline sitting in the H1 with no gentler framing) and has a couple of easy-to-fix UX gaps (empty alt text on every image, no reviews/social proof, no visible connection to Alma's curation). Nothing here is structurally broken, but the brand-voice issues need a fix before this reads as an Alma page rather than a generic booking template.

## Brand voice findings
- **Emoji, hardcoded in markup.** The "Lo que te llevas" section renders each outcome with an emoji glyph: `<span class="outcome-emoji">🌿</span>` (Transformación), `✦` (Presencia), `🤍` (Conexión), plus a `📍` pin next to the address ("📍 Fernando M. Villalpando 98..."). Brand book is explicit: no emoji, anywhere. This is the clearest hard-rule violation on the page.
- **All-caps brand/method name as the page's H1.** The headline is `EMOTIONS IN MOTION® by Belu Labanca` — the method name is in full caps as the primary heading of the page. Alma's rule is sentence case everywhere; a registered trademark name is a defensible exception in running copy, but using it verbatim, in caps, as the H1 reads like corporate branding was dropped in unedited rather than adapted to Alma's voice (e.g. a page-specific title in sentence case with the trademark referenced below it would fit better).
- **Section headings and body copy are otherwise clean.** "Itinerario," "Lo que te llevas," "Qué incluye," "No incluye," "Qué llevar," "Sobre Belu Labanca," "Política de cancelación" are all correct sentence case — no Title Case problem here despite an earlier automated read flagging it.
- **Tú voice is correctly used.** "para transformar *tus* emociones," "Lo que *te* llevas," CTA "Reservar *mi* lugar" (correctly first-person for the button, per the brand book's stated exception). No "usted" found anywhere.
- **No exclamation marks, no superlatives, no overclaimed medical/therapeutic language.** Checked the full page text — none found. The outcome copy ("Transformación," "Presencia," "Calma," "Conexión") stays abstract rather than promising a cure, which is appropriate.
- **Host bio reads warm and credentialed, not salesy.** "Belu Labanca es speaker internacional, coach de propósito y bienestar y creadora del método de liberación somática EMOTIONS IN MOTION®... Actualmente trabaja con personas, empresas y audiencias internacionales en más de 10 países." Factual, contemplative pacing, no hype.

## Conversion UX findings
- **Single clear CTA, no scroll-hunting.** "Reservar mi lugar →" appears in a persistent booking aside and again in a mobile price bar — easy to find on any viewport.
- **Trust/reassurance copy present but no social proof.** "Sin cargo hasta confirmar · Pago seguro" (no charge until confirmed, secure payment) is a good trust signal near the CTA. However there are no reviews, testimonials, or verification badges anywhere on the page — for a 40-person paid session this is a gap worth flagging.
- **Cancellation policy is unusually thorough and clear.** Full table: 15+ days = full refund, 8–14 days = 50%, <7 days = no refund, plus a paid "flexible cancellation" add-on for $120 MXN. This is a genuine strength — more transparent than most listings.
- **Pricing is a single flat rate, clearly shown.** $350 MXN per person, no tiers to compare, no hidden-cost ambiguity — displayed both in the desktop aside and the mobile sticky bar.
- **Logistics are all upfront.** Date/time (arrival 10:00 a.m., departure 12:00 p.m.), exact address (Fernando M. Villalpando 98, Guadalupe Inn, CDMX), group cap (40), languages offered (Spanish/English), what's included (90-minute movement session) and excluded (transportation) are all stated plainly.
- **Every image has empty `alt=""`.** All carousel images (`gc-bg`/`gc-fg` classes) ship with `alt=""` — a pure decorative-image pattern here would still benefit from at least one descriptive alt on the hero image for accessibility and SEO.
- **Mobile viewport meta tag is present** (`width=device-width, initial-scale=1`) — no responsiveness red flag.
- **No obvious page-weight red flags** from the HTML — images are served from Supabase storage with lazy loading on all but the hero image; nothing indicates oversized unoptimized assets from what's visible in markup.
- **Alma's own curation voice is invisible on this page.** Nothing on the page signals "Alma vetted/selected this" — it reads as a vendor booking page hosted on Alma's domain rather than an Alma-curated pick. Minor, but worth a product-level note since it's likely a shared template issue rather than specific to this listing.

## Recommended changes, prioritized
1. **Critical** — Remove the four emoji from the "Lo que te llevas" outcome icons and the 📍 before the address; replace with plain text or a non-emoji icon/SVG treatment consistent with the rest of the site's visual system. This is a direct brand-book violation.
2. **Important** — Reconsider the H1 treatment of "EMOTIONS IN MOTION®": keep the trademark name but don't let it be the entirety of the all-caps page title with no Alma framing (e.g. lead with the offering in sentence case, cite the method name as a proper noun within it).
3. **Important** — Add at least a placeholder for reviews/social proof, or explicitly design the template to note "nueva experiencia" when no reviews exist yet, so the absence doesn't read as untested.
4. **Nice to have** — Add descriptive `alt` text to the hero/carousel images (host in motion, the space, etc.) instead of leaving all `alt=""`.
5. **Nice to have** — Surface Alma's curation voice somewhere on the page (a short line on why this experience was selected) to distinguish it from a generic vendor booking flow.
