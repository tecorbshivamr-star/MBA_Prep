# 📐 DOC 2: Chapter-wise Formulas + 2 Solved Examples — Part 2 (Ch 7–11)
### Management Accounting | DU SOL MBA Sem 2

---

## 📦 CH 7: Budgets & Budgetary Control

```
┌─────────────────────────────────────────────────────────────┐
│              PRODUCTION & PURCHASE BUDGET                   │
│                                                             │
│  Production (units) = Sales Units                           │
│                     + Closing Stock of Finished Goods       │
│                     − Opening Stock of Finished Goods       │
│                                                             │
│  Materials to Purchase = Usage for Production               │
│                        + Closing Stock of Materials         │
│                        − Opening Stock of Materials         │
│                                                             │
│  Usage for Production = Production Units × Material/unit    │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Quarterly Budget:**
Expected sales: 60 projects. Desired closing WIP: 10 projects. Opening WIP: 5 projects.
Each project needs 3 server-hours. Closing server stock wanted: 50 hrs. Opening: 20 hrs.
```
Production Budget:
  Sales units           =  60
  + Closing WIP         = +10
  − Opening WIP         = − 5
  Production Required   =  65 projects

Materials (Server Hours) Budget:
  Usage = 65×3          = 195 hrs
  + Closing stock       = + 50 hrs
  − Opening stock       = − 20 hrs
  Purchase Required     = 225 server-hours
```

**Example 2 — Furniture Company:**
Sales forecast: 500 chairs. Closing FG: 80 chairs. Opening FG: 30 chairs.
Each chair needs 4 kg wood. Closing wood stock: 200 kg. Opening wood stock: 100 kg.
```
Production Budget:
  Sales                 = 500
  + Closing FG          = + 80
  − Opening FG          = − 30
  Production            = 550 chairs

Material Budget:
  Usage = 550×4         = 2,200 kg
  + Closing stock       = + 200 kg
  − Opening stock       = − 100 kg
  Purchase              = 2,300 kg
```

---

```
┌─────────────────────────────────────────────────────────────┐
│               FLEXIBLE BUDGET FORMULA                       │
│                                                             │
│  Flexible Budget Cost = Fixed Cost                          │
│                       + (Variable Cost per unit × Actual    │
│                          Output)                            │
│                                                             │
│  Fixed Cost   = Unchanged regardless of output level        │
│  Variable Cost per unit = VC ÷ Budgeted units               │
│  Actual Output = Real output achieved in the period         │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero:**
Budgeted: 100 projects, VC=₹40,000/project, FC=₹5,00,000. Actual output: 80 projects. Actual cost: ₹38,00,000.
```
Flexible Budget = ₹5,00,000 + (₹40,000×80)
               = ₹5,00,000 + ₹32,00,000 = ₹37,00,000

Actual Cost     = ₹38,00,000
True Variance   = ₹38,00,000 − ₹37,00,000 = ₹1,00,000 Adverse
(Fixed Budget would wrongly show ₹40L−₹38L=₹2L Favourable!)
```

**Example 2 — Shoe Factory:**
Budgeted: 1,000 pairs, VC=₹300/pair, FC=₹1,00,000. Actual: 1,200 pairs. Actual cost: ₹4,60,000.
```
Flexible Budget = ₹1,00,000 + (₹300×1,200)
               = ₹1,00,000 + ₹3,60,000 = ₹4,60,000

Actual Cost     = ₹4,60,000
True Variance   = NIL (perfectly on budget at actual output!) ✅
```

---

## 📦 CH 8: Cost Management

