# Strategy Learning Module

Process results to update baseline assumptions and channels.

## Execution Flow
1. Load `schemas/experiment-result.json`.
2. Extract actual conversion rate and calculate statistical learning confidence.
3. Update `schemas/strategy-state.json` to record winning and failed tactics.
4. Modify channel scoring multipliers based on results.
