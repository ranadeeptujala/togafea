# TOGAF ADM Phases - Outcomes Overview

> Quick reference for all ADM phases with key activities, deliverables, and outcomes

---

## Summary Table

| Phase | Name | Purpose | Key Activities | Key Deliverables |
|-------|------|---------|----------------|------------------|
| **Preliminary** | EA Setup | Setup EA capability (ONCE) | Define team, tools, principles, governance, standards | Organizational Model, Architecture Principles |
| **A** | Architecture Vision | Get approval to start | Identify stakeholders, confirm drivers, define scope, create vision | SOW, Architecture Vision Document |
| **B** | Business Architecture | Define business | Business flows, BPMN, org structure, capabilities | Business Architecture Document, Gap Analysis |
| **C** | Information Systems | Define data & apps | Data models, application portfolio, integrations | Data Architecture, Application Architecture |
| **D** | Technology Architecture | Define technology | Infrastructure, platforms, databases, tech stack | Technology Architecture Document |
| **E** | Opportunities & Solutions | Identify how to build | Work packages, dependencies, Build/Buy/Reuse | Implementation Strategy, Work Packages |
| **F** | Migration Planning | Plan the journey | Roadmap, budget, resources, contracts | Migration Plan, Architecture Contracts |
| **G** | Implementation Governance | Ensure compliance | Reviews, checklists, dispensations | Compliance Assessments, Governance Log |
| **H** | Change Management | Keep architecture alive | Monitor changes, manage ACRs, update docs | Architecture Updates, Change Requests |

---

## Detailed Phase Overview

