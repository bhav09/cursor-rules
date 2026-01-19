## Implementation guidelines (MVP)

- Follow existing repo patterns.
- Avoid new architecture unless required.
- All write paths must be safe to retry.
- Avoid per-item DB calls in loops.

If something breaks:
- ALSO load `07-debugging-and-failures.md`
