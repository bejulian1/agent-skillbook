---
name: explore
description: Trace an unfamiliar codebase from its entry points to one working flow and identify how to run and test it.
license: Apache-2.0
---

# Trace a working path

Use the user's question to bound the investigation. For a general overview, read the README, root manifest and the entry point of one representative feature. Follow that feature through configuration, implementation and output.

Distinguish the entry point used in production from fixtures, generated files and examples. Trace calls in both directions before assigning a module responsibility. Check how the project actually invokes its tests and build through package scripts, CI or the build configuration.

Return a short map with file references, one end-to-end example and the commands a contributor needs. Label commands you discovered separately from commands you ran.
