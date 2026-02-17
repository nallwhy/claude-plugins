---
name: pkg-setup
description: Install and configure Elixir packages into a project. Use when setting up any Elixir dependency.
argument-hint: [packages...]
allowed-tools: Read(~/.claude/plugins/marketplaces/nallwhy/plugins/elixir/skills/pkg-setup/**), Read(mix.exs), Read(config/**), Edit(mix.exs), Edit(config/**), WebFetch(domain:hexdocs.pm), Bash(mix *)
---

# Elixir Package Setup

Install and configure Elixir packages into a project.
Process each package in `$ARGUMENTS` sequentially.

## Process (for each package)

1. **Follow the official installation guide** — Find the installation guide at `https://hexdocs.pm/{package}`. Prefer the igniter-based method if documented, otherwise follow the manual installation guide.
2. **Check package-specific notes** — If the package has a matching file in the list below, read it and perform any additional steps described there.
3. **Verify compilation** — Run `mix compile`. Must pass with zero warnings. Fix any warnings before moving to the next package.
4. **Format** — Run `mix format`.
5. **Update usage_rules** — If `usage_rules` is installed as a dependency, run `mix usage_rules` to regenerate rules.

## Package-specific notes

- [ash.md](./ash.md)
- [usage_rules.md](./usage_rules.md)
