# Temazcal y ceremonia de cacao: escapada a Veracruz — landing page audit
URL: https://almawellness.io/experiencias/temazcal-y-ceremonia-de-cacao-escapada-a-veracruz
Audited: 2026-11-12

## Summary
The page is structurally solid — clear logistics, a real cancellation policy, and consistent tú voice with no exclamation marks or superlatives. But it breaks two hard brand rules (emoji use, all-caps day labels) and has several conversion-blocking inconsistencies (a possible pricing-total bug, a check-in time contradiction, and a broken image format) that a human should fix before this listing gets real traffic.

## Brand voice findings
- **Emoji present, which is a hard no.** The page uses 📍, 🌿, 🌬, 🤍, ✦ as section/tag markers (e.g. next to "Transformación," "Calma," "Conexión"). Brand rule is "no emoji, anywhere" — these need to go, likely replaced with plain text labels or simple icons that aren't emoji glyphs.
- **ALL CAPS day labels.** Itinerary headers like "SÁBADO 12 DE DICIEMBRE" use full caps for emphasis, violating "sentence case everywhere." Should read "Sábado 12 de diciembre."
- **Tú voice is correctly and consistently used.** "Escápate dos días a La Isla," "trae una botella," "Elige una fecha" — all second person, no "usted" slips. This is done right.
- **No exclamation marks, no superlatives, no overclaimed medical results** — compliant. The page uses "sanación," "transformación," "el poder transformador de los rituales" as soft experiential framing rather than medical claims, which stays within brand's contemplative tone and doesn't cross into "esto cura tu ansiedad" territory. Still, "Transformación" used as an isolated benefit tag with no supporting detail reads closer to generic wellness-marketing shorthand than Alma's curated, specific voice — worth a look, though not a hard violation.
- **Host bio inconsistency between languages.** The English bio claims "I spent two years living in the mountains," a detail the Spanish bio omits entirely. Minor, but it undercuts the "honesto" and "curado" (every word deliberate) standard if the two versions aren't telling the same story.

## Conversion UX findings
- **Single clear CTA, present three times** ("Reservar" in nav, "Reservar mi lugar →" in the booking panel, "Reservar →" in the sticky bottom bar) — easy to find, no scroll-hunting required.
- **Possible pricing bug:** the total still reads "$3,800" even when 5 places are selected, suggesting the total doesn't scale with group size selected. This should be verified with engineering — if real, it's a direct conversion blocker (wrong price shown to a group booker).
- **Check-in time contradiction:** check-in is listed as 3:00 p.m., but the itinerary separately shows reception at 1:30 p.m. This kind of logistics mismatch creates real friction/confusion for someone planning travel.
- **Grammar slip:** "2 días · 1 noches" should read "1 noche." Small, but it's the kind of detail "curado" branding should catch.
- **Possible meal-coverage conflict:** the itinerary mentions "comida durante el trayecto" (meal during the trip) while the "No incluye" section excludes meals during road stops — these may describe the same thing and contradict each other, or may need clearer wording to distinguish them.
- **Trust signals are present but thin.** Cancellation policy is clear and specific (full refund 15+ days out, 50% at 8–14 days, none inside 7 days), and "Pago seguro con Stripe" signals payment security. But there are no reviews, ratings, or host verification badge, and the lodging partner ("Mi Hotelito Bello") is named with no supporting photos or reviews on the page.
- **Host credentials lack specifics.** The bio mentions a curandera great-grandmother and shaman instruction, plus certifications in Yoga, Ayurveda, and "Salud Femenina," but names no certifying body, years of practice, or license info — thin for a page that's asking someone to book a ritual-based overnight retreat.
- **Image issues:** all images have empty `alt=""` attributes (accessibility gap), and one listing image is a `.HEIC` file, a format many browsers (especially non-Apple) don't render — this could show as a broken image to a meaningful share of visitors.
- **Minor link redundancy:** "Inspirarme" in navigation points to the same URL as "Experiencias" — not broken, just duplicate.
- **Viewport meta tag is present and correct** (`width=device-width, initial-scale=1`) — mobile responsiveness is fine at the markup level.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji (📍🌿🌬🤍✦) from the page; verify and fix the group-size pricing total bug; resolve the check-in time contradiction (3:00 p.m. vs. 1:30 p.m.).
2. **Important** — Replace ALL CAPS day labels with sentence case; convert the `.HEIC` image to a universally-supported format (JPG/PNG/WebP); add descriptive `alt` text to all images; reconcile the "comida durante el trayecto" vs. excluded road-stop meals wording; align the English and Spanish host bios so they tell the same story.
3. **Nice to have** — Fix "1 noches" → "1 noche"; add reviews/testimonials or a host verification signal if available; name the host's certifying bodies or years of experience; remove the duplicate "Inspirarme" nav link pointing to the same page as "Experiencias."
