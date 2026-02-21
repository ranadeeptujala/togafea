# TOGAF ADM - Phase F: Migration Planning

> **Purpose**: Finalize detailed implementation and migration plan

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE F: MIGRATION PLANNING                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PURPOSE: Create DETAILED plan to move from Baseline to Target        │
│                                                                         │
│   Phase E = WHAT to do (identify opportunities)                        │
│   Phase F = HOW & WHEN to do it (detailed plan)                        │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE F: KEY ACTIVITIES                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. FINALIZE ARCHITECTURE ROADMAP                                      │
│     └── Timeline: Baseline → Transition 1 → Transition 2 → Target      │
│                                                                         │
│  2. FINALIZE IMPLEMENTATION PLAN                                       │
│     └── Detailed: Schedule + Budget + Resources + Milestones           │
│                                                                         │
│  3. ENSURE BUSINESS VALUE IS REALIZED                                  │
│     └── Define KPIs, measure before/after, track benefits              │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## What "Migration" Means

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    WHAT "MIGRATION" MEANS IN PHASE F                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PHASE B, C, D                          PHASE F                       │
│   (DESIGN the Target)                    (PLAN the Migration)          │
│                                                                         │
│   ┌─────────────────┐                   ┌─────────────────┐            │
│   │ Phase B:        │                   │                 │            │
│   │ Target Business │───┐               │  HOW do we      │            │
│   │ Architecture    │   │               │  actually GET   │            │
│   └─────────────────┘   │               │  from Current   │            │
│                         │               │  to Target?     │            │
│   ┌─────────────────┐   │    ────►      │                 │            │
│   │ Phase C:        │───┤               │  • Timeline     │            │
│   │ Target Data &   │   │               │  • Budget       │            │
│   │ App Architecture│   │               │  • Resources    │            │
│   └─────────────────┘   │               │  • Milestones   │            │
│                         │               │                 │            │
│   ┌─────────────────┐   │               │  = MIGRATION    │            │
│   │ Phase D:        │───┘               │    PLAN         │            │
│   │ Target Tech     │                   │                 │            │
│   │ Architecture    │                   └─────────────────┘            │
│   └─────────────────┘                                                  │
│                                                                         │
│   WHAT we want                          HOW we get there               │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Roadmap

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE ROADMAP                                 │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   BASELINE          TRANSITION 1      TRANSITION 2         TARGET      │
│   (Today)           (6 months)        (12 months)          (18 months) │
│                                                                         │
│   ┌─────────┐      ┌─────────┐       ┌─────────┐         ┌─────────┐  │
│   │ Legacy  │ ───► │ Hybrid  │ ───►  │ Mostly  │ ───►    │ Full    │  │
│   │ On-Prem │      │ Cloud   │       │ Cloud   │         │ Cloud   │  │
│   │ Monolith│      │ +Legacy │       │ Micro-  │         │ Micro-  │  │
│   │         │      │         │       │ services│         │ services│  │
│   └─────────┘      └─────────┘       └─────────┘         └─────────┘  │
│                                                                         │
│   ◄────────────────────── TIME ──────────────────────────────────────► │
│                                                                         │
│   TRANSITION ARCHITECTURES provide incremental value                   │
│   and reduce risk of big-bang transformation                           │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Transition Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    TRANSITION ARCHITECTURE                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   • Intermediate state between Baseline and Target                     │
│   • Delivers partial business value                                    │
│   • Reduces implementation risk                                        │
│   • Allows gradual transformation                                      │
│                                                                         │
│   WHY NEEDED:                                                          │
│   • Big-bang is risky                                                  │
│   • Business can't wait years for value                                │
│   • Allows course correction                                           │
│   • Easier to manage and govern                                        │
│                                                                         │
│   EXAMPLE:                                                             │
│   • Transition 1: Core platform on cloud, legacy still running         │
│   • Transition 2: 80% migrated, critical legacy remaining              │
│   • Target: Full cloud, legacy decommissioned                          │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Implementation Plan Components

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    IMPLEMENTATION PLAN                                  │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   1. SCHEDULE                                                          │
│      └── Timeline with milestones                                      │
│          • Project start/end dates                                     │
│          • Phase gates                                                 │
│          • Go-live dates                                               │
│                                                                         │
│   2. BUDGET                                                            │
│      └── Cost breakdown                                                │
│          • Infrastructure costs                                        │
│          • License costs                                               │
│          • Development costs                                           │
│          • Training costs                                              │
│                                                                         │
│   3. RESOURCES                                                         │
│      └── People needed                                                 │
│          • Team composition                                            │
│          • Skills required                                             │
│          • External consultants                                        │
│                                                                         │
│   4. MILESTONES                                                        │
│      └── Key checkpoints                                               │
│          • Design Complete                                             │
│          • Development Complete                                        │
│          • UAT Complete                                                │
│          • Go-Live                                                     │
│                                                                         │
│   5. RISKS & MITIGATION                                                │
│      └── What could go wrong and how to handle                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Contracts

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE CONTRACTS                               │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   Agreement between EA team and Implementation team                    │
│                                                                         │
│   CONTAINS:                                                            │
│   • What architecture deliverables will be produced                    │
│   • What standards/principles must be followed                         │
│   • Roles and responsibilities                                         │
│   • Quality criteria                                                   │
│   • Review checkpoints                                                 │
│   • Compliance requirements                                            │
│                                                                         │
│   PURPOSE:                                                             │
│   • Ensures implementation follows architecture                        │
│   • Sets expectations clearly                                          │
│   • Provides basis for compliance reviews (Phase G)                    │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Implementation and Migration Plan** | Detailed project plans |
| **Architecture Roadmap** | Visual timeline of transitions |
| **Transition Architectures** | Intermediate state definitions |
| **Architecture Contracts** | Agreements with implementation teams |
| **Business Value Assessment** | KPIs and benefit tracking plan |

---

## Phase E vs Phase F Summary

| Phase E | Phase F |
|---------|---------|
| Identify work packages | Create detailed project plans |
| Group into projects | Define schedules & budgets |
| Build/Buy/Reuse decisions | Assign resources |
| Initial roadmap | Finalize roadmap with transitions |
| Dependencies identified | Architecture contracts created |
| **WHAT** to do | **HOW & WHEN** to do it |

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PHASE F = "PLAN THE JOURNEY"                                         │
│                                                                         │
│   • Finalize Architecture Roadmap (with transition states)             │
│   • Create detailed Implementation Plan                                │
│   • Define schedule, budget, resources                                 │
│   • Create Architecture Contracts                                      │
│   • Ensure business value tracking                                     │
│                                                                         │
│   OUTPUT: Implementation Plan + Roadmap + Architecture Contracts       │
│                                                                         │
│   Now ready to hand off to implementation teams (Phase G)!             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
