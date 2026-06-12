# 📘 DEEP DIVE: Production and Operation Management
### MBA 2nd Semester | DU SOL | Subject 14
**Prepared in IIM Format | Operations for Competitive Advantage**

---

> **How to Use:** POM combines strategy (where to locate, what to produce) with tools (MRP, EOQ, TQM). Connect every concept to real Indian manufacturing examples — Maruti, Tata, HUL, Amul. Diagrams matter here.

---

## 📌 CHAPTER 1: Introduction to Production & Operations Management

### 1.1 What is Production & Operations Management?

**Definition:**
Production and Operations Management (POM) is the design, operation, and improvement of the systems that create and deliver an organization's primary products and services. It encompasses all activities involved in transforming inputs into outputs.

**The Transformation Model:**
```
INPUTS                    TRANSFORMATION              OUTPUTS
(Materials, Labour,  ──►  (Manufacturing,        ──►  (Products,
 Capital, Energy,          Processing,                 Services,
 Information)              Assembly)                   Value Added)
```

**Types of Production Systems:**

| Type | Description | Example |
|------|-------------|---------|
| **Job Production** | One-off, unique items | Custom furniture, aircraft |
| **Batch Production** | Groups of identical items | Pharmaceutical tablets, biscuits |
| **Mass/Flow Production** | Continuous, high volume | Maruti cars, Coca-Cola |
| **Process Production** | Continuous chemical processes | Oil refining, cement, steel |
| **Project Production** | Large, unique, one-time | DMRC Metro, dam construction |

---

### 1.2 Operations Strategy

**Definition:**
Operations Strategy defines how the operations function will support and drive the organization's overall competitive strategy.

**Competitive Priorities (Trade-off Framework — Skinner):**

| Priority | Description | Example |
|----------|-------------|---------|
| **Cost** | Lowest cost operations | Decathlon, Walmart |
| **Quality** | Zero defects, high reliability | Toyota, Apple |
| **Speed** | Fast delivery, response | Amazon Prime, Zomato |
| **Flexibility** | Ability to change rapidly | Dell (custom PCs), Bata |
| **Dependability** | On-time delivery, reliability | FedEx, Indian Railways Freight |

**Order Winners vs Order Qualifiers (Terry Hill):**
- **Order Winner:** Factor that wins business (differentiates)
- **Order Qualifier:** Must have, but doesn't win business

**Example — Maruti Suzuki:**
- Order Qualifier: Car must be reliable (quality baseline)
- Order Winner: Low price, extensive service network, high resale value

---

### 1.3 Productivity

**Definition:**
Productivity is the ratio of output produced to inputs used.

```
Productivity = Output / Input

Partial Productivity = Output / One input (labour, capital, material)
Total Factor Productivity = Output / All inputs combined
```

**Productivity Improvement Methods:**
1. Technology upgrades (automation, robots)
2. Better methods (lean, kaizen)
3. Skill development (training)
4. Better materials (fewer defects → less waste)
5. Organizational changes (right structure, incentives)

---

## 📌 CHAPTER 2: Facilities Location and Supply Chain Linkage

### 2.1 Facility Location Decision

**Definition:**
Facility Location is the process of determining the optimal geographic placement of manufacturing plants, warehouses, or service facilities to minimize costs and maximize service levels.

**Location is a STRATEGIC decision** — once made, very costly to reverse.

---

### 2.2 Factors Affecting Location Decisions

| Factor | Manufacturing | Services |
|--------|--------------|---------|
| **Proximity to raw materials** | Critical | Less important |
| **Labour availability & cost** | Critical | Important |
| **Infrastructure** | Roads, power, water | Telecom, internet |
| **Market proximity** | Moderate | Critical |
| **Government incentives** | SEZ, tax holidays | Less |
| **Land cost** | Moderate | High in cities |
| **Climate** | Sometimes | Less |

