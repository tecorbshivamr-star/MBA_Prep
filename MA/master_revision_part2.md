# 📋 MASTER REVISION SHEET — Part 2 (Ch 7–11)
### Management Accounting | DU SOL MBA Sem 2 | Exam Tomorrow! 🔥

---

# 📘 CHAPTER 7: Budgets & Budgetary Control

## 🔑 Definitions

| Term | Definition | BugZero Analogy |
|------|-----------|----------------|
| **Budget** | Formal financial plan prepared IN ADVANCE for a specific future period | BugZero's annual plan: ₹50L revenue, ₹40L cost, ₹10L profit |
| **Budgetary Control** | System of preparing budgets, comparing with actuals, and taking corrective action | Monthly review: planned ₹4L revenue vs actual ₹3.5L → investigate why |
| **Principal Budget Factor (PBF)** | The KEY constraint that limits activity; budget built around this first | BugZero: only 10 QA engineers available → limits max projects |
| **Fixed Budget** | Prepared for ONE level of activity only; doesn't adjust for actual output | Budget assumes 100 projects; actual = 80 → comparison misleading |
| **Flexible Budget** | Prepared for MULTIPLE activity levels; adjusts costs to actual output level | Adjusts variable costs for actual 80 projects → fair comparison |
| **Zero-Based Budgeting (ZBB)** | Every expense justified from ZERO each period; no automatic carry-forward | BugZero justifies EVERY tool subscription — drops unused ones! |
| **Master Budget** | Summary of ALL functional budgets: Budgeted P&L + Balance Sheet + Cash Flow | BugZero's full annual financial plan in one document |

---

## 🔢 Key Formulas

### Production Budget
```
Production Required (units) = Sales Units Required
                             + Desired Closing Stock of Finished Goods
                             − Opening Stock of Finished Goods

[Logic: We need to produce enough to cover both sales AND build up closing stock,
 minus what we already have in opening stock]
```

### Materials Purchase Budget
```
Materials to Purchase = Materials Required for Production
                      + Desired Closing Stock of Materials
                      − Opening Stock of Materials

Materials Required = Production Units × Material per Unit
```

### Flexible Budget (Key Formula)
```
Flexible Budget Cost = Fixed Cost (unchanged)
                     + (Variable Cost per unit × Actual Output)

[Fixed costs stay the same regardless of output
 Variable costs adjust proportionately with actual output]
```
> **BugZero Example:** Budget: 100 projects, VC=₹40K/project, FC=₹5L
> Actual output = 80 projects
> Flexible Budget = ₹5L + (₹40K × 80) = ₹5L + ₹32L = ₹37L (fair comparison with actual ₹38L)

### ZBB Steps
```
Step 1: Identify Decision Units (each dept/activity)
Step 2: Create Decision Packages (min/current/enhanced options)
Step 3: Rank packages by cost-benefit
Step 4: Allocate budget from highest rank downward
Step 5: Prepare final budget
```

---

## ⚖️ Fixed vs Flexible Budget

| Feature | Fixed Budget | Flexible Budget |
|---------|-------------|----------------|
| **Activity level** | One predetermined level | Multiple levels |
| **Variance analysis** | Misleading if output differs | Meaningful & fair |
| **Cost behavior** | Ignores fixed/variable split | Recognizes behavior |
| **Best for** | Stable, predictable | Variable operations |

---

## 🧠 ZBB vs Traditional Budgeting

| Feature | Traditional | ZBB |
|---------|------------|-----|
| Starting point | Last year + adjustment | ZERO (fresh start) |
| Justification | Only changes justified | EVERY rupee justified |
| Waste | Carries forward inefficiencies | Eliminates waste |

---

