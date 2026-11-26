# Breath in Sound: Sigue tus sueños — landing page audit
URL: https://almawellness.io/experiencias/breath-in-sound-sigie-tus-suenos
Audited: 2026-11-26

## Summary
The page is well-structured and the body copy is genuinely warm and contemplative, but it ships with a visible typo in its own `<title>`/H1 and several brand-voice violations that look like they come from a shared template (ALL CAPS subheadings, emoji in the outcomes row) rather than this page specifically. Conversion UX is solid — clear single CTA, transparent pricing, a detailed cancellation table — undercut mainly by missing image alt text and a confusing duplicate nav link.

## Brand voice findings
- **Typo in the title itself:** the `<title>` and H1 literally read "Breath in Sound: **Sigie** TUS Sueños" — "Sigie" is a misspelling of "Sigue." The body text later gets it right ("Breath in Sound: Sigue tus sueños es una experiencia inmersiva..."), which makes the error in the headline more conspicuous, not less.
- **ALL CAPS used for emphasis, against the sentence-case rule:** confirmed in the raw HTML — "TUS" inside the title/H1, plus section headings "LA EXPERIENCIA," "¿QUÉ SIGNIFICA SEGUIR TUS SUEÑOS?," "ESTO ES PARA TI, SI:," and "LO QUE TE LLEVAS." Everything else on the page (section labels like "Itinerario," "Qué incluye," "Política de cancelación") correctly uses sentence case, so these read as inconsistent, not deliberate style.
- **Real emoji, not just symbols:** the "Lo que te llevas" outcome row is literally `<span class="outcome-emoji">🌿</span>` for Transformación, `✦` for Presencia, `🌬` for Calma, `🤍` for Conexión, plus a `📍` pin on the location line — confirmed in source, not a markdown-rendering artifact. This breaks the "no emoji, anywhere" rule outright.
- **Good example of the intended tone:** "La música no está de fondo: marca el ritmo, transforma la intensidad y acompaña la respiración." — short, specific, no hype, and it's honest about what the format actually is (a live DJ set as part of the practice, not ambient background music).
- **No exclamation marks, no empty superlatives, no overclaimed medical results** — the host-credibility line ("más de 10 años de experiencia combinada") is a reasonable, bounded claim, not a superlative.
- **Second person used correctly:** "No necesitas experiencia previa, solo ganas de sentir" and the CTA "Reservar mi lugar" are both consistent with the tú/first-person-CTA rule.

## Conversion UX findings
- **Single, easy-to-find CTA:** "Reservar mi lugar →" appears in the main form and is reinforced by a sticky "Reservar →" footer button, so it's never more than a short scroll away.
- **Pricing is fully transparent:** $888 MXN per person, shown consistently, plus an optional flexible-cancellation add-on at +$120 MXN that is clearly itemized at checkout rather than hidden.
- **Cancellation policy is unusually clear and tiered** (100% >14 days, 50% or credit 7–14 days, credit-only 48h–7 days, none under 48h) — this is a genuine trust signal and more detailed than most listings need to be.
- **Logistics are all upfront:** date (Sat, Dec 5, 2026), check-in time, 2-hour duration, exact address (Casa Una, Roma Norte), and a 1–4 person group-size selector.
- **Missing alt text on every image:** confirmed in the raw HTML — all four experience photos render as `<img alt="" ...>`. This is a real accessibility gap, not a false positive from the markdown conversion.
- **Confusing duplicate nav link:** "Inspirarme" and "Experiencias" in the top nav both point to `/experiencias` — minor, but it's dead weight in the nav that could be fixed trivially.
- **Thin trust signals beyond price/policy:** no reviews, ratings, or past-attendee social proof anywhere on the page; the only credibility signal is the one-line "más de 10 años de experiencia combinada" for the two hosts, with no detail on what that experience consists of.

## Recommended changes, prioritized
1. **Critical** — Fix the "Sigie" typo in the title/H1, and convert "TUS" and the four ALL-CAPS subheadings ("LA EXPERIENCIA," "ESTO ES PARA TI, SI:," etc.) to sentence case to match the brand book and the rest of the page.
2. **Critical** — Remove the emoji from the outcomes row (🌿 ✦ 🌬 🤍) and the 📍 pin; since this pattern is identical on the `unison` listing audited the same day, it's likely a shared template component and worth fixing once at the component level rather than per-listing.
3. **Important** — Add descriptive alt text to the four experience images.
4. **Nice to have** — Point "Inspirarme" to its own distinct content instead of duplicating the "Experiencias" link, and consider adding at least one past-attendee quote or rating to back up the "10 años de experiencia combinada" claim.
