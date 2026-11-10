---
type: policy
title: No compiled artifacts in commits
description: Python repos ignore bytecode, and pull requests never contain tracked compiled artifacts.
---
Every Python repo must have a .gitignore that excludes __pycache__/ and *.pyc. A pull request must not contain tracked bytecode or other compiled artifacts. Before opening or approving a PR, run `git ls-files` and check that no such files are tracked. If any are, remove them from the index (for example with `git rm --cached`) and add the ignore rule in the same PR. Generated files bloat diffs, cause needless merge conflicts, and have repeatedly been raised by reviewers as a major finding without being fully fixed.
