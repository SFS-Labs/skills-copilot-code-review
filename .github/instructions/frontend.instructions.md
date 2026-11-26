---
applyTo: "src/static/**"
---

# Frontend review instructions

- Keep the site dependency-free: plain HTML, CSS and JavaScript only.
- Use the palette and spacing tokens from `src/static/styles.css`; do not introduce new fonts or colors.
- Every new control must be reachable by keyboard and have an `aria-label` or visible label.
- Guard DOM queries: the page renders activity cards asynchronously, so handle the empty state.
- Prefer `textContent` over `innerHTML` when inserting user-provided values.
