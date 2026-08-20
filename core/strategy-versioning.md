# Strategy Versioning Specification

Keep historical track of strategy adjustments. Maintain ledger of version hops.

## Ledger Scheme
Each update must append to version ledger:
```json
{
  "version_id": "v2",
  "timestamp": "2026-08-20T14:49:00Z",
  "reason_for_change": "Paid social failed to hit minimum CTR threshold. Cold outbound exceeding target.",
  "changes_made": [
    "Deprecate Facebook Ads channel",
    "Double budget allocated to Outbound Email"
  ],
  "previous_version_id": "v1"
}
```

This prevents simple overwrites and creates a chronological narrative of the strategy pivots.
