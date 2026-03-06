# **MANTIS\_CONTEXT.md**

**Version:** 1.0 | **Last Updated:** March 2026 | **Owner:** CEO

This is the single source of truth for Mantis. It feeds every AI session and product decision. Update monthly or when a strategic bet is validated/invalidated.

---

## 

## **1\. The Problem**

The Department of War is procuring over 1,000,000 unmanned systems (UxS) in the next 2–3 years with no purpose-built system to manage them. This is not an incremental logistics gap, it is a phase transition that existing tools (built for manned, high-value, long-lifecycle platforms) cannot address.

This problem has two branches:

**Branch A — The Warfighter:** Military units managing heterogeneous UxS fleets across multiple OEMs have no unified system of record. They cannot answer the fundamental readiness question in real time. There is no fleet visibility, no predictive maintenance, and no closed feedback loop to OEMs when systems fail in the field.

**Branch B — The UxS OEM:** Manufacturers building unmanned and autonomous systems manage pre-shipment testing, evaluation, and maintenance through disparate, disconnected tools. They lack a unified platform for fleet management prior to customer delivery and receive little-to-no structured performance signal back from the field once systems are deployed.

The strategic consequence: these gaps don't just create inefficiency, they create a national security vulnerability. Adversaries who iterate their unmanned and autonomous systems weekly will outpace militaries that iterate yearly.

---

## 

## **2\. Who We're Building For**

### 

### **Primary (Now): UxS OEM Users**

We are building the commercial product first, targeting UxS OEMs across all domains — beginning with UAS and expanding to USVs and ASVs as demand signals warrant.

The OEM user base spans the full production lifecycle — from build through testing, evaluation, and customer-ready delivery. Exact titles vary by company but the functional roles are consistent. Current pipeline: GreenSight, Parrot, Titan Dynamics, Bavovna AI, Havoc AI, AeroVironment.

**Persona A: Production / Test Engineer**

* Day-to-day role: Building, testing, and evaluating UxS units during the pre-shipment production cycle

* Core pain: Managing test results, maintenance logs, issue tracking, and asset status across disconnected spreadsheets and tools

* What they need from Mantis: A unified system of record for each unit's build history, test outcomes, open issues, and readiness status

* Success signal: Faster issue identification and resolution during development; no data lost between build phases

**Persona B: Program Manager / Production Lead**

* Day-to-day role: Overseeing delivery timelines, fleet readiness rates, and program health across multiple vehicles or contracts

* Core pain: No single view of where each unit is in the build-to-delivery pipeline; status requires manual aggregation

* What they need from Mantis: Program-level dashboard showing fleet status, test completion rates, open issues by severity, and delivery readiness

* Success signal: Ability to report delivery confidence without manual data gathering; early visibility into blockers

**Persona C: Sales / Business Development**

* Day-to-day role: Managing customer relationships, demonstrating platform capability, and supporting contract negotiations

* Core pain: No easy way to show customers verified fleet performance data or readiness history

* What they need from Mantis: Customer-facing readiness reports and performance summaries generated from real operational data

* Success signal: Mantis data becomes a sales asset — proof of system reliability that accelerates customer confidence

### 

### **Secondary (Later): Warfighter Users**

The warfighter GTM will follow the OEM commercial motion. Three distinct personas:

**Persona C: Individual UxS Operator / Warfighter**

* Needs: Edge-accessible interface for reporting issues, viewing asset status, and logging mission performance

* Key constraint: Must work in low-connectivity environments; UX must be fast and simple

**Persona D: UxS Program Lead**

* Needs: Fleet-level readiness dashboard, maintenance workflow management, cross-OEM visibility

* Key constraint: Managing multi-vendor fleets; needs vendor-agnostic data normalization

**Persona E: Warfighter Leadership**

* Needs: High-level readiness and performance reporting; strategic visibility across units

* Key constraint: Summary-level data, not operational detail; needs to map to mission objectives

---

## 

## **3\. What Winning Looks Like in 12 Months**

By February 2027, Mantis has:

* **25+ UxS OEMs** actively using and paying for Mantis — primarily DCMA BlueList OEMs and OEMs selected under the Drone Dominance initiative (current pipeline includes GreenSight, Parrot, AeroVironment, Havoc AI)

* **2–3 completed warfighter pilot programs** with operational units (building on JIFX Feb 2026 and ANTX Coastal Trident 2026 relationships)

* **The OEM–Warfighter feedback loop is closed**: OEMs receive anonymized, mission-contextualized performance data from field deployments; warfighters receive faster design improvements and better-forecasted parts availability

* **USV/ASV OEM pipeline established**: At least 3 surface vessel OEMs in active conversations or early pilots (pipeline includes PacMar Technologies, Havoc AI, Bavovna AI, Shift Technologies, STR8 Technologies, Kraken Technologies, Splash Inc, and Blacksea Technologies)

* **Revenue**: First meaningful ARR from OEM subscriptions; at least one funded DoD pilot via OTA or SBIR pathway


---

## 

## **4\. What We Are NOT Building**

These are explicit decisions, not future possibilities. Do not build, scope, or prototype these without a CEO decision to revisit.

* **Not a general MRO platform**: Mantis is purpose-built for unmanned and autonomous systems. We are not building a horizontal maintenance solution for manned platforms, legacy equipment, or commercial aviation.

* **Not a C2 system**: Mantis does not tell systems where to go. That is Anduril Lattice, Palantir. We keep systems ready to get there.

* **Not a single-OEM tool**: We do not build deep integrations that only serve one vendor's ecosystem. Vendor-agnostic data normalization is non-negotiable.

* **Not a data visualization dashboard only**: Existing tools show you data. Mantis acts on it. We are building toward agentic sustainment workflows, not static reporting.

