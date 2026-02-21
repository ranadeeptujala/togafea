# TOGAF ADM - Requirements Management

> **Purpose**: Manage requirements throughout all ADM phases

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS MANAGEMENT                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   NOT A PHASE - It's a CONTINUOUS PROCESS at the CENTER of ADM        │
│                                                                         │
│   Operates THROUGHOUT all phases (Preliminary through H)               │
│                                                                         │
│   "The hub that connects all phases"                                   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Position in ADM

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS MANAGEMENT IN ADM                       │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│                    ┌─────────────────┐                                 │
│                    │   Preliminary   │                                 │
│                    └────────┬────────┘                                 │
│                             │                                          │
│                    ┌────────▼────────┐                                 │
│                    │    Phase A      │                                 │
│                    └────────┬────────┘                                 │
│                             │                                          │
│      ┌──────────────────────┼──────────────────────┐                  │
│      │                      │                      │                   │
│      ▼                      ▼                      ▼                   │
│   Phase B              Phase C              Phase D                    │
│      │                      │                      │                   │
│      └──────────────────────┼──────────────────────┘                  │
│                             │                                          │
│                    ┌────────▼────────┐                                 │
│                    │                 │                                 │
│                    │  REQUIREMENTS   │  ◄── AT THE CENTER!            │
│                    │   MANAGEMENT    │                                 │
│                    │                 │                                 │
│                    └────────┬────────┘                                 │
│                             │                                          │
│                    ┌────────▼────────┐                                 │
│                    │   Phase E-H     │                                 │
│                    └─────────────────┘                                 │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS MANAGEMENT ACTIVITIES                   │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   1. IDENTIFY REQUIREMENTS                                             │
│      └── Capture requirements from stakeholders in each phase          │
│                                                                         │
│   2. STORE REQUIREMENTS                                                │
│      └── Maintain Requirements Repository                              │
│                                                                         │
│   3. MANAGE CHANGES                                                    │
│      └── Handle requirement changes and additions                      │
│                                                                         │
│   4. ENSURE ADDRESSED                                                  │
│      └── Verify requirements are addressed in appropriate phases       │
│                                                                         │
│   5. MAINTAIN TRACEABILITY                                             │
│      └── Track which requirements map to which architecture elements   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Requirements Repository

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS REPOSITORY                              │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   Central storage for all architecture requirements                    │
│                                                                         │
│   CONTAINS:                                                            │
│   • Business requirements                                              │
│   • Functional requirements                                            │
│   • Non-functional requirements (NFRs)                                 │
│   • Constraints                                                        │
│   • Assumptions                                                        │
│                                                                         │
│   ATTRIBUTES FOR EACH REQUIREMENT:                                     │
│   • ID (unique identifier)                                             │
│   • Description                                                        │
│   • Source (who requested)                                             │
│   • Priority (High/Medium/Low)                                         │
│   • Status (New/Approved/Implemented/Rejected)                         │
│   • Phase(s) addressed                                                 │
│   • Traceability (which architecture elements address it)              │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Requirements by Phase

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS BY PHASE                                │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PHASE A (Vision):                                                    │
│   • High-level business requirements                                   │
│   • Stakeholder concerns                                               │
│   • Business drivers                                                   │
│                                                                         │
│   PHASE B (Business):                                                  │
│   • Business process requirements                                      │
│   • Organizational requirements                                        │
│   • Business capability requirements                                   │
│                                                                         │
│   PHASE C (Data & Application):                                        │
│   • Data requirements                                                  │
│   • Application functionality requirements                             │
│   • Integration requirements                                           │
│                                                                         │
│   PHASE D (Technology):                                                │
│   • Infrastructure requirements                                        │
│   • Platform requirements                                              │
│   • Security requirements                                              │
│   • Performance requirements (NFRs)                                    │
│                                                                         │
│   PHASE E-F (Implementation):                                          │
│   • Implementation constraints                                         │
│   • Migration requirements                                             │
│   • Transition requirements                                            │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Traceability Matrix

