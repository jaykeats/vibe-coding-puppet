# ROADMAP: Implementation Plan & Milestones 🚀

## Project timeline (short)
- **Phase 1 — Foundation (Weeks 1–2):** repo consolidation, docs, CI, basic dev server, SSD layout, scripts.
- **Phase 2 — Core Features (Weeks 3–4):** asset browser, search & filters, CodeMirror editor integration, export functions.
- **Phase 3 — Automation & Ops (Week 5):** scheduled backups, indexer, cleanup scripts, smoke tests, CI hardening.
- **Phase 4 — Polish & Release Prep (Week 6):** UI polish, tests, performance tuning, documentation finalization.

## Priorities
1. Consolidate docs and CI (this PR). ✅
2. Add a minimal Vitest smoke test so CI tests meaningfully. ⚠️
3. Ensure build steps are scoped correctly to `client/` when needed. 🔧
4. Add a small dataset and a scheduled backup to verify scripts. 📦

---

Code editor decision: Start with **CodeMirror** (lighter memory footprint); evaluate Monaco later if needed.