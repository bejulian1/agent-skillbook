---
name: skill-creator
description: Turn a recurring task into a discoverable SKILL.md with focused instructions and a realistic acceptance check.
license: Apache-2.0
---

# Write a reusable skill

Choose one recurring task and a realistic request that should activate the skill. Also identify a nearby request that belongs to a different workflow. Use the distinction to write a short description that makes the skill discoverable.

Create a directory named for the skill with a SKILL.md entry point. Use lowercase letters, digits and hyphens for the directory and matching name. Put name and description in YAML frontmatter. Write the workflow in the Markdown body. Include supporting files only when the workflow needs them, and link to them using relative paths.

Describe the decisions and checks that change the result. Use the current request for inputs and let the host supply available tools. Exercise the skill with a representative input and inspect its output against the intended result. Validate the metadata and links before delivering the folder.
