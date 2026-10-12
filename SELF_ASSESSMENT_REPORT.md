# Self-assessment — IA#1

Submitted by: 24127437 — [Họ và tên sinh viên]

Total I claim: 100 / 100

| Criterion | Max | I claim | Evidence                                                                                                                                                                                                        |
| --------- | --- | ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Behaviour | 30  | 30      | All specification rules hold: `npm test` green; `Math.round()` used for whole đồng; empty cart returns 0; invalid price or non-integer qty throws `RangeError`. See `src/cart.js`.                              |
| Tests     | 20  | 20      | 6 tests in `test/cart.test.js` covering worked example (returns 467400), empty cart, free-shipping threshold (500k), and all 3 RangeError cases. All pass.                                                      |
| Harness   | 20  | 20      | `RULES.md` with stack, commands, and three "never" rules; `npm run format:check` gate; GitHub Actions CI running on push and green at https://github.com/klinh16/WAD02/actions/runs/38250328644 (branch `IA1`). |
| Brief     | 15  | 15      | `BRIEF.md` specifies touched files, exact contract, edge/error cases, and "no dependencies" rule.                                                                                                               |
| AI-LOG.md | 15  | 15      | `AI-LOG.md` formatted strictly per course template with entries for each task, detailing tool, prompt, kept, changed, rejected, and by-hand work.                                                               |

## What I did not manage

None. All 5 criteria and edge cases were successfully implemented, tested locally, and verified green on GitHub Actions CI.

## What I would do differently

Next time, configure Prettier and CI triggers for all branches right from the initial commit to avoid any formatting hiccups during the first gate check.
