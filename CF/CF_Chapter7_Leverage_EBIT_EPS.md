# 📘 Corporate Finance — Chapter 7: Leverage and EBIT-EPS Analysis
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** This is a highly numerical chapter. Master DOL, DFL, and DCL formulas and be able to compute them from an income statement. EBIT-EPS indifference point is almost certain to appear as a numerical. Understand what each leverage measure tells you about risk.

---

## 7.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Define and explain the concept of leverage
- ✅ Explain the Contribution-to-Sales (P/V) ratio and Break-Even Analysis
- ✅ Calculate and interpret Operating Leverage (DOL)
- ✅ Calculate and interpret Financial Leverage (DFL)
- ✅ Calculate and interpret Combined / Total Leverage (DCL)
- ✅ Conduct EBIT-EPS analysis and find the indifference point
- ✅ Solve practical problems involving all three leverage measures

---

## 7.2 Introduction

### What is Leverage?

In finance, **leverage** refers to the use of **fixed costs** (either operating or financial) to **amplify the effect of changes in sales/EBIT on profit/EPS**.

> 📌 *"Leverage is a double-edged sword — it magnifies gains in good times and magnifies losses in bad times."*

### Types of Leverage:

```
LEVERAGE
   │
   ├── OPERATING LEVERAGE (OL)
   │       → Fixed Operating Costs (rent, depreciation, salaries)
   │       → Measures: Sales → EBIT sensitivity
   │
   ├── FINANCIAL LEVERAGE (FL)
   │       → Fixed Financial Costs (interest on debt)
   │       → Measures: EBIT → EPS sensitivity
   │
   └── COMBINED / TOTAL LEVERAGE (CL)
           → Both fixed operating + financial costs
           → Measures: Sales → EPS sensitivity (full effect)
```

---

## 7.3 Concept of Leverage

### The Income Statement Framework

The income statement links all three leverages:

```
Sales Revenue                     ← Starting point
  (−) Variable Costs              ← Varies with sales
─────────────────────────────────
CONTRIBUTION                      ← Key intermediate metric
  (−) Fixed Operating Costs       ← Does NOT vary with sales
─────────────────────────────────
EBIT (Earnings Before Interest & Tax)
  (−) Interest                    ← Fixed financial cost
─────────────────────────────────
EBT (Earnings Before Tax)
  (−) Tax                         ← % of EBT
─────────────────────────────────
EAT (Net Profit / PAT)
  (−) Preference Dividend         ← Fixed (if any)
─────────────────────────────────
Earnings for Equity Shareholders
  (÷) No. of Equity Shares
─────────────────────────────────
EPS (Earnings Per Share)          ← End point
```

### Key Definitions:

| Term | Formula |
|---|---|
| **Contribution (C)** | Sales − Variable Costs |
| **P/V Ratio (C/S)** | Contribution / Sales × 100 |
| **Variable Cost Ratio** | Variable Costs / Sales = 1 − P/V Ratio |
| **EBIT** | Contribution − Fixed Operating Costs |
| **EBT** | EBIT − Interest |
| **EAT** | EBT × (1 − Tax Rate) |
| **EPS** | EAT / Number of Equity Shares |

---

## 7.4 Relations Between Sales and Profit

### P/V Ratio (Profit-Volume Ratio / Contribution-to-Sales Ratio)

```
P/V Ratio = Contribution / Sales = (Sales − Variable Costs) / Sales

P/V Ratio = (SP − VC per unit) / SP per unit   [per unit basis]

P/V Ratio = 1 − (Variable Cost Ratio)
```

> 💡 **Higher P/V Ratio → Each additional rupee of sales generates more contribution → Better profitability.**

### Break-Even Point (BEP)

The **BEP** is the level of sales at which **Total Revenue = Total Cost** (EBIT = 0, i.e., no profit no loss).

```
BEP (Units)  = Fixed Costs / Contribution per unit

BEP (₹ Sales) = Fixed Costs / P/V Ratio

OR: BEP (₹ Sales) = Fixed Costs × (Sales / Contribution)
```

### Margin of Safety (MOS)

```
Margin of Safety = Actual Sales − Break-Even Sales

MOS Ratio = Margin of Safety / Actual Sales × 100

Profit = MOS × P/V Ratio
```

> 📌 **Higher MOS → Firm is safer** (sales can fall more before making a loss).

### Relationship:

