# MANTIS_PRODUCT.md

**Version:** 1.0 | **Last Updated:** March 2026 | **Owner:** CEO  
**Load this doc:** Sprint planning, PRD writing, feature scoping, product decisions. Always load alongside MANTIS_CONTEXT.md.

---

## 1. Who We're Building For

### Primary (Now): UxS OEM Users

OEM users are responsible for ensuring their unmanned and autonomous systems meet requirements and perform to spec — whether validating existing capability or testing new capability ahead of customer delivery. Personas below reflect the people most incentivized to have fleet management and performance data at their fingertips.

**Persona A: Hardware / Software Engineer**
- Day-to-day role: Building, testing, and validating UxS units — ensuring systems meet performance requirements and identifying issues before customer delivery
- Core pain: No unified system of record for asset status, test outcomes, and open issues across a fleet; data lives in spreadsheets and disconnected tools
- What they need from Mantis: A single view of asset readiness and performance per unit; clear signal on what is working, what isn't, and what needs attention
- Success signal: Faster issue identification and resolution; no performance data lost between test cycles

**Persona B: Program Manager / Production Lead**
- Day-to-day role: Overseeing delivery timelines, fleet readiness rates, and program health across multiple vehicles or contracts
- Core pain: Status requires manual aggregation; no single view of where each unit stands against requirements
- What they need from Mantis: Program-level dashboard showing fleet readiness, asset performance trends, open issues by severity, and delivery confidence
- Success signal: Ability to report delivery status without manual data gathering; early visibility into blockers before they affect timelines

### Secondary (Later): Warfighter Users

The warfighter GTM follows the OEM commercial motion. Do not prioritize warfighter-specific features until OEM traction validates the platform.

**Persona C: Individual UxS Operator / Warfighter**
- Needs: Edge-accessible interface for reporting issues, viewing asset status, and logging mission performance
- Key constraint: Must work in low-connectivity environments; UX must be fast and require no interpretation

**Persona D: UxS Program Lead**
- Needs: Fleet-level readiness dashboard, maintenance workflow management, cross-OEM visibility
- Key constraint: Managing multi-vendor fleets; needs vendor-agnostic data normalization

**Persona E: Warfighter Leadership**
- Needs: High-level readiness and performance reporting; strategic visibility across units
- Key constraint: Summary-level data only; must map clearly to mission objectives

---

## 2. Confirmed Capabilities

This section reflects capabilities that are actively scoped or in build. It is not a product roadmap. **Update this section after every meaningful customer conversation that validates or invalidates a capability.**

| Capability | Status | Notes |
|---|---|---|
| Fleet readiness visibility | ✅ Confirmed | Core OEM and warfighter use case |
| Asset performance | ✅ Confirmed | Core OEM use case; engineer and PM personas |
| Predictive maintenance | 🔲 Not yet confirmed | High-priority hypothesis; pending customer validation |
| Parts forecasting | 🔲 Not yet confirmed | High-priority hypothesis; pending customer validation |
| Inventory optimization | 🔲 Not yet confirmed | Pending customer validation |
| Operator performance | 🔲 Not yet confirmed | Pending customer validation |
| Customer-facing readiness reports | 🔲 Not yet confirmed | Pending customer validation |

---

## 3. Current Traction

Ground-truth facts only. Do not treat pipeline names or targets as confirmed unless explicitly marked.

- Working prototype demonstrated at JIFX February 2026
- Accepted to ANTX Coastal Trident 2026
- 10+ program office engagements across Army, Navy, SOCOM, OUSD R&E
- 5+ OEMs in active integration conversations
- Backed by Fairwater Labs
- Key relationships: Lt Col Whitney (25ID Lightning Labs), CW3 Morrison (3ID Marne Center), Maj Keary Salls (Army UAS Reqs Office), Lt Col Schueman (USMC)
- Acquisition pathways in play: OTA, SBIR Phase II/III, BAA; aligned with DIU, AFWERX, AAL, SOFWERX

---

## 4. North Star Test

Before building, scoping, or prioritizing anything, run it through this filter:

> *"Does this move a UxS system closer to being ready — to deliver, to deploy, or to fight — and does it generate signal that makes the next system better?"*

If the answer to both halves is no, it is not Mantis.

**For warfighter-specific features**, apply a secondary test: does this answer one question clearly — *"what do I need to do right now?"* If the UI requires interpretation, it is not ready for the field.

---

## 5. Active Bets

These are strategic hypotheses being tested right now. Treat them as hypotheses, not facts. Review monthly. When validated or invalidated, update this doc and log the learning in MANTIS_ANTI_PATTERNS.md.

**Bet 1: Commercial OEM First**
- Hypothesis: Starting with UxS OEMs as paying customers gets Mantis to revenue faster. OEMs have a commercial buying motion; the DoD demand side has a longer procurement cycle.
- Validation signal: 5+ OEMs in paid pilots by Q3 2026
- Risk: If OEM willingness-to-pay is lower than expected, or DoD opportunities accelerate faster, may need to rebalance

**Bet 2: DCMA BlueList + Drone Dominance OEMs as Beachhead**
- Hypothesis: These OEMs are procuring at scale, under government scrutiny, and need fleet management infrastructure now — making them the highest-density, highest-urgency segment
- Validation signal: 3+ BlueList or Drone Dominance OEMs in active Mantis pilots by Q2 2026
- Risk: Procurement constraints or existing vendor relationships may slow sales cycles

**Bet 3: UAS First, USV/ASV in Parallel if Demand Warrants**
- Hypothesis: UAS OEMs are the highest-volume, most urgent segment. USV/ASV is a logical second domain but only if inbound demand justifies investment.
- Validation signal: 2+ serious USV/ASV OEM conversations by Q3 2026 without active outreach investment
- Risk: Surface domain has different telemetry, environmental constraints, and buyer profiles — do not assume UAS features translate directly

**Bet 4: Two-Experience Architecture Is the Right Call**
- Hypothesis: OEM and warfighter product experiences will diverge meaningfully. Two tailored experiences is an accepted architectural decision, not a failure of product focus.
- Validation signal: OEM pilot feature requests confirm functionality that would be irrelevant or confusing in a warfighter context, and vice versa
- Watch out for: Two experiences mean two surface areas to maintain. Define the shared data layer early to minimize divergence cost and protect the feedback loop.

**Bet 5: The Feedback Loop Is the Moat**
- Hypothesis: Durable competitive advantage is the closed loop between warfighter field data and OEM design iteration — a network effect no existing tool occupies
- Validation signal: An OEM cites Mantis field data as informing a design or production decision; a warfighter cites improved platform performance as a result of OEM iteration enabled by Mantis data
- Risk: The loop requires both sides meaningfully on the platform. If adoption is lopsided, the moat doesn't compound.
