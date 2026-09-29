---
name: implement
description: "Build planned work (a spec, a ticket, or a plan agreed in the conversation) test-first, then review it and commit to the current branch. Use only when the user explicitly asks you to implement or build that work."
---

This skill writes code and commits it to the current branch, so it runs on the user's explicit request only. If the user has not asked you to implement this work, stop and ask them before writing any code.

Implement the work described by the user in the spec (`docs/specs/`) or ticket (`docs/tickets/`), or the plan agreed in the conversation.

Use /tdd where possible, at pre-agreed seams.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once done, call the Skill tool with the two-axis `code-review` (Standards + Spec) to review the work. The harness may also list a built-in `code-review`, a bug hunt at an effort level: that is a different skill. The two-axis one is usually namespaced by its plugin (`<plugin>:code-review`). Call a bare `code-review` only after checking that its description names the Standards and Spec axes.

If the work came from a ticket file, set its `**Status:**` to `done` and tick the acceptance criteria the work meets.

Commit your work to the current branch.