# 📘 CHAPTER 8: Cost Management

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Cost Management** | Strategic long-term approach to managing all costs to add value |
| **Cost Control** | Keeping costs within pre-set standards; monitoring and correcting |
| **Cost Reduction** | Permanently lowering costs without affecting quality |
| **ABC (Activity-Based Costing)** | Assigns overhead to products based on activities they consume and cost drivers |
| **Cost Driver** | The factor that CAUSES the cost of an activity (e.g., number of setups) |
| **Cost Pool** | Group of overhead costs related to one specific activity |
| **TOC (Theory of Constraints)** | Every system has a bottleneck limiting output; manage it! |
| **Throughput** | Sales Revenue MINUS Direct Material Cost only |
| **Target Costing** | Market Price − Desired Profit = Target Cost (work backwards from price!) |
| **Value Chain** | All activities from input to customer that create value (Porter's model) |
| **Life Cycle Costing** | Tracks total cost across ENTIRE product life — R&D to disposal |
| **JIT** | Produce only what needed, when needed, in quantity needed — zero waste |
| **Backflush Costing** | Simplified costing used with JIT; costs recorded only at completion |

---

## 🔢 Key Formulas

### ABC: Cost Driver Rate
```
Cost Driver Rate = Total Cost of Activity Pool ÷ Total Cost Driver Units

Overhead Charged to Product = Cost Driver Rate × Product's Driver Units

[Unlike traditional OAR which uses one rate for everything,
 ABC uses a SEPARATE rate for EACH activity]
```
> **BugZero:** Setup pool = ₹60,000 ÷ 30 setups = ₹2,000/setup
> Product Alpha used 5 setups → OH charged = 5 × ₹2,000 = ₹10,000

### Target Costing
```
Target Cost = Market Selling Price − Desired Profit Margin

Cost Gap = Current Estimated Cost − Target Cost
           [If positive → must reduce costs to meet target!]
```
> **BugZero:** Market price = ₹80,000. Desired profit = 25% = ₹20,000.
> Target Cost = ₹80,000 − ₹20,000 = **₹60,000**
> If current cost = ₹70,000 → Cost Gap = ₹10,000 (must find savings!)

### Throughput Accounting Ratio
```
Throughput per unit        = Selling Price − Direct Material Cost only
                            [Labour and overheads NOT deducted!]

TA Ratio = Throughput per Bottleneck Hour
           ÷ Total Operating Cost per Bottleneck Hour

TA Ratio > 1 → Product is worthwhile
Rank products: Higher TA Ratio → produce first at bottleneck
```

### TOC — 5 Steps (Memory: "**I-E-S-E-R**")
```
1. IDENTIFY   the constraint (bottleneck)
2. EXPLOIT    it (maximize output from bottleneck — no idle time!)
3. SUBORDINATE all other processes to serve the bottleneck
4. ELEVATE    the constraint (invest to increase capacity)
5. REPEAT     (once fixed, find the next constraint)
```

---

## ⚖️ Traditional vs Target Costing

| Feature | Traditional Costing | Target Costing |
|---------|--------------------|--------------------|
| Direction | Cost → Add profit → Price | Price → Deduct profit → Target Cost |
| Driver | Cost-driven | Market/Customer-driven |
| Origin | Western | Japanese (Toyota) |

---

# 📘 CHAPTER 9: Performance Measurement — Balanced Scorecard

## 🔑 Definitions — BSC (Kaplan & Norton, 1992)

> **Balanced Scorecard** = Performance framework measuring 4 perspectives: Financial, Customer, Internal Process, Learning & Growth

| Perspective | Question | Measures | BugZero |
|------------|---------|---------|---------|
| **Financial** | How do shareholders see us? | Profit, ROI, Revenue growth | 25% profit margin |
| **Customer** | How do customers see us? | Satisfaction score, retention, market share | 4.5/5 rating, 70% repeat |
| **Internal Process** | What must we excel at? | Defect rate, cycle time, efficiency | Bug escape < 3% |
| **Learning & Growth** | Can we improve? | Training hrs, certifications, retention | 10 training days/yr |

### Cause-Effect Chain
```
Learning & Growth → Better Internal Processes → Happier Customers → Financial Results
(Lead Indicators)                                                  (Lag Indicators)
```

### Key Formulas
```
ROI = Net Profit ÷ Capital Employed × 100
      [Higher ROI = Better return on investment]

RI  = Net Profit − (Capital Employed × Required Rate of Return)
      Positive RI → Creating value above minimum required return ✅
      Negative RI → NOT covering cost of capital ❌
```

### ROI vs RI Decision Problem
```
Division ROI = 20%. New project ROI = 18%. Company required rate = 15%.
→ ROI Method: REJECT (lowers division %) — WRONG decision!
→ RI Method:  ACCEPT (18% > 15% → positive RI) — CORRECT decision!
∴ RI gives BETTER goal congruence with company goals
```

### Memory Trick: **"FC IL"**
Financial → Customer → Internal Process → Learning & Growth

---

# 📘 CHAPTER 10: Inventory Management

## 🔑 Definitions — Inventory Control Techniques

| Technique | Basis | Classes | Key Point |
|-----------|-------|---------|-----------|
| **ABC** | ₹ Value of usage | A (high), B (medium), C (low) | A=tight control, C=loose |
| **VED** | Operational criticality | Vital, Essential, Desirable | V items stocked at all times even if expensive |
| **FSN** | Movement/usage rate | Fast, Slow, Non-moving | N items → dispose of (dead stock!) |
| **HML** | Unit price | High, Medium, Low | Controls purchasing authority levels |
| **SDE** | Availability | Scarce, Difficult, Easy | S items need high safety stock |
| **GOLF** | Source of supply | Govt, Ordinary, Local, Foreign | F items need longest lead time |

> **ABC vs VED Key Difference:** ABC = by financial value | VED = by operational criticality
> A cheap ₹2 rubber seal can be VITAL (V) — stops entire machine if unavailable!

---

## 🔢 Inventory Valuation Methods

### FIFO (First In, First Out)
```
Issues valued at OLDEST price first
Closing Stock = at LATEST (most recent) prices
In Rising Prices: Lower COGS → Higher Profit → More Tax
```

### LIFO (Last In, First Out)
```
Issues valued at NEWEST price first
Closing Stock = at OLDEST prices (undervalued!)
In Rising Prices: Higher COGS → Lower Profit → Less Tax
NOT accepted under Ind AS/IFRS
```

### Weighted Average Price (WAP)
```
WAP = Total Value of Stock in Hand ÷ Total Units in Hand
      [Recalculate EVERY time a new receipt arrives]

Issues valued at WAP | Result = between FIFO and LIFO
```

### Summary Table (Rising Prices)
```
Method  | Issue Cost | Closing Stock | Profit Effect
FIFO    | Lowest     | Highest       | Highest Profit
WAP     | Middle     | Middle        | Middle Profit
LIFO    | Highest    | Lowest        | Lowest Profit
```
> **Verify Store Ledger:** Opening Stock Value + Receipts = Issues + Closing Stock ✅

---

# 📘 CHAPTER 11: Performance Measurement & Evaluation

## 🔑 Responsibility Centres

| Type | Manager Controls | Key Measure |
|------|-----------------|-------------|
| **Cost Centre** | Costs only | Actual Cost vs Budget |
| **Revenue Centre** | Revenue only | Actual Revenue vs Target |
| **Profit Centre** | Revenue AND Costs | Profit |
| **Investment Centre** | Revenue, Costs AND Assets | ROI, RI, EVA |

> **Controllability Principle:** Judge managers ONLY on what they CAN control!

---

## 🔢 Economic Value Added (EVA) ⭐⭐⭐

```
EVA = NOPAT − (Capital Employed × WACC)

Where:
  NOPAT = Net Operating Profit After Tax
        = Operating Profit × (1 − Tax Rate)
        [Operating profit adjusted for tax; excludes interest/financing]

  WACC  = Weighted Average Cost of Capital
        = Weighted average of cost of debt + cost of equity
        [The minimum return investors expect from the business]

  Capital Employed = Total Assets − Current Liabilities

  EVA > 0 → Business creating value (earning more than cost of capital) ✅
  EVA < 0 → Business DESTROYING value ❌
```
> **BugZero:** Operating Profit=₹15L, Tax=30%, Capital=₹80L, WACC=12%
> NOPAT = ₹15L × 0.70 = ₹10.5L | Cost of Capital = ₹80L × 12% = ₹9.6L
> **EVA = ₹10.5L − ₹9.6L = ₹0.9L (Positive → Value Created ✅)**

---

## 🔢 Performance Frameworks ⭐⭐⭐

### Performance Pyramid (Lynch & Cross, 1991)
```
CORPORATE VISION  → Financial & Market measures
      ↓ (objectives flow DOWN)
BUSINESS UNITS    → Customer Satisfaction & Flexibility
      ↓
BUSINESS OPERATIONS → Quality & Delivery
      ↓
DEPARTMENTS       → Cycle Time & Waste
      ↑ (measures flow UP to top)
```
> **Key Idea:** Objectives DESCEND from top. Results ASCEND from bottom.

---

### Building Block Model (Fitzgerald & Moon, 1996) ⭐⭐⭐
> Designed for **SERVICE industries** (like BugZero!)

```
┌─────────────────┬──────────────────┬──────────────────┐
│  6 DIMENSIONS   │   3 STANDARDS    │    3 REWARDS      │
│  (What to       │  (How to set     │  (How to          │
│   measure)      │   targets)       │   motivate)       │
├─────────────────┼──────────────────┼──────────────────┤
│ 1. Financial    │ 1. Ownership     │ 1. Clarity        │
│    Performance  │    (Managers set │    (Rewards are   │
│ 2. Competitive- │    own targets)  │    understood)    │
│    ness         │ 2. Achievability │ 2. Motivation     │
│ 3. Quality      │    (Stretching   │    (Rewards drive │
│ 4. Flexibility  │    but realistic)│    right behavior)│
│ 5. Resource     │ 3. Equity        │ 3. Controllability│
│    Utilization  │    (Fair to all  │    (Only rewarded │
│ 6. Innovation   │    departments)  │    for what they  │
│                 │                  │    control)       │
└─────────────────┴──────────────────┴──────────────────┘
```

---

### Performance Prism (Neely et al., 2002) ⭐⭐

> **5 Facets** — starts with STAKEHOLDERS (not strategy!)

```
1. STAKEHOLDER SATISFACTION → What do stakeholders WANT?
2. STRATEGIES               → What strategies satisfy them?
3. PROCESSES                → What processes execute strategies?
4. CAPABILITIES             → What capabilities support processes?
5. STAKEHOLDER CONTRIBUTION → What must stakeholders give US?
```
> **Key Difference from BSC:** BSC starts with company strategy → Prism starts with **stakeholder needs**

### Stakeholders in Prism
```
Investors | Customers | Employees | Suppliers | Regulators | Communities
```

---

### Triple Bottom Line (Elkington, 1994) ⭐⭐

```
TBL = PROFIT + PEOPLE + PLANET (The 3 Ps)

PROFIT  (Economic)    → Financial sustainability: Revenue, Profit, EVA
PEOPLE  (Social)      → Social responsibility: Employee welfare, diversity, community
PLANET  (Environmental)→ Environmental impact: Carbon footprint, energy, waste
```
> Traditional accounting measures only PROFIT.
> TBL says: a truly successful company must also care for PEOPLE and PLANET.

---

## 📊 All Frameworks — Master Comparison

| Framework | Developed By | Year | Key Feature |
|-----------|-------------|------|-------------|
| **Performance Pyramid** | Lynch & Cross | 1991 | Objectives ↓ / Measures ↑ |
| **Balanced Scorecard** | Kaplan & Norton | 1992 | 4 Perspectives (F,C,I,L) |
| **Triple Bottom Line** | Elkington | 1994 | Profit + People + Planet |
| **Building Block Model** | Fitzgerald & Moon | 1996 | 6D + 3S + 3R (service sector) |
| **Performance Prism** | Neely et al. | 2002 | 5 Facets, stakeholder-first |

> **Memory:** "PP-BSC-TBL-BBM-Prism" → 1991 → 1992 → 1994 → 1996 → 2002

---

# 🚀 MASTER FORMULA CARD — PART 2

```
┌─────────────────────────────────────────────────────────────────────┐
│ CH7: Prod Budget = Sales + Closing FG − Opening FG                  │
│      Flex Budget Cost = FC + (VC/unit × Actual Output)              │
├─────────────────────────────────────────────────────────────────────┤
│ CH8: ABC Rate = Activity Cost ÷ Cost Driver Units                   │
│      Target Cost = Market Price − Desired Profit                    │
│      Throughput = Sales Revenue − Direct Material Only              │
│      TOC Steps: Identify→Exploit→Subordinate→Elevate→Repeat         │
├─────────────────────────────────────────────────────────────────────┤
│ CH9: ROI = Net Profit ÷ Capital × 100                               │
│      RI  = Net Profit − (Capital × Required Rate)                   │
│      BSC: Financial→Customer→Internal→Learning (cause-effect ↑)     │
├─────────────────────────────────────────────────────────────────────┤
│ CH10: FIFO→Lowest Cost, Highest Stock, Highest Profit               │
│       LIFO→Highest Cost, Lowest Stock, Lowest Profit                │
│       WAP = Total Value ÷ Total Units (recalculate each receipt)    │
│       VED: V=Vital, E=Essential, D=Desirable (criticality-based)    │
├─────────────────────────────────────────────────────────────────────┤
│ CH11: EVA = NOPAT − (Capital Employed × WACC) → +ve = value created│
│       Building Blocks: 6 Dimensions + 3 Standards + 3 Rewards       │
│       TBL: Profit + People + Planet                                  │
│       Prism: 5 Facets — starts with Stakeholder Satisfaction         │
└─────────────────────────────────────────────────────────────────────┘
```

---

# 🎯 EXAM STRATEGY — LAST NIGHT TIPS

## ⚡ High-Priority Numericals (Practice Tonight!)
1. **BEP + MOS calculation** (Ch. 5) — almost certain to appear
2. **Material/Labour Variance** (Ch. 6) — very likely
3. **Contract Costing Profit** (Ch. 3) — ⅓/⅔ rule numerical
4. **Process Account** (Ch. 4) — Normal/Abnormal Loss
5. **Store Ledger** (Ch. 10) — FIFO or WAP

## ⚡ High-Priority Theory
1. **Building Block Model** — 6 Dimensions + 3 Standards + 3 Rewards (Ch. 11)
2. **Balanced Scorecard** — 4 perspectives with examples (Ch. 9)
3. **ABC vs Traditional Costing** — steps + advantages (Ch. 8)
4. **Marginal vs Absorption Costing** — table + profit difference (Ch. 5)
5. **ZBB vs Traditional Budgeting** — table (Ch. 7)

## ⚡ Short Notes (5 marks each — likely 2-3 to appear)
Contribution | P/V Ratio | EOQ | ABC Analysis | VED Analysis |
Target Costing | JIT | Escalation Clause | Retention Money |
Notional Profit | EVA | Triple Bottom Line | Performance Prism

---

# 🌟 LAST-MINUTE MEMORY AIDS

```
Cost Sheet:      DM+DL+DE = Prime → +FOH = Works → +AOH = Production → +SOH = Total
BEP:             Fixed Cost ÷ Contribution/unit (units) | ÷ P/V Ratio (₹)
Variances:       MCV=MPV+MUV | LCV=LRV+LEV | Always: S minus A (Standard minus Actual)
Contract Profit: <25%=0 | 25-50%=1/3×NP | 50-90%=2/3×NP | >90%=Full
Stock Levels:    ROL→Min→Max→Avg→Danger (Really Mindful Managers Always Discuss)
Inv Valuation:   FIFO=High Profit | LIFO=Low Profit | WAP=Middle
BSC Trick:       FC IL → Financial, Customer, Internal, Learning (cause flows UP)
EVA:             NOPAT − (CE × WACC) → +ve = Value Created
TBL:             Profit + People + Planet
BBM:             6 Dimensions + 3 Standards + 3 Rewards (Service sector)
Prism:           5 Facets: Satisfaction→Strategy→Process→Capability→Contribution
Frameworks:      PP(1991)→BSC(1992)→TBL(1994)→BBM(1996)→Prism(2002)
```

---
> 💪 **You've studied ALL 11 chapters. You're well prepared!**
> Get 6-7 hours of sleep tonight — a rested brain retains and recalls better than a tired one!
> **All the best for tomorrow's Management Accounting exam! 🏆**

---
*📅 Part 2 of Master Revision | Ch 7–11 | Management Accounting | DU SOL MBA Sem 2*
