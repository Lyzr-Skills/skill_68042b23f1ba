# Quality Gates Specification

Validation checks before strategy output generation. Stop execution and output "Insufficient Information" if critical gates fail.

## Gate Criteria

### Gate 1: Measurable Goal
Is target metric specified and measurable?
- *Failure Mode*: "Grow fast" → Fail.

### Gate 2: Explicit Timeframe
Is deadline or timeframe defined?
- *Failure Mode*: "Get 20 customers" without timeframe → Fail.

### Gate 3: Known ICP
Is target market segment defined?
- *Failure Mode*: Target customer missing → Fail.

### Gate 4: Baseline Adequacy
Is there sufficient historical data?
- *Action*: Generate warnings if assumptions are used instead of actuals.

### Gate 5: Assumption Log Verification
Are assumptions documented and isolated from facts?
- *Failure Mode*: Missing source/references for numbers → Fail.

### Gate 6: Resource Check
Can the team actually execute the proposed strategy?
- *Failure Mode*: Proposed strategy requires 100 hours/week, capacity is 20 hours/week → Fail.

### Gate 7: Success Criteria Check
Does every single experiment have a measurable success/failure threshold?
- *Failure Mode*: Experiment has no numeric threshold → Fail.