* **Not consumer / commercial aviation / non-defense UxS (for now)**: Resources are focused entirely on the DoW mission. Commercial UxS operators are a future expansion, not a current bet.

---

## 

## **5\. Current Bets (Active Hypotheses)**

These are the strategic bets we are running right now. Each should be reviewed monthly. When validated or invalidated, update this document and log the learning in MANTIS\_ANTI\_PATTERNS.md.

**Bet 1: Commercial OEM First (Supply Side Before Demand Side)** *Hypothesis:* Starting with UxS OEMs as paying customers gets Mantis to revenue faster and builds the supply side of the marketplace before the warfighter GTM is accessible. The DoD demand side has a longer procurement cycle; OEMs have a commercial buying motion. *Validation signal:* 5+ OEMs in paid pilots by Q3 2026\. *Risk:* If OEM willingness-to-pay is lower than expected, or if DoD opportunities accelerate faster than the OEM motion, we may need to rebalance.

**Bet 2: DCMA BlueList \+ Drone Dominance OEMs as Beachhead** *Hypothesis:* DCMA BlueList OEMs and OEMs selected under the Drone Dominance initiative represent the highest-density, highest-urgency segment. They are procuring at scale, under government scrutiny, and need fleet management infrastructure now. *Validation signal:* 3+ BlueList or Drone Dominance OEMs in active Mantis pilots by Q2 2026\. *Risk:* These OEMs may have procurement constraints or existing vendor relationships that slow sales cycles.

**Bet 3: UAS First, USV/ASV in Parallel if Demand Is There** *Hypothesis:* UAS OEMs are the highest-volume, most urgent segment. We build depth here first. USV/ASV OEMs (autonomous surface vessels) are a logical second domain given similar fleet management needs and adjacent buyer relationships — but we only invest meaningfully if inbound demand justifies it. *Validation signal:* 2+ serious USV/ASV OEM conversations by Q3 2026 without active outreach investment. *Risk:* Surface domain has different telemetry, environmental constraints, and buyer profiles. Do not assume UAS features translate directly.

**Bet 4: Two-Experience Architecture Is Necessary and the Right Call** *Hypothesis:* The OEM product experience and the warfighter product experience will diverge meaningfully. OEM features (pre-shipment testing workflows, build-phase maintenance, engineering telemetry, sales reporting) do not 1:1 transfer to warfighter needs (edge accessibility, mission reporting, cross-unit readiness). Building two tailored experiences is an accepted architectural decision — not a failure of product focus — because the users, contexts, and workflows are fundamentally different. *Validation signal:* Feature requests from OEM pilots confirm functionality that would be irrelevant or confusing in a warfighter context, and vice versa. *Watch out for:* Two experiences mean two surface areas to maintain. Engineering overhead compounds over time. Define the shared data layer early to minimize divergence cost and protect the feedback loop that connects both sides.

**Bet 5: The Feedback Loop Is the Moat** *Hypothesis:* The durable competitive advantage is not fleet visibility (a feature anyone can build) — it is the closed loop between warfighter field data and OEM design iteration. This network effect means every additional OEM makes the platform more valuable to operators, and every additional operator makes the platform more valuable to OEMs. Nobody else occupies this position. *Validation signal:* An OEM cites Mantis field data as informing a design or production decision. A warfighter cites improved platform performance as a result of OEM iteration enabled by Mantis data. *Risk:* The feedback loop requires both sides to be meaningfully on the platform simultaneously. If OEM adoption outpaces warfighter adoption (or vice versa), the loop stays open and the moat doesn't compound.

---

## **6\. Tech Stack Reference**

| Layer | Tool | Purpose |
| ----- | ----- | ----- |
| Product Management | Linear | Issues, sprints, PRDs, roadmap |
| Design | Figma, Magic Patterns, Lovable | UI design, rapid prototyping, scaffold generation |
| Frontend | Cursor \+ Claude Code | Production implementation |
| Backend | Supabase | Database, auth, realtime |
| Deployment | Railway, Vercel | Hosting, CI/CD |
| Automation | n8n (future: Temporal) | Workflow automation, tool integrations |
| Observability | Datadog/Prometheus  | Logging, metrics, alerting |
| Communication | Slack | Team comms, async standups |
| Version Control | GitHub | Source of truth for code |
| AI (Extended) | Claude Pro Max, Claude Code | Architecture, planning, implementation |
| Rapid Prototyping | Replit | Natural language to visual prototype, fast concept validation before committing to production build |
| Rapid UI | Lovable, Magic Patterns | Fast concept-to-scaffold |

---

## 

## **7\. Current Stage & Context**

* **TRL:** 3 → targeting TRL 6 by end of 2026

* **Stage:** Pre-revenue, working prototype

* **Traction:** Working prototype demonstrated at JIFX Feb 2026; accepted to ANTX Coastal Trident 2026; 10+ program office engagements across Army, Navy, SOCOM, OUSD R\&E; 5+ OEMs in active integration conversations; backed by Fairwater Labs

* **Key relationships:** Lt Col Whitney (25ID Lightning Labs), CW3 Morrison (3ID Marne Center), Maj Keary Salls (Army UAS Reqs Office), Lt Col Schueman (USMC)

* **Acquisition pathways:** OTA, SBIR Phase II/III, BAA; aligned with DIU, AFWERX, AAL, SOFWERX

---

## 

## **8\. The North Star Test**

Before building, scoping, or prioritizing anything, run it through this filter:

*"Does this move a UxS system closer to being ready — to deliver, to deploy, or to fight — and does it generate signal that makes the next system better?"*

If the answer to both halves is no, it's not Mantis.

**For warfighter-specific features**, apply a secondary test: does this answer one question clearly — *"what do I need to do right now?"* If the UI requires interpretation, it's not ready for the field.

