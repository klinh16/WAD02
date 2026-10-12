# Self-assessment — IA#1

Submitted by: 24127437 — [Trịnh Khánh Linh]
Repository: https://github.com/klinh16/WAD02.git (Branch: IA1)

Total I claim: 97 / 100

| Criterion | Max | I claim | Evidence                                                                                                                                                                                                                                                    |
| --------- | --- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Behaviour | 30  | 30      | All specification rules hold: `npm test` green; `Math.round()` used for whole đồng; empty cart returns 0; invalid price or non-integer qty throws `RangeError`. See `src/cart.js`.                                                                          |
| Tests     | 20  | 20      | 6 tests in `test/cart.test.js` covering worked example (returns 467400), empty cart, free-shipping threshold (500k), and all 3 RangeError cases. All pass.                                                                                                  |
| Harness   | 20  | 20      | `RULES.md` with stack, commands, and three "never" rules; Prettier gate; GitHub Actions CI running on push and green at https://github.com/klinh16/WAD02/actions/runs/38255980969 (branch `IA1`).                                                           |
| Brief     | 15  | 15      | `BRIEF.md` specifies touched files, exact contract, edge/error cases, and "no dependencies" rule.                                                                                                                                                           |
| AI-LOG.md | 15  | 12      | Formatted per course template with entries for each task. Deducted 3 points because entries were reconstructed shortly after each task rather than written strictly in real time, omitting some minor prompt iterations and intermediate rejected snippets. |

## What I did not manage

In `AI-LOG.md`, entries were reconstructed shortly after completing the work rather than strictly written as I went, so a few intermediate prompt iterations and rejected snippets were not logged in full detail.

## What I would do differently

Write the AI-LOG entries immediately as each prompt runs instead of summarizing after the task, ensuring every rejected assistant output is captured with complete fidelity.
