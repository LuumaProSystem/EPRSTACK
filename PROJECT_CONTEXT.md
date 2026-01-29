# PROJECT_CONTEXT.md
> EPRStack — AI-Powered Compliance Operating System
> Last Updated: 2026-01-29

---

## 1. PROJECT IDENTITY

| Field | Value |
|-------|-------|
| **Name** | EPRStack |
| **Classification** | AI-Powered Compliance Operating System |
| **Domain** | Extended Producer Responsibility (EPR) for Packaging |

**One-Sentence Thesis:**
> EPRStack converts messy commerce + packaging data into audit-ready CO/OR/CA reporting, fee forecasting, approvals, and evidence packs—so brands can stay compliant with predictable cost and minimal internal labor.

**Purpose of this file:**
This document provides context for Claude (AI assistant) to understand the project scope, current progress, and operating constraints. **Read this file at the start of every session.**

---

## 2. ABOUT THE BUILDER

| Field | Value |
|-------|-------|
| **Name** | Antuan |
| **Experience** | First-time coder |
| **Timeline** | 12-week build plan (G0 → G20) |
| **Learning Approach** | Building by doing, understanding over speed |
| **Priority** | Explain everything—assume no prior coding knowledge |

---

## 3. CURRENT STATUS

| Field | Value |
|-------|-------|
| **Week** | 1 of 12 |
| **Module** | G0 (Strategic Foundation) |
| **Phase** | Ground Zero — Understanding the "why" |
| **Next Module** | G1 (Data Model & Audit Spine) |

---

## 4. THE THREE GUARANTEES

EPRStack delivers three guarantees to every customer:

| Guarantee | Definition | How It's Delivered |
|-----------|------------|-------------------|
| **Compliance Certainty** | Every filing is defensible under audit | Pinned hashes, CitationTriplets, Dual-Key approvals |
| **Financial Predictability** | Fee forecasts with explained variance | Low/Base/High bands, Variance Narrative Engine |
| **Operational Efficiency** | Minimal internal labor required | 14-agent automation with Founder-only binding actions |

---

## 5. TECH STACK

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Compute** | DigitalOcean VPS (8GB RAM baseline) | Application hosting |
| **Database** | PostgreSQL 15 + TimescaleDB | Relational data + time-series event_spine |
| **Backend API** | Python FastAPI | REST endpoints, domain services, RBAC |
| **Frontend** | Next.js 14 (React) | Client Dashboard + Internal Command Center |
| **Cache/Queue** | Redis 7 + Celery | Session cache, job queues, background tasks |
| **Object Storage** | S3-compatible (DO Spaces) | Evidence Vault, 7-year retention |
| **Orchestration** | Docker Compose v2 | Service orchestration (single-node) |
| **Proxy/TLS** | Caddy + Cloudflare | Auto TLS 1.3, DDoS protection |
| **Observability** | Prometheus + Grafana | SLO tracking, incident detection |
| **LLM Integration** | Anthropic Claude API | Agent reasoning, document parsing |

---

## 6. SIX FUNCTIONAL PLANES

EPRStack is organized into six functional planes:

```
┌─────────────────────────────────────────────────────────────┐
│  PLANE A: ACQUISITION & PRE-SALES                           │
│  Lead Vampire, Specright Fast-Track, InstantWin Composer    │
└─────────────────────────────────────────────────────────────┘
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PLANE B: CORE DATA & TRUTH LAYER                           │
│  SpecBridge SoR, Ingestion Hub, Evidence Vault, BOM Builder │
└─────────────────────────────────────────────────────────────┘
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PLANE C: COMPLIANCE COMPUTATION LAYER                      │
│  LexGuard (Rules-as-Code), Fee Engine, Obligation Periods   │
└─────────────────────────────────────────────────────────────┘
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PLANE D: CONTROL & SAFETY LAYER                            │
│  SKU Drift Detector, Dual-Key Approvals, FilingPackager     │
└─────────────────────────────────────────────────────────────┘
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PLANE E: AGENT LABOR LAYER                                 │
│  14-Agent Roster, Skills Registry, RBAC, Safety Harness     │
└─────────────────────────────────────────────────────────────┘
                              ▼
┌─────────────────────────────────────────────────────────────┐
│  PLANE F: RELIABILITY & OBSERVABILITY                       │
│  HealthScore, SLO Catalog, Audit Spine, ReleaseGate         │
└─────────────────────────────────────────────────────────────┘
```

