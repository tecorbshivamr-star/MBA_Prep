# 📋 MASTER REVISION SHEET — Part 1 (Ch 1–6)
### Management Accounting | DU SOL MBA Sem 2 | Exam Tomorrow! 🔥

---

# 📘 CHAPTER 1: Cost Concepts in Accounting

## 🔑 Definitions

| Term | Definition | BugZero Analogy |
|------|-----------|----------------|
| **Management Accounting** | Providing financial + non-financial information to internal management for planning, control & decisions | QA Lead's dashboard showing cost per bug, team efficiency, sprint budget |
| **Cost** | The amount of money spent to produce a product or deliver a service | Cost of running BugZero's test environment for 1 month |
| **Direct Cost** | Cost that can be directly traced to a specific product/job | QA engineer's salary working 100% on one client project |
| **Indirect Cost (Overhead)** | Cost shared across multiple products; cannot be directly traced | Office electricity bill split across all teams |
| **Fixed Cost** | Cost that does NOT change with output level | Monthly office rent ₹1L — same whether 1 or 100 projects |
| **Variable Cost** | Cost that changes proportionately with output | Cloud server cost — more tests = more cost |
| **Semi-Variable Cost** | Has both fixed and variable components | Internet: ₹2,000 fixed + ₹500 per extra 10GB |
| **Sunk Cost** | Already spent, cannot be recovered — IGNORE in decisions | ₹3L spent on a useless tool BugZero already bought |
| **Opportunity Cost** | Value of the best alternative foregone | If QA team tests Module A, they can't test Module B |
| **Marginal Cost** | Cost of producing ONE additional unit | Cost of running 1 extra automated test in CI/CD |
| **Normal Loss** | Expected, unavoidable loss in production | 10% rejection rate in quality checks |
| **Abnormal Loss** | Loss OVER and above normal → charged to P&L | 20% rejection instead of expected 10% |

---

## 🔢 Key Formulas

### Cost Sheet (Build-Up Formula)
```
Prime Cost         = Direct Material + Direct Labour + Direct Expenses
Works Cost         = Prime Cost + Factory Overhead
Cost of Production = Works Cost + Administration Overhead
Total Cost         = Cost of Production + Selling & Distribution Overhead
Profit             = Selling Price − Total Cost
```

### Reconciliation of Cost & Financial Accounts
```
Profit as per Cost Accounts
  ADD:   Purely Financial Income (interest received, dividend, profit on asset sale)
  ADD:   Over-absorbed Overhead
  LESS:  Purely Financial Expenses (interest paid, loss on asset sale)
  LESS:  Notional Charges in Cost A/c (notional rent, notional interest)
  LESS:  Under-absorbed Overhead
= Profit as per Financial Accounts
```
> **Variables:** Over-absorbed = Cost A/c charged MORE overhead than actual | Notional = Hypothetical cost in Cost A/c only

---

## 🧠 Cost Classification Memory Trick
**"DFTBCNT"** → Direct/Indirect | Function | Time | Behavior | Controllability | Normality | Type (Decision)

---

# 📘 CHAPTER 2: Material, Labour & Overhead Cost

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Material Control** | System to ensure right material available at right time, right quantity, minimum cost |
| **EOQ** | Order quantity that minimizes TOTAL inventory cost (ordering + carrying) |
| **ABC Analysis** | Classify inventory by value: A (10% items, 70% value), B (20% items, 15% value), C (70% items, 5% value) |
| **Time Rate** | Wages paid per hour worked, regardless of output |
| **Piece Rate** | Wages paid per unit produced, regardless of time taken |
| **Overhead** | All indirect costs = Indirect Material + Indirect Labour + Indirect Expenses |
| **OAR** | Overhead Absorption Rate — rate at which overhead is charged to products |

---

## 🔢 Key Formulas

### Stock Levels (Memory: "**Really Mindful Managers Always Discuss**")
```
Reorder Level = Maximum Consumption × Maximum Lead Time
              [The point at which to place a new order]

Minimum Level = Reorder Level − (Normal Consumption × Normal Lead Time)
              [Safety stock — stock should never fall below this]

Maximum Level = Reorder Level + EOQ − (Minimum Consumption × Minimum Lead Time)
              [Stock should never exceed this]

Average Level = (Minimum Level + Maximum Level) ÷ 2
              [Normal stock level]

Danger Level  = Normal Consumption × Emergency Lead Time
              [Below this = production STOPS]
```

