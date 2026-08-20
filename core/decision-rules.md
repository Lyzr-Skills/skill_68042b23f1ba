# Decision Rules Framework

Conditional logic mappings to manage experiment outcomes. Prevent perpetual testing of losing channels.

## Core States
- **SCALE**: Allocate more resource, budget, or volume (e.g. +100% volume).
- **CONTINUE**: Maintain experiment run to collect more data.
- **ITERATE**: Modify tactical variables (messaging, offer) but maintain target/channel.
- **PIVOT**: Shift channel tactic or target audience, keeping core hypothesis structure.
- **KILL**: Immediately stop work on experiment and freeze channel spend.

## Execution Matrix
| KPI Level | Condition | Confidence | Action |
|---|---|---|---|
| Primary Metric | $\ge$ Success Threshold | High | SCALE |
| Primary Metric | $\ge$ Success Threshold | Low | CONTINUE |
| Primary Metric | between Success & Failure | - | ITERATE |
| Primary Metric | < Failure Threshold | High | KILL |
| Primary Metric | < Failure Threshold | Low | PIVOT / ITERATE |
