---
name: pkg-setup
description: Install and configure Elixir packages into a project. Use when setting up any Elixir dependency.
argument-hint: [packages...]
---

# Elixir Package Setup

Install and configure Elixir packages into a project.
Process each package in `$ARGUMENTS` sequentially.

## Process (for each package)

1. **Follow the official installation guide** — Find the installation guide at `https://hexdocs.pm/{package}`. Prefer the igniter-based method if documented, otherwise follow the manual installation guide.
2. **Check package-specific notes** — Read `pkg-setup/{package}.md` in this skill's directory. If it exists, perform any additional steps described there.
3. **Verify compilation** — Run `mix compile`. Must pass with zero warnings. Fix any warnings before moving to the next package.
4. **Format** — Run `mix format`.
5. **Update usage_rules** — If `usage_rules` is installed as a dependency, run `mix usage_rules` to regenerate rules.
