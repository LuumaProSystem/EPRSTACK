# PROJECT_CONTEXT.md
> EPRStack - Extended Producer Responsibility Compliance Platform
> Last Updated: 2026-01-29

---

## 1. PROJECT OVERVIEW

**What is EPRStack?**
A compliance platform that helps brands navigate Extended Producer Responsibility (EPR) regulations. EPRStack automates fee calculations, filing preparation, and audit-readiness for packaging compliance across multiple jurisdictions.

**Purpose of this file:**
This document provides context for Claude (AI assistant) to understand the project scope, current progress, and operating constraints. Read this file at the start of every session.

---

## 2. ABOUT THE BUILDER

| Field | Value |
|-------|-------|
| **Name** | Antuan |
| **Experience** | First-time coder |
| **Learning Approach** | Building by doing, 12-week structured plan |
| **Priority** | Understanding over speed - explain everything |

---

## 3. CURRENT STATUS

| Field | Value |
|-------|-------|
| **Week** | 1 of 12 |
| **Module** | G0-G1 (Ground Zero) |
| **Phase** | Strategic Foundation + Data Model Setup |
| **Status** | Project initialization |

---

## 4. TECH STACK

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Backend** | Python FastAPI | REST API, business logic |
| **Frontend** | Next.js 14 | React framework, UI |
| **Database** | PostgreSQL 15 + TimescaleDB | Primary storage + time-series event_spine |
| **Cache/Queue** | Redis + Celery | Caching + background job processing |
| **Storage** | S3-compatible (DigitalOcean Spaces) | File/artifact storage |
| **Orchestration** | n8n | Lead Vampire workflow automation |
| **Deployment** | Docker Compose | Container orchestration |

---

## 5. BUILD ORDER (G0-G20)

| Module | Name | Description |
|--------|------|-------------|
| **G0** | Strategic Foundation | Customer validation, market reality |
| **G1** | Data Model & Audit Spine | event_spine, accounts, users, RBAC, evidence_artifacts |
| **G2** | BOM Builder & Confidence Ladder | SKU mapping, packaging components |
| **G3** | LexGuard | Rules-as-Code engine, CO/OR rulesets |
| **G4** | Fee Engine & Variance Controls | Deterministic calculations |
| **G5** | SKU Drift Detector | Detect silent packaging changes |
| **G6** | Dual-Key Approvals & Execution Controls | Ops + finance signatures |
| **G7** | FilingPackager & AuditPackBuilder | Reproducible outputs |
| **G8** | Agent Catalog | 14-agent AI workforce |
| **G9** | Agent Labor Layer & Safety Harness | Kill switches, RBAC |
| **G10** | Workflow Bindings & RACI Matrix | Human-VA-AI assignments |
| **G11** | Lead Vampire Integration | Acquisition funnel |
| **G12** | Customer Onboarding | Shopify/CSV/ERP playbooks |
| **G13** | Ops Cadence & Dashboards | Client + Internal Command Center |
| **G14** | Contracts & Scope Enforcement | Prevent margin leak |
| **G15** | Pricing & GTM | Core/Pro/Enterprise tiers |
| **G16** | Security & Continuity | BC/DR, incident response |
| **G17** | Reliability & HealthScore | SLO composite, staffing triggers |
| **G18** | MX-ROW Control Plane | 25 Pain→Relief→Capability chains |
| **G19** | YAML Policy Layer | 48 canonical policy files |
| **G20** | Launch Readiness | Pre-launch checklist, pilot cohort |

---

## 6. OPERATING RULES FOR CLAUDE

### Core Rules (MUST FOLLOW)

1. **Explain Before Doing**
   - Always explain what you're about to do and why
   - Use simple language - assume no prior coding knowledge
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

### Communication Style

- Use bullet points and tables for clarity
- Break complex concepts into steps
- Celebrate small wins - this is a learning journey

---

## 7. CHANGELOG

| Date | Module | Change | Notes |
|------|--------|--------|-------|
| 2026-01-29 | - | Project initialized | Created PROJECT_CONTEXT.md |

---

*End of PROJECT_CONTEXT.md*
