# TOGAF 9.2 Quick Reference Cheat Sheet

> Based on TOGAF 9.2 (April 2018)

## ADM Phases at a Glance

```
┌─────────────────────────────────────────────────────────────────────┐
│                         PRELIMINARY                                  │
│  → Prepare org for EA, define principles, establish capability      │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    PHASE A: VISION                                   │
│  → High-level vision, stakeholders, Statement of Architecture Work  │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│                 PHASE B: BUSINESS ARCHITECTURE                       │
│  → Business processes, organization, functions, services            │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│              PHASE C: INFORMATION SYSTEMS ARCHITECTURE               │
│  → Data Architecture + Application Architecture                     │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│               PHASE D: TECHNOLOGY ARCHITECTURE                       │
│  → Hardware, software, networks, infrastructure                     │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│              PHASE E: OPPORTUNITIES & SOLUTIONS                      │
│  → Work packages, transition architectures, initial roadmap         │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│                PHASE F: MIGRATION PLANNING                           │
│  → Detailed implementation plan, finalize roadmap                   │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│             PHASE G: IMPLEMENTATION GOVERNANCE                       │
│  → Architecture oversight, compliance reviews, contracts            │
└──────────────────────────────┬──────────────────────────────────────┘
                               ▼
┌─────────────────────────────────────────────────────────────────────┐
│            PHASE H: ARCHITECTURE CHANGE MANAGEMENT                   │
│  → Monitor changes, update architecture, manage change requests     │
└─────────────────────────────────────────────────────────────────────┘

          ★ REQUIREMENTS MANAGEMENT - Continuous across ALL phases ★
```

---

## Four Architecture Domains (BDAT)

| Domain | Focus | Key Questions |
|--------|-------|---------------|
| **B**usiness | Strategy, processes, governance | What does the business do? |
| **D**ata | Data entities, data management | What information is needed? |
| **A**pplication | Applications, interactions | What applications support the business? |
| **T**echnology | Infrastructure, platforms | What technology enables applications? |

---

## Building Blocks Comparison

| Aspect | ABB (Architecture) | SBB (Solution) |
|--------|-------------------|----------------|
| **Defines** | WHAT is needed | HOW it's implemented |
| **Abstraction** | High level | Detailed |
| **Technology** | Agnostic | Specific |
| **Example** | "Payment Processing" | "Stripe API Integration" |

---

## Enterprise Continuum Spectrum

```
Generic ◄─────────────────────────────────────────────────► Specific

Foundation    →    Common Systems    →    Industry    →    Organization
(TRM, III-RM)      (COTS patterns)     (Banking, etc.)    (Your company)
```

---

## Key Deliverables by Phase

| Phase | Key Deliverables |
|-------|-----------------|
| **Preliminary** | Architecture Principles, Organizational Model |
| **A** | Statement of Architecture Work, Architecture Vision |
| **B** | Business Architecture Document |
| **C** | Data Architecture, Application Architecture |
| **D** | Technology Architecture Document |
| **E** | Implementation Strategy, Transition Architectures |
| **F** | Implementation & Migration Plan |
| **G** | Architecture Contract, Compliance Assessments |
| **H** | Architecture Updates, Change Requests |

---

## Architecture Principle Template

```
┌────────────────────────────────────────────┐
│  NAME: [Principle Name]                    │
├────────────────────────────────────────────┤
│  STATEMENT: [What the principle is]        │
├────────────────────────────────────────────┤
│  RATIONALE: [Why it matters]               │
├────────────────────────────────────────────┤
│  IMPLICATIONS: [What it means in practice] │
└────────────────────────────────────────────┘
```

---

## Stakeholder Power/Interest Grid

```
                 INTEREST
                 Low     High
         ┌───────┬───────┐
    High │ Keep  │ Manage │  ← Key Players
POWER    │Satisfied│Closely│
         ├───────┼───────┤
    Low  │Monitor│  Keep  │
         │       │Informed│
         └───────┴───────┘
```

---

## Architecture Repository Components

| Component | Purpose |
|-----------|---------|
| **Architecture Metamodel** | Structure for organizing architecture |
| **Architecture Capability** | People, processes, tools for EA |
| **Architecture Landscape** | Current and future state views |
| **Standards Information Base** | Approved standards |
| **Reference Library** | Templates, patterns, guidelines |
| **Governance Log** | Decisions, compliance records |

---

## Key TOGAF Concepts - One Liners

| Concept | Definition |
|---------|------------|
| **View** | Representation of system from stakeholder perspective |
| **Viewpoint** | Template for creating views |
| **Concern** | Stakeholder interest in the system |
| **Artifact** | Work product describing aspect of architecture |
| **Deliverable** | Contractually specified output |
| **Gap Analysis** | Difference between baseline and target |
| **Architecture Contract** | Agreement on deliverables and conformance |
| **Dispensation** | Approved deviation from standards |

---

## Common Phase Activities

### All Phases Include:
1. Select reference models and tools
2. Develop architecture descriptions
3. Perform gap analysis
4. Define candidate roadmap components
5. Resolve impacts across landscape
6. Conduct stakeholder review
7. Create Architecture Definition Document

---

## Iteration Types in ADM

| Type | Description |
|------|-------------|
| **Architecture Capability** | Iterate to establish initial capability |
| **Architecture Development** | Iterate across phases to develop content |
| **Transition Planning** | Iterate to create transition architectures |
| **Architecture Governance** | Iterate to govern implementations |

---

## Quick Tips for Interviews

1. **ADM is iterative** - Not strictly linear
2. **Requirements Management is continuous** - Always at center
3. **Phase C has two parts** - Data AND Application
4. **Phase E creates strategy** - Phase F creates detailed plan
5. **Phase G is oversight** - Not implementation itself
6. **Business architecture FIRST** - Then technical (B→C→D)
7. **Stakeholders are key** - Address in every phase
8. **Principles guide decisions** - Established in Preliminary

---

## Acronyms to Know

| Acronym | Full Form |
|---------|-----------|
| ADM | Architecture Development Method |
| ABB | Architecture Building Block |
| SBB | Solution Building Block |
| TRM | Technical Reference Model |
| III-RM | Integrated Information Infrastructure Reference Model |
| SOW | Statement of Architecture Work |
| SIB | Standards Information Base |
| EA | Enterprise Architecture |

---

## Phase Mnemonics

**"Please Allow Business Changes During Every Full Governance Hour"**

- **P**reliminary
- **A**rchitecture Vision
- **B**usiness Architecture
- **C**hanges (Information Systems - Data/App)
- **D**uring (Technology)
- **E**very (Opportunities & Solutions)
- **F**ull (Migration Planning)
- **G**overnance (Implementation Governance)
- **H**our (Change Management)

---

*Print this out for quick review before your interview!*

