# usage_rules — Additional Setup

After following the official installation guide:

- [ ] Configure and run `mix usage_rules.sync`:
  - Set `file: "AGENTS.md"` in usage_rules config
  - Default content mode to `link: :markdown` unless user prefers otherwise (inline or link :at)
- [ ] Ask the user if they use Claude Code. If yes, create a symlink: `ln -s AGENTS.md CLAUDE.md`
