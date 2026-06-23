# 📘 Corporate Finance — Chapter 9: Working Capital Management
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** Working Capital is both theory and numerical. Master the Operating Cycle / Cash Conversion Cycle calculation, three WC policies (Conservative vs Aggressive), Baumol's Cash Management model, and Receivables Management (credit policy evaluation). These are high-frequency exam areas.

---

## 9.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Define Working Capital and classify it
- ✅ Explain the Operating Cycle and Cash Conversion Cycle
- ✅ Compare Conservative, Aggressive, and Moderate WC policies
- ✅ Explain the Risk-Return trade-off in WC management
- ✅ Apply Baumol and Miller-Orr models for cash management
- ✅ Evaluate credit policy changes using Receivables Management techniques

---

## 9.2 Introduction

### What is Working Capital?

**Working Capital** refers to the funds invested in **current assets** that are used in the **day-to-day operations** of the firm.

```
GROSS WORKING CAPITAL = Total Current Assets
                      = Cash + Marketable Securities + Debtors + Inventory + Prepaid Expenses

NET WORKING CAPITAL (NWC) = Current Assets − Current Liabilities
                           = Long-term funds invested in current assets
```

### Why is WC Management Critical?

| Reason | Explanation |
|---|---|
| **Liquidity** | Ensures firm can meet day-to-day obligations |
| **Profitability** | Too much WC = idle funds = lower returns |
| **Survival** | Cash crunch can bankrupt even profitable firms |
| **Efficiency** | Faster WC cycle = less funds locked up = higher returns |
| **Cost Management** | Reduces financing costs; optimises inventory and receivables |

> 📌 *"A firm may be profitable in the long run but fail in the short run due to poor working capital management."*

---

### Current Assets vs. Current Liabilities:

| **Current Assets** | **Current Liabilities** |
|---|---|
| Cash & Bank Balances | Creditors / Accounts Payable |
| Marketable Securities | Short-term Bank Borrowings |
| Debtors / Accounts Receivable | Outstanding Expenses |
| Inventory (RM, WIP, FG) | Advance received from customers |
| Prepaid Expenses | Provisions for Tax, Dividend |

---

## 9.3 Classification of Working Capital

### Classification 1: Gross vs. Net Working Capital

| Type | Definition |
|---|---|
| **Gross Working Capital (GWC)** | Total current assets; focus on efficient management of CA |
| **Net Working Capital (NWC)** | CA − CL; measures liquidity; focus on long-term funding of CA |

> 💡 **Positive NWC** = Long-term funds financing part of current assets = Safer but costlier.
> **Negative NWC** = Current liabilities > Current assets = Risky (short-term funds funding LT needs).

---

### Classification 2: Permanent vs. Temporary Working Capital

```
TOTAL WORKING CAPITAL
│
├── PERMANENT (FIXED) WORKING CAPITAL
│       → Minimum level of CA always maintained
│       → Remains constant regardless of business fluctuations
│       → Example: Minimum cash balance, minimum safety stock
│       → Should be financed by LONG-TERM sources
│
└── TEMPORARY (VARIABLE) WORKING CAPITAL
        → Fluctuates with seasonal/cyclical demand
        → Extra CA needed during peak seasons
        → Example: Extra inventory before Diwali, festival stock
        → Should be financed by SHORT-TERM sources
```

```
Current Assets (₹)
     │
     │     Temporary WC
     │   ╱╲╱╲╱╲╱╲  (fluctuates)
─────│──────────────────────────── Permanent WC level
     │   (constant minimum)
     └──────────────────────────────────────► Time
```

---

### Classification 3: By Concept

| Type | Definition |
|---|---|
| **Balance Sheet WC** | Based on accounting — difference between CA and CL |
| **Operating Cycle WC** | Based on time taken for cash to flow through operations |

---

## 9.4 Working Capital Policies and Management

### The Operating Cycle (OC)

**Definition**: The time period between the **purchase of raw materials** and the **collection of cash from customers**.

```
OPERATING CYCLE:

Cash → Raw Material → WIP → Finished Goods → Debtors → Cash

      ├──RM Storage──┤──Production──┤──FG Storage──┤──Collection──┤
      │              │              │               │              │
   Purchase of     RM converted   FG ready        Sale on      Cash
    Raw Material    to WIP        for sale         credit      received
```

