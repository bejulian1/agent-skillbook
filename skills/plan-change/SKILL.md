---
name: plan-change
description: Plan a change that spans components or admits several designs, with concrete decisions and acceptance checks.
license: Apache-2.0
---

# Plan a change

Identify what a user or caller should be able to do when the change is finished. Trace the current path and identify the interfaces, stored data and external consumers it crosses.

If two approaches have different consequences, name the trade-off that affects this project. For example, a stored format change may need a migration and an older client may still write the previous format. Resolve decisions you can answer from the repository.

Order the work by dependency. Give each step a concrete result and a way to check it. Surface the one decision that needs the user's input if it would change the plan materially. When the request is for a plan, deliver the plan itself.
