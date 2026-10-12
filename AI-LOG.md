# AI-LOG

## 2026-10-10 — project harness and brief

Tool: Gemini 3.1 Pro (via Antigravity IDE)
Asked for: Set up the project harness (RULES.md, CI workflow) and draft the BRIEF.md based on the assignment rubric.
Kept: the RULES.md file, the `.prettierrc` configuration, and the GitHub Actions CI workflow.
Changed: tweaked the `package.json` scripts to ensure `prettier --check` acts as a proper test gate alongside `node:test`.
Rejected: adding third-party test runners or heavy linters; stayed strictly with native node:test and minimal Prettier.
By hand: verified the failing test state locally before proceeding to implementation.

## 2026-10-10 — cartTotal implementation and tests

Tool: Gemini 3.1 Pro (via Antigravity IDE)
Asked for: Implement cartTotal in plain JS and write tests covering happy path, empty cart, threshold, and RangeError edge cases.
Kept: the core mathematical logic (subtotal, vat, shipping) and the separated test structure using the native `node:test` runner.
Changed: ensured the final calculation strictly uses `Math.round()` instead of `.toFixed()` so that it returns a pure Number, not a String, fulfilling the rubric.
Rejected: using any external libraries or dependencies for calculations.
By hand: reviewed the generated logic against the brief, verified tests failed before code was written, and checked edge cases.

## 2026-10-12 — formatting gate and CI verification on GitHub

Tool: Gemini 3.1 Pro (via Antigravity IDE)
Asked for: Diagnose why `npm run format:check` failed, fix formatting across markdown files, and configure CI on a separate branch.
Kept: the auto-formatting output from `prettier --write` and the branch `IA1` push workflow.
Changed: updated `.github/workflows/ci.yml` trigger so CI runs on push to any branch (including `IA1`), not just `main`.
Rejected: ignoring the Prettier check or bypassing the CI gate; ensured both local and remote checks are 100% green.
By hand: created remote repository `WAD02` on GitHub, checked the GitHub Actions run summary, and verified the green tick.
