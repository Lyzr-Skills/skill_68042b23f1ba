# Experiment Prioritization Module

Order experiment queue to optimize resources.

## ICE Score Execution
Use programmatic scoring rules:
$$\text{Score} = \frac{\text{Impact} \times \text{Confidence} \times \text{Speed}}{\text{Effort}}$$
Filter out experiments below config-level priority threshold.
