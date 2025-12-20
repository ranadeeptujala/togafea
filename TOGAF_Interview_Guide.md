# TOGAF 9.2 Interview Preparation Guide

> Based on TOGAF 9.2 (April 2018)

## Table of Contents
1. [What is TOGAF?](#what-is-togaf)
2. [TOGAF Architecture Development Method (ADM)](#togaf-adm)
3. [Key Concepts & Terminology](#key-concepts)
4. [Common Interview Questions](#interview-questions)
5. [Study Tips](#study-tips)

---

## What is TOGAF? <a name="what-is-togaf"></a>

**TOGAF** (The Open Group Architecture Framework) is an enterprise architecture framework that provides a comprehensive approach to designing, planning, implementing, and governing enterprise information technology architecture.

### Key Facts:
- Developed by **The Open Group**
- First introduced in **1995** (based on TAFIM from US DoD)
- Current version: **TOGAF 9.2** (released April 2018)
- Used by **80%+ of Global 50 companies**
- Provides a common vocabulary and methodology

### Four Architecture Domains:

| Domain | Description |
|--------|-------------|
| **Business Architecture** | Business strategy, governance, organization, and key business processes |
| **Data Architecture** | Structure of logical and physical data assets and data management resources |
| **Application Architecture** | Blueprint for individual applications, their interactions, and relationships |
| **Technology Architecture** | Software and hardware capabilities required to support business, data, and application services |

---

## TOGAF Architecture Development Method (ADM) <a name="togaf-adm"></a>

The **ADM** is the core of TOGAF - an iterative, step-by-step approach to developing enterprise architecture.

```
                    ┌─────────────────┐
                    │   Preliminary   │
                    │     Phase       │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │    Phase A:     │
                    │ Architecture    │
                    │    Vision       │
                    └────────┬────────┘
                             │
        ┌────────────────────┼────────────────────┐
        │                    │                    │
┌───────▼───────┐   ┌───────▼───────┐   ┌───────▼───────┐
│   Phase B:    │   │   Phase C:    │   │   Phase D:    │
│   Business    │   │  Information  │   │  Technology   │
│ Architecture  │   │   Systems     │   │ Architecture  │
└───────┬───────┘   │ Architecture  │   └───────┬───────┘
        │           └───────┬───────┘           │
        └────────────────────┼──────────────────┘
                             │
                    ┌────────▼────────┐
                    │    Phase E:     │
                    │ Opportunities   │
                    │  & Solutions    │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │    Phase F:     │
                    │   Migration     │
                    │   Planning      │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │    Phase G:     │
                    │ Implementation  │
                    │   Governance    │
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │    Phase H:     │
                    │ Architecture    │
                    │    Change       │
                    │   Management    │
                    └─────────────────┘

         Requirements Management (Center - All Phases)
```

### ADM Phases Explained:

#### **Preliminary Phase**
- **Purpose**: Prepare the organization for TOGAF projects
- **Key Activities**:
  - Define Architecture Capability(people,process ,tools,governance,standrds)
  ── People
│   ├── You (Senior EA / Head)
│   ├── Domain Architects (if any)
│   └── Supporting staff
│
├── Processes
│   ├── TOGAF ADM (tailored)
│   ├── Architecture Review process
│   └── Change management process
│
├── Tools
│   ├── Modeling tool (Sparx EA, Archi, etc.)
│   ├── Repository (SharePoint, Confluence, etc.,git hub )
│   └── Documentation templates
│
├── Governance
│   ├── Architecture Board / Review meetings(Review boards)
│   ├── Architecture Principles
│   └── Compliance checklist- Gaming certficatons tatndrs like rng ,DPDPA
│
└── Standards
    ├── Reference Architectures
    ├── Technology Standards
    └── Design Patterns
  - Establish Architecture Principles


| Architecture Principles          | Architecture Requirements (NFRs)   |
|----------------------------------|------------------------------------|
| Guiding philosophy               | Specific metrics                   |
| "Systems should be resilient"    | "99.99% uptime"                    |
| "Prefer cloud-first approach"    | "Must use AWS/Azure"               |
| "Design for performance"         | "100ms latency"                    |
| "Systems should be loosely coupled" | "Use microservices with REST APIs" |
| WHY we design a certain way      | WHAT we must achieve               |
  - Select and tailor frameworks/tools
  - Define Architecture Repository
- **Key Deliverable**: Organizational Model for EA, Architecture Principles

#### **Phase A: Architecture Vision**
- **Purpose**: Develop high-level vision of capabilities and business value
- **Key Activities**:



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
  -Stake holerds parrt

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
PHASE A: ARCHITECTURE VISION
│
├── 1. IDENTIFY Stakeholders
│       └── From Business, IT, External domains
│
├── 2. ANALYZE Stakeholders
│       ├── Power/Interest mapping
│       ├── Concerns identification
│       └── Communication needs
│
├── 3. DOCUMENT in Architecture Vision
│       ├── Stakeholder Map
│       ├── Concerns Matrix
│       └── Communication Plan
│
└── 4. GET APPROVAL
        └── Statement of Architecture Work signed by key stakeholders
RACI Matrix (R=Responsible, A=Accountable, C=Consulted, I=Informed)
┌──────────────────┬─────┬────────┬──────────┬──────────┐
│ ACTIVITY         │ CIO │ Sr. EA │ Bus.Owner│ Dev Team │
├──────────────────┼─────┼────────┼──────────┼──────────┤
│ Define Vision    │  A  │   R    │    C     │    I     │
│ Gather Reqmts    │  I  │   A    │    R     │    C     │
│ Approve Vision   │  A  │   R    │    C     │    I     │
│ Implementation   │  I  │   C    │    I     │    R     │
└──────────────────┴─────┴────────┴──────────┴──────────┘
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
  - Create Architecture Vision
  - Obtain approval for Statement of Architecture Work



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

┌─────────────────────────────────────────────────────────────────────────┐
│                    STEP 3: DEFINE SCOPE                                 │
│                                                                         │
│   "WHAT is included and WHAT is NOT included in this architecture?"    │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
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



on
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

4 + 4 + 4 + 2 = 14 items\

SECTION                    | DESCRIPTION
---------------------------|---------------------------------------------
1. Project Title           | Name of the architecture initiative
2. Project Request         | Why this project was initiated
3. Project Description     | Brief overview of what will be done
4. Scope                   | What's included and excluded
5. Architecture Vision     | Summary of target state
6. Roles & Responsibilities| Who does what (RACI)
7. Deliverables            | What will be produced
8. Acceptance Criteria     | How success is measured
9. Schedule & Milestones   | Timeline with key dates
10. Resources              | People, budget, tools needed
11. Risks & Mitigation     | Potential issues and plans
12. Constraints            | Limitations (time, budget, etc.)
13. Stakeholders           | Key people involved
14. Approvals              | Sign-off secti
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
**Key Deliverables**: Statement of Architecture Work, Architecture Vision documynet
#### **Phase B: Business Architecture**
- **Purpose**: Develop the Target Business Architecture
- **Key Activities**:



BUSINESS ARCHITECTURE IS ABOUT:
===============================

NOT about:
- Technical implementation details
- Specific software/hardware
- Coding/development

IS about:
- Business processes (how work flows)
- Business capabilities (what business can do)
- Business services (what business offers)
- Organization (who does what)
- Information flows (what data moves where)
- Gap between current and future state
  - Develop Baseline Business Architecture

BASELINE BUSINESS ARCHITECTURE = "As-Is" State

Documents HOW THE BUSINESS WORKS TODAY:
- Current business processes
- Current organization structure
- Current business capabilities
- Current business services
- Current information flows
- Current pain points & gaps
REASON                          | EXPLANATION
--------------------------------|------------------------------------------
Understand current state        | Can't improve what you don't understand
Identify gaps                   | Compare with target to find gaps
Stakeholder alignment           | Everyone agrees on "where we are"
Realistic planning              | Know what needs to change
Risk assessment                 | Understand dependencies & impacts
Measure progress                | Baseline for measuring improvement

BASELINE (As-Is)                | TARGET (To-Be)
--------------------------------|----------------------------------
How business works TODAY        | How business will work FUTURE
Current processes               | Improved/new processes
Current capabilities            | Enhanced capabilities
Current problems                | Problems solved
Documented FIRST                | Designed AFTER baseline

  - Develop Target Business Architecture





1. BASELINE BUSINESS FLOW  -->  Current state (As-Is)
          +
2. TARGET BUSINESS FLOW    -->  Future state (To-Be)
          +
3. GAP ANALYSIS            -->  What needs to change

  - Perform Gap Analysis
- **Key Deliverables**: Business Architecture document, Gap Analysis results

#### **Phase C: Information Systems Architecture**
- **Purpose**: Develop Data and Application Architectures
- **Key Activities**:
  - Develop Data Architecture (logical & physical data models)
  - Develop Application Architecture
  - Perform Gap Analysis
- **Key Deliverables**: Data Architecture, Application Architecture documents
DATA ARCHITECTURE:
├── Player Data (profiles, preferences, history)
├── Game Data (scores, achievements, leaderboards)  
├── Transaction Data (purchases, wallets, payouts)
└── Analytics Data (behavior, engagement metrics)

APPLICATION ARCHITECTURE:
├── Player Management System
├── Game Engine Integration
├── Payment Gateway
├── Bonus & Promotion Engine
├── Responsible Gaming Module
├── Reporting & Analytics Platform
└── Back Office Admin Portal

GAP ANALYSIS:
• Current: Separate DBs per game → Target: Unified Player 360 view
• Current: Batch reporting → Target: Real-time analytics
• Current: Point-to-point integrations → Target: Event-driven (Kafka)



#### **Phase D: Technology Architecture**
- **Purpose**: Develop the Technology Architecture
- **Key Activities**:
  - Define technology platforms
  - Map applications to technology
  - Perform Gap Analysis

Purpose: Define the technology infrastructure needed to support applications and data

┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE D: TECHNOLOGY ARCHITECTURE                     │
│                                                                         │
│   "What hardware, software, and infrastructure do we need?"             │
└─────────────────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────────────────┐
│                     TECHNOLOGY PLATFORM LAYERS                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  EDGE / DELIVERY LAYER (Entry Point for Users)                   │   │
│  │  • CDN (CloudFront, Akamai) - Cache & deliver static content     │   │
│  │  • Load Balancers (ALB, HAProxy) - Distribute traffic            │   │
│  │  • Web servers (Nginx, Apache) - Serve requests                  │   │
│  │  • API Gateway - Route API calls                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                              ▼                                          │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  APPLICATION LAYER                                               │   │
│  │  • Frontend: React, Angular, Vue, Mobile (Flutter, Swift, Kotlin)│   │
│  │  • Backend: Java, .NET, Node.js, Python, Go                      │   │
│  │  • Containers (Docker, Kubernetes)                               │   │
│  │  • Serverless (AWS Lambda, Azure Functions)                      │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                              ▼                                          │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  DATA LAYER                                                      │   │
│  │  • Databases (PostgreSQL, MongoDB, Redis)                        │   │
│  │  • Data Warehouse (Snowflake, BigQuery)                          │   │
│  │  • Message Queues (Kafka, RabbitMQ)                              │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                              ▼                                          │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  INFRASTRUCTURE LAYER                                            │   │
│  │  • Cloud (AWS, Azure, GCP)                                       │   │
│  │  • Compute (EC2, VMs, Bare Metal)                                │   │
│  │  • Storage (S3, EBS, NAS)                                        │   │
│  │  • Network (VPC, DNS, Firewalls)                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                              ▼                                          │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  SECURITY & OPERATIONS                                           │   │
│  │  • Identity (IAM, SSO, OAuth)                                    │   │
│  │  • Monitoring (Prometheus, Grafana, DataDog)                     │   │
│  │  • CI/CD (Jenkins, GitHub Actions, ArgoCD)                       │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────────────┐
│              APPLICATION ↔ TECHNOLOGY MAPPING MATRIX                    │
├─────────────────┬──────────┬──────────┬───────────┬─────────┬──────────┤
│   APPLICATION   │ COMPUTE  │ DATABASE │  RUNTIME  │  CLOUD  │ CONTAINER│
├─────────────────┼──────────┼──────────┼───────────┼─────────┼──────────┤
│ Player Portal   │ EKS      │ PostgreSQL│ Node.js  │ AWS     │ ✓        │
│ Payment Service │ EKS      │ PostgreSQL│ Java     │ AWS     │ ✓        │
│ Game Engine     │ EC2      │ Redis    │ C++      │ AWS     │ ✗        │
│ Analytics       │ EMR      │ Redshift │ Python   │ AWS     │ ✗        │
│ Admin Portal    │ Lambda   │ DynamoDB │ Node.js  │ AWS     │ ✗        │
│ Legacy ERP      │ On-Prem  │ Oracle   │ Java     │ N/A     │ ✗        │
└─────────────────┴──────────┴──────────┴───────────┴─────────┴──────────┘
- **Key Deliverables**: Technology Architecture document

#### **Phase E: Opportunities and Solutions**
- **Purpose**: Generate initial implementation and migration strategy
- **Key Activities**:
  - Identify major work packages
  - Group work packages into projects
  - Assess dependencies and priorities
- **Key Deliverables**: Implementation and Migration Strategy
┌─────────────────────────────────────────────────────────────────────────┐
│                   PHASE E: OPPORTUNITIES & SOLUTIONS                    │
│                                                                         │
│   "How do we actually BUILD what we designed in Phases B, C, D?"        │

└─────────────────────────────────────────────────────────────────────────┘


┌─────────────────────────────────────────────────────────────────────────┐
│                    GAP → WORK PACKAGE MAPPING                           │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   GAP (From B, C, D)              WORK PACKAGE                         │
│   ─────────────────────           ──────────────────────               │
│   No unified player view    →     WP1: Build Player 360 Platform       │
│   Manual payment process    →     WP2: Payment Gateway Integration     │
│   Legacy monolith app       →     WP3: Migrate to Microservices        │
│   No cloud infrastructure   →     WP4: AWS Cloud Setup                 │
│   No CI/CD pipeline         →     WP5: DevOps Implementation           │
│   No real-time analytics    →     WP6: Data Platform Setup             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘



┌─────────────────────────────────────────────────────────────────┐
│  WORK PACKAGE TEMPLATE                                          │
├─────────────────────────────────────────────────────────────────┤
│  Name:        Payment Gateway Integration                       │
│  Gap Addressed: Manual payment processing                       │
│  Scope:       Integrate with 3 payment providers               │
│  Effort:      3 months, 5 engineers                            │
│  Dependencies: WP4 (Cloud Setup) must complete first           │
│  Business Value: Reduce transaction time by 80%                │
│  Risk:        PCI-DSS compliance requirements                  │
└─────────────────────────────────────────────────────────────────┘


┌─────────────────────────────────────────────────────────────────────────┐
│              WORK PACKAGES → PROJECTS GROUPING                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  PROJECT 1: INFRASTRUCTURE MODERNIZATION                               │
│  ├── WP4: AWS Cloud Setup                                              │
│  ├── WP5: DevOps Implementation                                        │
│  └── WP7: Security & Compliance Setup                                  │
│                                                                         │
│  PROJECT 2: CORE PLATFORM                                              │
│  ├── WP1: Player 360 Platform                                          │
│  ├── WP2: Payment Gateway Integration                                  │
│  └── WP8: Bonus Engine Development                                     │
│                                                                         │
│  PROJECT 3: DATA & ANALYTICS                                           │
│  ├── WP6: Data Platform Setup                                          │
│  └── WP9: Reporting Dashboard                                          │
│                                                                         │
│  PROJECT 4: LEGACY MIGRATION                                           │
│  └── WP3: Migrate to Microservices                                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────────────────┐
│                      DEPENDENCY MATRIX                                   │
├──────────┬────────┬────────┬────────┬────────┬────────┬────────┬────────┤
│          │  WP1   │  WP2   │  WP3   │  WP4   │  WP5   │  WP6   │  WP7   │
├──────────┼────────┼────────┼────────┼────────┼────────┼────────┼────────┤
│ WP1      │   -    │        │        │   ✓    │   ✓    │        │   ✓    │
│ WP2      │   ✓    │   -    │        │   ✓    │   ✓    │        │   ✓    │
│ WP3      │        │        │   -    │   ✓    │   ✓    │        │        │
│ WP4      │        │        │        │   -    │        │        │        │
│ WP5      │        │        │        │   ✓    │   -    │        │        │
│ WP6      │   ✓    │        │        │   ✓    │   ✓    │   -    │        │
│ WP7      │        │        │        │   ✓    │        │        │   -    │
└──────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┘
  ✓ = Depends on (must be done first)
  ┌─────────────────────────────────────────────────────────────────────────┐
│              PHASE E: BUILD vs BUY vs REUSE DECISIONS                   │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   FOR EACH GAP, EVALUATE SOLUTIONS:                                    │
│                                                                         │
│   ┌─────────────┐     ┌─────────────┐     ┌─────────────┐              │
│   │    BUILD    │     │     BUY     │     │    REUSE    │              │
│   │   Custom    │     │   Product   │     │  Existing   │              │
│   │ Development │     │   / SaaS    │     │   Assets    │              │
│   └─────────────┘     └─────────────┘     └─────────────┘              │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
  Reading: WP2 (Payment) depends on WP1, WP4, WP5, WP7
#### **Phase F: Migration Planning**
- **Purpose**: Finalize detailed implementation and migration plan
- **Key Activities**:
  - Finalize Architecture Roadmap
  - Finalize Implementation Plan
  - Ensure business value is realized
- **Key Deliverables**: Implementation and Migration Plan, Architecture Roadmap
┌─────────────────────────────────────────────────────────────────────────┐
│                    PHASE F: MIGRATION PLANNING                          │
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
│  DELIVERABLES:                                                         │
│  • Implementation & Migration Plan (detailed project plans)            │
│  • Architecture Roadmap (visual timeline)                              │
│  • Architecture Contracts (agreements with implementation teams)       │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
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
#### **Phase G: Implementation Governance**
- **Purpose**: Provide architectural oversight during implementation
- **Key Activities**:
  - Ensure conformance with Target Architecture
  - Govern implementation projects
  - Perform Architecture Compliance reviews
- **Key Deliverables**: Compliance assessments, Architecture Contracts
┌─────────────────────────────────────────────────────────────────────────┐
│                 PHASE G: IMPLEMENTATION GOVERNANCE                      │
│                                                                         │
│   "Are the development teams building what we designed?"               │
│   "Is the implementation following the architecture?"                  │
└─────────────────────────────────────────────────────────────────────────┘


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
#### **Phase H: Architecture Change Management**
- **Purpose**: Keep architecture aligned with changing requirements
- **Key Activities**:
  - Monitor technology changes
  - Monitor business changes
  - Manage Architecture Change Requests
- **Key Deliverables**: Architecture updates, Change Requests
┌─────────────────────────────────────────────────────────────────────────┐
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



#### **Requirements Management (Central)**
- Operates throughout all phases
- Handles requirements identification, storage, and change management
- Ensures requirements are addressed in appropriate phases

---

## Key Concepts & Terminology <a name="key-concepts"></a>

### Architecture Content Framework

| Component | Description |
|-----------|-------------|
| **Deliverables** | Contractually specified work products (e.g., Architecture Definition Document) |
| **Artifacts** | Architectural work products (diagrams, catalogs, matrices) |
| **Building Blocks** | Components that can be combined to deliver architectures |

### Building Blocks

1. **Architecture Building Blocks (ABBs)**
   - Define what functionality is required
   - Capture architecture requirements
   - Direct and guide development of SBBs
   - Example: "A customer management capability"

2. **Solution Building Blocks (SBBs)**
   - Define how functionality is implemented
   - Product or vendor-aware
   - Example: "Salesforce CRM"

### Enterprise Continuum

                                                │
│   ENTERPRISE CONTINUUM = A LIBRARY of reusable architecture patterns   │
│                          organized from GENERIC to SPECIFIC on-specific:

```
Foundation    ──►    Common Systems    ──►    Industry    ──►    Organization
Architectures        Architectures          Architectures       Architectures
(Generic)                                                       (Specific)
```

Components:
- **Architecture Continuum**: Structural elements
- **Solutions Continuum**: Implementation elements

### Architecture Repository

| Component | Description |
|-----------|-------------|
| **Architecture Metamodel** | Describes how architecture is organized |
| **Architecture Capability** | Parameters, structures, processes for architecture |
| **Architecture Landscape** | Architectural representations at different levels |
| **Standards Information Base (SIB)** | Standards for architecture work |
| **Reference Library** | Guidelines, templates, patterns |
| **Governance Log** | Record of governance activity |

### Architecture Governance

**Purpose**: Ensure architectures are developed consistently and compliance is maintained

**Key Elements**:
- Architecture Board
- Architecture Compliance
- Architecture Contracts
- Dispensations (approved deviations)

### Stakeholder Management

**Key Stakeholders in EA**:
- Sponsors/Executives
- Business Users
- IT Operations
- Project Managers
- Developers
- External Partners

**Stakeholder Analysis Techniques**:
- Power/Interest Grid
- Stakeholder Map
- RACI Matrix

### Views and Viewpoints

- **View**: Representation of a system from the perspective of a stakeholder
- **Viewpoint**: Definition of the perspective from which a view is taken
- **Concern**: Interest in a system relevant to stakeholders

### Architecture Principles

**Structure of a Principle**:
1. Name
2. Statement
3. Rationale
4. Implications

**Example Principle**:
- **Name**: Technology Independence
- **Statement**: Applications are independent of specific technology choices
- **Rationale**: Allows technology to change without affecting applications
- **Implications**: Requires standard interfaces, may increase development cost

---

## Common Interview Questions <a name="interview-questions"></a>

### Basic Level Questions

**Q1: What is TOGAF?**
> TOGAF is an enterprise architecture framework that provides a comprehensive approach to designing, planning, implementing, and governing enterprise IT architecture. It includes the ADM methodology, content framework, and various reference models.

**Q2: What are the four architecture domains in TOGAF?**
> 1. Business Architecture
> 2. Data Architecture
> 3. Application Architecture
> 4. Technology Architecture

**Q3: What is ADM?**
> The Architecture Development Method is TOGAF's core - a step-by-step, iterative approach to developing enterprise architecture. It consists of a Preliminary Phase plus phases A through H, with Requirements Management at the center.

**Q4: What happens in the Preliminary Phase?**
> The organization prepares for TOGAF adoption by:
> - Defining the enterprise scope
> - Establishing architecture principles
> - Selecting/tailoring the framework
> - Setting up the Architecture Repository
> - Defining governance structures

**Q5: What is the difference between ABB and SBB?**
> - **ABB (Architecture Building Block)**: Defines WHAT functionality is required; technology-agnostic
> - **SBB (Solution Building Block)**: Defines HOW the functionality is implemented; product/vendor-specific

### Intermediate Level Questions

**Q6: Explain the Enterprise Continuum.**
> The Enterprise Continuum is a view of the Architecture Repository showing evolution from generic to organization-specific architectures. It includes:
> - Foundation Architectures (most generic)
> - Common Systems Architectures
> - Industry Architectures
> - Organization-Specific Architectures (most specific)
>
> It helps organizations leverage existing assets and accelerate architecture development.
┌─────────────────────────────────────────────────────────────────────────┐
│                 ENTERPRISE CONTINUUM FLOW                               │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│   GENERIC                                              SPECIFIC         │
│   (Reusable everywhere)                    (Only for your org)         │
│                                                                         │
│   ┌──────────────┐   ┌──────────────┐   ┌──────────────┐   ┌──────────┐│
│   │  Foundation  │ → │   Common     │ → │   Industry   │ → │   Org    ││
│   │ Architecture │   │   Systems    │   │ Architecture │   │ Specific ││
│   └──────────────┘   └──────────────┘   └──────────────┘   └──────────┘│
│                                                                         │
│   Most Generic                                        Most Specific    │
│   (TRM, standards)                                    (Your systems)   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
┌──────────────────────────────────────────────────────────────────────────────┐
│                    ENTERPRISE CONTINUUM LEVELS                               │
├────────────────────┬─────────────────────────────────────────────────────────┤
│ LEVEL              │ DESCRIPTION & EXAMPLES                                  │
├────────────────────┼─────────────────────────────────────────────────────────┤
│                    │                                                         │
│ FOUNDATION         │ Universal standards, applicable to ANY organization    │
│ ARCHITECTURES      │                                                         │
│ (Most Generic)     │ Examples:                                               │
│                    │ • TOGAF Technical Reference Model (TRM)                 │
│                    │ • Operating systems, networking, databases              │
│                    │ • TCP/IP, HTTP, SQL standards                           │
│                    │ • Basic security models                                 │
├────────────────────┼─────────────────────────────────────────────────────────┤
│                    │                                                         │
│ COMMON SYSTEMS     │ Architectures for common business functions            │
│ ARCHITECTURES      │                                                         │
│                    │ Examples:                                               │
│                    │ • ERP architecture patterns                             │
│                    │ • CRM system patterns                                   │
│                    │ • E-commerce patterns                                   │
│                    │ • Data warehouse patterns                               │
│                    │ • Identity & access management                          │
├────────────────────┼─────────────────────────────────────────────────────────┤
│                    │                                                         │
│ INDUSTRY           │ Specific to an industry vertical                       │
│ ARCHITECTURES      │                                                         │
│                    │ Examples:                                               │
│                    │ • Banking: Core banking, payment systems                │
│                    │ • Gaming: Player management, RNG, bonus engines         │
│                    │ • Healthcare: HL7, FHIR standards                       │
│                    │ • Retail: POS systems, inventory management             │
│                    │ • Telecom: Billing, network management                  │
├────────────────────┼─────────────────────────────────────────────────────────┤
│                    │                                                         │
│ ORGANIZATION-      │ Your company's specific implementations                │
│ SPECIFIC           │                                                         │
│ (Most Specific)    │ Examples:                                               │
│                    │ • Your custom player platform                           │
│                    │ • Your specific payment gateway integration             │
│                    │ • Your data lake architecture                           │
│                    │ • Your microservices for your business                  │
│                    │                                                         │
└────────────────────┴─────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────────────┐
│                    BENEFITS                                             │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  1. REUSE                                                              │
│     └── Don't reinvent the wheel - use existing patterns               │
│                                                                         │
│  2. ACCELERATE                                                         │
│     └── Start from industry patterns, customize for your org           │
│                                                                         │
│  3. CONSISTENCY                                                        │
│     └── Common vocabulary across organization                          │
│                                                                         │
│  4. LEVERAGE                                                           │
│     └── Learn from industry best practices                             │
│                                                                         │
│  5. CLASSIFY                                                           │
│     └── Organize architecture assets systematically                    │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

**Q7: What is the purpose of Phase E (Opportunities and Solutions)?**
> Phase E identifies work packages and projects to transform from baseline to target architecture. It:
> - Consolidates gaps across architecture domains
> - Groups changes into work packages
> - Identifies transition architectures
> - Assesses dependencies and priorities
> - Creates initial implementation strategy

**Q8: How does Requirements Management work in TOGAF?**
> Requirements Management is a continuous process operating at the center of the ADM. It:
> - Captures requirements throughout all phases
> - Manages the Requirements Repository
> - Handles requirement changes
> - Ensures requirements are addressed in appropriate phases
> - Maintains traceability

**Q9: What is Architecture Governance?**
> Architecture Governance is a framework for managing and controlling enterprise architecture at all levels. Key components include:
> - Architecture Board (governing body)
> - Architecture Compliance reviews
> - Architecture Contracts (agreements between teams)
> - Dispensations (approved deviations from standards)

**Q10: Explain the concept of Transition Architectures.**
> Transition Architectures are intermediate states between the Baseline and Target Architecture. They:
> - Provide incremental business value
> - Reduce implementation risk
> - Allow gradual transformation
> - Are defined in Phase E and refined in Phase F

### Advanced Level Questions

**Q11: How do you handle a situation where business requirements conflict with technical constraints?**
> 1. Document both perspectives clearly
> 2. Engage stakeholders from both sides
> 3. Analyze trade-offs using impact assessment
> 4. Consider transition architectures as compromise
> 5. Escalate to Architecture Board if needed
> 6. Document decisions and rationale
> 7. Update Architecture Principles if necessary

**Q12: How would you adapt ADM for Agile environments?**
> - Use iterative cycles aligned with sprints
> - Focus on "just enough" architecture
> - Prioritize Architecture Runway
> - Integrate with frameworks like SAFe
> - Use lightweight documentation
> - Continuous stakeholder engagement
> - Adapt Phase G for continuous delivery
> - Implement architecture as code where possible

**Q13: How do you measure architecture effectiveness?**
> - Time-to-market for new capabilities
> - Reuse of architecture assets
> - Compliance rates with standards
> - Technical debt reduction
> - Business agility improvements
> - Cost savings from standardization
> - Stakeholder satisfaction scores
> - Architecture maturity assessments

**Q14: Describe how you would handle a merger/acquisition from an EA perspective.**
> 1. **Phase A**: Reassess Architecture Vision for combined entity
> 2. **Phase B**: Analyze and merge business processes
> 3. **Phase C**: Assess data integration and application rationalization
> 4. **Phase D**: Consolidate infrastructure and platforms
> 5. **Phase E/F**: Plan integration roadmap with quick wins
> 6. Key considerations:
>    - Cultural alignment
>    - Data migration and quality
>    - Regulatory compliance
>    - Customer impact minimization

**Q15: What's the relationship between TOGAF and other frameworks?**
> - **COBIT**: Complements TOGAF for IT governance
> - **ITIL**: Aligned for service management
> - **Zachman**: Can use as taxonomy within TOGAF
> - **SAFe**: Integrates for Agile at scale
> - **ArchiMate**: Modeling language that complements TOGAF
> - **BPMN**: For business process modeling in Phase B

### Scenario-Based Questions

**Q16: Your organization wants to move to cloud. How would you approach this using TOGAF?**
> 1. **Preliminary**: Define cloud principles and standards
> 2. **Phase A**: Create Cloud Migration Vision, identify stakeholders
> 3. **Phase B**: Identify business processes impacted
> 4. **Phase C**: Assess applications for cloud readiness (6 Rs: Rehost, Replatform, Repurchase, Refactor, Retain, Retire)
> 5. **Phase D**: Design target cloud infrastructure
> 6. **Phase E**: Identify migration waves and dependencies
> 7. **Phase F**: Create detailed migration plan
> 8. **Phase G**: Govern implementation, ensure security compliance
> 9. **Phase H**: Establish cloud operations and optimization

**Q17: How do you handle resistance to enterprise architecture?**
> - Demonstrate business value with quick wins
> - Speak in business language, not technical jargon
> - Involve stakeholders early in the process
> - Show how EA enables rather than constrains
> - Provide training and awareness programs
> - Get executive sponsorship
> - Start small and scale successes
> - Measure and communicate benefits

---

## Study Tips <a name="study-tips"></a>

### For TOGAF Certification

**TOGAF 9.2 Certification Paths**:
1. **TOGAF 9 Foundation (Level 1)**: Basic understanding - 40 multiple choice questions
2. **TOGAF 9 Certified (Level 2)**: Applied knowledge - 8 scenario-based questions
3. **TOGAF 9 Certified (Combined)**: Both exams taken together

### Study Recommendations

1. **Read the Official TOGAF Standard**
   - Available free from The Open Group website
   - Focus on ADM, Content Framework, and Governance

2. **Practice with Sample Questions**
   - Official practice exams from The Open Group
   - Multiple choice format for Part 1
   - Scenario-based for Part 2

3. **Memorize Key Terms**
   - ADM phases and their objectives
   - Building blocks (ABB vs SBB)
   - Deliverables vs Artifacts
   - Governance components

4. **Understand, Don't Just Memorize**
   - Know WHY each phase exists
   - Understand relationships between phases
   - Be able to apply concepts to scenarios

5. **Create Mind Maps**
   - Visual representations help retention
   - Map relationships between concepts

### Key Areas to Focus

| Area | Weight in Exam |
|------|----------------|
| ADM Phases | High |
| Architecture Content | High |
| Enterprise Continuum | Medium |
| Architecture Governance | Medium |
| Architecture Capability | Medium |
| Reference Models | Low |

### Common Mistakes to Avoid

❌ Confusing phases (especially B, C, D)
❌ Mixing up deliverables and artifacts
❌ Forgetting Requirements Management is continuous
❌ Not understanding iteration in ADM
❌ Ignoring stakeholder concerns
❌ Over-engineering solutions

### Quick Reference - ADM Phase Outputs

| Phase | Primary Output |
|-------|---------------|
| Preliminary | Organizational Model, Principles |
| A | Architecture Vision, SOW |
| B | Business Architecture |
| C | Data & Application Architecture |
| D | Technology Architecture |
| E | Implementation Strategy |
| F | Migration Plan |
| G | Compliance Assessments |
| H | Change Requests |

---

## Additional Resources

- [The Open Group - TOGAF Official Site](https://www.opengroup.org/togaf)
- [TOGAF 9.2 Standard (free access)](https://pubs.opengroup.org/architecture/togaf9-doc/)
- [ArchiMate Specification](https://pubs.opengroup.org/architecture/archimate3-doc/)
- [Enterprise Architecture Books]:
  - "TOGAF 9 Foundation Study Guide" by Rachel Harrison
  - "Enterprise Architecture as Strategy" by Ross, Weill, Robertson
  - "A Pocket Guide to TOGAF 9.2" by Andrew Josey

---

*Good luck with your TOGAF interview! Remember: Enterprise Architecture is about business value, not just technology.*

