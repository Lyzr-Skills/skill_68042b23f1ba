# Growth Math Engine Specification

CRITICAL RULE: DO NOT let the LLM perform arithmetic when deterministic calculation is possible.

All numbers (deal requirements, conversion ratios, traffic, budget requirements) must be computed programmatically.

## Funnel Flow Equations

### 1. Retrograde Calculation (Bottom Up)
Given target customers $C_t$:
$$\text{Opportunities Required } (O) = \frac{C_t}{\text{Win Rate } (r_{opp\_to\_cust})}$$
$$\text{Meetings Required } (M) = \frac{O}{\text{Meeting-to-Opportunity Conversion } (r_{mtg\_to\_opp})}$$
$$\text{Leads Required } (L) = \frac{M}{\text{Lead-to-Meeting Conversion } (r_{lead\_to\_mtg})}$$
$$\text{Traffic Required } (T) = \frac{L}{\text{Visitor-to-Lead Conversion } (r_{vis\_to\_lead})}$$

### 2. Forward Calculation (Top Down)
Given traffic $T$:
$$L = T \times r_{vis\_to\_lead}$$
$$M = L \times r_{lead\_to\_mtg}$$
$$O = M \times r_{mtg\_to\_opp}$$
$$C = O \times r_{opp\_to\_cust}$$

## Execution Mode
Implement growth calculations using pure JSON objects passing through deterministic helper scripts/evaluators. No LLM estimation.
