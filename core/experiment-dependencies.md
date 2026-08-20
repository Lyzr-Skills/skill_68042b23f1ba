# Experiment Dependency Management

Manage relationships and execution sequences.

## Schema Support
Each experiment record contains:
- `dependencies`: List of experiment IDs that must complete first.
- `blocked_by`: List of experiment IDs actively blocking this experiment.

## Sequence Validation
1. **Linear dependency**: Exp B runs only if Exp A outcome is SCALE or CONTINUE.
2. **Resource lock**: Prevent overlapping experiments on same audience segment.