```
P/V Ratio × MOS Ratio = Net Profit Ratio (EBIT/Sales)
```

#### Full Example:
> Sales = ₹10,00,000; Variable Costs = ₹6,00,000; Fixed Costs = ₹2,00,000.

```
Contribution = 10,00,000 − 6,00,000 = ₹4,00,000
P/V Ratio    = 4,00,000 / 10,00,000 = 40%
EBIT         = 4,00,000 − 2,00,000  = ₹2,00,000
BEP (₹)      = 2,00,000 / 0.40      = ₹5,00,000
MOS          = 10,00,000 − 5,00,000 = ₹5,00,000
MOS Ratio    = 5,00,000 / 10,00,000 = 50%
```

---

## 7.5 Operating Leverage

### Definition

**Operating Leverage** measures the sensitivity of **EBIT to changes in Sales**. It arises from the presence of **fixed operating costs** in the cost structure.

> *High fixed costs → High DOL → A small change in sales causes a large change in EBIT.*

### Degree of Operating Leverage (DOL)

```
DOL = % Change in EBIT / % Change in Sales

DOL = Contribution / EBIT

DOL = (Sales − Variable Costs) / (Sales − Variable Costs − Fixed Operating Costs)

DOL = Q(SP − VC) / [Q(SP − VC) − FC]

Where:
  Q  = Quantity sold
  SP = Selling price per unit
  VC = Variable cost per unit
  FC = Fixed operating costs
```

> 📌 **At Break-Even Point: EBIT = 0 → DOL = ∞ (infinitely sensitive)**
> **As sales move far above BEP → DOL approaches 1 (less sensitive)**

### Interpretation of DOL:

| DOL Value | Meaning |
|---|---|
| **DOL = 2** | 1% increase in sales → 2% increase in EBIT |
| **DOL = 5** | 1% increase in sales → 5% increase in EBIT (high risk/reward) |
| **Higher DOL** | More fixed costs → More operating risk |
| **DOL = 1** | All variable costs — no operating leverage |

### DOL — Numerical Example:

> Sales = ₹10,00,000; VC = ₹6,00,000; FC = ₹2,00,000; EBIT = ₹2,00,000.

```
DOL = Contribution / EBIT
    = 4,00,000 / 2,00,000
    = 2

Interpretation: A 10% increase in sales will cause a 20% increase in EBIT.

Verification:
  New Sales = ₹11,00,000 (10% increase)
  New VC    = ₹6,60,000 (60% of sales — variable ratio constant)
  New Contribution = ₹4,40,000
  New EBIT  = 4,40,000 − 2,00,000 = ₹2,40,000
  % Change in EBIT = (2,40,000 − 2,00,000)/2,00,000 = 20% ✓
```

### What Determines DOL?

| Factor | Effect on DOL |
|---|---|
| Higher Fixed Costs | ↑ DOL (more operating leverage) |
| Higher Sales Volume | ↓ DOL (farther from BEP = safer) |
| Higher Contribution per Unit | ↓ DOL (EBIT rises faster relative to fixed costs) |

---

## 7.6 Financial Leverage

### Definition

**Financial Leverage** measures the sensitivity of **EPS (or EBT) to changes in EBIT**. It arises from the presence of **fixed financial costs** (interest) in the capital structure.

> *High debt → High interest → High DFL → A small change in EBIT causes a large change in EPS.*

### Degree of Financial Leverage (DFL)

```
DFL = % Change in EPS / % Change in EBIT

DFL = EBIT / (EBIT − Interest)

DFL = EBIT / EBT

[If preference dividend exists:]
DFL = EBIT / [EBIT − I − PD/(1−t)]

Where:
  I  = Annual interest on debt
  PD = Preference dividend (grossed up for tax since it's paid from post-tax profit)
  t  = Tax rate
```

> 📌 **With zero debt: DFL = 1** (EBIT change flows directly to EPS — no amplification)
> **DFL rises as debt (interest) increases**

### DFL — Numerical Example:

> EBIT = ₹2,00,000; Interest = ₹50,000; Tax = 30%; Shares = 10,000.

```
DFL = EBIT / (EBIT − Interest)
    = 2,00,000 / (2,00,000 − 50,000)
    = 2,00,000 / 1,50,000
    = 1.33

Interpretation: A 10% increase in EBIT → 13.3% increase in EPS.

Verification:
  Base EBT  = 1,50,000; EAT = 1,05,000; EPS = 10.50
  EBIT ↑10% → New EBIT = 2,20,000
  New EBT   = 2,20,000 − 50,000 = 1,70,000
  New EAT   = 1,70,000 × 0.70 = 1,19,000
  New EPS   = 11.90
  % Change in EPS = (11.90−10.50)/10.50 = 13.3% ✓
```