```
┌─────────────────────────────────────────────────────────────┐
│         ACTIVITY-BASED COSTING (ABC) FORMULA                │
│                                                             │
│  Cost Driver Rate = Activity Cost Pool ÷ Total Driver Units │
│                                                             │
│  OH to Product = Cost Driver Rate × Product's Driver Units  │
│                                                             │
│  Activity Cost Pool = All costs related to one activity     │
│  Cost Driver Units  = Total occurrences of the driver       │
│  Product's Driver   = How many times product uses driver    │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero (3 Activities):**

| Activity | Pool Cost | Driver | Total Driver Units | Rate |
|---------|----------|--------|--------------------|------|
| Test Setup | ₹60,000 | No. of setups | 30 | ₹2,000/setup |
| Inspection | ₹90,000 | Inspection hours | 450 | ₹200/hr |
| Reporting | ₹30,000 | No. of reports | 100 | ₹300/report |

Product Alpha: 5 setups, 80 inspection hrs, 15 reports
```
OH = (5×2000)+(80×200)+(15×300)
   = 10,000+16,000+4,500 = ₹30,500
```

**Example 2 — Manufacturing Company (2 Products):**
Machine setup pool: ₹50,000 | 25 setups → Rate = ₹2,000/setup
Quality control pool: ₹40,000 | 200 inspections → Rate = ₹200/inspection

Product X: 8 setups, 60 inspections | Product Y: 17 setups, 140 inspections
```
OH to Product X = (8×2,000)+(60×200) = 16,000+12,000 = ₹28,000
OH to Product Y = (17×2,000)+(140×200) = 34,000+28,000 = ₹62,000
Total = ₹28,000+₹62,000 = ₹90,000 ✅
```

---

```
┌─────────────────────────────────────────────────────────────┐
│              TARGET COSTING FORMULA                         │
│                                                             │
│  Target Cost = Market Selling Price − Desired Profit Margin │
│                                                             │
│  Cost Gap = Current Estimated Cost − Target Cost            │
│  (If positive → must find ways to reduce cost!)             │
│                                                             │
│  Desired Profit = Market Price × Desired Profit %           │
│  Market Price = Competitive price customers will pay        │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Security Testing:**
Market price = ₹80,000. Desired profit = 25%. Current cost estimate = ₹70,000.
```
Desired Profit = 25%×80,000 = ₹20,000
Target Cost    = 80,000−20,000 = ₹60,000
Cost Gap       = 70,000−60,000 = ₹10,000 (must reduce!)
→ BugZero automates 40% of checks → saves ₹12,000 → now within target ✅
```

**Example 2 — Car Manufacturer:**
Market price = ₹8,00,000. Required margin = 20%. Current cost = ₹7,00,000.
```
Desired Profit = 20%×8,00,000 = ₹1,60,000
Target Cost    = 8,00,000−1,60,000 = ₹6,40,000
Cost Gap       = 7,00,000−6,40,000 = ₹60,000 (value engineering needed)
```

---

## 📦 CH 9 & 11: Performance Measures (ROI, RI, EVA)

```
┌─────────────────────────────────────────────────────────────┐
│         ROI, RESIDUAL INCOME & EVA FORMULAS                 │
│                                                             │
│  ROI = Net Profit ÷ Capital Employed × 100                  │
│                                                             │
│  RI  = Net Profit − (Capital Employed × Required Rate)      │
│  Positive RI → Creating value | Negative RI → Destroying    │
│                                                             │
│  EVA = NOPAT − (Capital Employed × WACC)                    │
│  NOPAT = Operating Profit × (1 − Tax Rate)                  │
│                                                             │
│  CE   = Capital Employed (Total Assets − Current Liabilities)│
│  WACC = Weighted Avg Cost of Capital (min expected return)  │
│  NOPAT = Net Operating Profit After Tax                     │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero Full Analysis:**
Net Profit=₹6L. Capital Employed=₹30L. Required Rate=15%. Operating Profit=₹8.57L. Tax=30%. WACC=12%.
```
ROI   = 6,00,000÷30,00,000×100 = 20%

RI    = 6,00,000−(30,00,000×15%)
      = 6,00,000−4,50,000 = ₹1,50,000 (Positive ✅)

