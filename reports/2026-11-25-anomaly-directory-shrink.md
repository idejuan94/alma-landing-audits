# Anomaly note — the two chronic 404s are now 5+ weeks / 10+ days unresolved
Date: 2026-11-25

Continuing the thread from the 2026-10-22, 2026-11-15, 2026-11-22, and
2026-11-24 anomaly notes. No new experiences were published today (see the
`known-experiences.json` diff / commit message), so this note stands alone
for this run.

## What changed
The live directory page (`/experiencias`) shows **19** experiences today,
unchanged from 2026-11-24. `known-experiences.json` tracked 34
previously-seen slugs going into this run; all 19 live slugs are already
in that set, so 15 previously-seen slugs remain absent from the directory
— the same delisting pattern noted in all four prior notes
(6-of-14, 14-of-25, 15-of-28, 15-of-32, now 15-of-34).

I re-checked the HTTP status of the two slugs flagged as broken in prior
notes:

| slug | status | first flagged | days unresolved |
|---|---|---|---|
| `respirar-la-montana` | **HTTP 404** | 2026-10-22 | 34 |
| `ofrenda-laboratorio-creativo-multidisciplinar` | **HTTP 404** | 2026-11-15 | 10 |

## Why this matters
Both links are still broken. `respirar-la-montana` has now been 404ing for
**over a month (34 days)** across five consecutive checks with no fix,
redirect, or unpublish. `ofrenda-laboratorio-creativo-multidisciplinar` has
been 404ing for 10 days. These remain the single most concrete, actionable
items from this recurring check — they are reachable from stale references
(not simply rolled-off scheduled experiences, which return 200 per the
2026-11-22 note) and nobody appears to have fixed either one across five
flags.

## Not changed by this run
`known-experiences.json` still lists all 34 previously-known slugs — this
run adds none (zero new experiences today) and removes none (consistent
with prior precedent of never pruning delisted/404ing slugs from the known
set). The other 13 delisted slugs were not individually re-checked this
run; only the two chronic 404s were re-verified.
