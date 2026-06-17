# github-actions — composite actions

Reusable composite actions for the organization.

## Contents
- `yarn/install` · `yarn/lint` · `yarn/format` — Yarn Berry building blocks.
- `cargo/setup` — Rust toolchain (rustfmt + clippy) + cache.

## Using an action directly (ad-hoc)
```yaml
steps:
  - uses: digital-multiverse/github-actions/yarn/install@v2
    with:
      node-version: "24"
```
For day-to-day CI, prefer the reusable workflows in `github-workflows`.