### Components of Operating Cycle:

```
Operating Cycle (Days) =
  Raw Material Holding Period (RMHP)
+ Work-in-Progress Period (WIPP)
+ Finished Goods Holding Period (FGHP)
+ Debtors Collection Period (DCP)
− Creditors Payment Period (CPP)   [this is a spontaneous source — reduces WC need]
```

### Formulas for Each Component:

```
RMHP  = (Average RM Inventory / RM Consumed per day)
       = (Avg RM Stock / Annual RM Consumption) × 365

WIPP  = (Average WIP / Cost of Production per day)
       = (Avg WIP / Annual Cost of Production) × 365

FGHP  = (Average FG Inventory / Cost of Goods Sold per day)
       = (Avg FG Stock / Annual COGS) × 365

DCP   = (Average Debtors / Credit Sales per day)
       = (Avg Debtors / Annual Credit Sales) × 365

CPP   = (Average Creditors / Credit Purchases per day)
       = (Avg Creditors / Annual Credit Purchases) × 365

Gross Operating Cycle = RMHP + WIPP + FGHP + DCP
Net Operating Cycle   = Gross OC − CPP  (= Cash Conversion Cycle)
```

### Cash Conversion Cycle (CCC):

```
CCC = DCP + Inventory Days − CPP
    = Debtors Days + Inventory Days − Creditors Days

CCC = Days Sales Outstanding + Days Inventory Outstanding − Days Payable Outstanding
```

> 💡 **Lower CCC = Better** — Less time cash is tied up in operations = More efficient = Less WC needed.

#### Operating Cycle Example:
> Annual data: RM Consumption = ₹18L; WIP = ₹24L; COGS = ₹30L; Credit Sales = ₹40L; Credit Purchases = ₹18L
> Average balances: RM = ₹3L; WIP = ₹4L; FG = ₹5L; Debtors = ₹6L; Creditors = ₹3L

```
RMHP = (3/18) × 365 = 60.8 days ≈ 61 days
WIPP = (4/24) × 365 = 60.8 days ≈ 61 days
FGHP = (5/30) × 365 = 60.8 days ≈ 61 days
DCP  = (6/40) × 365 = 54.75 days ≈ 55 days
CPP  = (3/18) × 365 = 60.8 days ≈ 61 days

Gross OC = 61 + 61 + 61 + 55 = 238 days
Net OC   = 238 − 61 = 177 days (Cash Conversion Cycle)
```

---

### Working Capital Estimation — Requirement Calculation:

```
WC Requirement = Permanent WC + Temporary WC

Step 1: Estimate each CA (RM, WIP, FG, Debtors, Cash)
         using operating cycle periods × daily cost/sales

Step 2: Sum all CA = Gross WC

Step 3: Subtract CL (Creditors, Advance receipts)

Step 4: Net WC = Gross WC − CL
         Add safety margin (5–10%) for contingencies
```

---

## 9.4 (Cont'd): Working Capital Policies

Three strategies for financing current assets:

### Policy 1: Conservative (Matching / Hedging) Approach

```
Strategy: Finance ALL current assets (permanent + temporary) with LONG-TERM sources

CURRENT ASSETS:
  ├── Permanent CA    ← Financed by Long-term Debt + Equity ✅
  └── Temporary CA   ← Also financed by Long-term sources ✅

FIXED ASSETS        ← Financed by Long-term Debt + Equity ✅
```

**Characteristics:**
- Maintains high liquidity (large NWC buffer)
- **High current ratio**
- Higher cost (long-term funds are more expensive)
- Lower profitability (idle surplus funds during off-peak)

---

### Policy 2: Aggressive Approach

```
Strategy: Finance ALL current assets with SHORT-TERM sources
          (even permanent CA is funded by short-term debt)

CURRENT ASSETS:
  ├── Permanent CA    ← Financed by Short-term sources ⚠️
  └── Temporary CA   ← Financed by Short-term sources ⚠️

FIXED ASSETS        ← Financed by Long-term sources ✅
```

