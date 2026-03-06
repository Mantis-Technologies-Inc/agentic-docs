# MANTIS_CONTEXT.md

**Version:** 2.0 | **Last Updated:** March 2026 | **Owner:** CEO  
**Load this doc:** Every agent session, every task, without exception.

---

## 1. What Mantis Is

Mantis is an agentic logistics platform for unmanned and autonomous systems. We deliver UxS fleet readiness, predictive maintenance, parts forecasting, inventory optimization, and asset and operator performance intelligence — serving two customer segments: UxS OEMs and warfighter units (military).

**Primary customer now:** UxS OEMs. The warfighter GTM follows the OEM commercial motion.

The durable value is a two-sided marketplace: OEMs receive anonymized field performance data that accelerates design iteration; warfighters receive faster improvements. This feedback loop is the moat — no existing tool occupies this position.

---

## 2. What We Are NOT Building

These are hard architectural and strategic constraints. Do not scope, prototype, or implement anything in these categories without an explicit CEO decision to revisit.

- **Unmanned and autonomous systems only — no exceptions.** Mantis is exclusively for UxS fleets. Not manned platforms, legacy equipment, commercial aviation, or any non-UxS asset class. If a feature or integration does not serve an unmanned or autonomous system, it is out of scope.
- **Not a production lifecycle tool for OEMs.** Mantis does not manage pre-shipment build, test, or manufacturing workflows. Our OEM scope is post-production fleet management and the data feedback loop — not factory-floor or QA tooling.
- **Not a C2 system.** Mantis does not direct systems. It keeps systems ready. C2 is Anduril Lattice, Palantir. Do not blur this line.
- **Not a single-OEM tool.** No deep integrations that lock to one vendor ecosystem. Vendor-agnostic data normalization is non-negotiable.
- **Not a dashboard-only tool.** Existing tools display data. Mantis acts on it. Every feature should move toward agentic sustainment workflows, not static reporting.
- **Not consumer / commercial aviation / non-defense UxS (now).** All resources target the DoD mission. Commercial expansion is a future bet, not a current one.

---

## 3. Tech Stack

| Layer | Tool | Purpose |
|---|---|---|
| Product Management | Linear | Issues, sprints, PRDs, roadmap |
| Design | Figma | UI design |
| Frontend | Cursor + Claude Code | Production implementation |
| Backend | Supabase | Database, auth, realtime |
| Deployment | Railway, Vercel | Hosting, CI/CD |
| Automation | n8n (future: Temporal) | Workflow automation, tool integrations |
| Observability | Datadog / Prometheus | Logging, metrics, alerting |
| Communication | Slack | Team comms, async standups |
| Version Control | GitHub | Source of truth for code |
| AI (Extended) | Claude Pro Max, Claude Code | Architecture, planning, implementation |
| Rapid Prototyping | Replit | Concept validation before production build |

---

## 4. Related Docs

Load these in addition to this file when the task requires it.

| Doc | Contains | Load When |
|---|---|---|
| `MANTIS_PRODUCT.md` | Personas, current traction, north star test, active bets (flagged as hypotheses) | Sprint planning, PRD writing, feature scoping, product decisions |
| `MANTIS_STRATEGY.md` | Problem framing, 12-month targets, competitive moat narrative | Investor materials, strategic planning, narrative-level work |
