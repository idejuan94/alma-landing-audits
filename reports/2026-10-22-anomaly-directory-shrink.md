# Anomaly note — directory listing shrank, one listing now 404s
Date: 2026-10-22

This is not a new-experience audit (zero new slugs appeared today — all 7
experiences currently on https://almawellness.io/experiencias are already
in `known-experiences.json`). This note records an out-of-scope anomaly
noticed while diffing, for a human to follow up on.

## What changed
The live directory page (`/experiencias`) now shows only **7** experiences
and explicitly states "7 experiencias" as its count. `known-experiences.json`
tracks **14** previously-seen slugs. The 6 slugs below no longer appear on
the directory page:

- `moon-wellness-retreat`
- `renacer-al-amor`
- `activacion-kundalini-gong-bath`
- `soft-sunday-a-wellnes-treat`
- `soft-sunday-temazcal-en-teotihuacan`
- `respirar-la-montana`

I checked each of these 6 individual listing URLs directly:

| slug | individual page status |
|---|---|
| `moon-wellness-retreat` | loads fine, full content |
| `renacer-al-amor` | loads fine, full content |
| `activacion-kundalini-gong-bath` | loads fine; page itself says "Todavía no hay fechas abiertas" (no open dates) |
| `soft-sunday-a-wellnes-treat` | loads fine; page itself says "Todavía no hay fechas abiertas" (no open dates) |
| `soft-sunday-temazcal-en-teotihuacan` | loads fine, full content, dates appear open |
| `respirar-la-montana` | **HTTP 404 — page no longer exists** |

## Why this matters
- `respirar-la-montana` was audited by this process on 2026-10-19 (see
  `reports/2026-10-19-respirar-la-montana.md`) as a normal working listing.
  Three days later its page returns a hard 404. Either it was deliberately
  unpublished/deleted, or something broke on the site.
- The other 5 delistings are plausibly intentional: at least 2 of them
  (`activacion-kundalini-gong-bath`, `soft-sunday-a-wellnes-treat`) still
  render but show no open booking dates, which is a reasonable reason to
  pull them from the public directory until new dates are scheduled.
  `moon-wellness-retreat`, `renacer-al-amor`, and
  `soft-sunday-temazcal-en-teotihuacan` still render with no obvious
  "sold out" signal, so it's less clear why those are no longer linked
  from the directory.

## Not changed by this run
`known-experiences.json` still lists all 14 slugs — this run does not
remove delisted or 404ing slugs from the known set, since the task this
process runs does not define removal handling. If `respirar-la-montana`
(or others) should be pruned or explicitly marked gone, that's a call for
a human, not an automated diff.
