# Bottleneck Tests

Test funnel constraint identification logic.

## Test Case 1: Low Conversion Gap
- **Input baseline conversion rates**:
  - Traffic to Lead: 10% (Benchmark: 10%)
  - Lead to Demo: 20% (Benchmark: 20%)
  - Demo to Customer: 5% (Benchmark: 25%)
- **Expected primary bottleneck**: Sales Conversion (Demo to Customer).
- **Failure Mode**: Recommending traffic generation campaigns.

## Test Case 2: Low Traffic Gap
- **Input baseline conversion rates**:
  - Traffic to Lead: 1% (Benchmark: 10%)
  - Lead to Demo: 20% (Benchmark: 20%)
  - Demo to Customer: 25% (Benchmark: 25%)
- **Expected primary bottleneck**: Traffic / Lead Generation.
