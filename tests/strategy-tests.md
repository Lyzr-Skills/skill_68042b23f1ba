# Strategy Tests

Validate complete strategy generation reports against schemas.

## Test Case 1: Structure Matching
- **Input**: Complete Strategy output.
- **Expected validation**: Pass through JSON Schema validator for `schemas/strategy-report.json`.

## Test Case 2: Gate Enforcement
- **Input**: Run with goal "Increase sales next quarter".
- **Expected validation**: Assert output is exactly Gate 1 "Insufficient Information" message.