**Characteristics:**
- Low liquidity (small or negative NWC)
- **Low current ratio**
- Lower cost (short-term funds are cheaper)
- **Higher profitability** (minimises idle capital)
- **Higher risk** (refinancing risk; may face crisis if credit dries up)

---

### Policy 3: Moderate (Matching Principle) ✅ — Most Common

```
Strategy: Match maturity of financing with maturity of assets

CURRENT ASSETS:
  ├── Permanent CA    ← Long-term sources
  └── Temporary CA   ← Short-term sources

FIXED ASSETS        ← Long-term sources
```

**Characteristics:**
- Balanced risk and return
- Moderate liquidity and cost
- Practical and widely followed

---

### Policy Comparison Table:

| Feature | **Conservative** | **Moderate** | **Aggressive** |
|---|---|---|---|
| **CA Level** | High | Medium | Low |
| **Short-term financing** | Minimal | Moderate | Maximum |
| **NWC** | High (positive) | Moderate | Low / Negative |
| **Liquidity** | High | Medium | Low |
| **Profitability** | Low | Medium | High |
| **Risk** | Low | Medium | High |
| **Current Ratio** | High | Moderate | Low |
| **Best for** | Uncertain/seasonal demand | Most firms | Stable, predictable demand |

---

## 9.5 Risk-Return Trade-off in Working Capital

### Investment in Current Assets — Risk-Return:

| CA Level | Liquidity | Profitability | Risk |
|---|---|---|---|
| **High CA** | High | Low (idle funds) | Low |
| **Low CA** | Low | High (less idle) | High (stockout, credit risk) |

### Financing of Current Assets — Risk-Return:

| Financing | Cost | Risk | Profitability |
|---|---|---|---|
| **More ST Debt** | Low (cheaper) | High (refinancing risk) | High |
| **More LT Debt** | High (costlier) | Low (no rollover risk) | Low |

### Combined Effect:

```
Risk-Return Matrix:

                    FINANCING STRATEGY
              Conservative │ Moderate │ Aggressive
INVESTMENT  ──────────────┼──────────┼───────────
Conservative│ Lowest Risk │    ↓     │    ↓      │ Lowest Profit
            │             │          │           │
Moderate    │     ↑       │ Balanced │    ↓      │
            │             │          │           │
Aggressive  │     ↑       │    ↑     │Highest Risk│ Highest Profit
```

---

## 9.6 Cash Management

### Why Hold Cash? — Keynes' Three Motives:

| Motive | Explanation | Example |
|---|---|---|
| **Transaction Motive** | Cash needed for day-to-day payments | Paying salaries, suppliers, utilities |
| **Precautionary Motive** | Cash buffer for unexpected needs | Emergency repairs, sudden orders |
| **Speculative Motive** | Cash to take advantage of unexpected opportunities | Buying raw material when price drops |

> 💡 **Optimal Cash Balance** = Enough to meet needs (avoid shortage cost) without holding excess (avoid opportunity cost).

---

### Cash Management Goals:

```
1. Minimise idle cash (opportunity cost of holding cash)
2. Ensure sufficient liquidity (avoid transaction cost of raising emergency funds)
3. Speed up cash inflows (accelerate collections)
4. Slow down cash outflows (stretch payments within credit terms)
```

---

### Techniques to Accelerate Cash Collection:

| Technique | How It Works |
|---|---|
| **Prompt Invoicing** | Invoice immediately on delivery |
| **Cash Discounts** | Offer discount for early payment (e.g., 2/10 net 30) |
| **Lockbox System** | Regional collection centres; reduce postal float |
| **Electronic Payment** | NEFT/RTGS reduces collection time |
| **Factoring** | Sell receivables to a factor for immediate cash |

### Techniques to Slow Cash Outflows:

| Technique | How It Works |
|---|---|
| **Centralised Payment** | Delay disbursement using float |
| **Payable on Due Date** | Pay exactly on due date (not before) |
| **Negotiate Longer Credit** | Extend supplier credit terms |

---

### Model 1: Baumol's Cash Management Model

**Based on**: Economic Order Quantity (EOQ) logic applied to cash.

**Assumption**: Cash is used at a **steady, predictable rate**; cash is replenished by selling marketable securities.

