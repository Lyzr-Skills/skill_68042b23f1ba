# Regression Tests

Verify updates do not degrade prior validated plans.

## Checks
1. Re-run historical strategy inputs (v1 strategy files) with new code version.
2. Assert version updates increment correctly in the ledger.
3. Assert old learnings stored in `strategy-state` remain active and channel weight penalties are preserved.