### EOQ Formula
```
EOQ = Square Root of (2 × A × O ÷ C)

Where:
  A = Annual Demand (units per year)
  O = Ordering Cost per order (₹ per order)
  C = Carrying/Holding Cost per unit per year (₹)

At EOQ: Total Ordering Cost = Total Carrying Cost (minimum total cost!)
```
> **BugZero:** Annual dongle demand = 1,200. Order cost = ₹500. Carry cost = ₹2/unit.
> EOQ = √(2×1200×500÷2) = √6,00,000 = **775 units**

---

### Wage Payment Systems

| System | Formula | BugZero Example |
|--------|---------|----------------|
| **Time Rate** | Hours Worked × Rate per Hour | 8 hrs × ₹200 = ₹1,600 |
| **Piece Rate** | Units Produced × Rate per Unit | 50 tests × ₹10 = ₹500 |
| **Taylor's Diff.** | Output ≥ Standard → 120% rate; Output < Standard → 80% rate | Standard = 100 tests; Worker does 120 → rate = ₹6 (120%×₹5) |

### Halsey Incentive Plan
```
Earnings = (Time Taken × Rate) + 50% × Time Saved × Rate

Where:
  Time Taken = Actual hours worked
  Rate       = Wage rate per hour
  Time Saved = Standard Time − Actual Time (must be positive)
  50%        = Worker gets half of time saved as bonus
```
> **BugZero:** Std = 10 hrs, Actual = 6 hrs, Rate = ₹100/hr
> Earnings = (6×100) + 50%×4×100 = ₹600 + ₹200 = **₹800**

### Rowan Incentive Plan
```
Earnings = (Time Taken × Rate) + (Time Saved ÷ Standard Time) × Time Taken × Rate

Bonus = Time Saved ÷ Standard Time × Basic Wages
      [Bonus is a PROPORTION of basic wages based on time saved]
```
> **BugZero Same Example:**
> Bonus = (4÷10) × 6 × ₹100 = 0.4 × ₹600 = ₹240
> Earnings = ₹600 + ₹240 = **₹840**

> **Halsey vs Rowan Rule:** If Time Saved < 50% of Standard Time → Rowan gives MORE bonus

---

### Overhead Absorption Rate (OAR)
```
OAR = Budgeted Overhead ÷ Budgeted Base (Activity Level)

Overhead Absorbed = OAR × Actual Activity

Over-Absorbed  = Absorbed OH > Actual OH → Credit P&L (good!)
Under-Absorbed = Absorbed OH < Actual OH → Debit P&L (bad!)
```

---

# 📘 CHAPTER 3: Job, Batch & Contract Costing

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Job Costing** | Each unique job gets a separate cost sheet; costs collected per job |
| **Batch Costing** | Group of identical units costed together; cost per unit = total÷units |
| **Contract Costing** | Long-term (1+ years), large-scale costing for projects at client's site |
| **Work Certified** | Value of work completed AND certified by architect/engineer |
| **Work Uncertified** | Work done but NOT yet certified → shown as WIP at cost |
| **Retention Money** | % of Work Certified held back by client until full completion |
| **Escalation Clause** | Contract price can be revised if material/labour prices rise beyond a limit |
| **Notional Profit** | Estimated profit on work done to date = Work Certified − Cost of Work Certified |

---

## 🔢 Key Formulas

### Contract Costing: Profit on Incomplete Contracts ⭐
```
Stage of Completion (%) = Work Certified ÷ Contract Price × 100

Notional Profit = Work Certified − Cost of Work Certified
Cost of Work Certified = Total Cost to Date − WIP (Uncertified Work)

PROFIT RECOGNITION RULES:
  Stage < 25%   → Profit to P&L = NIL (too early, too uncertain)
  Stage 25–50%  → Profit = 1/3 × Notional Profit × (Cash Received ÷ Work Certified)
  Stage 50–90%  → Profit = 2/3 × Notional Profit × (Cash Received ÷ Work Certified)
  Stage > 90%   → Full estimated profit (near complete)
```
> **Variables:**
> - **1/3 or 2/3** = Prudence — recognize less profit early when outcome is uncertain
> - **Cash Received ÷ Work Certified** = Adjusts for money not yet collected (retention)

