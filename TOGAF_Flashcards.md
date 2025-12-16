# TOGAF 9.2 Interview Flashcards

> Based on TOGAF 9.2 (April 2018) - Use these for quick self-testing before your interview!

---

## Section 1: Fundamentals

### Card 1
**Q: What does TOGAF stand for?**

<details>
<summary>Answer</summary>

**The Open Group Architecture Framework**

It's an enterprise architecture framework for designing, planning, implementing, and governing enterprise IT architecture.
</details>

---

### Card 2
**Q: What are the four architecture domains in TOGAF?**

<details>
<summary>Answer</summary>

1. **Business Architecture** - Strategy, governance, organization, processes
2. **Data Architecture** - Logical and physical data assets
3. **Application Architecture** - Application blueprint and interactions
4. **Technology Architecture** - Hardware and software capabilities
</details>

---

### Card 3
**Q: What is ADM?**

<details>
<summary>Answer</summary>

**Architecture Development Method** - The core of TOGAF.

A step-by-step, iterative approach for developing enterprise architecture consisting of:
- Preliminary Phase
- Phases A through H
- Requirements Management (continuous, central)
</details>

---

### Card 4
**Q: Name all ADM phases in order.**

<details>
<summary>Answer</summary>

1. **Preliminary** - Prepare organization
2. **A** - Architecture Vision
3. **B** - Business Architecture
4. **C** - Information Systems Architecture (Data + Application)
5. **D** - Technology Architecture
6. **E** - Opportunities and Solutions
7. **F** - Migration Planning
8. **G** - Implementation Governance
9. **H** - Architecture Change Management

Plus: **Requirements Management** (continuous)
</details>

---

## Section 2: ADM Phases

### Card 5
**Q: What is the purpose of the Preliminary Phase?**

<details>
<summary>Answer</summary>

**Prepare the organization for TOGAF architecture projects**

Key activities:
- Define architecture capability
- Establish architecture principles
- Select and tailor frameworks
- Set up Architecture Repository
- Establish governance structures
</details>

---

### Card 6
**Q: What happens in Phase A: Architecture Vision?**

<details>
<summary>Answer</summary>

**Create a high-level vision of capabilities and business value**

Key activities:
- Identify stakeholders and their concerns
- Create Architecture Vision document
- Develop Statement of Architecture Work
- Obtain approval to proceed
</details>

---

### Card 7
**Q: What is Phase C responsible for?**

<details>
<summary>Answer</summary>

**Information Systems Architecture** - It has TWO parts:

1. **Data Architecture** - Logical and physical data models
2. **Application Architecture** - Application systems and interactions

Both require baseline → target → gap analysis
</details>

---

### Card 8
**Q: What's the difference between Phase E and Phase F?**

<details>
<summary>Answer</summary>

**Phase E (Opportunities & Solutions)**:
- Initial/high-level implementation strategy
- Identifies work packages
- Creates transition architectures

**Phase F (Migration Planning)**:
- Detailed implementation plan
- Finalizes roadmap
- Business case and prioritization
</details>

---

### Card 9
**Q: What is Phase G about?**

<details>
<summary>Answer</summary>

**Implementation Governance**

Provides architectural oversight during implementation:
- Ensure conformance to target architecture
- Perform compliance reviews
- Manage Architecture Contracts
- NOT about doing the implementation itself
</details>

---

### Card 10
**Q: When does Requirements Management happen?**

<details>
<summary>Answer</summary>

