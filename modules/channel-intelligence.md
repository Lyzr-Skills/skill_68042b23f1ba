# Channel Intelligence Module

Evaluate and select acquisition channels.

## Ranking Rules
- Calculate weights using `config/channel-scoring.yaml`.
- Score channels against target ICP accessibility.
- Map channels to primary and secondary funnel stages (e.g. SEO maps to Reach, Outbound maps to Meeting).
- Output prioritized channels as structured lists in `schemas/channel.json`.
