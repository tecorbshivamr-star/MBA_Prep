# 📐 DOC 2: Chapter-wise Formulas + 2 Solved Examples — Part 1 (Ch 1–6)
### Management Accounting | DU SOL MBA Sem 2

---

## 📦 CH 1: Cost Concepts

```
┌─────────────────────────────────────────────────────────────┐
│                    COST SHEET FORMULA                       │
│                                                             │
│  Prime Cost         = DM + DL + DE                         │
│  Works Cost         = Prime Cost + Factory Overhead         │
│  Cost of Production = Works Cost + Admin Overhead           │
│  Total Cost         = Cost of Production + Selling OH       │
│  Profit             = Selling Price − Total Cost            │
│                                                             │
│  DM = Direct Material | DL = Direct Labour                  │
│  DE = Direct Expenses | OH = Overhead                       │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Security Testing Project:**
| Item | ₹ |
|------|---|
| Direct Material (hardware) | 8,000 |
| Direct Labour (QA engineers) | 25,000 |
| Direct Expenses (subcontractor) | 5,000 |
| **Prime Cost** | **38,000** |
| Factory/Project Overhead | 7,000 |
| **Works Cost** | **45,000** |
| Admin Overhead | 5,000 |
| **Cost of Production** | **50,000** |
| Selling & Distribution OH | 3,000 |
| **Total Cost** | **53,000** |
| Profit (agreed) | 17,000 |
| **Invoice to Client** | **70,000** |

**Example 2 — Manufacturing Company (Shoe Factory):**
DM=₹200, DL=₹150, DE=₹50, Factory OH=₹100, Admin OH=₹60, Selling OH=₹40
```
Prime Cost         = 200+150+50         = ₹400
Works Cost         = 400+100            = ₹500
Cost of Production = 500+60             = ₹560
Total Cost         = 560+40             = ₹600
If Selling Price   = ₹750 → Profit      = ₹150 per pair
```

---

```
┌─────────────────────────────────────────────────────────────┐
│              RECONCILIATION OF ACCOUNTS                     │
│                                                             │
│  Profit (Cost A/c)                                          │
│  ADD:   Purely Financial Income (interest, dividend)        │
│  ADD:   Over-absorbed Overhead                              │
│  LESS:  Purely Financial Expenses (interest paid)           │
│  LESS:  Notional Charges in Cost A/c                        │
│  LESS:  Under-absorbed Overhead                             │
│  = Profit (Financial A/c)                                   │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero:**
Cost A/c Profit = ₹5,00,000. Bank interest received = ₹60,000.
Notional rent in Cost A/c = ₹30,000. Over-absorbed OH = ₹50,000.
```
Cost Profit          = ₹5,00,000
ADD: Interest recd   = + ₹60,000
ADD: Over-absorbed   = + ₹50,000
LESS: Notional rent  = − ₹30,000
Financial Profit     = ₹5,80,000 ✅
```

**Example 2 — Manufacturing Firm:**
Cost profit = ₹2,00,000. Dividend received = ₹20,000. Loss on asset sale = ₹15,000.
Under-absorbed OH = ₹10,000. Notional interest = ₹5,000.
```
Cost Profit              = ₹2,00,000
ADD: Dividend            = + ₹20,000
LESS: Loss on sale       = − ₹15,000
LESS: Under-absorbed OH  = − ₹10,000
LESS: Notional interest  = − ₹5,000
Financial Profit         = ₹1,90,000 ✅
```

---

## 📦 CH 2: Material, Labour & Overhead

