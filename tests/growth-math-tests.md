# Growth Math Tests

Test validation scenarios for deterministic calculations.

## Test Case 1: Standard Funnel Retrograde
- **Goal**: 20 customers
- **Baseline conversion rates**:
  - Demo to Customer = 25%
  - Lead to Demo = 20%
  - Traffic to Lead = 10%
- **Expected calculated outputs**:
  - Required demos = 80
  - Required leads = 400
  - Required traffic = 4000
- **Validation**: Calculate programmatically. Fail if outputs are estimated by LLM.

## Test Case 2: Zero Win Rate Guard
- **Goal**: 10 customers
- **Win rate**: 0%
- **Expected calculated outputs**: Catch division-by-zero error, throw validation error.
