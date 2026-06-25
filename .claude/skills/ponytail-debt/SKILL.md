---
name: ponytail-debt
description: >
  Harvests ponytail: comments throughout the codebase to produce a debt ledger. Prevents deliberate shortcuts from becoming permanent oversights. Use when the user says "ponytail debt", "/ponytail-debt", "what did ponytail defer", "list the shortcuts", "ponytail ledger", or "what did we mark to do later".
---

Scan the repo for `ponytail:` comments (exclude node_modules, .git, build dirs). For each one output the file, line number, simplified approach, ceiling (limit), and upgrade trigger.

Flag entries lacking an upgrade path as `no-trigger` — these have the highest rot risk.

Read-only. Reports findings, modifies nothing. Optionally persists results to a file if the user requests it.

"stop ponytail-debt" or "normal mode" to revert.