**Goal**: Find the **optimal cash replenishment amount (C*)** that minimises total cost.

```
Total Cost = Holding Cost + Transaction Cost

Holding Cost    = (C/2) × k     [opportunity cost of holding average cash = C/2]
Transaction Cost = (T/C) × F   [no. of transactions × cost per transaction]

Where:
  C = Cash replenishment amount (decision variable)
  k = Opportunity cost (interest rate on marketable securities)
  T = Total cash needed for the period
  F = Fixed cost per transaction (brokerage, etc.)

Optimal Cash Balance (C*):
  C* = √(2 × F × T / k)

Minimum Total Cost:
  TC* = √(2 × F × T × k)

Average Cash Balance = C* / 2
Number of Transactions = T / C*
```

#### Baumol Model — Numerical Example:

> Total annual cash need T = ₹12,00,000; Opportunity cost k = 10% p.a.; Transaction cost F = ₹150 per transaction.

```
C* = √(2 × 150 × 12,00,000 / 0.10)
   = √(3,60,00,00,000 / 0.10)

Wait — let me recalculate properly:
C* = √(2 × 150 × 12,00,000 / 0.10)
   = √(2 × 150 × 12,00,000 / 0.10)
   = √(2 × 18,00,00,000)
   = √(36,00,00,000)

Let me redo step by step:
  Numerator: 2 × F × T = 2 × 150 × 12,00,000 = 36,00,00,000
  Denominator: k = 0.10
  Fraction: 36,00,00,000 / 0.10 = 360,00,00,000

C* = √(360,00,00,000) = ₹60,000

Holding Cost     = (60,000/2) × 0.10 = 30,000 × 0.10 = ₹3,000
Transaction Cost = (12,00,000/60,000) × 150 = 20 × 150 = ₹3,000
Total Cost       = 3,000 + 3,000 = ₹6,000 ✓ (Holding = Transaction at optimum)

Average Cash Balance = 60,000 / 2 = ₹30,000
Number of Transactions per year = 12,00,000 / 60,000 = 20 times
```

**Baumol Model Diagram:**
```
Cash Balance
C* = ₹60,000  │ ╲     ╲     ╲
               │  ╲     ╲     ╲
               │   ╲     ╲     ╲
Avg = ₹30,000  │────╲─────╲─────╲──── Average Level
               │    ╲    ╲    ╲
           0   └─────────────────────► Time
                 ↑     ↑     ↑
              Replenish at zero
```

**Limitation**: Assumes constant, predictable cash outflows — unrealistic for most firms.

---

### Model 2: Miller-Orr Model (Stochastic Cash Model)

**Designed for**: Firms with **uncertain / random daily cash flows**.

**Concept**: Set **Upper Control Limit (UCL)** and **Lower Control Limit (LCL)** with a **Return Point (RP)** in between.

```
Action Rules:
  If Cash Balance hits UCL → BUY marketable securities → Return to RP
  If Cash Balance hits LCL → SELL marketable securities → Return to RP
  If Cash between LCL and UCL → Do nothing
```

**Formulas:**
```
Spread (Z) = 3 × [(3/4) × F × σ² / k]^(1/3)

Where:
  F  = Fixed cost per transaction
  σ² = Variance of daily cash flows
  k  = Daily opportunity cost (annual rate / 365)

Upper Control Limit (UCL) = LCL + Z
Return Point (RP)         = LCL + Z/3
```

**Miller-Orr Diagram:**
```
Cash Balance
UCL ─────────────────────────────── ← Sell securities, return to RP
     ↓                  ↓
RP  ────────────────────────────────  ← Target
     ↑                  ↑
LCL ─────────────────────────────── ← Buy securities, return to RP
```

> The LCL is typically set by management as the minimum safety cash balance.

**Advantage over Baumol**: Handles uncertainty; more realistic for real-world firms.

---

## 9.7 Receivable Management

### What are Receivables?

**Receivables (Debtors)** = Amounts owed to the firm by customers who purchased goods/services on **credit**.

> Offering credit increases sales but creates risks: **Bad debts, collection costs, opportunity cost of tied-up funds.**

---

### Benefits vs. Costs of Extending Credit:

| **Benefits** | **Costs** |
|---|---|
| Increased sales volume | Opportunity cost (funds tied up in debtors) |
| Competitive advantage | Bad debt losses |
| Customer loyalty/retention | Collection and administration costs |
| Higher revenue/profit | Risk of customer default |

---

### Key Metrics for Receivables Management:

```
Debtors Turnover Ratio = Credit Sales / Average Debtors
Average Collection Period (ACP) = 365 / Debtors Turnover
                                 = Average Debtors / Daily Credit Sales
```

**Lower ACP = Better** (faster collection = less funds tied up).

---

### The 5 C's of Credit Analysis:

| C | Factor | Assessment |
|---|---|---|
| **Character** | Willingness to pay | Payment history, references |
| **Capacity** | Ability to pay (cash flow) | Income, financial statements |
| **Capital** | Financial strength | Net worth, assets |
| **Collateral** | Assets pledged as security | Property, equipment |
| **Conditions** | Economic/industry conditions | Recession impact on buyer |

---

### Credit Policy Variables:

A firm's credit policy has four dimensions:

| Variable | Decision |
|---|---|
| **Credit Standards** | Who qualifies for credit? (Tight = fewer bad debts but less sales; Loose = more sales but more bad debts) |
| **Credit Terms** | How long to pay? Cash discount offered? (e.g., "2/10 net 30" = 2% discount if paid in 10 days, full due in 30 days) |
| **Credit Limit** | Maximum credit extended per customer |
| **Collection Policy** | How aggressively to pursue overdue accounts |

---

### Evaluating a Change in Credit Policy (Incremental Analysis):

**Decision Rule**: Implement change if **Incremental Benefit > Incremental Cost**

```
Incremental Contribution = ΔSales × P/V Ratio (or Contribution Margin)

Incremental Investment in Debtors:
  For new sales:  ΔDebtors = (ΔSales × New ACP) / 365 × (VC/Sales ratio)
  For old sales:  ΔDebtors = Old Sales × (New ACP − Old ACP) / 365 × (TC/Sales ratio)

Opportunity Cost of ΔDebtors = ΔDebtors × Cost of Capital (k)

Incremental Bad Debt Cost  = New Bad Debt % × New Sales − Old Bad Debt % × Old Sales

Incremental Collection Cost = Change in admin/collection expenses

Net Benefit = Incremental Contribution − Incremental Opportunity Cost
              − Incremental Bad Debt − Incremental Collection Cost

Accept if Net Benefit > 0
```

#### Numerical Example — Credit Policy Change:
> **Current**: Sales = ₹20,00,000; ACP = 30 days; Bad Debt = 1%; VC ratio = 60%
> **Proposed**: Relax credit → Sales = ₹25,00,000; ACP = 45 days; Bad Debt = 2%
> Cost of Capital = 15%; Fixed Costs unchanged.

```
Incremental Contribution:
  ΔSales = 5,00,000; Contribution Margin = 40% (= 1 − VC ratio)
  ΔContribution = 5,00,000 × 0.40 = ₹2,00,000

Incremental Investment in Debtors:
  On New Sales (₹5,00,000 × 45/365 × 0.60) =  ₹36,986
  On Old Sales (₹20,00,000 × (45−30)/365 × TC/S)
  → TC/S = (VC + FC)/Sales; assume TC = VC here for simplicity
  On Old Sales (₹20,00,000 × 15/365 × 0.60) = ₹49,315
  Total ΔDebtors = 36,986 + 49,315 = ₹86,301

Opportunity Cost = 86,301 × 0.15 = ₹12,945

Incremental Bad Debt:
  New: 2% × 25,00,000 = ₹50,000
  Old: 1% × 20,00,000 = ₹20,000
  ΔBad Debt = ₹30,000

Net Benefit = 2,00,000 − 12,945 − 30,000 = ₹1,57,055 > 0 → ACCEPT ✅
```

---

### Cash Discount Analysis:

**Offering a cash discount** accelerates collection but has a cost:

```
Cost of NOT taking discount (Opportunity cost for customer):
  = [Discount % / (1 − Discount %)] × [365 / (Payment Period − Discount Period)]

Benefit of offering discount:
  = Reduction in investment in debtors × Cost of Capital

Accept discount offer if: Benefit > Cost of discount
```

