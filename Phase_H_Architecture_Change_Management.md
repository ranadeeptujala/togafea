# TOGAF ADM - Phase H: Architecture Change Management

> **Purpose**: Keep architecture aligned with changing requirements

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                 PHASE H: ARCHITECTURE CHANGE MANAGEMENT                 │
│                                                                         │
│   "How do we keep the architecture relevant as things change?"         │
│   "How do we manage changes to the approved architecture?"             │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE H: KEY ACTIVITIES                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. MONITOR TECHNOLOGY CHANGES                                         │
│     ├── New technologies (AWS new services, new frameworks)            │
│     ├── End-of-Life (Java 11 EOL, deprecated libraries)                │
│     ├── Security vulnerabilities (CVEs, patches)                       │
│     └── Vendor changes (pricing, acquisitions)                         │
│                                                                         │
│  2. MONITOR BUSINESS CHANGES                                           │
│     ├── Strategy changes (new products, new markets)                   │
│     ├── Regulatory changes (DPDPA, GDPR, gaming compliance)            │
│     ├── Organizational changes (new teams, M&A)                        │
│     └── Market changes (competitors, customer needs)                   │
│                                                                         │
│  3. MANAGE ARCHITECTURE CHANGE REQUESTS                                │
│     ├── Receive change requests from teams                             │
│     ├── Classify (Minor / Incremental / Major / Emergency)             │
│     ├── Assess impact (systems, cost, risk)                            │
│     ├── Approve / Reject / Defer                                       │
│     └── Update architecture documents                                  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Types of Changes

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    TYPES OF ARCHITECTURE CHANGES                        │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   1. SIMPLIFICATION CHANGES                                            │
│      └── Reduce complexity, improve efficiency                         │
│          Example: Consolidate 3 databases into 1                       │
│                                                                         │
│   2. INCREMENTAL CHANGES                                               │
│      └── Small improvements within current architecture                │
│          Example: Add a new field to an API                            │
│                                                                         │
│   3. RE-ARCHITECTING CHANGES                                           │
│      └── Major changes to architecture approach                        │
│          Example: Move from monolith to microservices                  │
│                                                                         │
│   4. EMERGENCY CHANGES                                                 │
│      └── Urgent fixes for critical issues                              │
│          Example: Security vulnerability patch                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Change Request (ACR)

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE CHANGE REQUEST (ACR)                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   A formal request to modify the approved architecture                 │
│                                                                         │
│   ACR TEMPLATE:                                                        │
│   ┌─────────────────────────────────────────────────────────────────┐  │
│   │  ACR ID: ACR-2024-042                                           │  │
│   │  Title: Add Redis caching layer                                 │  │
│   │  Requestor: Payment Team                                        │  │
│   │  Date: 2024-01-15                                               │  │
│   │                                                                  │  │
│   │  Description:                                                   │  │
│   │  Add Redis cache to reduce database load for payment lookups    │  │
│   │                                                                  │  │
│   │  Reason/Driver:                                                 │  │
│   │  Current latency is 500ms, target is 100ms                      │  │
│   │                                                                  │  │
│   │  Impact:                                                        │  │
│   │  - New infrastructure component                                 │  │
│   │  - Code changes in Payment Service                              │  │
│   │  - Additional monitoring required                               │  │
│   │                                                                  │  │
│   │  Effort: 2 weeks, 2 engineers                                   │  │
│   │  Risk: Low                                                      │  │
│   │                                                                  │  │
│   │  Status: Pending Review                                         │  │
│   └─────────────────────────────────────────────────────────────────┘  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Change Management Process

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    CHANGE MANAGEMENT PROCESS                            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   ┌─────────────┐                                                      │
│   │  TRIGGER    │ ← Technology change, business change, team request   │
│   └──────┬──────┘                                                      │
│          │                                                              │
│          ▼                                                              │
│   ┌─────────────┐                                                      │
│   │  SUBMIT ACR │ ← Team submits Architecture Change Request           │
│   └──────┬──────┘                                                      │
│          │                                                              │
│          ▼                                                              │
│   ┌─────────────┐                                                      │
│   │  CLASSIFY   │ ← Minor / Incremental / Major / Emergency            │
│   └──────┬──────┘                                                      │
│          │                                                              │
│          ▼                                                              │
│   ┌─────────────┐                                                      │
│   │   ASSESS    │ ← Impact analysis: systems, cost, risk, effort       │
│   └──────┬──────┘                                                      │
│          │                                                              │
│          ▼                                                              │
│   ┌─────────────┐                                                      │
│   │   REVIEW    │ ← Architecture Board reviews                         │
│   └──────┬──────┘                                                      │
│          │                                                              │
│          ▼                                                              │
│   ┌─────────────────────────────────────────┐                          │
│   │              DECISION                    │                          │
│   │  ┌─────────┐  ┌─────────┐  ┌─────────┐  │                          │
│   │  │ APPROVE │  │ REJECT  │  │  DEFER  │  │                          │
│   │  └────┬────┘  └────┬────┘  └────┬────┘  │                          │
│   └───────┼────────────┼────────────┼───────┘                          │
│           │            │            │                                   │
│           ▼            ▼            ▼                                   │
│   ┌─────────────┐  ┌───────┐  ┌──────────┐                             │
│   │ UPDATE ARCH │  │ CLOSE │  │ BACKLOG  │                             │
│   │ DOCUMENTS   │  │ ACR   │  │ FOR LATER│                             │
│   └─────────────┘  └───────┘  └──────────┘                             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## When to Start New ADM Cycle

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    WHEN TO START NEW ADM CYCLE                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   Phase H may trigger a NEW ADM cycle when:                            │
│                                                                         │
│   1. MAJOR BUSINESS CHANGE                                             │
│      └── New product line, M&A, major strategy shift                   │
│                                                                         │
│   2. SIGNIFICANT TECHNOLOGY SHIFT                                      │
│      └── Cloud migration, platform change, major upgrade               │
│                                                                         │
│   3. REGULATORY REQUIREMENTS                                           │
│      └── New compliance needs (GDPR, DPDPA, industry regulations)      │
│                                                                         │
│   4. ARCHITECTURE DRIFT                                                │
│      └── Current state has drifted too far from target                 │
│                                                                         │
│   5. TARGET ACHIEVED                                                   │
│      └── Current target reached, time to define new target             │
│                                                                         │
│   ─────────────────────────────────────────────────────────────────    │
│                                                                         │
│   Phase H → (triggers) → Phase A (new cycle)                           │
│                                                                         │
│   This is why ADM is ITERATIVE!                                        │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Refresh

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE REFRESH                                 │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   Periodic review and update of architecture                           │
│                                                                         │
│   FREQUENCY:                                                           │
│   • Annual review (minimum)                                            │
│   • Quarterly for fast-changing domains                                │
│                                                                         │
│   WHAT TO REVIEW:                                                      │
│   • Are architecture principles still valid?                           │
│   • Is target state still relevant?                                    │
│   • What technology changes need attention?                            │
│   • What business changes need attention?                              │
│   • Is the roadmap still on track?                                     │
│                                                                         │
│   OUTPUT:                                                              │
│   • Updated Architecture Vision (if needed)                            │
│   • Updated Roadmap                                                    │
│   • New ADM cycle (if major changes)                                   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Architecture Updates** | Updated documentation reflecting changes |
| **Change Requests** | ACRs submitted and processed |
| **Governance Log** | Record of all changes and decisions |
| **Dispensation Updates** | Review and update of existing dispensations |
| **New ADM Cycle (if needed)** | Trigger for Phase A if major change |

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PHASE H = "KEEP ARCHITECTURE ALIVE"                                  │
│                                                                         │
│   • Monitor technology changes (new tech, EOL, vulnerabilities)        │
│   • Monitor business changes (strategy, regulations, market)           │
│   • Manage change requests (ACRs)                                      │
│   • Update architecture documents                                      │
│   • Trigger new ADM cycle when needed                                  │
│                                                                         │
│   OUTPUT: Architecture Updates + Change Requests + Governance Log      │
│                                                                         │
│   Without Phase H, architecture becomes outdated and irrelevant!       │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