---

## 7. THE THREE GATES

Every compliance cycle passes through three mandatory gates:

| Gate | Name | Question | Blocking Conditions |
|------|------|----------|---------------------|
| **Gate 1** | BOM Readiness | "Do we have sufficient packaging data?" | Any SKU with C4 (Missing), Bundle without decomposition, >5% orders missing ship_to_state |
| **Gate 2** | Variance | "Is the fee forecast within acceptable variance?" | Variance >$100 AND >5%, New jurisdiction detected, High-severity drift pending |
| **Gate 3** | Execution | "Are we authorized to submit/pay?" | Missing Ops Key, Missing Finance Key, Invalid SignatoryAuthorityRecord |

**State Transitions:**
```
OPEN → FROZEN → APPROVED → EXECUTED → CLOSED
```

---

## 8. BUILD ORDER (G0-G20)

### Phase: Ground Zero → Launch

| Module | Name | Week | Key Deliverables | Dependencies |
|--------|------|------|------------------|--------------|
| **G0** | Strategic Foundation | 0 | ICP confirmed, pricing locked, dossier reviewed | None |
| **G1** | Data Model & Audit Spine | 1 | event_spine, accounts, users, RBAC, evidence_artifacts | G0 |
| **G2** | BOM Builder & Confidence Ladder | 2 | SKU→component mapping, virtual bundles, confidence scores | G1 |
| **G3** | LexGuard (Rules-as-Code) | 2-3 | CO/OR rulesets, statute anchoring, CitationTriplets | G1 |
| **G4** | Fee Engine & Variance Controls | 3 | Deterministic fee calc, variance detection, cure tracking | G2, G3 |
| **G5** | SKU Drift Detector | 3 | Drift alerts, aggregation buffer, expansion gates | G4 |
| **G6** | Dual-Key Approvals | 4 | Approval workflow, delegate signer, smart waiver | G1 |
| **G7** | FilingPackager & AuditPackBuilder | 4 | Filing packs, audit packs, PDF generation | G3, G6 |
| **G8** | Agent Catalog (14 Agents) | 5 | All agents defined with skills + tools | G7 |
| **G9** | Agent Labor Layer & Safety | 5 | Kill switches, substitution rules, safety harness | G8 |
| **G10** | Workflow Bindings & RACI | 6 | Human-VA-AI matrix, Work OS tabs | G9 |
| **G11** | Lead Vampire Integration | 6 | LV Router, Instant Win, Specright Fast-Track | G10 |
| **G12** | Customer Onboarding | 7 | Shopify/CSV/ERP playbooks, supplier scorecards | G10 |
| **G13** | Ops Cadence & Dashboards | 7-8 | Client Dashboard (A1-A5), Command Center (B1-B5) | G1, G10 |
| **G14** | Contracts & Scope Enforcement | 8 | ContractBundle versioning, ScopeGuard, Small Producer Shield | G1 |
| **G15** | Pricing & GTM | 8 | Core/Pro/Enterprise tiers, sales motion | G14 |
| **G16** | Security & Continuity | 9 | BC/DR, incident runbooks, weekly restore tests | G1 |
| **G17** | Reliability & HealthScore | 9 | SLO composite, VA hiring triggers, OPEX BOM | G1 |
| **G18** | MX-ROW Control Plane | 10 | 25 Pain→Relief→Capability chains | G1 |
| **G19** | YAML Policy Layer | 10-11 | 48 canonical policy files in dependency order | G18 |
| **G20** | Launch Readiness | 11-12 | Pre-launch checklist, ReleaseGate, DR drill, pilot cohort | G19 |