> **BugZero:** ₹20L contract. Work Certified = ₹12L (60% stage). Notional Profit = ₹3.7L. Cash received = ₹10.8L.
> Profit = 2/3 × 3.7L × (10.8÷12) = 2/3 × 3.7L × 0.9 = **₹2.22L to P&L**

### Memory Trick for Profit Rules: **"Nothing → 1/3 → 2/3 → Full"**

---

# 📘 CHAPTER 4: Process Costing

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Process Costing** | Costs accumulated for each process stage; cost per unit = total cost ÷ output |
| **Normal Loss** | Expected, pre-estimated loss in a process; absorbed by good output |
| **Abnormal Loss** | Actual loss EXCEEDS normal loss → extra loss charged to P&L (debit) |
| **Abnormal Gain** | Actual loss is LESS than normal loss → saving credited to P&L |
| **Equivalent Units** | WIP expressed as equivalent fully-complete units based on % completion |
| **Joint Products** | Two or more significant products from the same process up to split-off point |
| **By-Products** | Minor value product produced incidentally alongside the main product |

---

## 🔢 Key Formulas

### Process Account Calculations
```
Normal Loss (units)   = Normal Loss % × Input Units
Scrap Value of NL     = Normal Loss Units × Scrap Price per unit

Cost per Unit = (Total Input Cost − Scrap Value of Normal Loss)
                ÷ (Input Units − Normal Loss Units)
              [Cost spread over EXPECTED good output only]

Abnormal Loss = Actual Loss − Normal Loss [Both valued at Cost per Unit]
Abnormal Gain = Normal Loss − Actual Loss [Both valued at Cost per Unit]
```

> **BugZero Analogy:** Testing pipeline expects 10% failure (Normal Loss). If 15% fail → Abnormal Loss = 5% extra failures (charged to P&L). If only 7% fail → Abnormal Gain = 3% better than expected (credited to P&L)!

### Equivalent Production (WIP Valuation)
```
WEIGHTED AVERAGE METHOD:
Equivalent Units = Completed Units + (Closing WIP × % of Completion)

Cost per EU = (Opening WIP Cost + Current Period Cost) ÷ Equivalent Units

FIFO METHOD:
Equivalent Units = (Opening WIP × % remaining to complete)
                  + Units started & completed this period
                  + (Closing WIP × % of Completion)
```

### Joint Cost Apportionment
```
By Sales Value = Joint Cost × (Sales Value of Product ÷ Total Sales Value of all products)
By NRV        = Joint Cost × (NRV of Product ÷ Total NRV)
NRV           = Final Selling Price − Further Processing Cost after split-off
```

---

# 📘 CHAPTER 5: Cost Concepts in Decision Making

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Marginal Costing** | Only variable costs charged to products; fixed costs = period cost written off entirely |
| **Contribution** | Amount each unit contributes toward fixed costs then profit |
| **P/V Ratio** | % of each rupee of sales that is contribution (profit-volume ratio) |
| **BEP** | Level of sales where Total Revenue = Total Cost (zero profit, zero loss) |
| **Margin of Safety** | Amount actual sales EXCEED break-even sales — the safety buffer |
| **Absorption Costing** | Both fixed AND variable costs charged to products |
| **Relevant Cost** | Future cost that CHANGES with a decision — include in analysis |
| **Irrelevant Cost** | Cost that does NOT change with decision (sunk cost, unavoidable fixed) — IGNORE |

---

## 🔢 Key Formulas ⭐⭐⭐

### Contribution & P/V Ratio
```
Contribution        = Sales − Variable Cost
Contribution        = Fixed Cost + Profit
Profit              = Contribution − Fixed Cost

P/V Ratio (%)       = Contribution ÷ Sales × 100
                    = (Sales − Variable Cost) ÷ Sales × 100
                    = Change in Profit ÷ Change in Sales × 100
```

### Break-Even Point (BEP)
```
BEP in Units        = Fixed Cost ÷ Contribution per Unit
                    [Fixed Cost = ₹60,000 | Contribution/unit = ₹80 → BEP = 750 units]

BEP in ₹ (Value)   = Fixed Cost ÷ P/V Ratio
                    [Fixed Cost = ₹60,000 | P/V = 40% → BEP = ₹1,50,000]

Where:
  Fixed Cost        = Total fixed costs for the period
  Contribution/unit = Selling Price per unit − Variable Cost per unit
  P/V Ratio         = Contribution ÷ Sales (as a decimal or %)
```

