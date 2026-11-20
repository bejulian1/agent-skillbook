---
name: tdd
description: Implement a behavior change through a failing test, a minimal implementation and a refactoring pass.
license: Apache-2.0
---

# Develop a change test first

Pick one user-visible behavior and express it through the project's usual public entry point. Use an existing nearby test as a guide to fixture setup and naming.

1. Run the new test against the current code. Check that it fails on the intended assertion. A missing dependency or a broken fixture does not establish the behavior gap.
2. Make the smallest implementation change that satisfies the case. Rerun that test, then the neighboring cases.
3. With the tests passing, simplify the implementation or fixture if doing so makes the next change clearer.

Repeat for the next distinct behavior. Report the observed failure and passing result, with the commands used to reproduce them.
