# ⚙️ CHAPTER 7: STRUCTURED SYSTEM ANALYSIS & SDLC
### MBA MIS Revision Notes | Exam-Ready

---

> [!IMPORTANT]
> **Top Exam Topics:** SDLC phases (always asked!), DFD symbols and levels, SDL Models comparison (Waterfall vs Spiral vs Agile). Diagrams + definitions = full marks!

---

## 🎯 LEARNING OBJECTIVES

After this chapter, you should be able to:
- Explain **Structured System Analysis** and its purpose
- Describe key **Structured Analysis Tools** (DFD, ERD, Data Dictionary)
- Distinguish between **Logical and Physical System Design**
- List and explain all **SDLC phases**
- Compare all major **SDL Models**

---

## 1. 📖 INTRODUCTION

### Why Systems Analysis?

> Before building any IS, you must deeply **understand the existing system** and **define what the new system must do**. This is **Systems Analysis** — the diagnostic phase of IS development.

> **Analogy:** Like a doctor diagnosing before prescribing — you can't build the right IS without first understanding the problem!

```
Problem / Opportunity Identified
         ↓
SYSTEMS ANALYSIS (Understand WHAT is needed)
         ↓
SYSTEM DESIGN (Decide HOW to build it)
         ↓
SYSTEM DEVELOPMENT (Actually build it)
         ↓
IMPLEMENTATION & MAINTENANCE
```

---

## 2. 🔍 STRUCTURED SYSTEM ANALYSIS (SSA)

### Definition:

> **Structured System Analysis** is a **systematic, disciplined approach** to analyzing an existing system or defining requirements for a new system using **graphical tools and structured techniques** — before any programming begins.

> Key word: **"Structured"** = disciplined, top-down, graphical, documented approach

### Goals of Structured System Analysis:

> **Mnemonic: "PURR"**
> - **P**roblem understanding — fully grasp existing system
> - **U**ser requirements — capture what users need
> - **R**equirements documentation — formally document findings
> - **R**ecommendation — propose feasible solution

### Steps in Structured System Analysis:

> **Mnemonic: "SCRIP"**
> 1. **S**tudy the current system (understand existing processes)
> 2. **C**ollect requirements (interviews, observations, questionnaires)
> 3. **R**equirements analysis (what must new system do?)
> 4. **I**dentify problems and opportunities in current system
> 5. **P**repare System Requirement Specification (SRS) document

### Key Outputs of Systems Analysis:
- **Feasibility Study Report** — Is the proposed system viable?
- **System Requirements Specification (SRS)** — What the system must do
- **Data Flow Diagrams (DFDs)** — How data flows through the system
- **Entity Relationship Diagrams (ERDs)** — Data structure

---

### Feasibility Study — TELOS Framework:

> **Mnemonic: "TELOS"**
> - **T**echnical Feasibility — Does technology exist to build it?
> - **E**conomic Feasibility — Is it cost-beneficial? (ROI positive?)
> - **L**egal Feasibility — Does it comply with laws and regulations?
> - **O**perational Feasibility — Will users adopt and use it?
> - **S**chedule Feasibility — Can it be built in the required time?

| Feasibility Type | Key Question | Example |
|-----------------|-------------|---------|
| **Technical** | Do we have the technology? | Can our servers handle 10M users? |
| **Economic** | Cost < Benefit? | ₹50L investment → ₹2Cr savings over 5 years → Yes! |
| **Legal** | Is it allowed by law? | Does the IS comply with DPDPA 2023? |
| **Operational** | Will people use it? | Will 60-year-old branch managers accept a new ERP? |
| **Schedule** | Can it be done in time? | 6 months to build vs 18 months needed → Not feasible |

---

## 3. 🛠️ STRUCTURED SYSTEM ANALYSIS TOOLS

### Main Tools:

> **Mnemonic: "DED-FC"**
> - **D**ata Flow Diagram (DFD)
> - **E**ntity Relationship Diagram (ERD)
> - **D**ata Dictionary
> - **F**lowchart
> - **C**ase (Decision Table / Decision Tree)

---

### Tool 1: 📊 DATA FLOW DIAGRAM (DFD)

