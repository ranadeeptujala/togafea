# TOGAF ADM - Phase A: Architecture Vision

> **Purpose**: Develop high-level vision of capabilities and business value

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE A: ARCHITECTURE VISION                         │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PURPOSE: Create a shared understanding of WHERE we're going          │
│                                                                         │
│   THIS IS WHERE EVERY PROJECT STARTS!                                  │
│                                                                         │
│   OUTCOME: Approval to proceed with architecture work                  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 6 Key Activities

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE A - 6 KEY ACTIVITIES                           │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. IDENTIFY STAKEHOLDERS & CONCERNS                                   │
│                                                                         │
│  2. CONFIRM BUSINESS GOALS & DRIVERS                                   │
│                                                                         │
│  3. DEFINE SCOPE                                                       │
│                                                                         │
│  4. CREATE ARCHITECTURE VISION                                         │
│                                                                         │
│  5. ASSESS READINESS FOR TRANSFORMATION                                │
│                                                                         │
│  6. OBTAIN APPROVAL (Statement of Architecture Work)                   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Activity 1: Identify Stakeholders & Concerns

### Stakeholder Domains

```
┌─────────────────────────────────────────────────────────────────┐
│                    STAKEHOLDER DOMAINS                          │
├─────────────────┬─────────────────┬─────────────────────────────┤
│    BUSINESS     │       IT        │      EXTERNAL               │
├─────────────────┼─────────────────┼─────────────────────────────┤
│ • CEO/COO       │ • CIO/CTO       │ • Customers                 │
│ • Business Unit │ • IT Operations │ • Vendors/Partners          │
│   Heads         │ • Developers    │ • Regulators                │
│ • Process Owners│ • Infrastructure│ • Auditors                  │
│ • End Users     │ • Security      │ • Industry Bodies           │
│ • Finance/CFO   │ • Data Teams    │ • Shareholders              │
│ • HR            │ • PMO           │ • Suppliers                 │
└─────────────────┴─────────────────┴─────────────────────────────┘
```

### Stakeholder Analysis Process

```
STEP 1: List all stakeholders
        └── From Stakeholder Map

STEP 2: Interview/Survey each stakeholder
        └── "What matters most to you?"

STEP 3: Document concerns
        └── Be specific, not vague

STEP 4: Prioritize concerns
        └── High / Medium / Low

STEP 5: Map to architecture views
        └── Which view addresses which concern?

STEP 6: Validate with stakeholders
        └── "Did I capture your concerns correctly?"
```

### Concerns Matrix

```
┌─────────────────────────────────────────────────────────────────┐
│                     CONCERNS MATRIX                             │
├──────────────────┬──────────────────────────────────────────────┤
│   STAKEHOLDER    │              CONCERNS                        │
├──────────────────┼──────────────────────────────────────────────┤
│ CEO              │ ROI, Business value, Risk                    │
├──────────────────┼──────────────────────────────────────────────┤
│ CIO              │ Cost, Timeline, Integration                  │
├──────────────────┼──────────────────────────────────────────────┤
│ End Users        │ Easy to use, Fast, Reliable                  │
├──────────────────┼──────────────────────────────────────────────┤
│ IT Operations    │ Maintainability, Availability, Support       │
├──────────────────┼──────────────────────────────────────────────┤
│ Security Officer │ Data protection, Compliance, Access control  │
└──────────────────┴──────────────────────────────────────────────┘
```

### RACI Matrix

```
RACI Matrix (R=Responsible, A=Accountable, C=Consulted, I=Informed)
┌──────────────────┬─────┬────────┬──────────┬──────────┐
│ ACTIVITY         │ CIO │ Sr. EA │ Bus.Owner│ Dev Team │
├──────────────────┼─────┼────────┼──────────┼──────────┤
│ Define Vision    │  A  │   R    │    C     │    I     │
│ Gather Reqmts    │  I  │   A    │    R     │    C     │
│ Approve Vision   │  A  │   R    │    C     │    I     │
│ Implementation   │  I  │   C    │    I     │    R     │
└──────────────────┴─────┴────────┴──────────┴──────────┘
```

---

