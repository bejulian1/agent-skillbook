---
name: debug
description: Trace unexpected application behavior to its cause, apply a scoped fix and check the original failure.
license: Apache-2.0
---

# Diagnose and fix a failure

Capture the smallest input that shows the reported behavior, the expected result and the observed result. Use a disposable fixture if the failing operation writes data. Follow the first useful application frame or incorrect state back to the point where it is produced.

Form a specific explanation that predicts an observable difference. Test it by changing one input or inspecting the value at the boundary. A second failure after the first one can be a consequence of the first.

Fix the cause within the requested scope. Rerun the original case and a nearby case that should still work. Where the suite misses this failure, add a regression check through the normal caller. Report the cause, the change and the evidence. If reproduction was unavailable, identify which part of the diagnosis is inferred.
