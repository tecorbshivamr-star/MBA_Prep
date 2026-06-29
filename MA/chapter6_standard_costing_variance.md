# 📘 Chapter 6: Standard Costing and Variance Analysis
### Management Accounting | DU SOL | 2nd Semester
> ⭐ **Formula-Heavy Chapter — Learn the variance tree cold!**

---

## 🎯 Learning Objectives
- Define Standard Cost and Standard Costing
- Understand types of standards
- Calculate **Material, Labour, Overhead and Sales Variances**
- Identify Favourable (F) vs Adverse/Unfavourable (A) variances

---

## 6.2 Introduction

> In business, **plans are made in advance** (standards). Reality is often different.
> **Variance Analysis** = Comparing what **SHOULD HAVE happened** vs what **ACTUALLY happened**, and finding out **WHY** there's a difference.

### 🧠 BugZero Analogy
BugZero estimates each testing contract takes **40 hours at ₹500/hour = ₹20,000 standard cost**.
Reality: It took **50 hours at ₹480/hour = ₹24,000 actual cost**.
**Variance = ₹4,000 Adverse** — the project cost more than planned. Why?
- Was it because the rate was different? (Price Variance)
- Was it because more hours were used? (Efficiency Variance)
→ That's Variance Analysis!

---

## 6.3 Standard Cost

> **Standard Cost** = A **pre-determined/estimated cost** of producing one unit of product under **efficient operating conditions**.

It is set **before** production begins, based on:
- Engineering specifications
- Historical data
- Management expectations

### 📌 Types of Standards

| Type | Description | Nature |
|------|-------------|--------|
| **Ideal Standard** | Perfect efficiency, no wastage, no idle time | Theoretical, rarely achieved |
| **Normal Standard** | Based on average past performance | Realistic over long term |
| **Current Standard** | Set for current period's expected conditions | Most practical |
| **Basic Standard** | Fixed standard set long ago, unchanged | Used as a base for comparison |