## Activity 2: Confirm Business Goals & Drivers

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ACTIVITY 2: CONFIRM BUSINESS GOALS & DRIVERS                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  WHAT TO DO:                                                           │
│  • Understand WHY this project exists                                  │
│  • Identify business problems to solve                                 │
│  • Confirm strategic goals being supported                             │
│                                                                         │
│  EXAMPLE BUSINESS DRIVERS:                                             │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │ • "We need to enter new markets faster"                         │   │
│  │ • "Our costs are too high"                                      │   │
│  │ • "Competitors are ahead of us"                                 │   │
│  │ • "Regulations require us to change"                            │   │
│  │ • "Customer experience is poor"                                 │   │
│  │ • "Legacy systems are holding us back"                          │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
│  OUTPUT: Business Goals document, Key Drivers list                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Activity 3: Define Scope

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    STEP 3: DEFINE SCOPE                                 │
│                                                                         │
│   "WHAT is included and WHAT is NOT included in this architecture?"    │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Why Scope Matters

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    WHY SCOPE MATTERS                                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  ❌ WITHOUT CLEAR SCOPE:                                               │
│     • Scope creep (project keeps growing)                              │
│     • Unclear expectations                                             │
│     • Wasted effort on wrong things                                    │
│     • Never-ending project                                             │
│     • Stakeholder conflicts                                            │
│                                                                         │
│  ✅ WITH CLEAR SCOPE:                                                  │
│     • Everyone knows what's included                                   │
│     • Clear boundaries = focused effort                                │
│     • Easier to estimate time & cost                                   │
│     • Can say "NO" to out-of-scope requests                            │
│     • Stakeholders aligned                                             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Scope Dimensions

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    SCOPE DIMENSIONS                                     │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. BREADTH (Organizational Scope)                                     │
│     └── WHICH parts of the organization?                               │
│         • Entire enterprise?                                           │
│         • One business unit?                                           │
│         • One department?                                              │
│         • One system/application?                                      │
│                                                                         │
│  2. DEPTH (Level of Detail)                                            │
│     └── HOW detailed will the architecture be?                         │
│         • Strategic (high-level overview)                              │
│         • Segment (business unit level)                                │
│         • Capability (detailed)                                        │
│                                                                         │
│  3. ARCHITECTURE DOMAINS                                               │
│     └── WHICH domains are included?                                    │
│         • Business Architecture? (B)                                   │
│         • Data Architecture? (C)                                       │
│         • Application Architecture? (C)                                │
│         • Technology Architecture? (D)                                 │
│         • All of them?                                                 │
│                                                                         │
│  4. TIME HORIZON                                                       │
│     └── WHEN is the target state?                                      │
│         • 1 year?                                                      │
│         • 3 years?                                                     │
│         • 5 years?                                                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Depth Levels Explained

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   DEPTH LEVELS = ZOOM LEVELS ON A MAP 🗺️                               │
│                                                                         │
│   STRATEGIC   = Country view     ("India wants digital economy")       │
│   SEGMENT     = City view        ("Mumbai needs better transit")       │
│   CAPABILITY  = Street view      ("Build Metro Line 3, Station X")     │
│                                                                         │
│   Same project, different zoom levels for different audiences!         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Time Horizon

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    TIME HORIZON                                         │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   TIME HORIZON = The DEADLINE to reach Target State Architecture       │
│                                                                         │
│   SHORT-TERM:    6 months - 1 year  (Quick wins, tactical)             │
│   MEDIUM-TERM:   1-3 years          (Major projects)                   │
│   LONG-TERM:     3-5 years          (Strategic transformation)         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Deliverables

### Architecture Vision Document

```
┌─────────────────────────────────────────────────────────────────┐
│              ARCHITECTURE VISION DOCUMENT                       │
├─────────────────────────────────────────────────────────────────┤
│  1. Problem Description                                         │
│  2. Objectives & Scope                                          │
│  3. Stakeholder Map & Concerns                                  │
│  4. Business Scenario (if used)                                 │
│  5. High-Level Baseline Architecture                            │
│  6. High-Level Target Architecture                              │
│  7. Gap Analysis (High-Level)                                   │
│  8. Key Architecture Requirements                               │
│  9. Risks & Constraints                                         │
│  10. Business Value & Benefits                                  │
│  11. Architecture Principles (Applicable)                       │
│  12. Approval & Sign-off                                        │
└─────────────────────────────────────────────────────────────────┘
```

### Statement of Architecture Work (SOW)

```
STATEMENT OF ARCHITECTURE WORK
==============================

┌─────────────────────────────────────┐
│ 1. TITLE        │ 2. REQUEST        │  PROJECT
│ 3. DESCRIPTION  │ 4. SCOPE          │  BASICS
├─────────────────────────────────────┤
│ 5. VISION       │ 6. ROLES          │  WORK
│ 7. DELIVERABLES │ 8. ACCEPTANCE     │  DETAILS
├─────────────────────────────────────┤
│ 9. SCHEDULE     │ 10. RESOURCES     │  HOW
│ 11. RISKS       │ 12. CONSTRAINTS   │  WE DO IT
├─────────────────────────────────────┤
│ 13. STAKEHOLDERS│ 14. APPROVALS     │  WHO
└─────────────────────────────────────┘
```

### SOW vs Architecture Vision Document

```
┌─────────────────────────────────────────────────────────────────────────┐
│  STATEMENT OF ARCHITECTURE WORK    │  ARCHITECTURE VISION DOCUMENT      │
│  (SOW)                             │                                    │
├────────────────────────────────────┼────────────────────────────────────┤
│  📋 PROJECT CONTRACT               │  🎯 ARCHITECTURE CONTENT           │
├────────────────────────────────────┼────────────────────────────────────┤
│  HOW we will do the work           │  WHAT the architecture looks like  │
├────────────────────────────────────┼────────────────────────────────────┤
│  • Schedule & Timeline             │  • Baseline Architecture           │
│  • Resources & Budget              │  • Target Architecture             │
│  • Roles & Responsibilities        │  • Gap Analysis                    │
│  • Deliverables list               │  • Business Value                  │
│  • Acceptance criteria             │  • Stakeholder Concerns            │
├────────────────────────────────────┼────────────────────────────────────┤
│  Like a PROJECT CHARTER            │  Like a SOLUTION OVERVIEW          │
├────────────────────────────────────┼────────────────────────────────────┤
│  Signed by: Sponsors/Management    │  Used by: Architecture team        │
├────────────────────────────────────┼────────────────────────────────────┤
│  "Here's how we'll run the         │  "Here's where we are, where       │
│   architecture project"            │   we're going, and why"            │
└────────────────────────────────────┴────────────────────────────────────┘
```

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PHASE A = "GET APPROVAL TO START"                                    │
│                                                                         │
│   • Identify WHO cares (stakeholders)                                  │
│   • Understand WHY (business drivers)                                  │
│   • Define WHAT's included (scope)                                     │
│   • Create VISION (where we're going)                                  │
│   • Get APPROVAL (SOW signed)                                          │
│                                                                         │
│   OUTPUT: Green light to proceed with detailed architecture work!      │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