NOPAT = 8,57,143×(1−0.30) = ₹6,00,000
EVA   = 6,00,000−(30,00,000×12%)
      = 6,00,000−3,60,000 = ₹2,40,000 (Creating real value ✅)
```

**Example 2 — Two Divisions Decision:**
Division A: Profit=₹5L, CE=₹20L, ROI=25%. New project: Profit=₹1L, CE=₹5L, ROI=20%. Required return=18%.
```
Division A current ROI = 25%

ROI Method (New Project ROI=20% < 25% Division):
→ Manager REJECTS project (lowers their division %) ❌ WRONG!

RI Method (New Project):
RI = 1,00,000−(5,00,000×18%) = 1,00,000−90,000 = ₹10,000 Positive
→ Manager ACCEPTS project (positive RI = value created) ✅ CORRECT!

∴ RI gives BETTER goal congruence
```

---

## 📦 CH 10: Inventory Valuation (Store Ledger)

```
┌─────────────────────────────────────────────────────────────┐
│           INVENTORY VALUATION METHODS                       │
│                                                             │
│  FIFO: Issue at OLDEST price first                          │
│        Closing Stock = at NEWEST (latest) prices            │
│        Rising prices → Highest Profit                       │
│                                                             │
│  LIFO: Issue at NEWEST price first                          │
│        Closing Stock = at OLDEST prices                     │
│        Rising prices → Lowest Profit                        │
│                                                             │
│  WAP:  WAP = Total Stock Value ÷ Total Stock Units          │
│        Recalculate EVERY time new receipt arrives           │
│        Issue at this average | Rising prices → Middle profit│
│                                                             │
│  Verification: Opening Value + Receipts = Issues + Closing  │
└─────────────────────────────────────────────────────────────┘
```

**Example 1 — BugZero USB Dongles (All 3 Methods):**

Transactions:
- Apr 1: Opening 100 units @ ₹20
- Apr 5: Received 200 units @ ₹25
- Apr 10: Issued 150 units
- Apr 30: Closing stock = 150 units

**FIFO:**
```
Issue 150 units:
  100 @ ₹20 = ₹2,000
   50 @ ₹25 = ₹1,250
Total Issue  = ₹3,250

Closing Stock = 150 @ ₹25 = ₹3,750
Verify: (100×20)+(200×25) = 2000+5000 = ₹7,000
        Issues + Closing = 3,250+3,750 = ₹7,000 ✅
```

**LIFO:**
```
Issue 150 units (newest first):
  150 @ ₹25 = ₹3,750
Total Issue  = ₹3,750

Closing Stock = 100@₹20 + 50@₹25 = 2,000+1,250 = ₹3,250
Verify: 3,750+3,250 = ₹7,000 ✅
```

**WAP:**
```
After Apr 5 receipt:
WAP = (100×20 + 200×25) ÷ (100+200)
    = (2,000+5,000) ÷ 300 = 7,000÷300 = ₹23.33/unit

Issue 150 @ ₹23.33 = ₹3,500
Closing 150 @ ₹23.33 = ₹3,500
Verify: 3,500+3,500 = ₹7,000 ✅
```

**Profit Comparison (Rising prices):**
```
Method | Issue Cost | Closing Stock | Effect
FIFO   | ₹3,250    | ₹3,750       | Highest Profit
WAP    | ₹3,500    | ₹3,500       | Middle Profit
LIFO   | ₹3,750    | ₹3,250       | Lowest Profit
```

**Example 2 — Pharma Store Ledger (WAP Focus):**
- Jan: Opening 50 units @ ₹100 = ₹5,000
- Jan 10: Received 100 units @ ₹120
- Jan 15: Issued 80 units
- Jan 20: Received 50 units @ ₹130
- Jan 25: Issued 60 units

```
After Jan 10 receipt:
  Stock = 150 units | Value = 5,000+(100×120) = ₹17,000
  WAP   = 17,000÷150 = ₹113.33/unit

Jan 15 Issue 80 @ ₹113.33 = ₹9,067
Remaining: 70 units @ ₹113.33 = ₹7,933

