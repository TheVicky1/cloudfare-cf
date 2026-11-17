---
"cf": patch
---

Support `CLOUDFLARE_PROFILE` and accurately report missing auth profiles

Support `CLOUDFLARE_PROFILE` as an environment variable alongside `CLOUDFLARE_AUTH_PROFILE`.
When commands resolve or are given a non-existent auth profile, report that the specified profile
was not found and list available profiles instead of emitting a misleading "No authentication token found" error.
