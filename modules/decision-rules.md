# Decision Rules Module

Enforce conditional action rules during experiment runtime.

## Core Checks
Assess metrics at scheduled checkpoints:
- **IF** conversion meets success threshold: Scale channel.
- **IF** conversion below failure threshold: Kill/Pivot channel.
Format output into `schemas/decision-rule.json`.
