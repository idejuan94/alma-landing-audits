# Donde descansa el ruido — landing page audit
URL: https://almawellness.io/experiencias/donde-descansa-el-ruido
Audited: 2026-11-22

## Summary
Tone and copy are mostly in line with Alma's voice (sentence case, no exclamation marks, no overclaimed medical results), but the page has two data-integrity problems that matter more than tone: a seat-count mismatch (15 vs. 25 people) and reviews that appear to belong to a different experience entirely. Those undercut the "honesto" brand pillar more than any copy choice would.

## Brand voice findings
- **Emoji (hard rule, site-wide template issue):** 🌿 🌬 🤍 📍 🕉️ ✦ appear via the same shared outcome-tag/location-icon components flagged on other listings audited today — platform-level, not specific to this page.
- **ALL CAPS:** "HARI OM" appears in caps where the rest of the page uses sentence case — flag for consistency, though it's a minor, isolated instance (a mantra/exclamation word, arguably stylistic rather than a heading).
- **Discount display bug, reads like urgency/e-commerce language:** The early-bird badge shows "-550%" next to "Precio anticipado (early bird)" — almost certainly a formatting bug, but as rendered it's a nonsensical, loud discount callout that reads worse than intentional discount language would.
- No exclamation marks, no usted, no overclaimed therapeutic language found in the brand's own copy — the sound-healing/meditation framing stays descriptive rather than claiming cures.

## Conversion UX findings
- **Reviews appear mismatched to this listing:** both 5-star reviews (Oct 2026) praise cacao, sound bath, and a beautiful venue — but this event's tags are meditation, soundhealing, and Bach flowers, with no cacao component mentioned anywhere in the description. This looks like reviews were pulled in from a different, similar experience (possibly from the same host/venue tag) rather than being specific to this one — worth checking whether the review-attribution logic is matching on venue/host instead of experience ID.
- **Capacity inconsistency:** the booking widget says "15 lugares" while the event details state "Grupo de 25 personas." A buyer can't tell how many people will actually be in the room.
- CTA is clear and present ("Reservar mi lugar," sticky bar).
- Host bio is solid: 15+ years of experience, specific training lineage (Hatha, Vinyasa, Ashtanga, India), named collaborators — good trust signal on its own, independent of the review-mismatch issue above.
- Cancellation policy is clear and tiered.
- Images carry empty `alt=""` attributes — same site-wide gap as other listings.

## Recommended changes, prioritized
1. **Critical** — Fix the mismatched reviews; showing testimonials for a different experience is a trust problem, not a cosmetic one.
2. **Critical** — Resolve the 15 vs. 25 person capacity discrepancy.
3. **Important** — Fix the "-550%" early-bird discount display bug.
4. **Nice to have** — Normalize "HARI OM" to sentence case for consistency with the rest of the page; add alt text to images.
