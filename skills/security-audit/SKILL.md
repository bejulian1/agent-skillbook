---
name: security-audit
description: Review application source for access-control, data-handling and configuration risks and suggest defensive fixes.
license: Apache-2.0
---

# Review defensive controls in source

Identify the assets and trust boundaries relevant to the requested code. Start with entry points that accept external data. Trace how the application authenticates the caller, authorizes access to the specific resource and validates data before storing, displaying or forwarding it.

Inspect the controls in context. For example, an authenticated request can still access another account's record if the query omits ownership. Check parameter binding, output escaping, path confinement, secret handling and safe failure behavior where those boundaries exist.

Tie each finding to a code location, affected asset and missing or insufficient control. Propose a scoped remediation and a safe regression check with synthetic fixtures. Keep secret values out of the report. Separate evidenced implementation defects from assumptions about deployment.