**India-Specific Factors:**
- SEZ (Special Economic Zones): Tax exemptions, plug-and-play infrastructure
- State industrial policies: Gujarat, Tamil Nadu, Maharashtra competitive in incentives
- Labour laws: Ease of hiring/firing varies by state
- DPIIT ranking: India improved to Top 10 in global FDI attractiveness

---

### 2.3 Location Analysis Techniques

**Factor Rating Method:**
1. List all factors
2. Assign weights (sum to 1.0)
3. Rate each location on each factor (1-10)
4. Weighted Score = Weight × Rating
5. Choose location with highest total weighted score

**Worked Example:**

| Factor | Weight | Location A | Score A | Location B | Score B |
|--------|--------|-----------|---------|-----------|---------|
| Labour cost | 0.30 | 8 | 2.4 | 6 | 1.8 |
| Infrastructure | 0.25 | 7 | 1.75 | 9 | 2.25 |
| Market proximity | 0.25 | 6 | 1.5 | 8 | 2.0 |
| Govt incentives | 0.20 | 9 | 1.8 | 7 | 1.4 |
| **Total** | **1.00** | | **7.45** | | **7.45** |

Tie → Use secondary analysis (break-even, qualitative factors).

**Centre of Gravity Method (for distribution centre):**
```
Cx = Σ(dix × Vi) / ΣVi    [x-coordinate]
Cy = Σ(diy × Vi) / ΣVi    [y-coordinate]
```
Where dix, diy = coordinates of each demand point; Vi = volume at each point

---

### 2.4 Location and Supply Chain Integration

**Supply Chain Design:**
- Location affects transportation costs (inbound + outbound)
- Hub-and-spoke vs distributed network
- **India:** Amazon's fulfillment center network — strategically placed in Delhi, Mumbai, Bangalore, Hyderabad, Chennai for next-day delivery coverage

**Make-in-India and Location:**
- PLI (Production Linked Incentive) schemes attract manufacturing to India
- Apple (Foxconn) in Tamil Nadu, Samsung in Noida — government-incentivized locations
- Semiconductor fab: India's first fab in Gujarat (Tata-Powerchip alliance)

---

## 📌 CHAPTER 3: Design of Production Process

### 3.1 Process Design

**Definition:**
Process Design involves selecting the appropriate technology, equipment, and sequence of operations to convert inputs into desired outputs efficiently.

**Process Types:**

| Process Type | Volume | Variety | Layout | Example |
|-------------|--------|---------|--------|---------|
| **Project** | Very low | Very high | Fixed position | Ship, bridge |
| **Jobbing** | Low | High | Functional | Repair shop |
| **Batch** | Medium | Medium | Functional/Cell | Bakery, printing |
| **Line/Mass** | High | Low | Product/Line | Car assembly |
| **Continuous** | Very high | Very low | Flow | Petrochemicals |

---

### 3.2 Process-Product Matrix (Hayes & Wheelwright)

```
         PRODUCT STRUCTURE
         │ Low Volume    High Volume
         │ High Variety  Low Variety
─────────┼──────────────────────────────
High     │ Job Shop     ← Natural
Variety  │              Diagonal
         │
Low      │              Mass Production
Variety  │              Flow Lines
```
Companies operate most efficiently along the **natural diagonal**. Off-diagonal = inefficiency.

---

### 3.3 Layout Design

**Types of Layout:**

**1. Process/Functional Layout:**
- Machines grouped by type (all lathes together, all presses together)
- Used for job and batch production
- Flexible but high material handling
- Example: General hospital (departments: Surgery, Radiology, Cardiology)

**2. Product/Line Layout:**
- Machines arranged in order of product operations
- Used for mass production
- Low flexibility but high efficiency
- Example: Car assembly line (Maruti Suzuki Manesar plant)

**3. Cellular Manufacturing Layout:**
- Machines grouped into cells to produce a family of similar products
- Middle ground — moderate flexibility, moderate efficiency
- Example: CNC cell in auto component manufacturing

