# Self-assessment — IA#1

Submitted by: 24127437 — [Trịnh Khánh Linh]

Total I claim: 97 / 100

| Criterion | Max | I claim | Evidence                                                                                                                                                                                                                                                                                                          |
| --------- | --- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Behaviour | 30  | 30      | All specification rules hold: `npm test` green; `Math.round()` used for whole đồng; empty cart returns 0; invalid price or non-integer qty throws `RangeError`. See `src/cart.js`.                                                                                                                                |
| Tests     | 20  | 20      | 6 tests in `test/cart.test.js` covering worked example (returns 467400), empty cart, free-shipping threshold (500k), and all 3 RangeError cases. All pass.                                                                                                                                                        |
| Harness   | 20  | 17      | `RULES.md` with stack, commands, and three "never" rules; Prettier gate; GitHub Actions CI running on push and green at https://github.com/klinh16/WAD02/actions/runs/38253581112 (branch `IA1`). Deducted 3 points because initial push required follow-up commits to fix Prettier and multi-branch CI triggers. |
| Brief     | 15  | 15      | `BRIEF.md` specifies touched files, exact contract, edge/error cases, and "no dependencies" rule.                                                                                                                                                                                                                 |
| AI-LOG.md | 15  | 15      | `AI-LOG.md` formatted strictly per course template with entries for each task, detailing tool, prompt, kept, changed, rejected, and by-hand work.                                                                                                                                                                 |

## What I did not manage

The initial commit was not completely clean on the first pass: Prettier detected formatting issues in the markdown files and the CI workflow initially lacked branch `IA1` triggers, requiring extra commits to reach all-green.

## What I would do differently

Run all gates (`npm run format:check` and `npm test`) locally and configure universal branch triggers before making the initial commit to keep the repository history pristine from the start.