```
┌─────────────────────────────────────────────────────────────┐
│                    STOCK LEVEL FORMULAS                     │
│                                                             │
│  ROL  = Max Consumption × Max Lead Time                     │
│  Min  = ROL − (Normal Consumption × Normal Lead Time)       │
│  Max  = ROL + EOQ − (Min Consumption × Min Lead Time)       │
│  Avg  = (Min Level + Max Level) ÷ 2                         │
│  Danger = Normal Consumption × Emergency Lead Time          │
│                                                             │
│  ROL = Reorder Level (when to order)                        │
│  LT  = Lead Time (time between order and delivery)          │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero USB Dongles:**
Max=50/week, Min=20/week, Normal=35/week. Max LT=4wk, Min=2wk, Normal=3wk.
EOQ=300. Emergency LT=1wk.
```
ROL     = 50 × 4          = 200 units
Min     = 200 − (35×3)    = 200−105 = 95 units
Max     = 200+300−(20×2)  = 500−40  = 460 units
Avg     = (95+460)÷2      = 277.5 units
Danger  = 35 × 1          = 35 units
```

**Example 2 — Pharma Company (Raw Material):**
Max=400 units/month, Min=150, Normal=280. Max LT=3months, Min=1, Normal=2. EOQ=1,800. Emergency LT=0.5month.
```
ROL     = 400×3           = 1,200 units
Min     = 1200−(280×2)    = 1200−560 = 640 units
Max     = 1200+1800−(150×1)= 3000−150 = 2,850 units
Avg     = (640+2850)÷2    = 1,745 units
Danger  = 280×0.5         = 140 units
```

---

```
┌─────────────────────────────────────────────────────────────┐
│                    EOQ FORMULA                              │
│                                                             │
│  EOQ = √(2 × A × O ÷ C)                                    │
│                                                             │
│  A = Annual Demand (units per year)                         │
│  O = Ordering Cost per order placed (₹)                    │
│  C = Carrying/Holding Cost per unit per year (₹)           │
│                                                             │
│  At EOQ: Total Ordering Cost = Total Carrying Cost          │
│  (This is the point of minimum total inventory cost)        │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Dongles:**
A=1,200/yr. O=₹500/order. C=₹2/unit/yr.
```
EOQ = √(2×1200×500÷2) = √(6,00,000) = 775 units
Orders/yr = 1200÷775 = 1.5 → 2 orders
Ordering Cost = 2×₹500 = ₹1,000
Avg Stock = 775÷2 = 387.5
Carrying Cost = 387.5×₹2 = ₹775 ≈ Min Total Cost
```

**Example 2 — Stationery Company:**
A=10,000 reams. O=₹250. C=₹5/ream/yr.
```
EOQ = √(2×10000×250÷5) = √(10,00,000) = 1,000 reams
Orders/yr = 10000÷1000 = 10 orders
Ordering Cost = 10×₹250 = ₹2,500
Avg Stock = 500 reams | Carrying = 500×₹5 = ₹2,500
Total Cost = ₹5,000 (minimum) ✅
```

---

```
┌─────────────────────────────────────────────────────────────┐
│              INCENTIVE WAGE PLAN FORMULAS                   │
│                                                             │
│  HALSEY PLAN:                                               │
│  Earnings = (Time Taken × Rate) + 50% × Time Saved × Rate  │
│  Time Saved = Standard Time − Actual Time                   │
│                                                             │
│  ROWAN PLAN:                                                │
│  Bonus    = (Time Saved ÷ Standard Time) × Time Taken × Rate│
│  Earnings = (Time Taken × Rate) + Bonus                     │
│                                                             │
│  TAYLOR'S DIFFERENTIAL PIECE RATE:                          │
│  Output ≥ Standard → Rate = 120% of Normal Piece Rate       │
│  Output < Standard → Rate = 80% of Normal Piece Rate        │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero QA Engineer (Halsey vs Rowan):**
Std=10hrs, Actual=7hrs, Rate=₹100/hr.
```
Time Saved = 10−7 = 3 hours | Basic = 7×₹100 = ₹700

HALSEY:
Bonus    = 50%×3×100 = ₹150
Earnings = ₹700+₹150 = ₹850

ROWAN:
Bonus    = (3÷10)×7×100 = 0.3×700 = ₹210
Earnings = ₹700+₹210 = ₹910

→ Rowan gives more (time saved 3 < 50% of std time 5)
```

**Example 2 — Taylor's Differential (Factory Worker):**
Standard=80 units/day. Normal rate=₹6/unit.
Worker A=100 units/day. Worker B=60 units/day.
```
Worker A (100 ≥ 80 → Efficient):
  Rate = 120%×₹6 = ₹7.20
  Wages = 100×₹7.20 = ₹720

