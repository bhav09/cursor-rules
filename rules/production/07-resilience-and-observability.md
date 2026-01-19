## Resilience & observability

Every major function must log:
- Start (with request/correlation ID)
- Success (duration)
- Failure (safe context)

Add where supported:
- Metrics
- Tracing
- Timeouts
- Retries with backoff
- Circuit breakers
