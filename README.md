# PPAIOS — KIND2 Workspace Seed

Per-brand workspace seed for KIND2. Imported into Houston as a workspace.

## Structure
- `.houston/` — workspace state (KPI snapshots, reviews, ledger, alerts).
- `agents/` — per-agent overrides (rare; most live in `caner-hue/ppaios`).
- `outputs/` — generated artefacts.
- `brand-brain.md` — voice, ICP, products, history.
- `kpi-targets.json` — ROAS, CAC, CVR, AOV targets.
- `budgets.json` — spend caps.
- `policies.json` — brand-specific overrides on the global PPAIOS policies.

## Linking to PPAIOS
Agent definitions and reusable skills live in `caner-hue/ppaios`. This repo is a thin per-brand seed.

When importing into Houston:
1. Houston pulls this repo as a workspace.
2. Houston also pulls `caner-hue/ppaios` for shared agents/skills/references.
3. Workspace `.houston/` writes happen in this repo (or are gitignored if state is local-only).

## Brand
- KIND2 — DTC haircare, UK + Amazon UK.
- 3PL: Sendcloud.
- Email: Klaviyo.