**4. Fixed Position Layout:**
- Product stays fixed; workers and machines come to it
- For very large, heavy products
- Example: Aircraft assembly, ship building, dam construction

---

### 3.4 Line Balancing

**Definition:**
Line Balancing ensures that the workload is evenly distributed across workstations in a production line to minimize idle time and maximize efficiency.

**Key Metrics:**
```
Cycle Time (C) = Available Production Time / Desired Output
Minimum Number of Workstations = Σ Task Times / Cycle Time (rounded up)
Efficiency = Σ Task Times / (Actual Workstations × Cycle Time) × 100
```

---

## 📌 CHAPTER 4: Design of Product and Services

### 4.1 Product Design

**Product Design** is the process of defining the features, specifications, and aesthetics of a product while ensuring manufacturability and customer value.

**Product Design Process:**
```
Idea Generation → Concept Development → Design Specification
→ Prototype Testing → Pilot Production → Full Launch
```

**Concurrent Engineering (Simultaneous Engineering):**
- Design, manufacturing, and marketing work simultaneously (not sequentially)
- Reduces time-to-market by 30-50%
- **Example:** Tata Nano — design, engineering, and manufacturing teams worked simultaneously

**Design for Manufacturability (DFM):**
- Design products that are easy and cheap to manufacture
- Reduce number of parts, use standard components, design for automation

**Quality Function Deployment (QFD) — House of Quality:**
- Translates customer requirements (VOC — Voice of Customer) into engineering specifications
- Ensures product design is customer-driven

---

### 4.2 Service Design

**Characteristics of Services (IIHP):**
- **Intangibility:** Cannot be touched/stored (haircut)
- **Inseparability:** Produced and consumed simultaneously (medical consultation)
- **Heterogeneity:** Quality varies (different waiters give different service)
- **Perishability:** Cannot be stored/inventoried (empty airline seat)

**Service Design Framework — Service Blueprint:**
Maps the service delivery process showing:
- Customer actions
- Front-office staff actions (visible)
- Back-office operations (invisible)
- Support processes

**Example — Swiggy Service Blueprint:**
- Customer: Orders on app
- Front stage: Delivery partner picks up food
- Back stage: Restaurant receives order notification
- Support: GPS tracking system, payment gateway

---

## 📌 CHAPTER 5: Inventory Management

### 5.1 Purpose of Inventory

**Definition:**
Inventory refers to stocks of raw materials, work-in-process, or finished goods held by an organization to meet future demand.

**Types of Inventory:**
- **Raw Material:** Purchased inputs awaiting production
- **WIP (Work-in-Process):** Partially completed products
- **Finished Goods:** Completed products awaiting sale
- **MRO (Maintenance, Repair, Operating):** Spare parts, consumables

**Costs of Inventory:**
| Cost Type | Description |
|-----------|-------------|
| **Ordering/Setup Cost** | Cost per order placed |
| **Holding/Carrying Cost** | Cost of storing inventory (storage, insurance, obsolescence) |
| **Stockout Cost** | Lost sales, customer dissatisfaction from running out |
| **Purchase Cost** | Price of the items themselves |

---

### 5.2 Economic Order Quantity (EOQ)

**EOQ Formula:**
```
EOQ = Q* = √(2DS/H)
Where: D = Annual Demand, S = Ordering Cost per order, H = Holding Cost per unit per year
```

**Total Inventory Cost:**
```
TC = (D/Q) × S + (Q/2) × H + D × P
   = Ordering Cost + Holding Cost + Purchase Cost
```
At EOQ, **Ordering Cost = Holding Cost** (point of minimum total cost).

**Reorder Point (ROP):**
```
ROP = Lead Time Demand = Average Daily Demand × Lead Time (days)
Safety Stock ROP = (Average demand × Lead time) + Safety Stock
Safety Stock = Z × σ_demand × √Lead Time
```

