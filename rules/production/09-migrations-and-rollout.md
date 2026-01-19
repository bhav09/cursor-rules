## Migrations & rollout

- Prefer additive migrations
- Backfill safely (batched, throttled)
- Deploy code supporting old + new schema
- Remove old schema later

Rollout must include:
- Feature flag or gradual rollout
- Revert steps
