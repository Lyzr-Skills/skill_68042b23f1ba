# Scoring Model Specification

Deterministic scoring for both Channels and Experiments.

## Channel Scoring Model
$$\text{Channel Score} = W_{icp}\text{ICP} + W_{reach}\text{Reach} + W_{intent}\text{Intent} + W_{speed}\text{Speed} + W_{cost}\text{Cost} + W_{team}\text{Team} + W_{traction}\text{Traction} - W_{comp}\text{Competition}$$

Values graded on a 1-10 scale. Weights defined in `config/channel-scoring.yaml`.

## Experiment Prioritization Model (ICE-Effort)
$$\text{Priority Score} = \frac{\text{Impact} \times \text{Confidence} \times \text{Speed}}{\text{Effort}}$$

All values graded on 1-10 scale. Handled via programmatic execution.
