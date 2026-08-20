# Resource Analysis Module

Analyze constraints to ensure feasibility of the growth plan.

## Operations
1. Pull capacity parameters from `schemas/resource-constraints.json`.
2. Sum required hours, budget, and sales tasks from proposed experiments.
3. Compare total demands against available constraints.
4. Scale back or defer lower priority experiments if limits are exceeded.
