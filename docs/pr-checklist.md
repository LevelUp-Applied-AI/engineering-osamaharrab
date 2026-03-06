# PR Self-Review Checklist

Before opening a pull request, confirm the following:

- [ ] The code implements exactly what the PR title describes — no hidden or unrelated changes.
- [ ] All existing tests pass locally, and new tests are added if behavior changed.
- [ ] Edge cases and failure scenarios have been considered and handled.
- [ ] The README and documentation reflect any new commands, dependencies, or behavior changes.
- [ ] The PR contains one logical change only (no scope creep).
- [ ] No debug artifacts remain (no breakpoint(), print statements, commented-out blocks).
- [ ] Dependencies added or removed are intentional and documented.
- [ ] The code follows project style and naming conventions.