**Continuously throughout ALL phases** (it's at the center of ADM)

Key functions:
- Identify and store requirements
- Handle requirement changes
- Ensure traceability
- Feed requirements to appropriate phases
</details>

---

## Section 3: Building Blocks & Content

### Card 11
**Q: What is an Architecture Building Block (ABB)?**

<details>
<summary>Answer</summary>

**Defines WHAT functionality is required**

Characteristics:
- Technology-agnostic
- High-level abstraction
- Captures architecture requirements
- Guides development of SBBs

Example: "Customer Management Capability"
</details>

---

### Card 12
**Q: What is a Solution Building Block (SBB)?**

<details>
<summary>Answer</summary>

**Defines HOW functionality is implemented**

Characteristics:
- Product/vendor-specific
- Detailed level
- Implementation-focused
- May be purchased, built, or reused

Example: "Salesforce CRM Platform"
</details>

---

### Card 13
**Q: What's the difference between Deliverables and Artifacts?**

<details>
<summary>Answer</summary>

**Deliverables**:
- Contractually specified work products
- Formally reviewed and signed off
- Example: Architecture Definition Document

**Artifacts**:
- Architectural work products that describe architecture
- Types: Catalogs, Matrices, Diagrams
- Example: Process flow diagram, CRUD matrix
</details>

---

### Card 14
**Q: What are the three types of artifacts?**

<details>
<summary>Answer</summary>

1. **Catalogs** - Lists of things (e.g., Application Catalog)
2. **Matrices** - Relationships between things (e.g., App/Data Matrix)
3. **Diagrams** - Visual representations (e.g., Business Process Diagram)
</details>

---

## Section 4: Enterprise Continuum

### Card 15
**Q: What is the Enterprise Continuum?**

<details>
<summary>Answer</summary>

**A view of the Architecture Repository** showing evolution of architecture from generic to organization-specific.

The spectrum:
```
Foundation → Common Systems → Industry → Organization
(Generic)                                  (Specific)
```

Contains both Architecture Continuum and Solutions Continuum.
</details>

---

### Card 16
**Q: What is the Standards Information Base (SIB)?**

<details>
<summary>Answer</summary>

**A repository of standards** that the organization has adopted or created for architecture work.

Includes:
- Industry standards
- Technology standards
- Organization-specific standards
- Legal/regulatory requirements
</details>

---

## Section 5: Governance & Views

### Card 17
**Q: What is Architecture Governance?**

<details>
<summary>Answer</summary>

**A framework for managing and controlling enterprise architecture**

Key components:
- Architecture Board (governing body)
- Architecture Compliance reviews
- Architecture Contracts
- Dispensations (approved deviations)
</details>

---

### Card 18
**Q: What is an Architecture Contract?**

<details>
<summary>Answer</summary>

**A joint agreement** between development partners and sponsors on:
- Deliverables
- Quality
- Fitness-for-purpose of architecture

Used in Phase G to govern implementation projects.
</details>

---

### Card 19
**Q: What is a Dispensation in TOGAF?**

<details>
<summary>Answer</summary>

**An approved deviation from architecture standards**

Used when:
- Full compliance isn't possible
- Business need requires exception
- Time-limited deviation needed

Must be formally documented and approved by Architecture Board.
</details>

---

### Card 20
**Q: Explain View vs Viewpoint**

<details>
<summary>Answer</summary>

**View**: A representation of a system from the perspective of a specific stakeholder or stakeholder concern.

**Viewpoint**: The definition or template that describes how a view is constructed. It specifies what to include and how to present it.

Think: Viewpoint is the "recipe", View is the "dish"
</details>

---

## Section 6: Architecture Principles

### Card 21
**Q: What are the components of an Architecture Principle?**

<details>
<summary>Answer</summary>

Four components:

1. **Name** - Short identifier
2. **Statement** - What the principle is
3. **Rationale** - Why it's important
4. **Implications** - What it means in practice
</details>

---

### Card 22
**Q: Give an example of a business architecture principle.**

<details>
<summary>Answer</summary>

**Name**: Primacy of Principles

**Statement**: These principles apply to all organizations within the enterprise.

**Rationale**: Ensures consistent decision-making and resource allocation across the organization.

**Implications**: All projects must comply. Exceptions require formal approval.
</details>

---

## Section 7: Scenario Questions

### Card 23
**Q: Your organization is planning cloud migration. Which ADM phases are most critical?**

<details>
<summary>Answer</summary>

All phases are involved, but emphasis on:

- **Phase C**: Assess applications for cloud readiness (6 Rs analysis)
- **Phase D**: Design cloud infrastructure architecture
- **Phase E**: Identify migration waves, transition architectures
- **Phase F**: Detailed migration planning
- **Phase G**: Ensure security and compliance during migration
</details>

---

### Card 24
**Q: How do you handle stakeholder resistance to EA?**

<details>
<summary>Answer</summary>

Strategies:
1. Demonstrate value with quick wins
2. Speak in business language
3. Involve stakeholders early
4. Show EA as enabler, not constraint
5. Get executive sponsorship
6. Provide training/awareness
7. Start small, scale success
8. Measure and communicate benefits
</details>

---

### Card 25
**Q: How would you adapt TOGAF for Agile environments?**

<details>
<summary>Answer</summary>

Adaptations:
- Shorter iteration cycles
- "Just enough" architecture
- Continuous stakeholder engagement
- Lightweight documentation
- Integrate with SAFe or similar
- Architecture as code
- Focus on Architecture Runway
- Continuous delivery in Phase G
</details>

---

## Section 8: TOGAF 9.2 Specifics

### Card 26
**Q: What's new in TOGAF 9.2 compared to 9.1?**

<details>
<summary>Answer</summary>

Key updates in TOGAF 9.2:
- Improved structure and navigation
- Better alignment with other Open Group standards
- Enhanced Business Architecture content
- Clarified terminology and definitions
- Updated Architecture Content Framework
- Improved guidance on security architecture
- Better integration with ArchiMate
</details>

---

### Card 27
**Q: What are the TOGAF 9.2 certification levels?**

<details>
<summary>Answer</summary>

**Two certification levels**:

1. **TOGAF 9 Foundation (Level 1)**
   - 40 multiple choice questions
   - 60 minutes, 55% pass mark
   - Tests basic knowledge

2. **TOGAF 9 Certified (Level 2)**
   - 8 scenario-based questions
   - 90 minutes, 60% pass mark
   - Tests applied knowledge
</details>

---

## Section 9: Related Frameworks

### Card 28
**Q: How does ArchiMate relate to TOGAF?**

<details>
<summary>Answer</summary>

**ArchiMate** is a modeling language that complements TOGAF:

- Provides visual notation for architecture
- Covers Business, Application, Technology layers
- Open standard from The Open Group
- Used to create diagrams and views in TOGAF
- Not required, but commonly used together
</details>

---

### Card 29
**Q: How does TOGAF relate to COBIT?**

<details>
<summary>Answer</summary>

**COBIT** (Control Objectives for Information Technologies):

- Focuses on IT governance and management
- Complements TOGAF for governance aspects
- TOGAF provides architecture framework
- COBIT provides control/governance framework
- Often used together in enterprises
</details>

---

### Card 30
**Q: What is Zachman Framework and how does it relate to TOGAF?**

<details>
<summary>Answer</summary>

**Zachman Framework**:
- A taxonomy for organizing architecture artifacts
- Uses a 6x6 matrix (What, How, Where, Who, When, Why)
- Doesn't provide methodology (unlike TOGAF's ADM)

Relationship:
- Can be used as classification scheme within TOGAF
- TOGAF provides process, Zachman provides taxonomy
- Complementary, not competing
</details>

---

## Quick Self-Test

Try to answer these without looking:

1. What are the four architecture domains?
2. Name the ADM phases in order
3. What's the difference between ABB and SBB?
4. What happens in Phase E vs Phase F?
5. What are the components of an architecture principle?
6. When does Requirements Management occur?
7. What is the Enterprise Continuum?
8. What is an Architecture Contract?

---

*Score yourself: 8/8 = Ready! | 6-7 = Almost there | <6 = Review the guide again*

