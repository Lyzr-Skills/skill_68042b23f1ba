# Assumption Management Specification

Isolate facts from guesses. Prevent AI from inventing metrics.

## Categorization
Every metric used in calculations must be logged with one of:
- **Actual**: Verified historical company data.
- **Benchmark**: Industry standard conversion rates (e.g. SaaS email reply rate = 2%).
- **Assumption**: Educated guess for a new tactic.
- **Target**: Needed performance to hit goal.

## Math Verification Rule
Growth math engine must tag every cell in the calculated model with its category. If a path contains an `Assumption`, the final result must be flagged as "Unvalidated Model".