### What Determines DFL?

| Factor | Effect on DFL |
|---|---|
| Higher Interest (more debt) | ↑ DFL (more financial leverage) |
| Higher EBIT | ↓ DFL (interest is smaller relative to EBIT) |
| Zero Debt | DFL = 1 (no financial leverage) |

---

## 7.7 Combined Leverage

### Definition

**Combined (Total) Leverage** measures the sensitivity of **EPS to changes in Sales**. It captures the **combined effect of both operating and financial fixed costs**.

### Degree of Combined Leverage (DCL):

```
DCL = DOL × DFL

DCL = % Change in EPS / % Change in Sales

DCL = Contribution / (EBIT − Interest)

DCL = (Sales − Variable Costs) / (EBIT − Interest)

DCL = (Sales − VC) / (Sales − VC − FC − Interest)

[With preference dividend:]
DCL = Contribution / [EBIT − I − PD/(1−t)]
```

### DCL — Numerical Example:

> Continuing from above: Contribution = ₹4,00,000; EBIT = ₹2,00,000; Interest = ₹50,000.

```
DCL = Contribution / (EBIT − Interest)
    = 4,00,000 / (2,00,000 − 50,000)
    = 4,00,000 / 1,50,000
    = 2.67

Interpretation: A 10% increase in sales → 26.7% increase in EPS.

Verification via DOL × DFL:
  DOL = 2.0 × DFL = 1.33 = 2.67 ✓
```

### Leverage Relationship Summary:

```
% Change in EBIT = DOL × % Change in Sales
% Change in EPS  = DFL × % Change in EBIT
% Change in EPS  = DCL × % Change in Sales  =  DOL × DFL × % Change in Sales
```

---

### Comprehensive Leverage Summary Table:

| Feature | **Operating Leverage (DOL)** | **Financial Leverage (DFL)** | **Combined Leverage (DCL)** |
|---|---|---|---|
| **Measures** | Sales → EBIT sensitivity | EBIT → EPS sensitivity | Sales → EPS sensitivity |
| **Fixed Cost Used** | Fixed Operating Costs | Interest (Fixed Financial Cost) | Both |
| **Formula** | Contribution / EBIT | EBIT / EBT | DOL × DFL = Contribution / EBT |
| **Risk Type** | Operating / Business Risk | Financial Risk | Total / Combined Risk |
| **Minimum Value** | 1 (no fixed costs) | 1 (no debt) | 1 (no fixed costs, no debt) |
| **At BEP** | ∞ | — | ∞ |
| **High value means** | More operating risk | More financial risk | More total risk |

---

### Effect of Leverage on Risk-Return Trade-off:

```
HIGH LEVERAGE → Higher EPS in good times (↑ Sales)
             → Lower EPS or losses in bad times (↓ Sales)

LOW LEVERAGE → Stable EPS regardless of sales fluctuations
             → Misses upside potential

Management must balance: Leverage Benefit vs. Risk of Financial Distress
```

---

## 7.8 EBIT-EPS Analysis

*(Expanded from Chapter 6 — detailed numerical focus here)*

### Purpose

EBIT-EPS analysis compares alternative financing plans by examining how **EPS varies with EBIT** for each plan. Used to find:
1. **Indifference Point** — where both plans give equal EPS
2. **Which plan is better at a given EBIT level**

### Formula:

```
EPS = [(EBIT − Interest) × (1 − Tax)] − Preference Dividend
      ─────────────────────────────────────────────────────
                    Number of Equity Shares
```

### Indifference Point Calculation:

```
Set EPS_Plan A = EPS_Plan B and solve for EBIT*

[(EBIT* − I_A)(1−t) − PD_A] / n_A = [(EBIT* − I_B)(1−t) − PD_B] / n_B
```

---

## 7.9 Practical Problems — Worked Numericals

### Problem 1: Calculate DOL, DFL, DCL

> **Given:**
> - Selling Price per unit = ₹20
> - Variable Cost per unit = ₹12
> - Fixed Operating Costs = ₹40,000/yr
> - Output = 10,000 units
> - Interest on Debt = ₹20,000/yr
> - Tax Rate = 35%
> - Equity Shares = 5,000

