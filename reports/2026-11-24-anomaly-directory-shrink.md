# Anomaly note — the two chronic 404s are now 1+ month unresolved
Date: 2026-11-24

Continuing the thread from the 2026-10-22, 2026-11-15, and 2026-11-22 anomaly
notes. This is a note on an out-of-scope anomaly noticed while diffing the
directory page, alongside the normal 2-new-experience audit for this run
(see the two `2026-11-24-*.md` reports).

## What changed
The live directory page (`/experiencias`) now shows **19** experiences (up
from 17 on 2026-11-22), including the 2 new listings audited today.
`known-experiences.json` tracked 32 previously-seen slugs going into this
run; of those, 17 are still live and 15 are currently absent from the
directory — consistent with the same delisting pattern noted in all three
prior notes (6-of-14, then 14-of-25, then 15-of-28, now 15-of-32).

I re-checked the HTTP status of the two slugs flagged as broken in the last
two notes:

| slug | status | first flagged |
|---|---|---|
| `respirar-la-montana` | **HTTP 404** | 2026-10-22 |
| `ofrenda-laboratorio-creativo-multidisciplinar` | **HTTP 404** | 2026-11-15 |

## Why this matters
**`respirar-la-montana` has now been 404ing for over a month (33 days,
2026-10-22 → 2026-11-24)** with no fix, redirect, or unpublish.
`ofrenda-laboratorio-creativo-multidisciplinar` has been 404ing for at least
9 days. Neither looks like a scheduled-experience-rolled-off case (those
pages still return 200 per the 2026-11-22 note) — these are broken links
still reachable from stale references, and nobody appears to have noticed
or fixed either one across three prior flags. This is the single most
concrete, actionable item to come out of this recurring check.

## Not changed by this run
`known-experiences.json` still lists all 32 previously-known slugs plus the
2 new ones found today — this run does not remove delisted or 404ing slugs
from the known set, consistent with prior precedent. The other 13 delisted
slugs were not individually re-checked this run (last fully re-checked
2026-11-22); only the two chronic 404s were re-verified.
