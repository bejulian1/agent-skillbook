---
name: web-qa
description: Exercise a user journey in a browser and document reproducible usability, layout or functional problems.
license: Apache-2.0
---

# Exercise a browser journey

Establish the URL, the user journey and how success is visible. Use a disposable account or fixture for actions with side effects. Record the starting viewport and state so another person can repeat the check.

Walk the journey with the available browser controls. Inspect the page after each consequential action. Try keyboard navigation and a relevant edge case, such as an empty input, a failed request or a narrow viewport. If the expected result is uncertain, check the specification or nearby behavior before filing a defect.

For each issue, give the smallest reproducible sequence, expected and observed outcomes, and the evidence that connects them. Use a screenshot for a visual defect or a relevant console message for a functional failure. Omit personal information from evidence. State which parts of the journey you exercised.