> ✅ **Most commonly used: Current Standard** (reflects today's realistic conditions)

---

## 6.4 Standard Costing

> **Standard Costing** = A system where **standard costs are pre-determined**, actual costs are recorded, and **variances are calculated and analyzed** to improve efficiency and control costs.

### 📌 Objectives
1. **Cost Control** — Compare actual vs standard, investigate variances
2. **Performance Measurement** — Rate departments/managers
3. **Budgeting** — Standards form the basis for budgets
4. **Simplify Costing** — Standard prices simplify stock valuation
5. **Decision Making** — Standard costs aid pricing decisions

### ✅ Advantages
- Highlights inefficiencies quickly
- Motivates employees through targets
- Simplifies bookkeeping
- Basis for management by exception

### ❌ Limitations
- Expensive and time-consuming to set up
- Standards become outdated quickly
- May demotivate if standards are too tight
- Not suitable for non-standard/custom work

---

## 6.5 Classification of Variances ⭐⭐⭐

### 🌳 Master Variance Tree

```
TOTAL COST VARIANCE
│
├── MATERIAL COST VARIANCE (MCV)
│   ├── Material Price Variance (MPV)
│   └── Material Usage Variance (MUV)
│       ├── Material Mix Variance (MMV)
│       └── Material Yield Variance (MYV)
│
├── LABOUR COST VARIANCE (LCV)
│   ├── Labour Rate Variance (LRV)
│   └── Labour Efficiency Variance (LEV)
│       ├── Labour Mix Variance (LMV)
│       └── Labour Idle Time Variance (LITV)
│
├── OVERHEAD VARIANCE
│   ├── Fixed OH Variance
│   │   ├── FOH Expenditure Variance
│   │   └── FOH Volume Variance
│   │       ├── FOH Efficiency Variance
│   │       └── FOH Capacity Variance
│   └── Variable OH Variance
│       ├── VOH Expenditure Variance
│       └── VOH Efficiency Variance
│
└── SALES VARIANCE
    ├── Sales Price Variance
    └── Sales Volume Variance
```

### 📌 Golden Rule: Favourable vs Adverse

```
FAVOURABLE (F)  = Actual Cost < Standard Cost  → GOOD (saved money)
ADVERSE (A)     = Actual Cost > Standard Cost  → BAD (spent more)

For Sales Variances:
FAVOURABLE (F)  = Actual > Standard/Budgeted   → More revenue = GOOD
ADVERSE (A)     = Actual < Standard/Budgeted   → Less revenue = BAD
```

---

### 📌 Key Abbreviations

```
SP  = Standard Price per unit
AP  = Actual Price per unit
SQ  = Standard Quantity for ACTUAL output
AQ  = Actual Quantity used
SR  = Standard Rate per hour (labour)
AR  = Actual Rate per hour (labour)
SH  = Standard Hours for ACTUAL output
AH  = Actual Hours worked
```

---

## A) MATERIAL VARIANCES ⭐⭐⭐

---

### 1️⃣ Material Cost Variance (MCV) — The Total

```
MCV = (SQ × SP) − (AQ × AP)
    = Standard Cost of Actual Output − Actual Cost

MCV = MPV + MUV
```

---

### 2️⃣ Material Price Variance (MPV)

> Caused by **difference in price** paid vs standard price.

```
MPV = AQ × (SP − AP)

Favourable  → Actual Price < Standard Price (bought cheaper)
Adverse     → Actual Price > Standard Price (paid more)
```

---

### 3️⃣ Material Usage Variance (MUV)

> Caused by **difference in quantity** used vs standard quantity.

```
MUV = SP × (SQ − AQ)

Favourable  → Used LESS than standard (efficient)
Adverse     → Used MORE than standard (wasteful)

MUV = MMV + MYV
```

---

### 4️⃣ Material Mix Variance (MMV)

> When **multiple materials** are used — caused by using a different **proportion/mix** of materials than standard.

```
MMV = SP × (Revised SQ − AQ)

Where:
Revised SQ = Total Actual Quantity in Standard Proportion
           = (Standard Proportion of material / Total Standard) × Total Actual Quantity

Favourable  → Used cheaper mix than standard
Adverse     → Used more expensive mix than standard
```

---

### 5️⃣ Material Yield Variance (MYV)

> Caused by difference in **actual output yield** from material vs expected (standard) yield.

```
MYV = Standard Cost per unit × (Actual Yield − Standard Yield)

Where Standard Yield = Actual Input × Expected yield %

Favourable  → Got more output than expected
Adverse     → Got less output than expected
```

---

### 📊 Solved Numerical: Material Variances

**Standard:** 5 kg of material per unit at ₹10/kg.
**Actual:** Produced 100 units. Used 520 kg at ₹11/kg.

```
SQ = 5 × 100 = 500 kg (standard for actual output)
SP = ₹10/kg
AQ = 520 kg
AP = ₹11/kg

MCV = (500 × 10) − (520 × 11)
    = ₹5,000 − ₹5,720 = ₹720 (Adverse)

MPV = 520 × (10 − 11) = 520 × (−1) = ₹520 (Adverse)

MUV = 10 × (500 − 520) = 10 × (−20) = ₹200 (Adverse)

Check: MCV = MPV + MUV = 520 + 200 = ₹720 (A) ✅
```

---

## B) LABOUR VARIANCES ⭐⭐⭐

---

### 1️⃣ Labour Cost Variance (LCV) — The Total

```
LCV = (SH × SR) − (AH × AR)
    = Standard Labour Cost − Actual Labour Cost

LCV = LRV + LEV
```

---

### 2️⃣ Labour Rate Variance (LRV)

> Caused by **difference in wage rate** paid vs standard rate.

```
LRV = AH × (SR − AR)

Favourable  → Paid less per hour than standard
Adverse     → Paid more per hour than standard
```

---

### 3️⃣ Labour Efficiency Variance (LEV)

> Caused by **difference in hours** taken vs standard hours.

```
LEV = SR × (SH − AH)

Favourable  → Finished in FEWER hours (efficient workers)
Adverse     → Took MORE hours than standard (slow/idle)

LEV = LMV + LITV
```

---

### 4️⃣ Labour Mix Variance (LMV)

> When **different grades of labour** are used — caused by using different mix than standard.

```
LMV = SR × (Revised SH − AH)

Where Revised SH = Total Actual Hours in Standard Proportion
```

---

### 5️⃣ Labour Idle Time Variance (LITV)

> Hours **paid but not worked** (idle time) charged at standard rate.

```
LITV = Idle Hours × Standard Rate  (Always ADVERSE)
```

---

### 📊 Solved Numerical: Labour Variances

**Standard:** 4 hours per unit at ₹50/hr.
**Actual:** 100 units produced. Workers worked 420 hours at ₹55/hr.

```
SH = 4 × 100 = 400 hrs
SR = ₹50/hr
AH = 420 hrs
AR = ₹55/hr

LCV = (400 × 50) − (420 × 55)
    = ₹20,000 − ₹23,100 = ₹3,100 (Adverse)

LRV = 420 × (50 − 55) = 420 × (−5) = ₹2,100 (Adverse)

LEV = 50 × (400 − 420) = 50 × (−20) = ₹1,000 (Adverse)

Check: LCV = LRV + LEV = 2,100 + 1,000 = ₹3,100 (A) ✅
```

---

## C) OVERHEAD VARIANCES ⭐⭐

---

### Fixed Overhead Variances

```
Standard FOH Rate = Budgeted Fixed OH / Budgeted Hours (or units)
Absorbed FOH      = Standard Hours for Actual Output × Standard FOH Rate
```

| Variance | Formula |
|---------|---------|
| **FOH Cost Variance** | Absorbed FOH − Actual FOH |
| **FOH Expenditure Variance** | Budgeted FOH − Actual FOH |
| **FOH Volume Variance** | Absorbed FOH − Budgeted FOH |
| **FOH Efficiency Variance** | Std FOH Rate × (SH − AH) |
| **FOH Capacity Variance** | Std FOH Rate × (AH − Budgeted Hours) |

```
FOH Cost Variance = FOH Expenditure Variance + FOH Volume Variance
FOH Volume Variance = FOH Efficiency Variance + FOH Capacity Variance
```

---

### Variable Overhead Variances

| Variance | Formula |
|---------|---------|
| **VOH Cost Variance** | Absorbed VOH − Actual VOH |
| **VOH Expenditure Variance** | (AH × Std VOH Rate) − Actual VOH |
| **VOH Efficiency Variance** | Std VOH Rate × (SH − AH) |

```
VOH Cost Variance = VOH Expenditure + VOH Efficiency
```

---

### 📊 Solved Numerical: Fixed Overhead Variances

**Given:**
- Budgeted Output = 500 units, Budgeted Hours = 1,000 hrs, Budgeted FOH = ₹10,000
- Actual Output = 480 units, Actual Hours = 980 hrs, Actual FOH = ₹10,500

```
Standard FOH Rate = ₹10,000 / 1,000 = ₹10/hr
Standard Hours per unit = 1,000 / 500 = 2 hrs/unit
SH for Actual Output = 480 × 2 = 960 hrs

Absorbed FOH = 960 × ₹10 = ₹9,600

FOH Cost Variance = ₹9,600 − ₹10,500 = ₹900 (Adverse)

FOH Expenditure Variance = ₹10,000 − ₹10,500 = ₹500 (Adverse)

FOH Volume Variance = ₹9,600 − ₹10,000 = ₹400 (Adverse)

FOH Efficiency Variance = ₹10 × (960 − 980) = ₹200 (Adverse)
FOH Capacity Variance   = ₹10 × (980 − 1,000) = ₹200 (Adverse)

Check: FOH Volume = Efficiency + Capacity = 200 + 200 = ₹400 (A) ✅
Check: FOH Cost = Expenditure + Volume = 500 + 400 = ₹900 (A) ✅
```

---

## D) SALES VARIANCES ⭐

---

| Variance | Formula | F or A? |
|---------|---------|---------|
| **Sales Value Variance** | Actual Sales − Budgeted Sales | Actual > Budget = F |
| **Sales Price Variance** | AQ × (AP − SP) | AP > SP = F |
| **Sales Volume Variance** | SP × (AQ − BQ) | AQ > BQ = F |

```
Sales Value Variance = Sales Price Variance + Sales Volume Variance
```

---

### 📊 Quick Example: Sales Variances

**Standard:** Sell 500 units at ₹100 each.
**Actual:** Sold 480 units at ₹105 each.

```
Sales Value Variance = (480 × 105) − (500 × 100)
                     = ₹50,400 − ₹50,000 = ₹400 (F)

Sales Price Variance = 480 × (105 − 100) = 480 × 5 = ₹2,400 (F)

Sales Volume Variance = 100 × (480 − 500) = 100 × (−20) = ₹2,000 (A)

Check: 2,400 (F) − 2,000 (A) = ₹400 (F) ✅
```

---

## 6.6 📝 Summary

```
┌──────────────────────────────────────────────────────────────┐
│                    CHAPTER 6 SNAPSHOT                        │
├──────────────────────────────────────────────────────────────┤
│ MATERIAL VARIANCES                                           │
│  MCV = (SQ×SP) − (AQ×AP)    = MPV + MUV                    │
│  MPV = AQ(SP−AP)                                            │
│  MUV = SP(SQ−AQ)             = MMV + MYV                   │
│                                                              │
│ LABOUR VARIANCES                                             │
│  LCV = (SH×SR) − (AH×AR)    = LRV + LEV                    │
│  LRV = AH(SR−AR)                                            │
│  LEV = SR(SH−AH)             = LMV + LITV                  │
│                                                              │
│ OVERHEAD VARIANCES                                           │
│  FOH Cost = Expenditure + Volume                             │
│  FOH Volume = Efficiency + Capacity                          │
│  VOH Cost = Expenditure + Efficiency                         │
│                                                              │
│ SALES VARIANCES                                              │
│  Sales Value = Price Variance + Volume Variance              │
│                                                              │
│ F = Actual BETTER than Standard                              │
│ A = Actual WORSE than Standard                               │
└──────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. **Calculate MCV, MPV, MUV** from given data ← Most likely numerical!
> 2. **Calculate LCV, LRV, LEV** from given data ← Very likely!
> 3. What is Standard Costing? State its objectives and advantages
> 4. What are the different types of standards? Explain each
> 5. **Fixed Overhead Variance** — full tree with numerical
> 6. Draw and explain the **Variance Classification Tree**
> 7. What is Material Mix Variance? How is it calculated?

> [!TIP]
> **Memory Trick for Material Variances:**
> **MCV = MPV + MUV** → "Cost = Price + Usage"
> **MUV = MMV + MYV** → "Usage = Mix + Yield"
>
> **For Labour:**
> **LCV = LRV + LEV** → "Cost = Rate + Efficiency"
> **LEV = LMV + LITV** → "Efficiency = Mix + Idle Time"

> [!NOTE]
> **The ONE formula that generates ALL variances:**
> Always compare: **Standard for Actual** vs **Actual**
> - Standard PRICE × Standard QTY for Actual Output
> - vs Actual PRICE × Actual QTY
> Break down the gap → Price difference + Quantity difference!

---
*📅 Created: 2026-06-29 | Chapter 6 | Management Accounting | DU SOL MBA Sem 2*