```
┌────────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                    ADM PHASES OVERVIEW                                             │
├──────────────┬─────────────────────┬────────────────────────────┬──────────────────────────────────┤
│    PHASE     │      PURPOSE        │     KEY ACTIVITIES         │       KEY DELIVERABLES           │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PRELIMINARY  │ Setup EA            │ • Create EA team           │ • Organizational Model for EA    │
│ (One-time)   │ Capability          │ • Setup tools              │ • Architecture Principles        │
│              │                     │ • Define principles        │ • Tailored Framework             │
│              │                     │ • Establish governance     │ • Architecture Repository        │
│              │                     │ • Define standards         │                                  │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE A      │ Get approval        │ • Identify stakeholders    │ • Statement of Architecture      │
│ Architecture │ to start            │ • Confirm business drivers │   Work (SOW)                     │
│ Vision       │                     │ • Define scope             │ • Architecture Vision Document   │
│              │                     │ • Create vision            │ • Stakeholder Map                │
│              │                     │ • Assess readiness         │ • RACI Matrix                    │
│              │                     │ • Get sign-off             │ • Communication Plan             │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE B      │ Define how          │ • Baseline business arch   │ • Business Architecture Document │
│ Business     │ business works      │ • Target business arch     │ • Business Process Models (BPMN) │
│ Architecture │                     │ • Gap analysis             │ • Organization Chart             │
│              │                     │ • Business flows           │ • Capability Map                 │
│              │                     │ • BPMN diagrams            │ • Gap Analysis Results           │
│              │                     │ • Org structure            │ • Value Stream Maps              │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE C      │ Define data         │ DATA:                      │ DATA:                            │
│ Information  │ and applications    │ • Logical data models      │ • Data Architecture Document     │
│ Systems      │                     │ • Physical data models     │ • Data Models (Logical/Physical) │
│ Architecture │                     │ • Data flow diagrams       │ • Data Catalog                   │
│              │                     │                            │                                  │
│              │                     │ APPLICATION:               │ APPLICATION:                     │
│              │                     │ • App portfolio            │ • Application Architecture Doc   │
│              │                     │ • App ↔ Business mapping   │ • Application Portfolio          │
│              │                     │ • Integration patterns     │ • Interface Catalog              │
│              │                     │ • Gap analysis             │ • Gap Analysis Results           │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE D      │ Define              │ • Define platforms         │ • Technology Architecture Doc    │
│ Technology   │ infrastructure      │ • Technology layers        │ • Platform Decomposition         │
│ Architecture │                     │ • App ↔ Tech mapping       │ • App/Technology Matrix          │
│              │                     │ • Gap analysis             │ • Technology Standards           │
│              │                     │                            │ • Gap Analysis Results           │
│              │                     │ COVERS:                    │                                  │
│              │                     │ • Edge/Delivery layer      │                                  │
│              │                     │ • Application layer        │                                  │
│              │                     │ • Data layer               │                                  │
│              │                     │ • Infrastructure layer     │                                  │
│              │                     │ • Security & Ops           │                                  │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE E      │ Identify how        │ • Identify work packages   │ • Implementation Strategy        │
│ Opportunities│ to implement        │ • Group into projects      │ • Work Package List              │
│ & Solutions  │                     │ • Assess dependencies      │ • Project Groupings              │
│              │                     │ • Build vs Buy vs Reuse    │ • Dependency Matrix              │
│              │                     │ • Initial roadmap          │ • Build/Buy/Reuse Decisions      │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE F      │ Plan the            │ • Finalize roadmap         │ • Implementation & Migration     │
│ Migration    │ transformation      │ • Finalize impl. plan      │   Plan                           │
│ Planning     │                     │ • Define transitions       │ • Architecture Roadmap           │
│              │                     │ • Budget & resources       │ • Transition Architectures       │
│              │                     │ • Business value tracking  │ • Architecture Contracts         │
│              │                     │ • Create contracts         │ • Business Value Assessment      │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE G      │ Ensure teams        │ • Ensure conformance       │ • Compliance Assessments         │
│ Implementation│ follow architecture│ • Govern projects          │ • Architecture Contracts         │
│ Governance   │                     │ • Compliance reviews       │   (enforced)                     │
│              │                     │ • Create checklists        │ • Dispensation Log               │
│              │                     │ • Grant dispensations      │ • Governance Log                 │
│              │                     │ • Report to leadership     │ • Recommendations                │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ PHASE H      │ Keep architecture   │ • Monitor tech changes     │ • Architecture Updates           │
│ Architecture │ current             │ • Monitor business changes │ • Change Requests (ACRs)         │
│ Change Mgmt  │                     │ • Manage change requests   │ • Governance Log                 │
│              │                     │ • Update architecture      │ • New ADM Cycle (if needed)      │
│              │                     │ • Assess impact            │                                  │
│              │                     │ • Trigger new cycle        │                                  │
│              │                     │                            │                                  │
├──────────────┼─────────────────────┼────────────────────────────┼──────────────────────────────────┤
│              │                     │                            │                                  │
│ REQUIREMENTS │ Manage requirements │ • Identify requirements    │ • Requirements Repository        │
│ MANAGEMENT   │ throughout ADM      │ • Store requirements       │ • Traceability Matrix            │
│ (Central)    │                     │ • Manage changes           │ • Impact Assessments             │
│              │                     │ • Ensure addressed         │                                  │
│              │                     │ • Maintain traceability    │                                  │
│              │                     │                            │                                  │
└──────────────┴─────────────────────┴────────────────────────────┴──────────────────────────────────┘
```

---

## Phase Categories