After Jan 20 receipt:
  Stock = 120 units | Value = 7,933+(50×130) = ₹14,433
  WAP   = 14,433÷120 = ₹120.28/unit

Jan 25 Issue 60 @ ₹120.28 = ₹7,217
Closing: 60 units @ ₹120.28 = ₹7,217

Verify: 5,000+12,000+6,500 = ₹23,500 (Total in)
        9,067+7,217+7,217  = ₹23,501 ≈ ₹23,500 ✅ (rounding)
```

---

## 📊 COMPLETE FORMULA QUICK-REFERENCE CARD

```
╔═══════════════════════════════════════════════════════════════╗
║              ALL FORMULAS — AT A GLANCE                      ║
╠═══════════════════════════════════════════════════════════════╣
║ CH1: Prime=DM+DL+DE | Works=Prime+FOH | Total=Works+AOH+SOH  ║
╠═══════════════════════════════════════════════════════════════╣
║ CH2: ROL=MaxC×MaxLT | Min=ROL−(NC×NLT) | EOQ=√(2AO/C)       ║
║      Halsey = Basic + 50%×Saved×Rate                         ║
║      Rowan  = Basic + (Saved÷Std)×Basic                      ║
║      OAR = Budgeted OH ÷ Budgeted Base                       ║
╠═══════════════════════════════════════════════════════════════╣
║ CH3: Stage=Cert÷Price×100 | NP=Cert−CostOfCert               ║
║      <25%=0 | 25-50%=1/3×NP×Cash/Cert | 50-90%=2/3×NP×C/C   ║
╠═══════════════════════════════════════════════════════════════╣
║ CH4: CPU=(InputCost−NLScrap)÷(Input−NLunits)                 ║
║      AL=ActualLoss−NL | AG=NL−ActualLoss (both ×CPU)         ║
║      EU(WA)=Completed+(ClosingWIP×%)                         ║
╠═══════════════════════════════════════════════════════════════╣
║ CH5: C=S−V | PV=C/S×100 | BEP(u)=FC/CPU | BEP(₹)=FC/PV     ║
║      MOS=Actual−BEP | Profit=MOS×PV | MOS=Profit/PV          ║
╠═══════════════════════════════════════════════════════════════╣
║ CH6: MCV=(SQ×SP)−(AQ×AP)=MPV+MUV                            ║
║      MPV=AQ(SP−AP) | MUV=SP(SQ−AQ)                          ║
║      LCV=(SH×SR)−(AH×AR)=LRV+LEV                            ║
║      LRV=AH(SR−AR) | LEV=SR(SH−AH)                          ║
╠═══════════════════════════════════════════════════════════════╣
║ CH7: Prod=Sales+ClFG−OpFG | Flex=FC+(VC/u×ActualOutput)      ║
╠═══════════════════════════════════════════════════════════════╣
║ CH8: ABC Rate=Pool÷Driver | TargetCost=Price−Profit           ║
║      Throughput=Sales−DirectMaterial                         ║
╠═══════════════════════════════════════════════════════════════╣
║ CH9: ROI=Profit/CE×100 | RI=Profit−(CE×Rate)                 ║
╠═══════════════════════════════════════════════════════════════╣
║ CH10: WAP=TotalValue÷TotalUnits (recalculate each receipt)    ║
║       FIFO=High Profit | LIFO=Low Profit | WAP=Middle         ║
╠═══════════════════════════════════════════════════════════════╣
║ CH11: EVA=NOPAT−(CE×WACC) | NOPAT=OpProfit×(1−TaxRate)       ║
╚═══════════════════════════════════════════════════════════════╝
```

---
> 💪 **All formulas covered with 2 real examples each!**
> **Best of luck for tomorrow's exam! You've prepared thoroughly! 🏆🔥**

---
*📅 Doc 2 Part 2 | Ch 7–11 Formulas + Examples | Management Accounting | DU SOL MBA Sem 2*
