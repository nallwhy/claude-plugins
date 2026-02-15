# ash — Additional Setup

After following the official installation guide, verify these are all configured:

- [ ] mix.exs: `picosat_elixir` dependency (SAT solver for policies). If compilation fails, use `simple_sat` instead
- [ ] config/config.exs: `ash_domains: []` registered in app config