**Step 1: Build Income Statement**
```
Sales Revenue    = 10,000 × 20    = ₹2,00,000
Variable Costs   = 10,000 × 12    = ₹1,20,000
                                  ───────────
Contribution     = 10,000 × 8     = ₹  80,000
Fixed Op. Costs  =                  ₹  40,000
                                  ───────────
EBIT             =                  ₹  40,000
Interest         =                  ₹  20,000
                                  ───────────
EBT              =                  ₹  20,000
Tax (35%)        =                  ₹   7,000
                                  ───────────
EAT              =                  ₹  13,000
EPS              = 13,000/5,000   =     ₹2.60
```

**Step 2: Calculate Leverage Measures**
```
DOL = Contribution / EBIT = 80,000 / 40,000 = 2.0

DFL = EBIT / EBT = 40,000 / 20,000 = 2.0

DCL = DOL × DFL = 2.0 × 2.0 = 4.0

OR: DCL = Contribution / EBT = 80,000 / 20,000 = 4.0 ✓
```

**Step 3: Interpret Results**
```
DOL = 2.0 → 10% increase in sales → 20% increase in EBIT
DFL = 2.0 → 10% increase in EBIT → 20% increase in EPS
DCL = 4.0 → 10% increase in sales → 40% increase in EPS
```

**Step 4: Break-Even Analysis**
```
BEP (units) = FC / (SP − VC) = 40,000 / (20−12) = 40,000 / 8 = 5,000 units
BEP (₹)     = 40,000 / 0.40 = ₹1,00,000

MOS = 10,000 − 5,000 = 5,000 units = ₹1,00,000 (50% of sales)
```

---

### Problem 2: EBIT-EPS Indifference Point

> **Company needs ₹15,00,000:**
> - **Plan I (All Equity)**: Issue 15,000 shares at ₹100
> - **Plan II (Debt + Equity)**: Borrow ₹6,00,000 at 10% p.a. + Issue 9,000 shares
> - **Existing shares**: 10,000
> - **Tax Rate**: 30%

**Setup:**

| | Plan I (Equity) | Plan II (Debt+Equity) |
|---|---|---|
| Total Shares | 10,000 + 15,000 = **25,000** | 10,000 + 9,000 = **19,000** |
| Interest | ₹0 | 10% × 6,00,000 = **₹60,000** |

**Indifference Point:**
```
EPS_I = EPS_II

[(EBIT − 0)(1 − 0.30)] / 25,000 = [(EBIT − 60,000)(1 − 0.30)] / 19,000

0.70 × EBIT / 25,000 = 0.70 × (EBIT − 60,000) / 19,000

[Note: 0.70 cancels from both sides]

19,000 × EBIT = 25,000 × (EBIT − 60,000)
19,000 × EBIT = 25,000 × EBIT − 15,00,00,000
15,00,00,000  = 6,000 × EBIT
EBIT*         = 15,00,00,000 / 6,000 = ₹2,50,000

∴ Indifference Point = EBIT* = ₹2,50,000
```

**Verification at EBIT = ₹2,50,000:**
```
Plan I:  EPS = (2,50,000 × 0.70) / 25,000 = 1,75,000 / 25,000 = ₹7.00
Plan II: EPS = [(2,50,000 − 60,000) × 0.70] / 19,000
             = [1,90,000 × 0.70] / 19,000
             = 1,33,000 / 19,000 = ₹7.00 ✓
```

**Decision Rule:**
```
If Expected EBIT > ₹2,50,000 → Plan II (Debt) gives HIGHER EPS
If Expected EBIT < ₹2,50,000 → Plan I (Equity) gives HIGHER EPS
If Expected EBIT = ₹2,50,000 → Indifferent between plans
```

---

### Problem 3: Effect of Leverage on Different EBIT Levels

> Using Problem 2 data, calculate EPS at EBIT = ₹1,00,000; ₹2,50,000; ₹4,00,000.

| EBIT | Plan I EPS | Plan II EPS | Better Plan |
|---|---|---|---|
| ₹1,00,000 | (1,00,000×0.70)/25,000 = **₹2.80** | (40,000×0.70)/19,000 = **₹1.47** | Plan I ✅ |
| ₹2,50,000 | (2,50,000×0.70)/25,000 = **₹7.00** | (1,90,000×0.70)/19,000 = **₹7.00** | Indifferent |
| ₹4,00,000 | (4,00,000×0.70)/25,000 = **₹11.20** | (3,40,000×0.70)/19,000 = **₹12.53** | Plan II ✅ |

