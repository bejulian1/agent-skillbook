---
name: git
description: Prepare a scoped Git commit, branch, push or GitHub pull request when the user asks for repository work.
license: Apache-2.0
---

# Prepare a scoped Git change

Use the requested repository and branch. Inspect status and both staged and unstaged diffs. Keep existing staged work from other tasks out of the commit. If the index contains unrelated changes, use an isolated worktree or a path-scoped operation that preserves them.

Stage the files or hunks that belong to the request. Review the staged diff and run the relevant checks before committing. Follow the repository's commit style and confirm the final commit contains the intended paths.

For a requested push, inspect the remote and destination branch first. For a requested pull request, check its base and head, summarize the user-visible change and report the checks actually run. Verify the remote commit or pull request before returning its link. A request to inspect a repository authorizes read-only work.