```
┌──────────────────────────────────────────────────────────────────────────────┐
│                    REQUIREMENTS TRACEABILITY MATRIX                          │
├────────────┬────────────────────────┬────────┬────────────────────────────────┤
│ REQ ID     │ REQUIREMENT            │ PHASE  │ ARCHITECTURE ELEMENT           │
├────────────┼────────────────────────┼────────┼────────────────────────────────┤
│ REQ-001    │ 100ms response time    │ D      │ Redis caching, CDN             │
│ REQ-002    │ 99.99% availability    │ D      │ Multi-AZ, Auto-scaling         │
│ REQ-003    │ Real-time analytics    │ C      │ Kafka, Streaming pipeline      │
│ REQ-004    │ Unified player view    │ C      │ Player 360 Platform            │
│ REQ-005    │ PCI-DSS compliance     │ D      │ Payment service isolation      │
│ REQ-006    │ Automated onboarding   │ B      │ Onboarding process redesign    │
│ REQ-007    │ Cloud-native           │ D      │ EKS, Kubernetes deployment     │
└────────────┴────────────────────────┴────────┴────────────────────────────────┘
```

---

## Handling Requirement Changes

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    HANDLING REQUIREMENT CHANGES                         │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   STEP 1: RECEIVE CHANGE REQUEST                                       │
│           └── New requirement or change to existing                    │
│                                                                         │
│   STEP 2: ASSESS IMPACT                                                │
│           └── Which phases are affected?                               │
│           └── What architecture elements need to change?               │
│                                                                         │
│   STEP 3: EVALUATE                                                     │
│           └── Is this change justified?                                │
│           └── What's the cost/benefit?                                 │
│                                                                         │
│   STEP 4: DECIDE                                                       │
│           ├── Accept: Update requirements & architecture               │
│           ├── Reject: Document reason                                  │
│           └── Defer: Schedule for future phase/cycle                   │
│                                                                         │
│   STEP 5: UPDATE                                                       │
│           └── Update Requirements Repository                           │
│           └── Update affected architecture documents                   │
│           └── Communicate to stakeholders                              │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Requirements vs Constraints vs Assumptions

```
┌─────────────────────────────────────────────────────────────────────────┐
│         REQUIREMENTS vs CONSTRAINTS vs ASSUMPTIONS                      │
├────────────────────┬────────────────────────────────────────────────────┤
│ REQUIREMENTS       │ What the system MUST do or achieve                 │
│                    │ Example: "System must support 10,000 concurrent    │
│                    │ users"                                             │
├────────────────────┼────────────────────────────────────────────────────┤
│ CONSTRAINTS        │ Limitations that RESTRICT design choices           │
│                    │ Example: "Must use existing Oracle database"       │
│                    │ Example: "Budget limited to $500K"                 │
├────────────────────┼────────────────────────────────────────────────────┤
│ ASSUMPTIONS        │ Things we BELIEVE to be true but haven't verified  │
│                    │ Example: "IT team has Kubernetes expertise"        │
│                    │ Example: "Vendor API will remain stable"           │
└────────────────────┴────────────────────────────────────────────────────┘
```

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Requirements Repository** | Central storage of all requirements |
| **Traceability Matrix** | Mapping requirements to architecture |
| **Impact Assessments** | Analysis of requirement changes |
| **Requirements Sign-off** | Stakeholder approval of requirements |

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   REQUIREMENTS MANAGEMENT = "THE HUB OF ADM"                           │
│                                                                         │
│   • NOT a phase - operates THROUGHOUT all phases                       │
│   • Captures requirements from stakeholders                            │
│   • Stores in central repository                                       │
│   • Manages changes                                                    │
│   • Ensures requirements are addressed                                 │
│   • Maintains traceability                                             │
│                                                                         │
│   OUTPUT: Requirements Repository + Traceability Matrix                │
│                                                                         │
│   Without Requirements Management, architecture loses connection       │
│   to what stakeholders actually need!                                  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
