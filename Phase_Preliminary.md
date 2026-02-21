# TOGAF ADM - Preliminary Phase

> **Purpose**: Prepare the organization for TOGAF projects (ONE-TIME setup)

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PRELIMINARY PHASE                                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PURPOSE: Set up the Enterprise Architecture CAPABILITY                │
│                                                                         │
│   DONE: ONCE for the organization (not for every project)              │
│                                                                         │
│   OUTCOME: EA team, tools, principles, governance ready to guide       │
│            ALL future architecture projects                            │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

### Define Architecture Capability (5 Pillars)

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    EA CAPABILITY (5 PILLARS)                            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   1. CREATE TEAM (People)                                              │
│      └── Enterprise Architects, Domain Architects, support staff       │
│                                                                         │
│   2. SETUP TOOLS                                                       │
│      └── Sparx EA, Archi, Confluence, Draw.io, GitHub                  │
│                                                                         │
│   3. DEFINE PRINCIPLES                                                 │
│      └── Cloud-First, Security by Design, Buy over Build               │
│                                                                         │
│   4. ESTABLISH GOVERNANCE                                              │
│      └── Architecture Board, Review process, Compliance                │
│                                                                         │
│   5. DEFINE STANDARDS                                                  │
│      └── Technology standards, Patterns, Reference architectures       │
│                                                                         │
│   All this happens in PRELIMINARY PHASE (once)                         │
│   Then EA GUIDES all projects using these!                             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Architecture Principles

Principles are **guiding rules** that help make consistent decisions across ALL projects.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PRINCIPLES GUIDE EVERY PROJECT                       │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PRELIMINARY: Define Principles (ONCE)                                │
│   ─────────────────────────────────────                                │
│   • Cloud-First                                                        │
│   • Security by Design                                                 │
│   • Buy over Build                                                     │
│   • API-First                                                          │
│   • Data is an Asset                                                   │
│                                                                         │
│         │                                                               │
│         │ These GUIDE every project                                     │
│         ▼                                                               │
│   ┌─────────────────────────────────────────────────────────────────┐  │
│   │                                                                  │  │
│   │  PROJECT 1: Payment System                                      │  │
│   │  Driver: "Reduce latency"                                       │  │
│   │  Decision: "Should we use on-prem or cloud?"                    │  │
│   │  → Check Principle: "Cloud-First" → Use Cloud ✅                │  │
│   │                                                                  │  │
│   │  PROJECT 2: CRM Selection                                       │  │
│   │  Driver: "Need better customer management"                      │  │
│   │  Decision: "Should we build custom CRM or buy?"                 │  │
│   │  → Check Principle: "Buy over Build" → Buy Salesforce ✅        │  │
│   │                                                                  │  │
│   │  PROJECT 3: Mobile App                                          │  │
│   │  Driver: "Launch mobile experience"                             │  │
│   │  Decision: "How to handle authentication?"                      │  │
│   │  → Check Principle: "Security by Design" → OAuth from start ✅  │  │
│   │                                                                  │  │
│   └─────────────────────────────────────────────────────────────────┘  │
│                                                                         │
│   PRINCIPLES = Consistent decision-making across ALL projects          │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Principle Structure

Each principle has 4 parts:

| Component | Description | Example |
|-----------|-------------|---------|
| **Name** | Short identifier | "Cloud-First" |
| **Statement** | What it means | "All new applications should be deployed on cloud unless there's a valid reason not to" |
| **Rationale** | Why this principle | "Cloud provides scalability, cost efficiency, and modern capabilities" |
| **Implications** | What it means for decisions | "Teams must evaluate cloud options first; on-prem needs Architecture Board approval" |

---

## Architecture Principles vs Architecture Requirements (NFRs)

| Architecture Principles | Architecture Requirements (NFRs) |
|-------------------------|-----------------------------------|
| Guiding philosophy | Specific metrics |
| "Systems should be resilient" | "99.99% uptime" |
| "Prefer cloud-first approach" | "Must use AWS/Azure" |
| "Design for performance" | "100ms latency" |
| "Systems should be loosely coupled" | "Use microservices with REST APIs" |
| WHY we design a certain way | WHAT we must achieve |

---

## Reference Architectures

Reference Architectures are **proven, reusable templates** for solving common architecture problems.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    REFERENCE ARCHITECTURE                               │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT IS:                                                          │
│   ───────────                                                          │
│   • A TEMPLATE / BLUEPRINT for a common solution                       │
│   • Pre-approved, proven pattern                                       │
│   • Ready-to-use starting point                                        │
│   • Standardized across organization                                   │
│                                                                         │
│   EXAMPLES:                                                            │
│   ─────────                                                            │
│   • Microservices Reference Architecture                               │
│   • Data Lake Reference Architecture                                   │
│   • E-commerce Reference Architecture                                  │
│   • Cloud-Native Web App Reference Architecture                        │
│                                                                         │
│   BENEFITS:                                                            │
│   ─────────                                                            │
│   ✅ SPEED        → Don't design from scratch                          │
│   ✅ CONSISTENCY  → All teams follow same patterns                     │
│   ✅ QUALITY      → Proven, tested designs                             │
│   ✅ COMPLIANCE   → Pre-approved by Architecture Board                 │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Organizational Model for EA** | Team structure, roles, processes |
| **Architecture Principles** | Guiding rules for all decisions |
| **Architecture Repository** | Storage for all architecture assets |
| **Architecture Governance Framework** | How decisions are made and enforced |
| **Tailored Architecture Framework** | TOGAF customized for your organization |

---

## Common Misconception

```
┌─────────────────────────────────────────────────────────────────────────┐
│           ❌ WRONG vs ✅ CORRECT UNDERSTANDING                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   ❌ WRONG:                                                            │
│   "Preliminary Phase is done for EVERY project"                        │
│                                                                         │
│   ✅ CORRECT:                                                          │
│   "Preliminary Phase is done ONCE to set up the EA capability"         │
│   "Projects start from Phase A (Architecture Vision)"                  │
│                                                                         │
│   ─────────────────────────────────────────────────────────────────    │
│                                                                         │
│   PRELIMINARY (Year 1):                                                │
│   ┌─────────────────────────────────────────────────────────────────┐  │
│   │ Setup: Team + Tools + Principles + Governance + Standards       │  │
│   └─────────────────────────────────────────────────────────────────┘  │
│                              │                                          │
│                              │ (Done ONCE)                              │
│                              ▼                                          │
│   ─────────────────────────────────────────────────────────────────    │
│                                                                         │
│   PROJECT 1 (uses EA):       PROJECT 2 (uses EA):                      │
│   ┌─────────────────┐        ┌─────────────────┐                       │
│   │ Phase A → H     │        │ Phase A → H     │                       │
│   │ (Starts at A)   │        │ (Starts at A)   │                       │
│   └─────────────────┘        └─────────────────┘                       │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PRELIMINARY PHASE = SETUP THE "ARCHITECTURE KITCHEN"                 │
│                                                                         │
│   • Create the EA team (chefs)                                         │
│   • Setup tools (equipment)                                            │
│   • Define principles (recipes & standards)                            │
│   • Establish governance (quality control)                             │
│   • Define standards (ingredients list)                                │
│                                                                         │
│   Once the kitchen is ready, it serves ALL projects!                   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
