# Project rules

Stack: Vanilla JavaScript, Node.js native test runner (`node:test`), Prettier. Nothing else without asking.
Style: 2-space indent, no semicolons, single quotes (enforced by Prettier).
Commands: npm run format:check · npm run format · npm test
Tests: every requirement in the brief gets a test under test/.
Never: use external dependencies for the main logic, skip writing tests for edge cases, commit without running gates.
