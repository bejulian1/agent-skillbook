---
name: verify
description: Check whether a finished change satisfies the request using its diff, normal entry points and relevant tests.
license: Apache-2.0
---

# Verify a finished change

Translate the user's request into observable acceptance checks. Read the complete relevant diff and confirm the changed path is reachable through its normal entry point. Check older data or existing callers when a format or interface changed.

Run the smallest check that exercises the reported case and then the project's relevant type, test or build checks. For UI changes, interact with the affected control and inspect the resulting state. For exported files, reopen the actual deliverable. A successful build alone answers only the build question.

Record the command or action, its result and the revision or artifact it covers. Distinguish existing failures from regressions using a baseline when needed. Finish with any acceptance condition still unverified.