---

### 5.3 Inventory Classification — ABC Analysis

```
A Items: Top 20% items by value = 70-80% of total inventory value → Tight control
B Items: Next 30% items = 15-25% of value → Moderate control
C Items: Bottom 50% items = 5-10% of value → Simple control
```

**Indian Application:**
- In Tata Steel: Iron ore and coal = A items (70% of material cost)
- Consumables, stationery = C items
- Maintenance spares = VED analysis (Vital, Essential, Desirable)

---

## 📌 CHAPTER 6: Aggregate Production Planning, MPS and MRP

### 6.1 Aggregate Production Planning (APP)

**Definition:**
Aggregate Production Planning determines the optimal combination of production rate, workforce level, and inventory to meet demand over a medium-term planning horizon (typically 3-18 months).

**APP Strategies:**

| Strategy | Description | Cost Implication |
|----------|-------------|-----------------|
| **Chase Strategy** | Match production to demand (hire/fire) | High HR costs, low inventory |
| **Level Strategy** | Constant production rate; use inventory to absorb fluctuations | Low HR costs, high inventory |
| **Mixed Strategy** | Combination of both | Moderate both |

**APP Costs:**
- Hiring/Training costs
- Firing/Layoff costs
- Overtime premium costs
- Inventory holding costs
- Subcontracting costs
- Backorder/shortage costs

---

### 6.2 Master Production Schedule (MPS)

**Definition:**
MPS disaggregates the Aggregate Plan into a detailed schedule specifying exactly what products will be produced, in what quantities, and when (week by week).

**MPS bridges APP and MRP:**
```
Aggregate Plan (Monthly) → MPS (Weekly) → MRP (Daily/Lot)
```

**MPS Inputs:**
- Demand forecast
- Customer orders (confirmed)
- Inventory on hand
- Production capacity constraints

**Available to Promise (ATP):**
```
ATP = MPS Quantity - Committed Customer Orders in that period
```

---

### 6.3 Material Requirements Planning (MRP)

**Definition:**
MRP is a computer-based information system that translates the MPS for end products into the time-phased requirements for sub-assemblies, components, and raw materials.

**MRP Inputs:**
1. **Master Production Schedule (MPS):** What to produce and when
2. **Bill of Materials (BOM):** What components make up the product
3. **Inventory Records:** Current stock on hand and on order

**MRP Logic:**
```
Gross Requirements = Demand from MPS or parent item
Net Requirements = Gross Requirements - Available Inventory
Planned Order Releases = Net Requirements (adjusted for lead time)
```

**Bill of Materials (BOM) Example — Bicycle:**
```
Level 0: Bicycle (1)
Level 1: Frame (1), Wheels (2), Handlebars (1), Drivetrain (1)
Level 2: Tyre (1 per wheel), Tube (1 per wheel), Rim (1 per wheel)
```

**MRP Time-Phased Record:**

| Week | 1 | 2 | 3 | 4 |
|------|---|---|---|---|
| Gross Requirements | 50 | 0 | 80 | 60 |
| Scheduled Receipts | 0 | 100 | 0 | 0 |
| On-Hand Inventory | 20 | 70 | 70 | 0 |
| Net Requirements | 30 | 0 | 10 | 60 |
| Planned Order Releases | 30 | 0 | 10 | 60 |

**MRP Extensions:**
- **MRP II (Manufacturing Resource Planning):** Extends MRP to include capacity planning, financial planning
- **ERP (Enterprise Resource Planning):** Integrates ALL business functions (SAP, Oracle) — MRP logic embedded

---

## 📌 CHAPTER 7: Quality Management

### 7.1 Quality — Definition

**Definition:**
Quality is the degree to which a product or service meets or exceeds customer expectations.

