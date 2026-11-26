---
applyTo: "src/**/*.py"
---

# Backend review instructions

- Keep the Flask handlers thin; move validation into small helper functions with type hints.
- Validate email addresses and activity names before mutating the in-memory store.
- Never log or return participant email addresses in error messages.
- Preserve the existing REST contract: `GET /activities`, `POST /activities/{name}/signup`,
  `DELETE /activities/{name}/participants/{email}`.
- Add or update a test in `tests/` for every behaviour change.
