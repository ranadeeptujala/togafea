# Stakeholder Conflict Resolution - EA Scenarios

> **Purpose**: Document real-world conflict resolution scenarios for Enterprise Architects

---

## Scenario: Technology Choice Conflict

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                    CONFLICT SCENARIO: Technology Choice                          │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│   PROJECT: New Customer Onboarding System for Gaming Platform                   │
│   STAKEHOLDER: Head of Operations (Business)                                    │
│   MY ROLE: Enterprise Architect                                                 │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

---

## The Conflict

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                    THE PROBLEM                                                   │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│   BUSINESS STAKEHOLDER WANTED:                                                  │
│   ════════════════════════════                                                  │
│   "Buy a ready-made vendor solution (Salesforce) for customer onboarding"       │
│                                                                                  │
│   Their reasoning:                                                              │
│   • Faster time to market (2 months)                                            │
│   • Proven solution, less risk                                                  │
│   • Vendor support available                                                    │
│   • "I've used it before at my previous company"                                │
│                                                                                  │
│   ─────────────────────────────────────────────────────────────────────────     │
│                                                                                  │
│   ARCHITECTURE RECOMMENDATION:                                                  │
│   ════════════════════════════                                                  │
│   "Build a custom microservice integrated with existing platform"               │
│                                                                                  │
│   Our reasoning:                                                                │
│   • Better integration with existing gaming platform                            │
│   • No vendor lock-in                                                           │
│   • Lower long-term cost                                                        │
│   • Aligned with architecture principles                                        │
│                                                                                  │
│   ─────────────────────────────────────────────────────────────────────────     │
│                                                                                  │
│   THE CONFLICT:                                                                 │
│   "Business wants to BUY, Architecture wants to BUILD"                          │
│                                                                                  │
│   Stakeholder was frustrated:                                                   │
│   "You architects always want to build everything! You're blocking my project!" │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

---

## Resolution Approach

### Step 1: LISTEN First

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│  STEP 1: LISTEN & UNDERSTAND                                                     │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  Instead of defending architecture position, I asked:                           │
│                                                                                  │
│  • "Help me understand - what's driving the urgency?"                           │
│  • "What specific features are most important to you?"                          │
│  • "What concerns do you have with building custom?"                            │
│  • "Tell me about your experience with Salesforce before"                       │
│                                                                                  │
│  WHAT I LEARNED:                                                                │
│  • Marketing campaign launching in 3 months (hard deadline)                     │
│  • KYC verification was the critical feature                                    │
│  • Previous company had good Salesforce experience                              │
│  • Fear that custom build would be delayed (past experience)                    │
│                                                                                  │
│  KEY INSIGHT:                                                                   │
│  The REAL concern was TIME and RISK, not Salesforce specifically                │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