```
EBIT-EPS Graph:
     EPS
      │                          ╱ Plan II (steeper slope = higher DFL)
  12  │                         ╱
      │                        ╱
   7  │──────────────────────X ← Indifference Point (₹2,50,000)
      │                 ╱────
      │            ╱────
      │       ╱────  Plan I (less steep = lower DFL)
      └────────────────────────────────► EBIT
           1L     2.5L     4L

Below X: Plan I (Equity) better (steeper loss for Plan II)
Above X: Plan II (Debt) better (steeper gain for Plan II)
```

---

## Summary

### 🔑 Key Takeaways — Chapter 7

| Concept | Key Point |
|---|---|
| **Leverage** | Use of fixed costs to amplify the effect of sales changes on profit/EPS |
| **Contribution** | Sales − Variable Costs; key metric for all leverage calculations |
| **P/V Ratio** | Contribution/Sales; higher = more profitable per sale |
| **BEP** | Fixed Costs / (SP−VC per unit); where profit = zero |
| **DOL** | Contribution/EBIT; measures sales→EBIT sensitivity; driven by fixed operating costs |
| **DFL** | EBIT/EBT; measures EBIT→EPS sensitivity; driven by interest |
| **DCL** | DOL × DFL = Contribution/EBT; total Sales→EPS sensitivity |
| **EBIT-EPS** | Compares financing plans; indifference point where EPS is equal |
| **Above indifference EBIT** | Debt plan gives higher EPS |
| **Below indifference EBIT** | Equity plan gives higher EPS |
| **High DOL** | More operating risk; near BEP is most dangerous |
| **High DFL** | More financial risk; fixed interest obligation amplifies EPS swings |

---

### ⚡ Master Formula Sheet

```
Contribution (C) = Sales − Variable Costs = Q × (SP − VC per unit)
P/V Ratio        = C / Sales
BEP (Units)      = FC / (SP − VC per unit)
BEP (₹)          = FC / P/V Ratio
MOS              = Actual Sales − BEP Sales
MOS Ratio        = MOS / Actual Sales

DOL = C / EBIT = Q(SP−VC) / [Q(SP−VC) − FC]
DFL = EBIT / EBT = EBIT / (EBIT − I)
    [With Pref Div]: DFL = EBIT / [EBIT − I − PD/(1−t)]
DCL = DOL × DFL = C / EBT = C / (C − FC − I)

EPS = [(EBIT − I)(1−t) − PD] / n

Indifference Point:
  [(EBIT* − I_A)(1−t)] / n_A = [(EBIT* − I_B)(1−t)] / n_B
  Solve for EBIT*

% Change in EBIT = DOL × % Change in Sales
% Change in EPS  = DFL × % Change in EBIT
% Change in EPS  = DCL × % Change in Sales
```

---

### 📝 Likely Exam Questions — Chapter 7

1. **What is Leverage? Distinguish between Operating, Financial, and Combined Leverage.**
2. **Define P/V Ratio and Break-Even Point. How are they calculated?**
3. **Calculate BEP, MOS, and P/V Ratio given sales, variable costs, and fixed costs.** *(Numerical)*
4. **Define Operating Leverage. Derive the formula for DOL and explain what it measures.**
5. **What is the significance of DOL? How does it relate to business risk?**
6. **Define Financial Leverage. Derive the formula for DFL. What happens to DFL when interest = 0?**
7. **Calculate DOL, DFL, and DCL from the following income statement data.** *(Numerical)*
8. **A 20% increase in sales leads to what % increase in EPS if DCL = 3.5?** *(Application)*
9. **Explain Combined Leverage. How is DCL related to DOL and DFL?**
10. **What is EBIT-EPS analysis? What is the indifference point and how is it calculated?**
11. **A company can raise ₹10 lakhs through equity or debt (10%). Find the EBIT-EPS indifference point.** *(Numerical)*
12. **Using the data from Q11, calculate EPS at three different EBIT levels and state which plan is better.** *(Numerical + Decision)*
13. **Draw and explain the EBIT-EPS graph showing the indifference point for two financing plans.**
14. **"Financial leverage is beneficial only when EBIT exceeds the indifference level." Explain with an example.**

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
