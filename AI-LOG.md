# AI-LOG.md

## 2026-10-10 — project harness and brief

Tool: Gemini 3.1 Pro (via Antigravity IDE)
Asked for: Set up the project harness (RULES.md, CI workflow) and draft the BRIEF.md based on the assignment rubric.
Kept: the RULES.md file, the `.prettierrc` configuration, and the GitHub Actions CI workflow.
Changed: tweaked the `package.json` scripts to ensure `prettier --check` acts as a proper test gate alongside `node:test`.
Rejected: nothing, the initial setup provided a solid starting point.
By hand: verified the failing test state locally before proceeding to implementation.

## 2026-10-10 — cartTotal implementation and tests

Tool: Gemini 3.1 Pro (via Antigravity IDE)
Asked for: Implement cartTotal in plain JS and write tests covering happy path, empty cart, threshold, and RangeError edge cases.
Kept: the core mathematical logic (subtotal, vat, shipping) and the separated test structure using the native `node:test` runner.
Changed: ensured the final calculation strictly uses `Math.round()` instead of `.toFixed()` so that it returns a pure Number, not a String, fulfilling the rubric.
Rejected: using any external libraries or dependencies for calculations.
By hand: reviewed the generated logic against the brief, ran the final `npm test` and `npm run format`, and zipped the submission files.