---

### Collection Policy:

| Level of Aggressiveness | Effect |
|---|---|
| **Lenient** | Lower collection cost; higher bad debts; higher ACP |
| **Strict** | Higher collection cost; lower bad debts; lower ACP; may lose customers |

**Collection Tools**: Reminder letters → Phone calls → Collection agencies → Legal action.

---

## 9.8 Summary

### 🔑 Key Takeaways — Chapter 9

| Concept | Key Point |
|---|---|
| **Gross WC** | Total current assets; **Net WC** = CA − CL |
| **Permanent WC** | Minimum CA always needed → Finance with LT sources |
| **Temporary WC** | Seasonal fluctuations → Finance with ST sources |
| **Operating Cycle** | RMHP + WIPP + FGHP + DCP − CPP |
| **CCC** | Debtors Days + Inventory Days − Creditors Days; lower = better |
| **Conservative Policy** | High CA, LT financing; low risk, low return |
| **Aggressive Policy** | Low CA, ST financing; high risk, high return |
| **Moderate Policy** | Match asset maturity with financing maturity |
| **Baumol Model** | C* = √(2FT/k); minimises holding + transaction cost of cash |
| **Miller-Orr Model** | UCL/LCL/RP framework for uncertain cash flows |
| **Motives for Cash** | Transaction, Precautionary, Speculative |
| **5 C's of Credit** | Character, Capacity, Capital, Collateral, Conditions |
| **Credit Policy Change** | Accept if Incremental Contribution > Opportunity Cost + Bad Debt Cost |
| **ACP** | Average Debtors / Daily Credit Sales; lower = faster collection |

---

### ⚡ Master Formula Sheet

```
Net Working Capital:
  NWC = Current Assets − Current Liabilities

Operating Cycle:
  OC  = RMHP + WIPP + FGHP + DCP − CPP
  CCC = Debtor Days + Inventory Days − Creditor Days

Baumol's Model:
  C*  = √(2 × F × T / k)
  TC* = √(2 × F × T × k)
  Avg Cash = C*/2; No. of transactions = T/C*

Miller-Orr Model:
  Spread Z = 3 × [(3F × σ²) / (4k)]^(1/3)
  UCL = LCL + Z;   RP = LCL + Z/3

Receivables:
  Debtors Turnover = Credit Sales / Avg Debtors
  ACP = 365 / Debtors Turnover = Avg Debtors / (Credit Sales/365)

Credit Policy Evaluation:
  Net Benefit = ΔContribution − Opportunity Cost of ΔDebtors − ΔBad Debt − ΔCollection Cost
  Accept if Net Benefit > 0

Cost of NOT taking discount:
  = [d/(1−d)] × [365/(N−D)]
  Where d = discount%, N = net period, D = discount period
```

---

### 📝 Likely Exam Questions — Chapter 9

1. **Define Working Capital. Distinguish between Gross and Net Working Capital.**
2. **Explain Permanent and Temporary Working Capital with a diagram.**
3. **What is the Operating Cycle? How does it differ from the Cash Conversion Cycle?**
4. **Calculate the Operating Cycle and Net Working Capital requirement from the given data.** *(Numerical)*
5. **Compare Conservative, Aggressive, and Moderate WC policies. Which is most risky and why?**
6. **Explain the Risk-Return trade-off in Working Capital Management.**
7. **What are the three motives for holding cash? (Keynes)**
8. **Explain Baumol's Model for cash management. Derive the formula for optimal cash balance C*.**
9. **A company needs ₹15,00,000 annually in cash. Opportunity cost = 12%, Transaction cost = ₹200. Find C*, average balance, and total cost.** *(Numerical)*
10. **What is the Miller-Orr Model? How does it differ from Baumol's Model?**
11. **What are the components of a firm's Credit Policy? Explain the 5 C's of credit.**
12. **A firm is considering relaxing its credit standards: sales will increase by ₹5L, ACP from 30 to 45 days, bad debts rise from 1% to 2%. Evaluate the proposal.** *(Numerical)*
13. **What is a cash discount? How do you calculate the cost of NOT taking a discount?**
14. **Explain Collection Policy. What are the tools available for debt collection?**

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