Worker B (60 < 80 → Inefficient):
  Rate = 80%×₹6 = ₹4.80
  Wages = 60×₹4.80 = ₹288
```

---

```
┌─────────────────────────────────────────────────────────────┐
│           OVERHEAD ABSORPTION RATE (OAR)                    │
│                                                             │
│  OAR = Budgeted Overhead ÷ Budgeted Base (Activity)         │
│                                                             │
│  OH Absorbed = OAR × Actual Activity Level                  │
│                                                             │
│  Over-absorbed  = OH Absorbed − Actual OH (if positive)     │
│  Under-absorbed = Actual OH − OH Absorbed (if positive)     │
│                                                             │
│  Base can be: Machine Hours, Labour Hours, Units, % of Cost │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero (Machine Hour Rate):**
Budgeted OH=₹1,20,000. Budgeted Machine Hrs=6,000.
Actual Hrs=5,500. Actual OH=₹1,15,000.
```
OAR = 1,20,000÷6,000 = ₹20/machine hour
OH Absorbed = 5,500×₹20 = ₹1,10,000
Actual OH   = ₹1,15,000
Under-absorbed = 1,15,000−1,10,000 = ₹5,000 (Adverse → Debit P&L)
```

**Example 2 — Textile Factory (Labour Hour Rate):**
Budgeted OH=₹80,000. Budgeted Labour Hrs=16,000.
Actual Hrs=17,000. Actual OH=₹82,000.
```
OAR = 80,000÷16,000 = ₹5/labour hour
OH Absorbed = 17,000×₹5 = ₹85,000
Actual OH   = ₹82,000
Over-absorbed = 85,000−82,000 = ₹3,000 (Favourable → Credit P&L)
```

---

## 📦 CH 3: Contract Costing

```
┌─────────────────────────────────────────────────────────────┐
│             CONTRACT COSTING PROFIT FORMULA                 │
│                                                             │
│  Stage (%) = Work Certified ÷ Contract Price × 100          │
│                                                             │
│  Notional Profit = Work Certified − Cost of Work Certified  │
│  Cost of Work Cert = Total Cost to Date − WIP (Uncertified) │
│                                                             │
│  Stage < 25%   → Profit = NIL                               │
│  Stage 25–50%  → Profit = 1/3 × NP × (Cash ÷ Certified)    │
│  Stage 50–90%  → Profit = 2/3 × NP × (Cash ÷ Certified)    │
│  Stage > 90%   → Full estimated profit                      │
│                                                             │
│  NP = Notional Profit | Cash = Cash Received from client    │
│  Certified = Value of Work Certified                        │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Bank Contract:**
Contract Price=₹20L. Work Certified=₹12L. Total Cost to Date=₹8.8L.
WIP (Uncertified)=₹50K. Cash received=₹10.8L.
```
Stage = 12÷20×100 = 60% → Use 2/3 formula

Cost of Work Cert = 8.8L−0.5L = ₹8.3L
Notional Profit   = 12L−8.3L  = ₹3.7L

Profit to P&L = 2/3 × 3.7L × (10.8÷12)
              = 2/3 × 3.7L × 0.9
              = 2/3 × 3.33L = ₹2.22L ✅
```

**Example 2 — Construction Company:**
Contract Price=₹50L. Work Certified=₹15L. Cost to Date=₹12L.
WIP=₹1L. Cash received=₹13.5L.
```
Stage = 15÷50×100 = 30% → Use 1/3 formula

Cost of Work Cert = 12−1  = ₹11L
Notional Profit   = 15−11 = ₹4L

Profit to P&L = 1/3 × 4L × (13.5÷15)
              = 1/3 × 4L × 0.9
              = 1/3 × 3.6L = ₹1.2L ✅
