# Bloom & Balance 2nd edition — landing page audit
URL: https://almawellness.io/experiencias/bloom-balance-2nd-edition
Audited: 2026-11-09

## Summary
The page is logistically solid — clear schedule, location with map link, itemized inclusions/exclusions, and a tiered cancellation policy — but it breaks two of Alma's non-negotiable brand-voice rules (emoji use, and discount/urgency phrasing that reads as e-commerce rather than curated wellness). There's also a factual inconsistency between the stated group size and the booking selector, and the hormonal-health framing sits close to the line on therapeutic claims.

## Brand voice findings
- **Emoji used throughout, in violation of the hard "no emoji" rule.** The rendered page uses 📍, 🌿, ✦, 🌬, 🤍, and 👥 as section/label markers (alongside neutral UI glyphs ✓, ×, →). This is a clear, unambiguous violation — not a borderline case.
- **Discount/urgency language reads as e-commerce, not Alma's curated tone.** The page offers "Compra dos boletos y ahorra" with a -10% tag, plus a separate -10% "precio anticipado" (early-bird) discount. Neither is a false claim, but stacking two percentage-off badges next to the price is the "discount-shouting" pattern the brand book calls out — it reads as a retail promo, not a contemplative one-line price.
- **Host description is thin and borderline-corporate.** "MindEase experiences" gets no bio beyond the brand name; the only named specialist, "Pau," is introduced simply as "Nutriologa experta en hormonas" with no credentials, license, or background. This isn't a rule violation but it undercuts the "curado" (deliberate, considered) tone — there's nothing here that reads as hand-picked versus a generic vendor listing.
- **Borderline therapeutic framing.** The talk topic is described around "salud hormonal" (hormonal health) and "mitos y realidades," and the event promotes a third-party supplement ("Genoia") during the social portion. No explicit disease-cure claim appears (e.g. nothing like "esto cura tu ansiedad"), so this doesn't clearly cross the hard rule, but a human editor should check the actual on-page copy around the nutrition talk and the supplement promotion — product-adjacent health claims are exactly the kind of thing the brand book is trying to keep Alma's editorial voice separate from.
- No usted, no ALL CAPS/Title-Case emphasis headlines, and no exclamation marks were found — those three rules are respected.

## Conversion UX findings
- **Group size is internally inconsistent.** The page states the event is a "Grupo de 50 personas," but the booking quantity selector only allows 1–35 seats. A prospective guest can't tell whether the event is actually capped at 35, is a 50-person event with a UI bug, or whether 35 is some unexplained sub-limit — this is a trust-eroding inconsistency worth fixing before more bookings come in.
- **Pricing display doesn't reflect the discounts it advertises.** The page shows both a "buy two and save 10%" badge and a separate 10% early-bird badge, but the visible total still shows the flat $1,100 MXN with no discounted total calculated. A guest has to do their own math (and isn't told whether the two discounts stack), which adds friction right at the point of decision.
- **Trust signals are present but shallow.** There's a clear, well-tiered cancellation/refund policy (100% / 50%-or-credit / credit-only / no-refund bands) and a named payment processor ("Pago seguro con Stripe"), which is good. But there are no reviews, ratings, or verification badges for the host, and no credentialing for the specialist running the health talk — for a category (hormonal health advice) where expertise matters, this is a gap.
- **Accessibility/alt text:** images on the page appear to carry empty alt attributes, which is a real but minor accessibility issue, not something a typical guest will notice.
- **Could not verify:** the mobile-viewport meta tag and actual image file sizes aren't visible through the rendered-text fetch used for this audit — flagging as unchecked rather than guessing either way; a human (or a tool that can inspect the raw HTML `<head>` and network payload) should confirm these.

## Recommended changes, prioritized
1. **Critical** — Remove all emoji from the page; this is a hard, non-negotiable brand rule and currently fails outright (📍🌿✦🌬🤍👥 all appear).
2. **Critical** — Fix the group-size vs. booking-selector mismatch (50 people stated vs. 35-seat cap) — this looks like a bug and will confuse or mistrust guests.
3. **Important** — Collapse the two stacked discount badges into a single clear, calculated price (or drop the discount-badge treatment entirely in favor of Alma's plainer "cálido/honesto" pricing style) to avoid reading as e-commerce discount-shouting.
4. **Important** — Add a short host/specialist bio with real credentials for "Pau" and for MindEase experiences generally, to support the hormonal-health talk and justify guest trust.
5. **Nice to have** — Add alt text to the event images for accessibility.
6. **Nice to have** — Have a human confirm the supplement promotion and hormonal-health talk copy don't drift into overclaimed therapeutic language, since this audit could only review the rendered page text, not verify there's no stronger claim buried in copy the fetch summarized rather than quoted in full.
