# Waza Pull Request Requirements

- Use the repository PR template and reference the related issue when there is one.
- Keep the change scoped; preserve compatibility and all existing passing tests.
- Run relevant targeted checks during development. Before pushing Go code, run the
  full Go tests and required formatting/lint checks documented in `AGENTS.md`.
- For dashboard changes, run the build, lint, and Chromium Playwright suite; update
  affected screenshots. Build public docs when they change.
- Record exact validation commands and outcomes, including anything not run.
  Mock or offline success is not evidence of live model quality.
- Document changed CLI flags, YAML/results contracts, user-visible behavior, and
  private/opt-in limitations in the affected README, guides, reference, and examples.
- Select independent review under `.squad/governance.md`; code reviews use
  `gpt-5.6-terra` per `.squad/model-policy.md`. Never self-approve.
- Required `Build and Test Go Implementation` and `Lint Go Code` checks must pass.
  Do not bypass branch protection or merge without explicit authorization.
- Do not publish releases, social announcements, or captured evidence as a PR side effect.
