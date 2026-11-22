# Retiro de yoga en el bosque — landing page audit
URL: https://almawellness.io/experiencias/retiro-de-yoga-en-el-bosque
Audited: 2026-11-22

## Summary
This is the closest to "on-brand" of today's four new listings — sentence-case headline, no exclamation marks, no overclaimed medical results, a solid host bio, and a genuinely contemplative itinerary (silent walk, fire ritual, closing circle). The main problems are a text-encoding bug that mangles the host bio with garbled capitalization, and the usual site-wide emoji/alt-text issues.

## Brand voice findings
- **Emoji (hard rule, site-wide template issue):** 🌿 🌬 🤍 📍 from the same shared template components flagged on other listings today.
- **Text-encoding/capitalization bug in host bio:** the bio contains garbled words like "despuÉs," "certificÉ," "enSeÑar," and "BOSQUE" — looks like an auto-capitalization bug firing after accented vowels (é, é, ñ) rather than intentional ALL CAPS emphasis. Separate from the brand-voice "no caps for emphasis" rule, but it actively undermines "curado" (every word deliberate) — a host bio riddled with typos reads as careless, not curated.
- **ALL CAPS used for emphasis:** day labels in the itinerary ("VIERNES," "SÁBADO," "DOMINGO") are in caps while the rest of the page uses sentence case — flag per the hard rule, even though day-of-week labels are a common, low-stakes case for this.
- Minor Title Case in itinerary line items ("Vinyasa Yoga," "Sound Healing," "Moodboard") — low-severity, these read more like activity/program names than headline emphasis.
- Tone is otherwise genuinely warm/contemplative: "medicina" used metaphorically for the walk, journaling described as having "poder aclarador" — this is the kind of unhurried, specific language the brand book asks for, not generic wellness-marketing filler.

## Conversion UX findings
- CTA clear and repeated ("Reservar mi lugar →," sticky bar).
- Logistics are complete and specific: 3-day/2-night dates, exact location with map link, host certifications and retreat count, included/not included, what's excluded (transportation).
- Date ambiguity: the main date field reads "22–24 January" without a year; the description separately specifies 2027. A buyer skimming just the date field could be confused about which January.
- No reviews, ratings, or verification badge are visible — notable gap given the $18,000 MXN price point for a multi-day retreat; this is a bigger purchase than most of today's other listings and would benefit more from social proof.
- Cancellation policy is clear and tiered.
- Images carry empty `alt=""` attributes — same site-wide gap as other listings.

## Recommended changes, prioritized
1. **Important** — Fix the text-encoding bug in the host bio (garbled "despuÉs," "certificÉ," "enSeÑar," "BOSQUE").
2. **Important** — Add the year directly next to the main date range so it doesn't rely on the buyer reading the full description.
3. **Important** — Add reviews or ratings given the price point, once available.
4. **Nice to have** — Lower-case the day-of-week labels in the itinerary; add alt text to images.
