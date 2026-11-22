# Agent Skillbook

A collection of 28 Markdown skills for AI agents. Each folder teaches one task, from turning meeting notes into action items to tracing a failed CI run. Pick the skills you need and use them with a client that reads `SKILL.md`.

## Pick a skill

| If you have… | Try | What you get |
| --- | --- | --- |
| Meeting notes with corrections and loose ends | [action-items](skills/action-items/SKILL.md) | Agreed actions, owners, deadlines and the passage behind each entry |
| Two sources that seem to disagree | [source-brief](skills/source-brief/SKILL.md) | A cited answer that accounts for dates, versions and gaps |
| A CSV and a question about a change | [analyze-data](skills/analyze-data/SKILL.md) | A checked comparison with units, denominators and group contributions |
| A slow operation with two implementations | [benchmark](skills/benchmark/SKILL.md) | Comparable timings, the spread between trials and a repeatable procedure |
| A pull request with a red check | [ci-triage](skills/ci-triage/SKILL.md) | The failed step, the diagnostic that explains it and the next check |

[Browse all 28 skills](CATALOG.md), including code review, browser QA, Excel, Word and PowerPoint.

## Try it with meeting notes

Open [action-items](skills/action-items/SKILL.md), use its instructions in your agent and give it this note.

> Monday planning, item 3. Maya will send the draft after Legal approves it. Ben suggested a Friday release. The team agreed to keep the current price.

The resulting register should identify Maya's conditional task, leave its due date unspecified, preserve Friday as a suggestion and record the pricing decision separately. This example works with text alone.

## Install one skill

Download or clone the collection, then copy one folder from `skills/` into your client's skills directory. In a local coding project, Codex reads `.agents/skills/` and Claude Code reads `.claude/skills/`. The installation guide includes a copy command and a discovery check. [Installation and usage](docs/INSTALLATION.md)

Each skill uses the tools available in your session. For example, diagnosing a CI failure can start from a pasted log, while measuring a benchmark requires a way to run the workload or comparable measurements supplied by you.

## Contributing

Contributions are welcome, especially worked examples that expose a failure in an existing skill. [Contribution guide](CONTRIBUTING.md) · [Credits](CREDITS.md) · [Apache License 2.0](LICENSE)
