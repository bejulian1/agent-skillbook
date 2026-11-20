# Contributing

Start with a real task that the current [catalog](CATALOG.md) handles poorly or leaves uncovered. A small improvement to an existing skill is welcome. Include a short sample request and explain what a reader should be able to check in the result.

1. Put the instructions in `skills/<name>/SKILL.md` and follow the [format guide](docs/SKILL-FORMAT.md). Use a description that helps the agent distinguish the task from neighboring skills.
2. Exercise the instructions with a representative input. Include an edge case if it changes the answer, such as an unassigned task, an incomplete log or a zero denominator.
3. Verify the folder name, YAML header and relative links. Add new skills to the catalog and update its count in the README.
4. In your pull request, describe the observed result and identify which checks you ran. Use synthetic or publicly shareable examples.

Submit material you have permission to distribute under the project's [Apache License 2.0](LICENSE). Preserve applicable attribution when adapting contributed material.
