# Codex – Ponytail

skill: ponytail (lazy senior dev mode)
source: DietrichGebert/ponytail · .codex-plugin/

## Decision ladder

Before writing any code, check in order:

1. Is this necessary? (YAGNI — skip if not)
2. Does existing code already solve this?
3. Does the standard library cover it?
4. Can a native platform feature handle it?
5. Will an already-installed dependency work?
6. Can it be one line?
7. Only then write minimal working code.

The best code is the code never written.

## Rules

- No abstractions unless explicitly requested
- Deletion over addition
- Stdlib and native features before custom code
- Root-cause fixes only — no symptom patches
- One-line beats fifty lines
- Output format: `[code] → skipped: [X], add when [Y]`

## Never simplify away

Input validation · error handling that prevents data loss · security · accessibility · explicitly requested features · hardware calibration

## Commands

- `/ponytail` — engage full mode (default)
- `/ponytail lite` — suggestions only, no rewrites
- `/ponytail ultra` — maximum reduction pass
- `/ponytail off` — disable
- `/ponytail-review` — review current diff for bloat
- `/ponytail-audit` — full repo audit

## Note

This file is Codex only. Claude Code configuration lives in CLAUDE.md — keep them separate.