### Margin of Safety (MOS)
```
MOS in ₹    = Actual Sales − BEP Sales
MOS %       = (Actual Sales − BEP Sales) ÷ Actual Sales × 100
Profit      = MOS × P/V Ratio
MOS         = Profit ÷ P/V Ratio
```
> **BugZero:** FC=₹60K, Contribution/unit=₹80, Actual sales=1,000 units
> BEP=750 units | MOS=250 units | Profit=250×₹80=₹20,000

### Target Sales
```
Sales to Achieve Target Profit = (Fixed Cost + Target Profit) ÷ P/V Ratio
Units for Target Profit         = (Fixed Cost + Target Profit) ÷ Contribution per Unit
```

### Marginal vs Absorption Profit Difference
```
Difference = Change in Stock × Fixed Overhead per Unit

If Closing Stock > Opening Stock → Absorption Profit > Marginal Profit
If Closing Stock < Opening Stock → Marginal Profit > Absorption Costing Profit
```

---

## 🔢 Decision-Making Rules

| Decision | Rule | BugZero Example |
|---------|------|----------------|
| **Make or Buy** | Compare Variable Cost of Making vs Buy Price; ignore unavoidable fixed costs | If making costs ₹45 and buying costs ₹60 → MAKE |
| **Accept Special Order** | Accept if Price > Variable Cost (positive contribution); ignore fixed costs if spare capacity | Client offers ₹55K, Variable Cost=₹40K → ACCEPT (₹15K contribution) |
| **Key Factor / Limiting Factor** | Rank by Contribution per unit of scarce resource (NOT total contribution) | 200 QA hours: rank projects by ₹ contribution per hour |
| **Shut Down** | Continue if Contribution > 0; Shut only if Contribution ≤ 0 or avoidable FC > Contribution | Division earns ₹50K contribution → CONTINUE even if net loss |

### Key Factor Ranking Formula
```
Ranking = Contribution per Unit ÷ Units of Scarce Resource per Unit
         [Allocate scarce resource starting from highest rank]
```

---

# 📘 CHAPTER 6: Standard Costing & Variance Analysis

## 🔑 Definitions

| Term | Definition |
|------|-----------|
| **Standard Cost** | Pre-determined cost of producing one unit under efficient conditions |
| **Variance** | Difference between Standard (what SHOULD happen) and Actual (what DID happen) |
| **Favourable (F)** | Actual cost < Standard cost (spent LESS than planned — good!) |
| **Adverse (A)** | Actual cost > Standard cost (spent MORE than planned — bad!) |

---

## 🔢 Variance Formulas ⭐⭐⭐

### Abbreviations
```
SP = Standard Price per unit of material
AP = Actual Price per unit of material
SQ = Standard Quantity of material for ACTUAL output produced
AQ = Actual Quantity of material used
SR = Standard Rate (wage per hour)
AR = Actual Rate (actual wage per hour paid)
SH = Standard Hours for ACTUAL output produced
AH = Actual Hours worked
```

### Material Variances
```
Material Cost Variance (MCV)  = (SQ × SP) − (AQ × AP)
                               = Standard Cost of Actual Output − Actual Cost

Material Price Variance (MPV) = AQ × (SP − AP)
                               [Caused by paying different price than standard]
                               Favourable → AP < SP (bought cheaper!)

Material Usage Variance (MUV) = SP × (SQ − AQ)
                               [Caused by using more/less material than standard]
                               Favourable → Used LESS material than expected

CHECK: MCV = MPV + MUV ✅
```

### Labour Variances
```
Labour Cost Variance (LCV)      = (SH × SR) − (AH × AR)
                                 = Standard Labour Cost − Actual Labour Cost

Labour Rate Variance (LRV)      = AH × (SR − AR)
                                 [Caused by paying different wage than standard]
                                 Favourable → AR < SR (paid less per hour)

Labour Efficiency Variance (LEV)= SR × (SH − AH)
                                 [Caused by taking more/less time than standard]
                                 Favourable → AH < SH (finished faster!)

CHECK: LCV = LRV + LEV ✅
```