> **Definition:** A DFD is a **graphical representation of how data flows through a system** — showing inputs, outputs, processes, and data stores.

> DFD shows WHAT the system does (not how) — the **logical view** of the system.

### DFD Symbols (Yourdon-DeMarco Notation):

| Symbol | Shape | Represents |
|--------|-------|-----------|
| **External Entity** | Rectangle/Square | Source or destination of data (person, system, organization) |
| **Process** | Circle / Rounded Rectangle | Transforms or manipulates data |
| **Data Store** | Open Rectangle (two parallel lines) | Where data is stored (database, file) |
| **Data Flow** | Arrow (→) | Movement of data between components |

```
[Customer] ──Order──→ (Process Order) ──Order Details──→ =Order DB=
                              │
                         ──Invoice──→ [Customer]
```

### Levels of DFD:

| Level | Name | Description |
|-------|------|-------------|
| **Context Diagram (Level 0)** | Highest level | Shows the ENTIRE system as ONE process; shows all external entities and their connections |
| **Level 1 DFD** | First expansion | Breaks system into major sub-processes |
| **Level 2 DFD** | Second expansion | Breaks each Level 1 process into sub-processes |
| **Level N** | Progressive detail | Continue until processes are atomic (can't be broken further) |

**Example — Online Shopping System:**
```
Context (Level 0):
[Customer] ←→ (Online Shopping System) ←→ [Bank]
                                         ←→ [Warehouse]

Level 1:
[Customer] → (1.0 Browse Products) → =Product DB=
[Customer] → (2.0 Place Order) → =Order DB=
[Customer] → (3.0 Make Payment) → [Bank]
[Warehouse] ← (4.0 Fulfill Order) ← =Order DB=
```

### Rules for Drawing DFD:
1. Every process must have at least ONE input and ONE output
2. External entities cannot communicate directly — must go through a process
3. Data stores cannot communicate directly — must go through a process
4. Every data flow must be named
5. Processes must be numbered (1.0, 2.0 or 1.1, 1.2 for sub-processes)

---

### Tool 2: 📋 DATA DICTIONARY (DD)

> **Definition:** A **Data Dictionary** is a **repository of metadata** — it defines and documents all data elements, data structures, data flows, and data stores used in the system.

> "A dictionary for data" — tells you what every piece of data means, its format, and where it comes from/goes.

### What Data Dictionary Contains:

| Element | Description | Example |
|---------|-------------|---------|
| **Data Element** | Smallest unit of data | Customer_ID: Numeric, 8 digits, mandatory |
| **Data Structure** | Group of related data elements | Customer_Record = {Customer_ID + Name + Phone + Email} |
| **Data Flow** | Description of data movement | Order_Request: flows from Customer to Process_Order |
| **Data Store** | Description of stored data | Order_DB: stores all confirmed orders, updated by Process_Order |
| **Process** | Description of transformation | Process_Payment: validates card, deducts amount, confirms |

### Importance of Data Dictionary:
- **Single source of truth** for all data definitions
- Eliminates confusion when different teams use different terms
- Essential for system maintenance and future development

---

### Tool 3: 🗃️ ENTITY RELATIONSHIP DIAGRAM (ERD)

> **Definition:** ERD is a **graphical representation of entities (objects) and their relationships** in a system — used for database design.

### ERD Symbols:

| Symbol | Shape | Represents |
|--------|-------|-----------|
| **Entity** | Rectangle | Real-world object (Customer, Product, Order) |
| **Attribute** | Oval/Ellipse | Property of an entity (Customer_Name, Product_Price) |
| **Relationship** | Diamond | Association between entities (Customer PLACES Order) |
| **Cardinality** | Lines/Numbers | How many instances relate (1:1, 1:N, M:N) |

### Cardinality Types:

| Type | Meaning | Example |
|------|---------|---------|
| **1:1 (One-to-One)** | One entity relates to exactly one of another | One Employee has one Passport |
| **1:N (One-to-Many)** | One entity relates to many of another | One Customer places MANY Orders |
| **M:N (Many-to-Many)** | Many of one relate to many of another | Many Students enroll in Many Courses |

```
[Customer] ──places── <ORDER> ──contains── [Product]
  (1)         1:N        (N)     M:N          (M)
```

---

### Tool 4: 📈 FLOWCHART

> **Definition:** A Flowchart is a **graphical representation of the sequence of steps or decisions** in a process using standardized symbols.

### Common Flowchart Symbols:

| Symbol | Shape | Meaning |
|--------|-------|---------|
| **Start/End** | Oval/Rounded rectangle | Beginning or end of process |
| **Process** | Rectangle | A step or operation |
| **Decision** | Diamond | Yes/No branching point |
| **Input/Output** | Parallelogram | Data input or output |
| **Flow** | Arrow | Direction of process flow |
| **Connector** | Circle | Connect parts of flowchart |

**Example — Login Process:**
```
(Start) → [Enter Username & Password] → ◇ Valid? 
                                        YES → [Show Dashboard] → (End)
                                        NO → [Show Error] → [Enter again]
```

---

### Tool 5: 🌳 DECISION TREES & DECISION TABLES

#### Decision Tree:
> **Graphical representation of decisions and their possible consequences** — looks like a tree branching out.

```
Order Amount?
├── > ₹500 → Free Shipping
└── ≤ ₹500 → Shipping Cost?
              ├── Express → ₹100
              └── Standard → ₹40
```

#### Decision Table:
> **Tabular representation of conditions and corresponding actions** — useful for complex logic with multiple conditions.

| | Rule 1 | Rule 2 | Rule 3 | Rule 4 |
|-|--------|--------|--------|--------|
| **Amount > ₹500** | Y | Y | N | N |
| **Prime Member** | Y | N | Y | N |
| **Action: Free Shipping** | ✓ | ✓ | ✓ | ✗ |
| **Action: ₹40 Charge** | ✗ | ✗ | ✗ | ✓ |

---

## 4. 🏗️ SYSTEM DESIGN

### Definition:
> **System Design** = The process of **planning and specifying HOW the new system will be built** to satisfy the requirements identified in system analysis.

> Analysis says WHAT; Design says HOW.

### Two Levels of Design:

| | Logical Design | Physical Design |
|--|---------------|----------------|
| **Focus** | WHAT the system will do | HOW it will be technically implemented |
| **Technology** | Technology-independent | Technology-specific |
| **Output** | Logical DFD, ERD, process specs | Database schema, UI screens, code specs, hardware |
| **Who** | Systems analyst | System designer + programmer |
| **Example** | "System must store customer orders" | "Customer orders stored in MySQL table with fields: order_id INT, customer_id INT, date DATE..." |

### Components of System Design:

> **Mnemonic: "DIOPS"**
> - **D**atabase design (tables, relationships, indexes)
> - **I**nput design (forms, screens, UI)
> - **O**utput design (reports, dashboards)
> - **P**rocessing design (program logic, algorithms)
> - **S**ecurity design (access controls, encryption)

---

## 5. 🔄 SYSTEM DEVELOPMENT LIFE CYCLE (SDLC)

### Definition:
> **SDLC** = A structured process that defines the **phases involved in developing, maintaining, and replacing information systems**.

> It is the overall **framework** — specific models (Waterfall, Agile, etc.) are ways of executing this framework.

### SDLC Phases:

> **Mnemonic: "PADIME"** *(Padhai mein Dedication Inspires Mastery Every time!)*
> - **P**lanning
> - **A**nalysis
> - **D**esign
> - **I**mplementation
> - **M**aintenance/Testing
> - **E**valuation

---

### Phase-by-Phase Explanation:

#### Phase 1: 🔵 PLANNING (System Initiation)
- Define project **scope, objectives, timeline, budget**
- Conduct **feasibility study (TELOS)**
- Get management approval
- Form project team
- **Output:** Project Charter, Feasibility Report

#### Phase 2: 🟡 ANALYSIS (System Analysis)
- Study the **current system** in detail
- Gather **user requirements** (interviews, observations, surveys)
- Identify problems, opportunities, constraints
- Create DFDs, ERDs, Data Dictionary
- **Output:** System Requirements Specification (SRS)

#### Phase 3: 🟢 DESIGN (System Design)
- **Logical Design:** How the system will function (data flows, processes)
- **Physical Design:** Technical specifications (DB schema, UI mockups, hardware)
- Design input forms, output reports, database structure, security
- **Output:** Design Specification Document

#### Phase 4: 🟠 IMPLEMENTATION (Development)
- Write actual **code** based on design specifications
- **Database creation** and population
- **Unit testing** (individual modules tested)
- **Integration testing** (modules tested together)
- User training
- **Output:** Working IS system, test reports, user manuals

#### Phase 5: 🔴 TESTING & DEPLOYMENT
- **System Testing** — entire system tested against requirements
- **User Acceptance Testing (UAT)** — actual users test the system
- **Deployment strategies:**
  - **Direct Cutover** — Old system off, new system on (risky!)
  - **Parallel Running** — Both old and new run simultaneously
  - **Phased Conversion** — New system deployed in stages
  - **Pilot Conversion** — Deploy in one location first

#### Phase 6: 🟣 MAINTENANCE & EVALUATION
- Fix bugs discovered post-deployment (**corrective maintenance**)
- Add new features (**adaptive maintenance**)
- Improve performance (**perfective maintenance**)
- Evaluate if system meets original objectives
- **Types of Maintenance:**
  - **Corrective** — Fix bugs
  - **Adaptive** — Adapt to new environment (new OS, new law)
  - **Perfective** — Improve performance, add features
  - **Preventive** — Prevent future problems

---

### Deployment/Conversion Strategies Comparison:

| Strategy | How | Risk | Cost | Best For |
|----------|-----|------|------|---------|
| **Direct Cutover** | Switch off old, switch on new on Day 1 | Very High | Low | Small, non-critical systems |
| **Parallel Running** | Both old and new run simultaneously | Very Low | Very High | Critical systems (banking, hospitals) |
| **Phased Conversion** | Deploy module by module, location by location | Medium | Medium | Large geographically distributed systems |
| **Pilot Conversion** | Deploy in one branch/location first, then expand | Low-Medium | Medium | When risk needs to be minimized, national rollout |

---

## 6. 📐 SDL MODELS

> SDL Models are specific **methodologies** for executing the SDLC. Each has a different approach to organizing and sequencing the phases.

> **Mnemonic: "WISP-RAD"**
> - **W**aterfall
> - **I**ncremental
> - **S**piral
> - **P**rototype
> - **R**AD
> - **A**gile
> - **D**evOps (modern)

---

### Model 1: 🌊 WATERFALL MODEL (Classic SDLC)

> Linear, sequential — each phase must be fully completed before the next begins.

```
Planning → Analysis → Design → Implementation → Testing → Maintenance
  ↓            ↓         ↓           ↓              ↓           ↓
(Complete     (Complete  (Complete  (Complete     (Complete   (Ongoing)
 before        before    before     before        before
 Analysis)     Design)   Impl.)     Testing)      Maint.)
```

**Advantages:**
- Simple, easy to understand and manage
- Well-documented at each phase
- Works well for small, well-defined projects

**Disadvantages:**
- **Rigid** — very hard/expensive to go back and change
- **No working software** until late in the project
- **Users see system only at the end** — too late to fix fundamental issues
- Not suitable for complex or changing requirements

**When to use:** Small projects with clear, stable requirements.

---

### Model 2: 🔁 PROTOTYPE MODEL

> Build a quick working model (prototype), get user feedback, refine, repeat — until final system emerges.

```
Requirements → Quick Prototype → User Feedback → Refine → More Feedback → Final System
                    ↑___________________________|
                         (iteration loop)
```

**Advantages:**
- User involvement from the start
- Reduces misunderstanding between users and developers
- Flexible — incorporates changes easily

**Disadvantages:**
- **Scope creep** — users keep asking for more
- **Poor documentation** — focus on working prototype, not docs
- Developer may use quick-and-dirty code that becomes permanent

**When to use:** When requirements are unclear; user interface-heavy systems.

---

### Model 3: 🌀 SPIRAL MODEL

> Combines Waterfall's structure with Prototype's iteration + **adds RISK ANALYSIS** at each cycle.

```
Each Spiral = 4 Quadrants:
1. Planning (define objectives, alternatives)
2. Risk Analysis (identify and resolve risks)
3. Engineering (develop and test)
4. Evaluation (user review, plan next spiral)
```

**Key Feature:** **RISK ANALYSIS** at every cycle — most risk-conscious model.

**Advantages:**
- Excellent **risk management**
- User feedback at every cycle
- Works for **large, complex, high-risk projects**

**Disadvantages:**
- **Complex and expensive** to manage
- Requires **expertise in risk assessment**
- Not suitable for small/simple projects

**When to use:** Large, complex, high-risk projects (defense systems, aerospace, banking core systems).

---

### Model 4: 📈 INCREMENTAL MODEL

> Divide the system into **small increments/releases** — build and deliver core features first, then add more features in each release.

```
Release 1: Core Features (Minimal viable product)
Release 2: Core + Feature Set A
Release 3: Core + A + Feature Set B
Release 4: Full System
```

**Advantages:**
- **Working software delivered early** (after first increment)
- Users get value faster
- Risk spread across multiple small deliveries

**Disadvantages:**
- **Integration issues** — combining increments can be complex
- Needs good **architecture upfront** to accommodate future increments

**When to use:** When early partial delivery is valuable; large systems with phased needs.

---

### Model 5: ⚡ RAD — Rapid Application Development

> Emphasizes **speed** through parallel development teams, heavy user workshops, pre-built components, and timeboxed delivery.

```
Requirements Planning → User Design (JOINT sessions) → Construction → Cutover
(Short)                  (Workshops, rapid prototyping)  (Parallel teams) (Fast)
```

**Key Features:**
- **JRAD (Joint Application Development)** workshops
- Use of **CASE tools** and code generators
- **Parallel development** by multiple teams
- **Timeboxing** — fixed deadline, adjust scope to fit

**Advantages:** Very fast delivery, strong user involvement, reduced rework

**Disadvantages:** Requires highly skilled teams, difficult for large complex projects

**When to use:** When speed is priority and requirements are reasonably clear.

---

### Model 6: 🏃 AGILE MODEL

> Work in **short sprints (2-4 weeks)**, deliver working software every sprint, adapt to changing requirements continuously.

```
Sprint 1 (2 wks) → Sprint 2 (2 wks) → Sprint 3 (2 wks) → ... → Final Product
(User Story 1-5)   (User Story 6-10)   (User Story 11-15)
Each sprint = Plan → Build → Test → Review → Retrospect
```

**Core Principles (Agile Manifesto 2001):**
1. **Individuals and interactions** over processes and tools
2. **Working software** over comprehensive documentation
3. **Customer collaboration** over contract negotiation
4. **Responding to change** over following a plan

**Popular Agile Frameworks:**
- **Scrum** — Sprints, Daily standups, Sprint Review, Retrospective
- **Kanban** — Visual board, continuous flow, WIP limits
- **XP (Extreme Programming)** — Test-first development, pair programming

**Advantages:**
- Highly flexible — welcomes changing requirements
- Continuous delivery of working software
- Strong customer collaboration

**Disadvantages:**
- Hard to predict final cost and timeline
- Requires active customer participation throughout
- Less documentation — maintenance harder later

**When to use:** Software projects with changing/unclear requirements; startups; digital products.

---

### SDL Models — Master Comparison Table:

| Feature | Waterfall | Prototype | Spiral | Incremental | RAD | Agile |
|---------|-----------|-----------|--------|-------------|-----|-------|
| **Approach** | Linear, sequential | Iterative | Risk-driven cycles | Phased delivery | Fast parallel | Short sprints |
| **Flexibility** | Very Low | High | Medium | Medium | Medium | Very High |
| **User Involvement** | Low (only at start/end) | Very High | High | Medium | Very High | Continuous |
| **Documentation** | Very High | Low | High | Medium | Low | Low |
| **Risk Management** | Poor | Medium | Excellent | Medium | Medium | Good |
| **Speed** | Slow | Fast | Slow | Medium | Very Fast | Fast |
| **Best For** | Small, stable projects | Unclear requirements | Large, complex, risky | Phased large systems | Speed priority | Dynamic requirements |
| **Weakness** | Rigid, late feedback | Scope creep | Complex, expensive | Integration issues | Skilled team needed | Hard to estimate cost |

---

## 🧠 MASTER MNEMONIC SHEET — CHAPTER 7

| Topic | Mnemonic | Full Form |
|-------|----------|-----------|
| SSA goals | **PURR** | Problem understanding, User requirements, Requirements doc, Recommendation |
| SSA steps | **SCRIP** | Study, Collect, Requirements analysis, Identify, Prepare SRS |
| Feasibility Study | **TELOS** | Technical, Economic, Legal, Operational, Schedule |
| SSA Tools | **DED-FC** | DFD, ERD, Data Dictionary, Flowchart, Cases/Decision Tables |
| SDLC Phases | **PADIME** | Planning, Analysis, Design, Implementation, Maintenance, Evaluation |
| Maintenance types | **CAPP** | Corrective, Adaptive, Perfective, Preventive |
| Deployment methods | **DPPP** | Direct, Parallel, Phased, Pilot |
| SDL Models | **WISP-RAD** | Waterfall, Incremental, Spiral, Prototype, RAD, Agile, DevOps |
| System Design components | **DIOPS** | Database, Input, Output, Processing, Security |

---

## ⚡ QUICK REVISION FLASHCARDS

**Q: What is Structured System Analysis?**
A: Systematic, disciplined approach to analyzing existing systems or defining requirements using graphical tools — before programming begins.

**Q: What are the 4 DFD symbols?**
A: External Entity (Rectangle), Process (Circle), Data Store (Open Rectangle), Data Flow (Arrow)

**Q: Levels of DFD?**
A: Context Diagram (Level 0) → Level 1 → Level 2 → Level N (increasingly detailed)

**Q: TELOS feasibility framework?**
A: Technical, Economic, Legal, Operational, Schedule feasibility.

**Q: Logical Design vs Physical Design?**
A: Logical = WHAT the system does (technology-independent). Physical = HOW it's built (technology-specific, DB schema, UI mockups).

**Q: SDLC phases (PADIME)?**
A: Planning → Analysis → Design → Implementation → Maintenance/Testing → Evaluation

**Q: Which SDL model is best for risk management?**
A: **Spiral Model** — performs risk analysis in every cycle.

**Q: Waterfall's biggest disadvantage?**
A: Users see the system only at the very end — too late and expensive to make fundamental changes.

**Q: What is UAT?**
A: User Acceptance Testing — actual end users test the system to verify it meets their needs before go-live.

**Q: Which conversion strategy is safest?**
A: **Parallel Running** — old and new systems run simultaneously. Most expensive but safest (lowest risk).

---

## 📌 EXAM PATTERN LIKELY QUESTIONS

| Type | Question |
|------|---------|
| **Long (10 marks)** | Explain the SDLC with all its phases in detail |
| **Long (10 marks)** | Compare and contrast different SDL models (Waterfall, Prototype, Spiral, Agile) |
| **Short (5 marks)** | What is a DFD? Explain its symbols and levels with an example |
| **Short (5 marks)** | What is Structured System Analysis? Explain the TELOS feasibility study |
| **Short (5 marks)** | Distinguish between Logical and Physical System Design |
| **Short (5 marks)** | What are the types of system conversion/deployment? |
| **Short (5 marks)** | What are the types of maintenance in SDLC? |
| **Short (5 marks)** | Explain the Spiral Model with its key feature |
| **Definition** | Define: Data Dictionary, ERD, Cardinality, UAT, Prototype, Sprint |
| **Short** | What is Agile development? What are its core principles? |

---

> [!NOTE]
> **Chapter 7 ke Top 3 Must-Know:**
> 1. **SDLC Phases (PADIME)** — 6 phases — har ek ek paragraph mein explain karo with output of each phase
> 2. **SDL Models Comparison Table** — Waterfall vs Agile vs Spiral ek table mein — 10-marker ka perfect format
> 3. **DFD Symbols (4 types) + Context Diagram concept** — diagram draw karna aaye toh bonus marks!
>
> **Next chapter bhej bhai! 🔥💪**