---

## 9. SIX STRATEGIC AXIOMS

These are non-negotiable design principles:

| # | Axiom | Rule |
|---|-------|------|
| 1 | **Audit-Grade Reproducibility** | If a number appears in a filing, EPRStack can show exactly how it was computed |
| 2 | **Truth Before Outputs** | Build the truth pipeline first, not the UI. Objects → Versions → Gates → Dashboards |
| 3 | **No Manual "Fix in Prod"** | All changes go through ReleaseGate with tests + approvals + rollback readiness |
| 4 | **Dual-Key for Binding Actions** | Ops approves the package, Finance approves the payment. Never bypass. |
| 5 | **Statute-First Enforcement** | PRO guidance informs operations; statute text governs compliance |
| 6 | **Progressive Agent Autonomy** | Start with Agent-Run + Founder Review; earn autonomy through sustained reliability |

---

## 10. OPERATING RULES FOR CLAUDE

### Core Rules (MUST FOLLOW)

1. **Explain Before Doing**
   - Always explain what you're about to do and why
   - Use simple language—assume no prior coding knowledge
   - Show the "why" before the "how"

2. **Stop at Checkpoints**
   - Pause after completing each logical unit of work
   - Ask for confirmation before proceeding to next step
   - Never chain multiple file changes without approval

3. **Keep Code Simple**
   - Favor readability over cleverness
   - Add comments explaining non-obvious logic
   - Avoid premature optimization

4. **Test Immediately**
   - After writing code, verify it works
   - Show test results or output
   - Fix issues before moving on

5. **Never Overwrite Without Permission**
   - Never overwrite existing files without explicit permission
   - Create new versions instead (e.g., `file_v2.py`)
   - Always show diff or changes before applying

6. **Follow "Truth → Outputs → UI"**
   - Build data model first, then logic, then UI
   - Never build dashboards before the truth pipeline exists

7. **Version Everything**
   - Every compliance-affecting change must be versioned and pinned
   - No manual fixes in production

### Communication Style

- Use bullet points and tables for clarity
- Break complex concepts into steps
- Celebrate small wins—this is a learning journey

---

## 11. MONOREPO STRUCTURE

```
eprstack/
├── apps/
│   ├── dashboard-nextjs/          # Client + Internal UI
│   └── api-core-fastapi/          # Auth, orchestration, RBAC
│
├── services/
│   ├── lexguard/                  # Rules-as-Code engine
│   ├── filing-packager/           # Filing + audit packs
│   ├── eprstacklv-router/         # Lead Vampire funnel
│   └── aegis-gateway/             # Policy enforcement
│
├── packages/
│   ├── shared-schemas/            # JSON Schemas (versioned)
│   └── shared-utils/              # Hashing, ID generation
│
├── infra/
│   ├── docker-compose.yml
│   ├── caddy/
│   ├── grafana/
│   ├── prometheus/
│   └── db/
│       ├── migrations/
│       └── seeds/
│
├── docs/
│   ├── dossier/                   # Canonical specs (frozen)
│   └── adr/                       # Architecture Decision Records
│
├── tests/
│   ├── fixtures/
│   └── regression/
│
├── policies/                      # YAML policy files
│   ├── core/
│   └── modules/
│
├── schemas/
│   ├── objects.yaml
│   └── events.yaml
│
├── evals/                         # ReleaseGate test suites
│
└── PROJECT_CONTEXT.md             # This file
```

---

## 12. CHANGELOG

| Date | Module | Change | Notes |
|------|--------|--------|-------|
| 2026-01-29 | G0 | Project initialized | Created PROJECT_CONTEXT.md (dossier-aligned) |

---

*End of PROJECT_CONTEXT.md*
