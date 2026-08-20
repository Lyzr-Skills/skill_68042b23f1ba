# Architecture Specification

GTM Strategy Engine system architecture.

## Modules Structure
- **Goal Definition**: Resolves input targets and deadlines.
- **Growth Math Engine**: Performs programmatic retrograde/forward funnel calculation.
- **Resource Constraints**: Confirms feasibility.
- **Channel Intelligence**: Scores matching acquisition channels.
- **Experiment Engine**: Design structured trials with dependencies and decision rules.
- **Strategy State & Memory**: Logs outcomes and increments strategy version.

## Data Schemas Mapping
```
Goal -> Baseline -> GrowthModel -> Bottleneck -> Hypothesis -> Channel -> Experiment -> KPI -> Result -> Learning -> Version Update
```
