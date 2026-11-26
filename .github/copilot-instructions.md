# Copilot review instructions

This repository is the Mergington High School activities site: a framework-free front end in
`src/static/` and a small Python API in `src/`.

## Review priorities

- Accessibility: interactive elements need accessible names; keep keyboard focus visible.
- Consistency: reuse the CSS custom properties declared in `:root` instead of hard-coded colors.
- Safety: no secrets, no inline event handlers, no `eval`, and no unescaped user input in the DOM.
- Tests: behaviour changes should come with a test in `tests/`.

## Style

- Match the existing naming and indentation in the file you touch.
- Keep pull requests small and describe the user-visible effect.