```

---

## 📦 CH 4: Process Costing

```
┌─────────────────────────────────────────────────────────────┐
│              PROCESS COSTING FORMULAS                       │
│                                                             │
│  Normal Loss (units) = Normal Loss % × Input Units          │
│  Scrap Value of NL   = NL Units × Scrap Price               │
│                                                             │
│  Cost per Unit = (Total Input Cost − Scrap Value of NL)     │
│                  ÷ (Input Units − Normal Loss Units)         │
│                                                             │
│  Abnormal Loss = Actual Loss − Normal Loss                  │
│  Abnormal Gain = Normal Loss − Actual Loss                  │
│  (Both valued at Cost per Unit computed above)              │
│                                                             │
│  Equivalent Units (Weighted Avg):                           │
│  EU = Completed Units + (Closing WIP × % Completion)        │
│                                                             │
│  Cost per EU = (Opening WIP Cost + Current Cost) ÷ EU       │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Code Testing (Abnormal Loss):**
Input=1,000 builds. Cost=₹50,000. Normal Loss=10%. Scrap=₹2/build. Actual output=860 builds.
```
Normal Loss   = 10%×1000     = 100 builds
Scrap Value   = 100×₹2       = ₹200
Net Cost      = 50000−200    = ₹49,800
Cost per unit = 49800÷900    = ₹55.33/build

Actual Loss   = 1000−860     = 140 builds
Abnormal Loss = 140−100      = 40 builds
Value         = 40×₹55.33   = ₹2,213 (Charged to P&L as loss)
```

**Example 2 — Pharma (Abnormal Gain):**
Input=500 kg. Cost=₹25,000. Normal Loss=8%. Scrap=₹5/kg. Actual output=475 kg.
```
Normal Loss   = 8%×500       = 40 kg
Scrap Value   = 40×₹5        = ₹200
Net Cost      = 25000−200    = ₹24,800
Cost per unit = 24800÷460    = ₹53.91/kg

Actual Loss   = 500−475      = 25 kg
Abnormal Gain = 40−25        = 15 kg
Value         = 15×₹53.91   = ₹808.70 (Credited to P&L as gain)
```

---

## 📦 CH 5: Marginal Costing & BEP

```
┌─────────────────────────────────────────────────────────────┐
│         MARGINAL COSTING & BEP FORMULAS                     │
│                                                             │
│  Contribution (C) = Sales − Variable Cost                   │
│  Contribution (C) = Fixed Cost + Profit                     │
│  Profit           = Contribution − Fixed Cost               │
│                                                             │
│  P/V Ratio = Contribution ÷ Sales × 100                     │
│                                                             │
│  BEP (units) = Fixed Cost ÷ Contribution per Unit           │
│  BEP (₹)     = Fixed Cost ÷ P/V Ratio                      │
│                                                             │
│  MOS (₹)  = Actual Sales − BEP Sales                       │
│  MOS (%)  = MOS ÷ Actual Sales × 100                       │
│  Profit   = MOS × P/V Ratio                                 │
│  MOS      = Profit ÷ P/V Ratio                              │
│                                                             │
│  Target Sales = (FC + Target Profit) ÷ P/V Ratio           │
│                                                             │
│  FC = Fixed Cost | VC = Variable Cost per unit              │
│  CPU = Contribution per Unit = SP − VC                      │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Contracts:**
SP=₹1,00,000/contract. VC=₹40,000. FC=₹3,00,000/month. Actual=8 contracts.
```
Contribution/contract = 1,00,000−40,000 = ₹60,000
P/V Ratio             = 60,000÷1,00,000 = 60%

BEP (units) = 3,00,000÷60,000 = 5 contracts
BEP (₹)     = 3,00,000÷0.60   = ₹5,00,000

Actual Sales = 8×1,00,000 = ₹8,00,000
MOS (₹)      = 8,00,000−5,00,000 = ₹3,00,000
MOS (%)      = 3,00,000÷8,00,000 = 37.5%
Profit       = 3,00,000×60% = ₹1,80,000
Verify: (8×60,000)−3,00,000 = 4,80,000−3,00,000 = ₹1,80,000 ✅
```

**Example 2 — Textile Company:**
SP=₹500/unit. VC=₹300. FC=₹2,00,000. Actual sales=2,000 units. Target profit=₹1,50,000.
```
Contribution/unit = 500−300 = ₹200
P/V Ratio         = 200÷500 = 40%

