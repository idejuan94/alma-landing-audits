# Run blocked — network egress denied

**Date:** 2026-09-28

This run could not reach the live site at all. Fetching
`https://almawellness.io/experiencias` failed with:

```
EGRESS_BLOCKED: Access to almawellness.io is blocked by the network egress proxy.
```

This is different from the "client-rendered app shell" case the audit
process anticipates — it's not that the page returned empty content, it's
that the sandboxed environment's network policy denies outbound requests
to `almawellness.io` entirely. No page content was retrieved, so no diffing
or auditing could be performed this run.

## What needs to happen
A human needs to update this environment's network access settings (cloud
environment menu → Edit → Network access) to either allow a broader access
level or explicitly add `almawellness.io` to the allowed domains. Once that
is done, the next scheduled run should be able to fetch the site normally.

No changes were made to `known-experiences.json` since no data was
retrieved.