### Fixed Overhead Variances
```
Standard FOH Rate = Budgeted Fixed OH ÷ Budgeted Hours (or Units)
Absorbed FOH      = Standard Hours for Actual Output × Standard FOH Rate

FOH Cost Variance         = Absorbed FOH − Actual FOH
FOH Expenditure Variance  = Budgeted FOH − Actual FOH
                           [Caused by spending more/less than budget]
FOH Volume Variance       = Absorbed FOH − Budgeted FOH
                           [Caused by producing more/less than budgeted]
FOH Efficiency Variance   = Standard FOH Rate × (SH − AH)
FOH Capacity Variance     = Standard FOH Rate × (AH − Budgeted Hours)

CHECK: FOH Cost = Expenditure + Volume ✅
CHECK: FOH Volume = Efficiency + Capacity ✅
```

### Sales Variances
```
Sales Value Variance  = Actual Sales Value − Budgeted Sales Value
Sales Price Variance  = Actual Quantity × (Actual Price − Standard Price)
                       Favourable → Sold at HIGHER price than planned
Sales Volume Variance = Standard Price × (Actual Quantity − Budgeted Quantity)
                       Favourable → Sold MORE units than planned

CHECK: Sales Value = Price Variance + Volume Variance ✅
```

### Quick Solved Example (Material)
```
Standard: 5 kg/unit at ₹10/kg. Actual: 100 units, used 520 kg at ₹11/kg.

SQ = 5×100 = 500 kg  |  AQ = 520 kg  |  SP = ₹10  |  AP = ₹11

MCV = (500×10) − (520×11) = 5,000 − 5,720 = ₹720 Adverse
MPV = 520 × (10−11)       = 520 × (−1)    = ₹520 Adverse
MUV = 10 × (500−520)      = 10 × (−20)    = ₹200 Adverse
Check: 520 + 200 = ₹720 ✅
```

---

## 🧠 Variance Memory Tricks
- **Material:** "MCV = MPV + MUV" → Cost = Price + Usage
- **Labour:** "LCV = LRV + LEV" → Cost = Rate + Efficiency
- **Favourable** = Actual BETTER than Standard (saved money or time)
- **Adverse** = Actual WORSE than Standard (spent more or took longer)

---

# 📊 PART 1 MASTER FORMULA CARD

```
┌─────────────────────────────────────────────────────────────────────┐
│ CH1: Prime Cost = DM+DL+DE | Works = Prime+FOH | Total = Works+AOH+SOH│
├─────────────────────────────────────────────────────────────────────┤
│ CH2: ROL=MaxCons×MaxLT | Min=ROL−(NormCons×NormLT)                 │
│      EOQ=√(2AO/C) | Halsey=Basic+50%×Saved×Rate                    │
│      Rowan=Basic+(Saved/Std)×Basic | OAR=Budgeted OH/Budgeted Base  │
├─────────────────────────────────────────────────────────────────────┤
│ CH3: Profit on Contract:                                            │
│      <25%=Nil | 25-50%=1/3×NP×Cash/Cert | 50-90%=2/3×NP×Cash/Cert │
├─────────────────────────────────────────────────────────────────────┤
│ CH4: Cost/unit=(InputCost−NLScrap)÷(Input−NL units)                │
│      Eq.Units(WA)=Completed+(ClosingWIP×%)                          │
├─────────────────────────────────────────────────────────────────────┤
│ CH5: Contribution=S−V | P/V=C/S×100 | BEP(units)=FC/CPU            │
│      BEP(₹)=FC/PV | MOS=Actual−BEP | Profit=MOS×PV                │
├─────────────────────────────────────────────────────────────────────┤
│ CH6: MCV=(SQ×SP)−(AQ×AP)=MPV+MUV                                   │
│      MPV=AQ(SP−AP) | MUV=SP(SQ−AQ)                                 │
│      LCV=(SH×SR)−(AH×AR)=LRV+LEV                                   │
│      LRV=AH(SR−AR) | LEV=SR(SH−AH)                                 │
└─────────────────────────────────────────────────────────────────────┘
```

---
*📅 Part 1 of Master Revision | Ch 1–6 | Management Accounting | DU SOL MBA Sem 2*
