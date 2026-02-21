# TOGAF ADM - Phase C: Information Systems Architecture

> **Purpose**: Develop Data Architecture and Application Architecture

---

## Overview

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE C: INFORMATION SYSTEMS ARCHITECTURE            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   PURPOSE: Define DATA and APPLICATIONS needed to support business     │
│                                                                         │
│   TWO SUB-PHASES:                                                      │
│   • Data Architecture (what data do we need?)                          │
│   • Application Architecture (what applications do we need?)           │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Key Activities

### 1. Develop Data Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    DATA ARCHITECTURE                                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT DEFINES:                                                     │
│   • What data entities exist                                           │
│   • How data is structured (logical models)                            │
│   • Where data is stored (physical models)                             │
│   • How data flows between systems                                     │
│   • Data ownership and governance                                      │
│                                                                         │
│   KEY ARTIFACTS:                                                       │
│   • Conceptual Data Model                                              │
│   • Logical Data Model                                                 │
│   • Physical Data Model                                                │
│   • Data Flow Diagrams                                                 │
│   • Data Catalog                                                       │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### 2. Develop Application Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    APPLICATION ARCHITECTURE                             │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   WHAT IT DEFINES:                                                     │
│   • What applications are needed                                       │
│   • How applications interact                                          │
│   • Application boundaries                                             │
│   • Integration patterns                                               │
│   • Application lifecycle                                              │
│                                                                         │
│   KEY ARTIFACTS:                                                       │
│   • Application Portfolio Catalog                                      │
│   • Application Communication Diagram                                  │
│   • Application/Function Matrix                                        │
│   • Interface Catalog                                                  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### 3. Perform Gap Analysis

- Compare Baseline vs Target for both Data and Application
- Identify what needs to be built, changed, or retired

---

## Example: Gaming Platform

### Data Architecture

```
DATA ARCHITECTURE:
├── Player Data (profiles, preferences, history)
├── Game Data (scores, achievements, leaderboards)  
├── Transaction Data (purchases, wallets, payouts)
└── Analytics Data (behavior, engagement metrics)
```

### Application Architecture

```
APPLICATION ARCHITECTURE:
├── Player Management System
├── Game Engine Integration
├── Payment Gateway
├── Bonus & Promotion Engine
├── Responsible Gaming Module
├── Reporting & Analytics Platform
└── Back Office Admin Portal
```

### Gap Analysis

```
GAP ANALYSIS:
• Current: Separate DBs per game → Target: Unified Player 360 view
• Current: Batch reporting → Target: Real-time analytics
• Current: Point-to-point integrations → Target: Event-driven (Kafka)
```

---

## Data vs Application Architecture

| Data Architecture | Application Architecture |
|-------------------|-------------------------|
| WHAT data exists | WHAT applications exist |
| HOW data is structured | HOW applications interact |
| WHERE data is stored | WHERE applications run |
| Data models, schemas | Application portfolio |
| Data flows | Integration patterns |

---

## Key Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Data Architecture Document** | Complete data architecture |
| **Application Architecture Document** | Complete application architecture |
| **Gap Analysis Results** | What needs to change |
| **Data Models** | Conceptual, Logical, Physical |
| **Application Portfolio** | List of all applications |
| **Interface Catalog** | All integrations documented |

---

## Summary

```
┌─────────────────────────────────────────────────────────────────────────┐
│                                                                         │
│   PHASE C = "WHAT DATA AND APPS DO WE NEED?"                           │
│                                                                         │
│   DATA ARCHITECTURE:                                                   │
│   • What data entities?                                                │
│   • How is data structured?                                            │
│   • Where is data stored?                                              │
│                                                                         │
│   APPLICATION ARCHITECTURE:                                            │
│   • What applications?                                                 │
│   • How do they interact?                                              │
│   • What integrations?                                                 │
│                                                                         │
│   OUTPUT: Data Architecture + Application Architecture + Gap Analysis  │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```
