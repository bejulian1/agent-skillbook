---
name: docs
description: Write or update project documentation with commands, options and examples checked against the implementation.
license: Apache-2.0
---

# Document a working interface

Choose one intended reader and identify what they need to accomplish. Read the implementation, public entry point and existing documentation before describing an option, default or behavior.

Put a complete example near the task it solves. Use the actual command, path, configuration keys and expected result. Test the example in a disposable workspace if practical. For a command that publishes or changes external state, verify its syntax and describe the effect.

Update the existing source of documentation and its links. When behavior varies by version or environment, state the condition where it matters. Report which examples you exercised and which details you checked from source.
