# MASTER HANDOFF — EXTENDED

Hardware & runtime optimization guidance for constrained machines (8GB RAM, older CPU). Key points summarized:

- Set `NODE_OPTIONS="--max-old-space-size=512"` for dev when memory constrained.
- Use CodeMirror (lighter) as the initial editor (Monaco documented as future enhancement).
- Keep `node_modules` on C:\; set pnpm store and npm cache to E:\ when needed.
- Run monthly `scripts/cleanup.ps1` to prune caches and old backups.
- See `docs/SSD_OPTIMIZATION_STRATEGY.md` for more details.