BEP (units) = 2,00,000÷200 = 1,000 units
BEP (₹)     = 2,00,000÷0.40 = ₹5,00,000

MOS = 2000−1000 = 1,000 units (₹5,00,000 in value)
Profit = 1,000×200 = ₹2,00,000

Target Sales = (2,00,000+1,50,000)÷0.40 = 3,50,000÷0.40 = ₹8,75,000
Target Units = 3,50,000÷200 = 1,750 units ✅
```

---

## 📦 CH 6: Variance Analysis

```
┌─────────────────────────────────────────────────────────────┐
│              MATERIAL VARIANCE FORMULAS                     │
│                                                             │
│  MCV = (SQ × SP) − (AQ × AP)  = MPV + MUV                 │
│  MPV = AQ × (SP − AP)                                      │
│  MUV = SP × (SQ − AQ)                                      │
│                                                             │
│  SQ = Standard Qty for Actual Output | SP = Standard Price  │
│  AQ = Actual Quantity used | AP = Actual Price paid         │
│                                                             │
│  MPV Favourable → AP < SP (bought cheaper than planned)     │
│  MUV Favourable → AQ < SQ (used less material than planned) │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Dongles:**
Standard: 5 dongles/project at ₹10 each. Actual: 100 projects, used 520 dongles at ₹11 each.
```
SQ=500 | SP=₹10 | AQ=520 | AP=₹11

MCV = (500×10)−(520×11) = 5000−5720 = ₹720 Adverse
MPV = 520×(10−11)       = 520×(−1)  = ₹520 Adverse
MUV = 10×(500−520)      = 10×(−20)  = ₹200 Adverse
Check: 520+200 = ₹720 ✅
```

**Example 2 — Cloth Manufacturing:**
Standard: 3m fabric/unit at ₹80/m. Actual: 200 units, used 580m at ₹75/m.
```
SQ=600m | SP=₹80 | AQ=580m | AP=₹75

MCV = (600×80)−(580×75) = 48000−43500 = ₹4,500 Favourable
MPV = 580×(80−75) = 580×5 = ₹2,900 Favourable
MUV = 80×(600−580) = 80×20 = ₹1,600 Favourable
Check: 2900+1600 = ₹4,500 ✅
```

---

```
┌─────────────────────────────────────────────────────────────┐
│              LABOUR VARIANCE FORMULAS                       │
│                                                             │
│  LCV = (SH × SR) − (AH × AR)  = LRV + LEV                 │
│  LRV = AH × (SR − AR)                                      │
│  LEV = SR × (SH − AH)                                      │
│                                                             │
│  SH = Standard Hours for Actual Output | SR = Standard Rate │
│  AH = Actual Hours Worked | AR = Actual Rate paid per hour  │
│                                                             │
│  LRV Favourable → AR < SR (paid less per hour than planned) │
│  LEV Favourable → AH < SH (finished faster than planned)    │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero QA Engineers:**
Standard: 4 hrs/project at ₹500/hr. Actual: 50 projects, took 210 hrs at ₹520/hr.
```
SH=200 | SR=₹500 | AH=210 | AR=₹520

LCV = (200×500)−(210×520) = 1,00,000−1,09,200 = ₹9,200 Adverse
LRV = 210×(500−520) = 210×(−20) = ₹4,200 Adverse
LEV = 500×(200−210) = 500×(−10) = ₹5,000 Adverse
Check: 4200+5000 = ₹9,200 ✅
```

**Example 2 — Garment Factory:**
Standard: 2 hrs/shirt at ₹60/hr. Actual: 500 shirts, took 950 hrs at ₹55/hr.
```
SH=1000 | SR=₹60 | AH=950 | AR=₹55

LCV = (1000×60)−(950×55) = 60000−52250 = ₹7,750 Favourable
LRV = 950×(60−55) = 950×5 = ₹4,750 Favourable
LEV = 60×(1000−950) = 60×50 = ₹3,000 Favourable
Check: 4750+3000 = ₹7,750 ✅
```

---
*📅 Doc 2 Part 1 | Ch 1–6 Formulas + Examples | Management Accounting | DU SOL MBA Sem 2*
