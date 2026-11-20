# Skill format

Each `skills/<name>/SKILL.md` starts with YAML frontmatter followed by instructions in Markdown. The folder name matches the lowercase, hyphenated `name`. The `description` tells a client when to offer the skill. This collection uses the optional `license` field. [Agent Skills specification](https://agentskills.io/specification)

```markdown
---
name: action-items
description: Extract decisions, owners, deadlines and open questions from meeting notes.
license: Apache-2.0
---

# Extract decisions and commitments

Identify what was agreed, who took responsibility and where the source records it.
```

Use the current conversation for task inputs. Describe the capabilities the task needs in ordinary language, and supply a fallback where a missing capability would change the answer. Keep reusable examples or references inside the skill folder if the instructions depend on them.