### Step 2: ACKNOWLEDGE Concerns

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│  STEP 2: ACKNOWLEDGE (Don't Dismiss)                                             │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  What I said:                                                                   │
│                                                                                  │
│  "You're absolutely right that:                                                 │
│   • Time to market is critical for business success                             │
│   • Vendor solutions reduce implementation risk                                 │
│   • Past custom builds have had delays                                          │
│   • Your experience with Salesforce is valuable"                                │
│                                                                                  │
│  "These are valid concerns and I want to address them, not dismiss them"        │
│                                                                                  │
│  WHY THIS MATTERS:                                                              │
│  • Stakeholder felt HEARD, not blocked                                          │
│  • Reduced defensive posture                                                    │
│  • Opened dialog for collaboration                                              │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

### Step 3: PRESENT Data

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│  STEP 3: PRESENT DATA & ANALYSIS                                                 │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  I prepared a comparison (shared in next meeting):                              │
│                                                                                  │
│  ┌─────────────────────┬─────────────────────┬─────────────────────┐            │
│  │ Criteria            │ Salesforce (Buy)    │ Custom Build        │            │
│  ├─────────────────────┼─────────────────────┼─────────────────────┤            │
│  │ Time to MVP         │ 2 months            │ 3 months            │            │
│  │ Integration effort  │ 4 months additional │ Included            │            │
│  │ Year 1 Cost         │ $500K (license+impl)│ $300K               │            │
│  │ Year 2-5 Cost       │ $200K/year license  │ $50K/year maint     │            │
│  │ 5-Year Total Cost   │ $1.3M               │ $500K               │            │
│  │ Integration risk    │ HIGH (different tech)│ LOW (same stack)   │            │
│  │ Vendor lock-in      │ YES                 │ NO                  │            │
│  │ Gaming-specific KYC │ Customization needed│ Built for us        │            │
│  └─────────────────────┴─────────────────────┴─────────────────────┘            │
│                                                                                  │
│  KEY FINDING:                                                                   │
│  Salesforce MVP = 2 months, BUT integration with gaming platform = 4 more months│
│  TOTAL time with Salesforce = 6 months (LONGER than custom!)                    │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

### Step 4: FIND Common Ground

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│  STEP 4: PROPOSE COMPROMISE                                                      │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  My proposal addressed THEIR concerns:                                          │
│                                                                                  │
│  "What if we do this:                                                           │
│                                                                                  │
│   1. BUILD custom onboarding service (3 months)                                 │
│      BUT use a 3RD PARTY KYC vendor (Jumio) for verification                    │
│      → Addresses time concern (proven KYC component)                            │
│                                                                                  │
│   2. PHASE 1: Core onboarding + Jumio KYC (3 months) ✓ Meets deadline           │
│      PHASE 2: Advanced features (2 months later)                                │
│      → Addresses risk concern (smaller scope first)                             │
│                                                                                  │
│   3. Weekly demos to business stakeholders                                      │
│      → Addresses visibility concern (no surprises)                              │
│                                                                                  │
│   4. Architecture team commits to 3-month deadline with penalty clause          │
│      → Addresses trust concern (skin in the game)"                              │
│                                                                                  │
│  COMPROMISE:                                                                    │
│  • Business gets: Speed, proven KYC, visibility, commitment                     │
│  • Architecture gets: Custom build, no vendor lock-in, platform alignment       │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

### Step 5: DOCUMENT Agreement

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│  STEP 5: DOCUMENT & COMMIT                                                       │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  Created ADR (Architecture Decision Record):                                    │
│                                                                                  │
│  ADR-015: Customer Onboarding Approach                                          │
│  ─────────────────────────────────────                                          │
│  Decision: Build custom service with Jumio KYC integration                      │
│                                                                                  │
│  Options Considered:                                                            │
│  - Salesforce (rejected - integration time, cost)                               │
│  - Full custom (rejected - KYC complexity)                                      │
│  - Hybrid: Custom + Jumio (SELECTED)                                            │
│                                                                                  │
│  Stakeholders: Head of Operations (agreed), CTO (approved)                      │
│                                                                                  │
│  Commitments:                                                                   │
│  - Phase 1 delivery: 3 months                                                   │
│  - Weekly demos every Friday                                                    │
│  - Go/No-Go checkpoint at week 6                                                │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

---

## The Outcome

```
┌──────────────────────────────────────────────────────────────────────────────────┐
│                    OUTCOME                                                       │
├──────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  RESULT:                                                                        │
│  ✅ Delivered Phase 1 in 2.5 months (ahead of schedule!)                        │
│  ✅ Marketing campaign launched on time                                         │
│  ✅ 5-year cost savings: $800K vs Salesforce                                    │
│  ✅ Seamless integration with gaming platform                                   │
│  ✅ Stakeholder became architecture advocate                                    │
│                                                                                  │
│  RELATIONSHIP:                                                                  │
│  • Head of Operations became ally, not adversary                                │
│  • Now consults architecture early on new initiatives                           │
│  • Trusts architecture recommendations                                          │
│                                                                                  │
│  LESSON LEARNED:                                                                │
│  "The conflict was never about Salesforce vs Custom.                            │
│   It was about TRUST, TIME, and RISK.                                           │
│   Address the REAL concerns, not the surface argument."                         │
│                                                                                  │
└──────────────────────────────────────────────────────────────────────────────────┘
```

---

## Conflict Resolution Framework

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    5-STEP CONFLICT RESOLUTION FRAMEWORK                          │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  1. LISTEN FIRST      - Understand their perspective, ask questions             │
│                                                                                  │
│  2. ACKNOWLEDGE       - Validate their concerns (don't dismiss)                 │
│                                                                                  │
│  3. PRESENT DATA      - Facts, not opinions; show analysis                      │
│                                                                                  │
│  4. FIND COMMON GROUND- Compromise that addresses both sides                    │
│                                                                                  │
│  5. DOCUMENT          - ADR, commitments, checkpoints                           │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Communication Tips

| NEVER SAY | INSTEAD SAY |
|-----------|-------------|
| "You're wrong" | "Help me understand..." |
| "Architecture says no" | "Let's look at the options together" |
| "That won't work" | "What if we tried..." |
| "We always build custom" | "What's most important to you?" |
| "That's not how we do things" | "Let me share our approach and get your input" |

---

## Key Takeaways

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                    KEY TAKEAWAYS                                                 │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                  │
│  • Stakeholders aren't enemies - they have valid business concerns              │
│                                                                                  │
│  • Architecture serves business, not the other way around                       │
│                                                                                  │
│  • Win-win solutions build long-term trust                                      │
│                                                                                  │
│  • Address the REAL concerns (often hidden), not surface arguments              │
│                                                                                  │
│  • Data beats opinions in resolving conflicts                                   │
│                                                                                  │
│  • Document agreements to prevent future misunderstandings                      │
│                                                                                  │
│  • Follow through on commitments to build credibility                           │
│                                                                                  │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## Interview Answer Template

When asked about stakeholder conflicts in interviews, structure your answer using **STAR**:

**Situation**: "In my previous role, we had a conflict about technology choice for a new onboarding system..."

**Task**: "As the Enterprise Architect, I needed to resolve this while maintaining platform alignment..."

**Action**: "I followed a 5-step approach: Listen, Acknowledge, Present Data, Find Common Ground, Document..."

**Result**: "We delivered ahead of schedule, saved $800K over 5 years, and the stakeholder became an architecture advocate..."
