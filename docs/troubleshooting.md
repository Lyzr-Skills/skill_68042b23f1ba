# Troubleshooting Guide

Diagnose common execution issues.

## Errors Checklist
- **Goal Ambiguity**: Ensure inputs explicitly include deadlines and target values.
- **Arithmetic Inconsistencies**: If funnel conversions do not reconcile, verify the deterministic calculations are enabled in `config/defaults.yaml`.
- **Quality Gate Failures**: Consult `core/quality-gates.md` to see which metrics triggered the block.
