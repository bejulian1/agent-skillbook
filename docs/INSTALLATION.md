# Install and use a skill

Read the skill you want in the [catalog](../CATALOG.md). Each folder under `skills/` is independently usable. The collection currently consists of Markdown instructions.

## Copy into a local project

For local projects, Codex discovers skills in `.agents/skills/` and Claude Code discovers them in `.claude/skills/`. Other clients may use a different location or an import dialog. [Codex skill locations](https://learn.chatgpt.com/docs/build-skills) · [Claude Code skill locations](https://code.claude.com/docs/en/skills)

Download the [source archive](https://github.com/bejulian1/agent-skillbook/archive/refs/heads/main.zip) or clone the collection.

```console
git clone https://github.com/bejulian1/agent-skillbook.git
```

From your **destination project's root**, run this example in a POSIX shell. Set `skillbook` to the path where you unpacked or cloned the collection. For Claude Code, change the `skills_dir` assignment to `.claude/skills`.

```sh
skillbook=/path/to/agent-skillbook
skills_dir=.agents/skills
name=action-items

(
  set -e
  test -f "$skillbook/skills/$name/SKILL.md"
  test -f "$skillbook/LICENSE"
  mkdir -p "$skills_dir"
  mkdir "$skills_dir/$name"
  cp -R "$skillbook/skills/$name/." "$skills_dir/$name/"
  cp "$skillbook/LICENSE" "$skills_dir/$name/LICENSE"
)
```

The separate `mkdir` stops the copy if a skill with that name already exists. To update an installed skill, compare the two folders first and keep any local edits you need.

Open a session in the destination project and look for `action-items` in the skill picker. In Codex, choose it with `$action-items`. In Claude Code, use `/action-items`. Give it a few lines of meeting notes. Check the owner, due date and quoted evidence against the notes.

## Use the instructions directly

If your client has no skills directory, open the relevant `SKILL.md`, copy the Markdown below its YAML header into your conversation and add your own inputs. A pasted log is enough for CI triage. A downloadable workbook requires a client that can create files. See the [skill format](SKILL-FORMAT.md) for the file structure.