**Quality Dimensions (Garvin's 8 Dimensions):**

| Dimension | Description | Example |
|-----------|-------------|---------|
| **Performance** | Primary operating characteristics | Car acceleration |
| **Features** | Secondary characteristics | Sunroof, GPS |
| **Reliability** | Probability of failure-free operation | Car starts every time |
| **Conformance** | Meeting specifications | Dimensions within tolerance |
| **Durability** | Product life | Car runs 2 lakh km |
| **Serviceability** | Ease of repair | Maruti's wide service network |
| **Aesthetics** | Look, feel, sound | Car interior design |
| **Perceived Quality** | Customer perception/brand | Toyota = reliable |

---

### 7.2 Total Quality Management (TQM)

**Definition:**
TQM is a management philosophy committed to continuous improvement, involving ALL employees, at ALL levels, in ALL functions to satisfy or exceed customer expectations.

**TQM Principles:**
1. Customer Focus (external + internal customers)
2. Continuous Improvement (Kaizen)
3. Employee Involvement (quality circles)
4. Process Approach
5. Data-driven decision making
6. Supplier partnerships

**Quality Gurus:**

| Guru | Key Contribution |
|------|----------------|
| **W.E. Deming** | PDCA Cycle (Plan-Do-Check-Act); 14 Points for Management |
| **Joseph Juran** | Quality Trilogy (Planning, Control, Improvement); Pareto Principle |
| **Philip Crosby** | "Quality is Free"; Zero Defects; Cost of Quality |
| **Kaoru Ishikawa** | Fishbone/Cause-Effect Diagram; QC Circles |
| **Shigeo Shingo** | Poka-Yoke (mistake proofing); SMED (quick setup) |

---

### 7.3 Quality Tools

**Seven QC Tools:**
1. **Check Sheet:** Data collection form
2. **Pareto Chart:** 80-20 rule; prioritize problems
3. **Cause-Effect Diagram (Fishbone/Ishikawa):** Identify root causes
4. **Histogram:** Distribution of data
5. **Scatter Diagram:** Relationship between variables
6. **Control Chart (Shewhart Chart):** Monitor process over time
7. **Flowchart:** Process mapping

**Six Sigma:**
- A data-driven approach targeting near-zero defects
- **DMAIC:** Define → Measure → Analyze → Improve → Control
- **Target:** 3.4 defects per million opportunities (DPMO)
- **Belt System:** Green Belt, Black Belt, Master Black Belt
- **India:** Wipro (first Indian company to achieve Six Sigma in IT), GE India, HCL

---

### 7.4 Quality Standards — ISO 9001

**ISO 9001:2015:** International standard for Quality Management Systems
- Certification demonstrates commitment to quality processes
- India: 1,14,000+ certified organizations (2023)
- Benefits: Market credibility, export access, customer confidence

**India Quality Awards:**
- **Deming Prize:** Japan-origin; Tata Steel, Sundaram Clayton winners
- **Rajiv Gandhi National Quality Award:** India's national quality recognition
- **CII-EXIM Bank Award:** Business excellence

---

### 7.5 Case Study — Maruti Suzuki Quality Journey

**Background:** Maruti Suzuki transformed from quality-challenged (early 1990s) to India's quality leader.

**Quality Initiatives:**
- Implemented **Suzuki Production System** (variant of Toyota Production System)
- **Zero Defect** program with supplier development
- **Quality Circles:** Over 4,000 active quality circles across all plants
- **Poka-Yoke devices:** Mistake-proofing installed at 500+ assembly points
- Regular **Kaizen** activities with workers

**Results:**
- Initial Quality Study (JD Power India): Consistently #1 or #2
- 99%+ of cars pass final inspection first time
- Customer satisfaction scores in top quartile

**Lesson:** Quality is NOT a department — it's everyone's job. Maruti's culture of employee involvement and systematic tools (poka-yoke, kaizen, QC circles) created sustainable quality excellence.

---

## 📌 CHAPTER 8: Lean Operations

### 8.1 What is Lean?

**Definition:**
Lean Operations (derived from Toyota Production System) is a philosophy of eliminating waste (muda) in all forms while maximizing value for the customer.

**Father of Lean:** Taiichi Ohno (Toyota) — developed TPS (Toyota Production System)

---

### 8.2 The 8 Wastes (TIMWOODS Mnemonic)

| Waste | Description | Example |
|-------|-------------|---------|
| **T**ransportation | Unnecessary movement of materials | Moving parts across a large factory |
| **I**nventory | Excess stock | Piles of raw material |
| **M**otion | Unnecessary worker movement | Worker walking to get tools |
| **W**aiting | Idle time | Machine waiting for materials |
| **O**verproduction | Making more than needed | Producing 1,000 when demand is 700 |
| **O**verprocessing | Doing more than required | Extra features customer doesn't want |
| **D**efects | Rework, scrap | Rejected parts |
| **S**kills underutilization | Not using employee knowledge | Ignoring worker improvement ideas |

---

### 8.3 Lean Tools

**5S Methodology:**
| S | Japanese | Meaning |
|---|---------|---------|
| **S**ort (Seiri) | Remove unnecessary items | Clear clutter |
| **S**et in Order (Seiton) | Organize what's left | A place for everything |
| **S**hine (Seiso) | Clean and inspect | Sparkling clean workplace |
| **S**tandardize (Seiketsu) | Create standards | Make it the norm |
| **S**ustain (Shitsuke) | Maintain and improve | Continuous habit |

**Just-In-Time (JIT):**
- Produce only what is needed, when needed, in the quantity needed
- Zero inventory goal
- Requires: Reliable suppliers, short setup times, quality at source, flexible workforce

**Kanban System:**
- Visual signal system to control production flow
- Card/container triggers production of next batch
- Prevents overproduction
- **India:** Maruti Suzuki, Bosch India use Kanban in their plants

**Value Stream Mapping (VSM):**
- Maps all value-adding and non-value-adding steps in a process
- Identifies waste (non-value-adding steps)
- Creates future-state map (after waste elimination)

---

### 8.4 Case Study — Toyota Production System (TPS)

**Background:** TPS is the most studied and emulated manufacturing system in the world, forming the basis of global lean manufacturing.

**Two Pillars of TPS:**
1. **Just-In-Time (JIT):** Right part, right time, right quantity
2. **Jidoka (Autonomation):** Machines stop automatically when defect detected; don't pass defects downstream

**Key Elements:**
- **Heijunka:** Production leveling (avoid batch-and-queue)
- **Standardized Work:** Best-known method documented and followed
- **Kaizen:** Continuous improvement by all workers
- **Andon System:** Workers pull cord to stop line if defect found

**Results:**
- Toyota consistently among world's most profitable automakers
- Defect rates far below industry average
- Inventory turnover 2x industry norm

**Indian Adoption:** Maruti Suzuki (Toyota's partner), Mahindra & Mahindra, and Bajaj Auto have all implemented TPS principles in their plants.

---

## 📌 CHAPTER 9: Theory of Constraints (TOC)

### 9.1 What is TOC?

**Definition:**
The Theory of Constraints (TOC), developed by Dr. Eliyahu Goldratt (1984, "The Goal"), states that every system has at least one constraint (bottleneck) that limits its overall performance. Improving the constraint improves the whole system.

> *"The Goal of a firm is to make money. Everything else is a means to that end."* — Eliyahu Goldratt

---

### 9.2 The Five Focusing Steps (TOC Process)

```
Step 1: IDENTIFY the constraint (bottleneck)
Step 2: EXPLOIT the constraint (maximize its output)
Step 3: SUBORDINATE everything else to the constraint
Step 4: ELEVATE the constraint (increase capacity if needed)
Step 5: REPEAT — Once constraint is broken, find the next one
```

**The Chain Analogy:** The strength of a chain = strength of its weakest link. Improving a non-bottleneck link does NOT improve the chain.

---

### 9.3 Throughput Accounting (TOC Metrics)

TOC measures performance using:

| Metric | Definition | Traditional Accounting |
|--------|------------|----------------------|
| **Throughput (T)** | Rate at which system generates money through sales = Sales - Truly Variable Costs | Net Profit |
| **Investment/Inventory (I)** | Money invested in things you intend to sell | Inventory + Fixed Assets |
| **Operating Expense (OE)** | All money spent to turn Inventory into Throughput | Cost of Goods Sold + Expenses |

**TOC Goal:** Increase T; Decrease I and OE simultaneously.

**Net Profit = T - OE**

---

### 9.4 Drum-Buffer-Rope (DBR)

**Drum:** The constraint (bottleneck) that sets the pace of production — it beats the "drum" for the whole factory.

**Buffer:** Protective inventory placed BEFORE the drum to ensure it never starves.

**Rope:** Communication mechanism from drum back to the start of production — "release material only as fast as the drum can process it."

**Example:** In a factory where the painting station is the bottleneck:
- Drum = Painting station (sets pace)
- Buffer = WIP inventory before painting (ensures painting never waits)
- Rope = Signal to release raw materials at painting's pace (not faster)

---

### 9.5 Case Study — TOC at an Indian Textile Factory

**Background:** A textile manufacturer had 5 production stages: Spinning → Weaving → Dyeing → Printing → Finishing. Dyeing capacity = 800 m/day was the bottleneck. Other stages had capacity of 1,200+ m/day.

**Before TOC:**
- Factory scheduled all machines at 100% utilization
- WIP piled up BEFORE dyeing; other stages were starved AFTER dyeing
- On-time delivery: 60%; huge WIP inventory

**After TOC (5 Steps Applied):**
1. **Identified** constraint: Dyeing (800 m/day)
2. **Exploited:** No idle time on dyeing machines; preventive maintenance during breaks; priority scheduling at dyeing
3. **Subordinated:** All upstream and downstream stages scheduled to dyeing's pace
4. **Elevated:** Added one shift at dyeing; moved one dyeing machine from another plant
5. **Result:** Dyeing capacity → 1,100 m/day; new constraint = Printing

**Results After TOC:**
- On-time delivery: 60% → 92%
- WIP inventory: Reduced by 40%
- Revenue increased 30% (more orders fulfilled on time)
- Factory-wide throughput increased despite NO major capital investment

**Lesson:** Improving a non-bottleneck resource is wasteful. Focus 100% of improvement energy on the CONSTRAINT. Once fixed, identify the new constraint and repeat.

---

## MASTER SUMMARY TABLE

| Chapter | Core Concept | Key Tool/Model | Key Author |
|---------|-------------|---------------|-----------|
| 1 | POM Introduction | Transformation Model; Competitive Priorities | Skinner, Hayes |
| 2 | Facility Location | Factor Rating; Centre of Gravity | — |
| 3 | Process Design | Process-Product Matrix; Layout Types | Hayes & Wheelwright |
| 4 | Product & Service Design | DFM; QFD; Service Blueprint | — |
| 5 | Inventory Management | EOQ; ABC Analysis; ROP | Harris (EOQ) |
| 6 | APP, MPS, MRP | MRP Logic; BOM; Time-Phased Record | — |
| 7 | Quality Management | TQM; Six Sigma DMAIC; 7 QC Tools | Deming, Juran, Crosby, Ishikawa |
| 8 | Lean Operations | 8 Wastes (TIMWOODS); 5S; JIT; Kanban | Ohno (Toyota) |
| 9 | Theory of Constraints | 5 Steps; DBR; Throughput Accounting | Goldratt |

---

*Document prepared for MBA 2nd Semester, DU SOL | Subject: Production & Operations Management*
*For Academic Use Only*
