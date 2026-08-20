# Bottleneck Detection Module

Analyze funnel to pinpoint growth constraints.

## Logic
1. Compare baseline conversion rates to industry benchmarks (from `schemas/assumption.json`).
2. Identify the funnel stage with the largest negative percentage gap.
3. Classify constraint (e.g. "Primary bottleneck: Sales conversion").
4. Pass constraint to hypothesis generator so targeting focus is optimized.
