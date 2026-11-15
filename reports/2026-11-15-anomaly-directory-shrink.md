# Anomaly note — directory listing shrank sharply, 2 slugs now 404
Date: 2026-11-15

This is a note on an out-of-scope anomaly noticed while diffing the directory
page, alongside the normal 2-new-experience audit for this run (see
`2026-11-15-codigo-origen.md` and
`2026-11-15-ayurveda-sensorial-reset-regresa-a-tu-centro.md`). Flagging for a
human to review — this is a much larger shrink than the one noted on
2026-10-22.

## What changed
The live directory page (`/experiencias`) now shows only **13** experiences
and states "13 experiencias" as its count (confirmed directly against the raw
HTML, not just a rendered summary). `known-experiences.json` tracked **25**
previously-seen slugs going into this run. Of those 25, only 11 are still
listed on the directory; the other **14** no longer appear there. I checked
each of the 14 individually:

| slug | individual page status |
|---|---|
| `moon-wellness-retreat` | loads fine (200), full content, no "no dates" signal |
| `ofrenda-laboratorio-creativo-multidisciplinar` | **HTTP 404** |
| `labrinto-al-mictlan` | loads fine (200); page says no open dates |
| `play-ground-retreat` | loads fine (200), full content, no "no dates" signal |
| `renacer-al-amor` | loads fine (200), full content, no "no dates" signal |
| `emotions-in-motion-by-belu-labanca` | loads fine (200); page says no open dates |
| `activacion-kundalini-gong-bath` | loads fine (200); page says no open dates |
| `cacao-mantra-sounbath` | loads fine (200); page says no open dates |
| `soft-sunday-a-wellnes-treat` | loads fine (200); page says no open dates |
| `soft-sunday-temazcal-en-teotihuacan` | loads fine (200); page says no open dates |
| `respirar-la-montana` | **HTTP 404** (already 404 as of the 2026-10-22 anomaly note — still broken, unresolved almost a month later) |
| `alaya-14-anima` | loads fine (200); page says no open dates |
| `bano-de-gong` | loads fine (200); page says no open dates |
| `breath-in-sound-vision-clara` | loads fine (200); page says no open dates |

## Why this matters
- 8 of the 14 delisted pages still render but explicitly show no open booking
  dates — plausibly intentional delisting until new dates are scheduled, same
  pattern as the 2026-10-22 note.
- 3 delisted pages (`moon-wellness-retreat`, `play-ground-retreat`,
  `renacer-al-amor`) render with full content and no visible "no dates" or
  "sold out" signal, so it's unclear why they were pulled from the directory.
- 2 pages hard-404 (`ofrenda-laboratorio-creativo-multidisciplinar`,
  `respirar-la-montana`). `respirar-la-montana` was first flagged broken on
  2026-10-22 — it has now been 404ing for at least 24 days without being
  fixed, unpublished with a redirect, or otherwise resolved.
- The scale here (14 of 25 known slugs gone at once, over half the tracked
  catalog) is notably larger than the 6-of-14 shrink from 2026-10-22 and may
  warrant checking whether this is a deliberate catalog cleanup, a bug in how
  the directory queries/filters listings, or an unrelated site issue.

## Not changed by this run
`known-experiences.json` still lists all 25 previously-known slugs plus the 2
new ones found today — this run does not remove delisted or 404ing slugs from
the known set, consistent with the 2026-10-22 precedent. If any of the above
should be pruned or explicitly marked gone, that's a call for a human.
