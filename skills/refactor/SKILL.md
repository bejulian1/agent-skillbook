---
name: refactor
description: Restructure existing code while preserving its observable behavior and the interfaces its callers use.
license: Apache-2.0
---

# Restructure code while preserving behavior

Identify the observable contract first, including inputs, return values, errors, ordering, side effects and any serialized form. Find the callers, including configuration, tests and names referenced as strings.

Establish a baseline with the most relevant existing checks. Split the change into reviewable steps and use the checks between moves. When extracting shared logic, compare the original callers' edge cases before folding them together.

Review the resulting diff for incidental behavior changes and formatting churn. Report which public entry points you exercised and any behavior the existing suite leaves unverified.
