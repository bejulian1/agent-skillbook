---
name: review
description: Review a diff or a bounded area of code and report concrete bugs, regressions and missing coverage.
license: Apache-2.0
---

# Review a change

Read the diff and its base, then follow changed behavior to callers and relevant tests. For a review of the working tree, include staged and unstaged changes and inspect in-scope new files. Use the scope the user gave.

Check defaults, error paths, interrupted writes, older stored data and concurrent operations where they affect the change. For each candidate finding, identify the input or state that reaches it and the observable consequence. Verify the line reference against the revision reviewed.

Present the highest-impact findings first. Give the location, trigger, consequence and a focused correction. Separate verified defects from unanswered questions. If no findings survive that check, say what you reviewed and where coverage is limited. A request for review calls for findings in the response.
