# TOGAF ADM - Phase G: Implementation Governance

> **Purpose**: Provide architectural oversight during implementation

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                 PHASE G: IMPLEMENTATION GOVERNANCE                      │
│                                                                         │
│   "Are the development teams building what we designed?"               │
│   "Is the implementation following the architecture?"                  │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

1. **Ensure conformance with Target Architecture** - Are teams following the design?
2. **Govern implementation projects** - Oversight and guidance
3. **Perform Architecture Compliance reviews** - Formal assessments

---

## Architecture Review Board

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE REVIEW BOARD                            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   A governance body that reviews and approves architecture decisions   │
│                                                                         │
│   MEMBERS:                                                             │
│   • Chief Architect / Head of EA                                       │
│   • Enterprise Architects                                              │
│   • Domain Architects                                                  │
│   • Senior Technical Leaders                                           │
│   • Business Representatives (optional)                                │
│                                                                         │
│   RESPONSIBILITIES:                                                    │
│   • Review solution designs                                            │
│   • Approve/Reject/Request changes                                     │
│   • Grant dispensations (approved deviations)                          │
│   • Ensure compliance with standards                                   │
│   • Resolve architecture conflicts                                     │
│                                                                         │
│   MEETS:                                                               │
│   • Weekly or bi-weekly                                                │
│   • At key project milestones                                          │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Compliance Review Process

```
┌─────────────────────────────────────────────────────────────────────────┐
│                 COMPLIANCE REVIEW PROCESS                               │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  STEP 1: SCHEDULE REVIEW                                               │
│          └── At key milestones (design complete, before go-live)       │
│                                                                         │
│  STEP 2: PREPARE CHECKLIST                                             │
│          ├── Architecture principles followed?                         │
│          ├── Technology standards used?                                │
│          ├── Security requirements met?                                │
│          ├── Integration patterns correct?                             │
│          └── Data standards followed?                                  │
│                                                                         │
│  STEP 3: CONDUCT REVIEW                                                │
│          └── Review with development team, document findings           │
│                                                                         │
│  STEP 4: DOCUMENT RESULTS                                              │
│          ├── Conformant items                                          │
│          ├── Deviations found                                          │
│          └── Recommendations                                           │
│                                                                         │
│  STEP 5: DECISION                                                      │
│          ├── ✅ Approved                                               │
│          ├── ✅ Approved with conditions (fix minor issues)            │
│          └── ❌ Not approved (rework required)                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Compliance Checklist

```
┌──────────────────────────────────────────────────────────────────────────────┐
│                 ARCHITECTURE COMPLIANCE CHECKLIST                            │
├───────────────────────────────────┬──────────┬──────────┬────────────────────┤
│ CHECK ITEM                        │ EXPECTED │ ACTUAL   │ STATUS             │
├───────────────────────────────────┼──────────┼──────────┼────────────────────┤
│ API Design follows REST standards │ REST     │ REST     │ ✅ Compliant       │
│ Database is PostgreSQL            │ PostgreSQL│PostgreSQL│ ✅ Compliant       │
│ Runs on Kubernetes (EKS)          │ EKS      │ EKS      │ ✅ Compliant       │
│ Uses approved auth (OAuth 2.0)    │ OAuth 2.0│ JWT only │ ⚠️ Deviation       │
│ Logging to centralized system     │ DataDog  │ DataDog  │ ✅ Compliant       │
│ Secrets in Vault                  │ Vault    │ Env vars │ ❌ Non-compliant   │
│ CI/CD via GitHub Actions          │ GH Actions│GH Actions│ ✅ Compliant       │
├───────────────────────────────────┴──────────┴──────────┴────────────────────┤
│ RESULT: Approved with conditions - Fix secrets management before go-live     │
└──────────────────────────────────────────────────────────────────────────────┘
```

---

## Key Milestones for Review

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    KEY MILESTONES FOR REVIEW                            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   MILESTONE 1: DESIGN COMPLETE                                         │
│   └── Review solution design before development starts                 │
│       • Does it align with target architecture?                        │
│       • Are standards followed?                                        │
│                                                                         │
│   MILESTONE 2: DEVELOPMENT COMPLETE                                    │
│   └── Review implementation before testing                             │
│       • Is the code following architecture?                            │
│       • Are integrations correct?                                      │
│                                                                         │
│   MILESTONE 3: PRE-GO-LIVE                                             │
│   └── Final review before production deployment                        │
│       • Is everything compliant?                                       │
│       • Are all conditions met?                                        │
│                                                                         │
│   MILESTONE 4: POST-GO-LIVE                                            │
│   └── Review after deployment                                          │
│       • Is it working as designed?                                     │
│       • Any issues to address?                                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Dispensations

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    DISPENSATIONS                                        │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   An APPROVED DEVIATION from architecture standards                    │
│                                                                         │
│   WHEN NEEDED:                                                         │
│   • Technical constraint prevents compliance                           │
│   • Time/budget doesn't allow full compliance                          │
│   • Legacy integration requires exception                              │
│   • Business urgency overrides standard                                │
│                                                                         │
│   PROCESS:                                                             │
│   1. Team requests dispensation                                        │
│   2. Documents reason and impact                                       │
│   3. Proposes remediation plan (if temporary)                          │
│   4. Architecture Board reviews and decides                            │
│   5. If approved, dispensation is logged                               │
│                                                                         │
│   TYPES:                                                               │
│   • Temporary: Must be fixed by certain date                           │
│   • Permanent: Accepted as ongoing exception                           │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Contracts in Phase G

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    ARCHITECTURE CONTRACTS                               │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   CREATED IN: Phase F (Migration Planning)                             │
│   ENFORCED IN: Phase G (Implementation Governance)                     │
│                                                                         │
│   CONTRACT SAYS:                                                       │
│   • What the team agreed to build                                      │
│   • What standards to follow                                           │
│   • What quality criteria to meet                                      │
│   • When reviews will happen                                           │
│                                                                         │
│   PHASE G CHECKS:                                                      │
│   • Is the team honoring the contract?                                 │
│   • Are deliverables meeting criteria?                                 │
│   • Are standards being followed?                                      │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Compliance Assessments** | Results of architecture reviews |
| **Architecture Contracts** | Enforced and tracked |
| **Dispensation Log** | Approved deviations recorded |
| **Implementation Recommendations** | Guidance for teams |
| **Governance Log** | Record of all governance activities |

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PHASE G = "ENSURE THEY BUILD WHAT WE DESIGNED"                       │
│                                                                         │
│   • Architecture Review Board oversees implementation                  │
│   • Compliance reviews at key milestones                               │
│   • Check against standards and principles                             │
│   • Grant dispensations when needed                                    │
│   • Document everything in governance log                              │
│                                                                         │
│   OUTPUT: Compliance Assessments + Governance Log                      │
│                                                                         │
│   Without Phase G, architecture becomes shelfware!                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