```
┌─────────────────────────────────────────────────────────────────────────┐
│              PHASE CATEGORIES                                           │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   SETUP (One-time):                                                    │
│   ─────────────────                                                    │
│   • Preliminary - EA Capability Setup                                  │
│                                                                         │
│   INITIATION:                                                          │
│   ────────────                                                         │
│   • Phase A - Vision & Approval                                        │
│                                                                         │
│   DESIGN (Architecture Domains):                                       │
│   ─────────────────────────────                                        │
│   • Phase B - Business Architecture                                    │
│   • Phase C - Data + Application Architecture                          │
│   • Phase D - Technology Architecture                                  │
│                                                                         │
│   PLANNING:                                                            │
│   ─────────                                                            │
│   • Phase E - Opportunities & Solutions                                │
│   • Phase F - Migration Planning                                       │
│                                                                         │
│   EXECUTION & GOVERNANCE:                                              │
│   ───────────────────────                                              │
│   • Phase G - Implementation Governance                                │
│   • Phase H - Change Management                                        │
│                                                                         │
│   CONTINUOUS:                                                          │
│   ────────────                                                         │
│   • Requirements Management (center of all phases)                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Quick Reference - One Line Per Phase

| Phase | One-Line Summary |
|-------|------------------|
| **Preliminary** | Setup EA team, tools, principles, governance, standards (ONCE) |
| **A** | Get approval: SOW + Architecture Vision |
| **B** | Business flows, BPMN, org structure, capabilities |
| **C** | Data models + Application portfolio |
| **D** | Technology stack (infra, languages, databases) |
| **E** | Work packages + Build/Buy + Dependencies |
| **F** | Budget + Resources + Roadmap + Contracts |
| **G** | Checklist + Reviews + Compliance |
| **H** | Change requests + Architecture updates |
| **Req Mgmt** | Requirements throughout all phases |

---

## Deliverables by Category

### Documents

| Phase | Documents |
|-------|-----------|
| A | Statement of Architecture Work (SOW), Architecture Vision Document |
| B | Business Architecture Document |
| C | Data Architecture Document, Application Architecture Document |
| D | Technology Architecture Document |
| F | Implementation & Migration Plan |

### Diagrams/Models

| Phase | Diagrams |
|-------|----------|
| B | BPMN Process Flows, Org Chart, Capability Map, Value Streams |
| C | Data Models (Logical/Physical), Application Portfolio, Integration Diagrams |
| D | Platform Decomposition, Technology Layers |
| F | Architecture Roadmap, Transition Architectures |

### Catalogs/Matrices

| Phase | Catalogs/Matrices |
|-------|-------------------|
| A | Stakeholder Map, RACI Matrix, Concerns Matrix |
| C | Data Catalog, Interface Catalog, App/Function Matrix |
| D | App/Technology Matrix, Technology Standards Catalog |
| E | Dependency Matrix, Work Package List |
| G | Compliance Checklist, Dispensation Log |

### Governance Artifacts

| Phase | Governance Artifacts |
|-------|----------------------|
| F | Architecture Contracts |
| G | Compliance Assessments, Governance Log |
| H | Architecture Change Requests (ACRs) |

---

## Phase Input/Output Flow

```
┌─────────────────────────────────────────────────────────────────────────┐
│              INPUT → PHASE → OUTPUT                                     │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   Business Request  ──►  PHASE A  ──►  SOW + Vision                    │
│                              │                                          │
│   SOW + Vision      ──►  PHASE B  ──►  Business Architecture           │
│                              │                                          │
│   Business Arch     ──►  PHASE C  ──►  Data + App Architecture         │
│                              │                                          │
│   Data + App Arch   ──►  PHASE D  ──►  Technology Architecture         │
│                              │                                          │
│   All Architectures ──►  PHASE E  ──►  Work Packages + Strategy        │
│                              │                                          │
│   Work Packages     ──►  PHASE F  ──►  Migration Plan + Contracts      │
│                              │                                          │
│   Plan + Contracts  ──►  PHASE G  ──►  Compliance Assessments          │
│                              │                                          │
│   Implementation    ──►  PHASE H  ──►  Architecture Updates            │
│                              │                                          │
│                              └──►  (Back to Phase A if major change)   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Memory Aid - Keywords

```
┌─────────────────────────────────────────────────────────────────────────┐
│              MEMORY AID                                                 │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PRELIMINARY = SETUP (Team, Tools, Principles, Governance, Standards) │
│                                                                         │
│   A = APPROVE      (Vision, SOW, Stakeholders, Scope)                  │
│   B = BUSINESS     (Flows, BPMN, Org, Capabilities)                    │
│   C = CONTENT      (Data models, App portfolio)                        │
│   D = DEVICES      (Technology, Infra, Platforms)                      │
│   E = EXPLORE      (Work packages, Build/Buy, Dependencies)            │
│   F = FINALIZE     (Budget, Resources, Roadmap, Contracts)             │
│   G = GOVERN       (Reviews, Checklists, Compliance)                   │
│   H = HANDLE       (Changes, ACRs, Updates)                            │
│                                                                         │
│   REQ MGMT = REQUIREMENTS (Throughout all phases)                      │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Interview Quick Answer

> "TOGAF ADM starts with **Phase A** where we create the Architecture Vision and get approval through SOW. Then we design in **Phases B, C, D** - Business, Data/Application, and Technology architectures. In **Phase E** we identify work packages and Build/Buy decisions. **Phase F** creates the detailed migration plan with budget and contracts. **Phase G** governs implementation through compliance reviews. **Phase H** manages ongoing changes. Requirements Management runs throughout all phases as the central hub."
