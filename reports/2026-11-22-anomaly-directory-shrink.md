# Anomaly note — directory listing shrank again; one 404 now unresolved for a month+
Date: 2026-11-22

This is a note on an out-of-scope anomaly noticed while diffing the directory
page, alongside the normal 4-new-experience audit for this run (see the four
`2026-11-22-*.md` reports). Flagging for a human to review, continuing the
thread from the 2026-10-22 and 2026-11-15 anomaly notes.

## What changed
The live directory page (`/experiencias`) now shows only **17** experiences.
`known-experiences.json` tracked **28** previously-seen slugs going into this
run. Of those 28, only 13 are still listed on the directory; the other
**15** no longer appear there (the new 4 audited today bring the live count
to 17). I checked the HTTP status of all 15 delisted slugs directly:

| slug | individual page status |
|---|---|
| `moon-wellness-retreat` | 200 — loads fine |
| `ofrenda-laboratorio-creativo-multidisciplinar` | **HTTP 404** |
| `labrinto-al-mictlan` | 200 — loads fine |
| `play-ground-retreat` | 200 — loads fine |
| `renacer-al-amor` | 200 — loads fine |
| `emotions-in-motion-by-belu-labanca` | 200 — loads fine |
| `activacion-kundalini-gong-bath` | 200 — loads fine |
| `cacao-mantra-sounbath` | 200 — loads fine |
| `soft-sunday-a-wellnes-treat` | 200 — loads fine |
| `soft-sunday-temazcal-en-teotihuacan` | 200 — loads fine |
| `respirar-la-montana` | **HTTP 404** |
| `alaya-14-anima` | 200 — loads fine |
| `bano-de-gong` | 200 — loads fine |
| `breath-in-sound-vision-clara` | 200 — loads fine |
| `ttre-y-tambor-chamanico` | 200 — loads fine (newly delisted since 2026-11-15; was still listed as of that check) |

## Why this matters
- The two chronic 404s are unchanged from the 2026-11-15 note:
  `ofrenda-laboratorio-creativo-multidisciplinar` and `respirar-la-montana`.
  **`respirar-la-montana` was first flagged broken on 2026-10-22 and is still
  404ing today, 2026-11-22 — roughly a month with no fix, redirect, or
  unpublish.** This is the most concrete, actionable item across all three
  anomaly notes: a listing that visibly 404s for over a month suggests either
  a bug that's gone unnoticed or a listing nobody remembered to clean up.
- The other 13 delisted pages still render with full content (200), so this
  continues the same pattern as prior notes — most likely scheduled
  experiences whose dates have passed or which lack open booking dates, and
  are therefore filtered out of the live directory by design. This run did
  not re-check each one's specific "open dates" content state (that was
  already done in detail on 2026-10-22 and 2026-11-15); the status check here
  is limited to confirming none of them have newly 404'd.
- Scale: 15 of 28 tracked slugs (54%) are now absent from the live directory,
  consistent with the growing-delisting trend already noted twice before
  (6-of-14, then 14-of-25, now 15-of-28). If this is expected behavior for a
  marketplace where dated experiences roll off once their dates pass, no
  action is needed beyond fixing the two 404s. If it's not expected, it may
  be worth a human checking whether the directory's filtering logic is
  working as intended.

## Not changed by this run
`known-experiences.json` still lists all 28 previously-known slugs plus the 4
new ones found today — this run does not remove delisted or 404ing slugs from
the known set, consistent with prior precedent.
