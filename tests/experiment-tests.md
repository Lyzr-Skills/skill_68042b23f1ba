# Experiment Tests

Verify experiment design structure and scoring rules.

## Test Case 1: Threshold Presence
- **Input**: Generated Experiment draft.
- **Expected validation**: Fail if `threshold` field is missing or qualitative (e.g. "high engagement" is invalid; must be numeric "CTR > 2%").

## Test Case 2: Dependencies Check
- **Input**: Linear dependency chain.
- **Expected validation**: Throw error if dependency graph has circular blocks.
