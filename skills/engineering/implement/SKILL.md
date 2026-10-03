---
name: implement
description: "Build planned work (a spec, a ticket, or a plan agreed in the conversation) test-first, then review it and commit to the current branch. Use only when the user explicitly asks you to implement or build that work."
---

This skill writes code and commits it to the current branch, so it runs on the user's explicit request only. If the user has not asked you to implement this work, stop and ask them before writing any code.

Implement the work described by the user in the spec (`docs/specs/`) or ticket (`docs/tickets/`), or the plan agreed in the conversation.

Use /tdd where possible, at pre-agreed seams.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once done, call the Skill tool with `codereview` (one word, not the built-in `code-review`) to review the work.

If the work came from a ticket file, set its `**Status:**` to `done` and tick the acceptance criteria the work meets.

Commit your work to the current branch.
