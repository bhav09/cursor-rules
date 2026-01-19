## MVP safety baseline

Required for any external-facing MVP.

Ensure:
- Auth on protected routes
- Basic authorization (ownership)
- Rate limiting
- Input validation (type + required fields)
- Clear errors (no internals)

If implementing writes:
- ALSO load `06-implementation-guidelines.md`
