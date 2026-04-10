# LAKESHORE UNIVERSITY

**Lakeshore Homes Professional Development & Knowledge Platform**

## Overview

Lakeshore University is the internal knowledge assessment and professional development program for Lakeshore Homes, a Florida-based home builder operating across 5 counties (Marion, Citrus, Charlotte, Lake, Sumter).

The platform serves three purposes:
1. **Employee Development** — Assess and strengthen professional knowledge across all 21 departments
2. **Knowledge Capture** — Document operational expertise, tribal knowledge, and decision-making processes
3. **AI Agent Training** — Unified knowledge base that powers both human training and AI agent decision-making

## Structure

```
LAKESHORE-UNIVERSITY/
├── README.md
├── database/                      # Unified Knowledge Database (JSON)
│   ├── INDEX.json                 # Master index of all database files
│   ├── departments/               # 21 Department Knowledge Files
│   │   ├── scheduling.json        # Scheduling & Trade Coordination
│   │   ├── supervisao.json        # Field Supervision & Quality Control
│   │   ├── inspecao.json          # Municipal Inspections
│   │   ├── core_craft.json        # Internal Services (CoreCraft)
│   │   ├── permits.json           # Permitting & Regulatory
│   │   ├── orcamento.json         # Budget & Cost Estimation
│   │   ├── takeoff.json           # Material Takeoff & Quantification
│   │   ├── escritorio_projetos.json # Project Office & Design
│   │   ├── financeiro.json        # Finance (AP/AR/Draws)
│   │   ├── compras.json           # Purchasing & Procurement
│   │   ├── deposito.json          # Warehouse & Inventory
│   │   ├── client_relations.json  # Client Relations & Sales
│   │   ├── warranty.json          # Warranty & Post-Sale Service
│   │   ├── utilities.json         # Utilities Coordination
│   │   ├── coordenador.json       # Operations Coordination
│   │   ├── qps.json               # Quality, Process & Safety
│   │   ├── land_dev.json          # Land Development
│   │   ├── rh.json                # Human Resources
│   │   ├── ti.json                # IT & Systems
│   │   ├── compliance.json        # Compliance & Code Enforcement
│   │   └── preacher.json          # Company Chaplain
│   ├── cross-references/          # Cross-Department Knowledge
│   │   ├── handoffs.json          # 15 Critical Inter-Department Handoffs
│   │   ├── workflow_chains.json   # 9 Major Workflow Chains
│   │   ├── pain_points.json       # 18 Identified Pain Points
│   │   ├── business_rules.json    # CPM Gates, Payment Rules, KPIs
│   │   └── systems_inventory.json # All Software Systems Used
│   ├── ai-agents/                 # AI Agent Configurations
│   ├── platform-modules/          # LakeshoreSoftware.inc Module Maps
│   └── training/                  # Training Curriculum Plans
├── quizzes/                       # 21 Department Knowledge Assessments
│   ├── quiz_*.md                  # 30 questions each (A/B/C sections)
│   └── pdf/                       # Print-ready PDF versions
├── knowledge/                     # Department Knowledge Base (Markdown)
│   ├── dept_*.md                  # 21 department-specific knowledge files
│   ├── shared_*.md                # Shared company knowledge
│   ├── 01_ORGANOGRAMA.md          # Org chart (72 employees, 24 departments)
│   ├── 02_INVENTARIO_FERRAMENTAS.md # Software & tools inventory
│   ├── 03_GLOSSARIO.md            # 111-term construction glossary
│   ├── 04_MAPA_DEPENDENCIAS.md    # 142 pain points, 73 process flows
│   ├── 05_FLUXO_SPEC_HOME.md      # Spec home pipeline
│   ├── 06_FLUXO_CUSTOM_HOME.md    # Custom home pipeline
│   └── 07_CATALOGO_DORES.md       # Pain point catalog by department
└── responses/                     # Employee quiz responses (future)
```

## Knowledge Database

The `database/` directory contains a **structured JSON knowledge base** designed to serve both human training and AI agent decision-making. Each department file contains:

| Section | Purpose | Used By |
|---------|---------|---------|
| `ai_agent` | AI agent configuration (port, MCP tools, workflows) | AI Agents |
| `staff` | Team members and roles | HR, Training |
| `core_knowledge` | What employees need to know | Training Programs |
| `daily_workflows` | Step-by-step daily procedures | New Hires, AI Agents |
| `platform_modules` | LakeshoreSoftware.inc features used | IT, Training |
| `handoffs` | Cross-department dependencies | Operations, AI Agents |
| `pain_points` | Identified challenges with solutions | Management, IT |
| `tribal_knowledge` | Undocumented expertise at risk | Knowledge Management |
| `training_curriculum` | Training modules with priority | Training Programs |
| `compliance_requirements` | Regulatory requirements | Compliance, Legal |
| `key_metrics` | Performance targets | Management, QPS |

### Cross-References

| File | Content |
|------|---------|
| `handoffs.json` | 15 critical inter-department handoffs (H-01 to H-15) |
| `workflow_chains.json` | 9 major end-to-end workflow chains |
| `pain_points.json` | 18 high-severity operational pain points |
| `business_rules.json` | CPM gates, payment triggers, KPIs, contractor splits |
| `systems_inventory.json` | All software systems across departments |

## Data Sources

This knowledge base was synthesized from three primary sources:

1. **METAVERSE-LAKESHORE** — 21 AI agent definitions, 61+ MCP tools, 23 workflow chains, prompt engineering, and decision criteria from the Lakeshore Metaverse agent system
2. **LakeshoreSoftware.inc** — 20 platform modules, 100+ API endpoints, data models, and employee feature requirements from the construction management platform
3. **Lakeshore Knowledge Base** — 63 employee interviews, 19 departments, 72 people, tribal knowledge, pain points, and operational workflows from field research

## Quiz Format

Each quiz contains **30 questions** across 3 sections:

| Section | Questions | Type | Purpose |
|---------|-----------|------|---------|
| **A: Core Knowledge** | Q1-Q10 | Multiple Choice | Validate foundational knowledge |
| **B: Process & Decision-Making** | Q11-Q20 | Open Response | Capture workflows and decision criteria |
| **C: Advanced Scenarios** | Q21-Q30 | Open Response | Extract edge cases, tribal knowledge |

## Departments Covered (21)

| Category | Departments |
|----------|------------|
| **Construction** | Scheduling, Supervision, Inspection, CoreCraft |
| **Projects** | Permits, Takeoff, Project Office |
| **Financial** | Budget, Finance |
| **Purchasing** | Purchasing, Warehouse |
| **Client** | Client Relations, Warranty, Utilities |
| **Support** | Coordinator, QPS, Land Dev, HR, IT, Compliance, Chaplain |

## Key Statistics

| Metric | Value |
|--------|-------|
| Departments | 21 |
| Employees | 72 |
| AI Agents | 21 (ports 8001-8021) |
| MCP Tools | 61+ |
| Workflow Chains | 9 |
| Critical Handoffs | 15 |
| Pain Points | 18 high-severity |
| Platform Modules | 20 |
| API Endpoints | 100+ |
| Quiz Questions | 630 (30 per dept) |
| Knowledge Files | 28 (21 dept + 7 shared) |
| Counties | 5 (Marion, Citrus, Charlotte, Lake, Sumter) |

## Integration with Other Systems

| System | Repository | Purpose |
|--------|-----------|---------|
| **METAVERSE-LAKESHORE** | `JPVLakes/METAVERSE-LAKESHORE` | AI agent system (21 agents, MCP tools, workflows) |
| **LakeshoreSoftware.inc** | `JPVLakes/LakeshoreSoftware.inc` | Construction management platform (20 modules) |
| **Lakeshore Knowledge Base** | `Blira7/lakeshore` | Raw interview data (63 interviews) |

## Usage

### For Employee Training
1. Review department knowledge file in `database/departments/`
2. Take the corresponding quiz from `quizzes/`
3. Compare responses against `knowledge/` base
4. Identify gaps and create development plans

### For AI Agent Development
1. Load department JSON from `database/departments/`
2. Reference `cross-references/` for inter-department coordination
3. Use `handoffs.json` for workflow routing decisions
4. Apply `business_rules.json` for decision criteria

### For Management
1. Review `cross-references/pain_points.json` for operational issues
2. Check `tribal_knowledge` sections for knowledge-at-risk
3. Use `key_metrics` for performance monitoring
4. Reference `workflow_chains.json` for process optimization

---

*Lakeshore University is part of the Lakeshore Homes operational excellence initiative.*
*Knowledge database built from METAVERSE-LAKESHORE AI agents + LakeshoreSoftware.inc platform + 63 employee interviews.*
