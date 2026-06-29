# 📘 Chapter 7: Budgets and Budgetary Control
### Management Accounting | DU SOL | 2nd Semester

---

## 🎯 Learning Objectives
- Define **Budget** and **Budgetary Control**
- Understand the **steps** in budgetary control
- Know the **types of budgets** and their purposes
- Understand the difference between **Fixed and Flexible budgets**
- Learn **Zero-Based Budgeting (ZBB)** — its concept, advantages, limitations

---

## 7.2 Introduction

> Every organization — from a government ministry to a Bootstrap startup — needs a **financial plan** before spending money. That plan is called a **Budget**.

### 🧠 BugZero Analogy
BugZero is growing fast. At the start of the year, the CEO sits down and plans:
- "We'll earn ₹50L from contracts" → **Sales Budget**
- "We'll need 5 QA engineers for 12 months" → **Labour Budget**
- "We'll buy ₹2L worth of testing tools" → **Capital Budget**
- "Total expenses should not exceed ₹40L" → **Master Budget**

This entire process of planning, executing, comparing, and correcting = **Budgetary Control**

---

## 7.3 Budget and Budgetary Control

### 📌 Budget — Definition

> **Budget** = A formal, quantitative statement prepared **in advance** for a specific future period, expressing the **plans of management** in financial and/or physical terms.

**Key Points:**
- Prepared **before** the period (future-oriented)
- Expressed in **money or quantity** (or both)
- Covers a **specific time period** (monthly, quarterly, annually)
- Approved by **top management**

---

### 📌 Budgetary Control — Definition

> **Budgetary Control** = A system where **budgets are prepared and continuously compared with actual results** to identify variances, investigate causes, and take **corrective action** to achieve organizational objectives.

```
Plan → Budget → Execute → Record Actuals → Compare → Variance → Correct
  ↑_______________________________________________|
                  (Feedback Loop)
```

---

### 📌 Steps in Budgetary Control ⭐

| Step | Action |
|------|--------|
| **1. Set Objectives** | Define goals — profit target, growth % |
| **2. Identify Limiting Factor** | Find the Principal Budget Factor (PBF) |
| **3. Prepare Functional Budgets** | Sales, Production, Material, Labour, Cash |
| **4. Coordinate Budgets** | Align all department budgets |
| **5. Prepare Master Budget** | Summarise into P&L + Balance Sheet |
| **6. Communicate** | Share budgets with all departments |
| **7. Execute** | Carry out actual operations |
| **8. Record Actuals** | Collect actual cost/revenue data |
| **9. Compare** | Actual vs Budget → calculate variances |
| **10. Take Corrective Action** | Fix what went wrong |
| **11. Report** | Report to top management |

---

### 📌 Principal Budget Factor (Limiting Factor) ⭐

> **Principal Budget Factor (PBF)** = The factor that **constrains the activities** of an organization and limits its output. The budget must be built around this factor first.

**Common Examples:**

| PBF | Situation |
|-----|-----------|
| **Sales Demand** | Most common — can't sell more than market wants |
| **Production Capacity** | Factory can't produce beyond machine hours |
| **Raw Material Supply** | Shortage of key input material |
| **Labour / Skilled Staff** | Can't find enough qualified workers |
| **Finance/Cash** | Can't afford to expand without funding |

> 💼 **BugZero Example:** BugZero can handle max 20 contracts/month (limited by 10 QA engineers). Even if 30 clients want to hire them, the **PBF = Labour (QA engineer hours)**. So the Production/Sales Budget is built around this limit.

---

## 7.4 Types of Budgets ⭐⭐

### 🗂️ Classification Overview

```
BUDGETS
│
├── By TIME
│   ├── Short-term (< 1 year) — Operating budgets
│   └── Long-term (> 1 year) — Capital, Strategic budgets
│
├── By FUNCTION (Functional Budgets)
│   ├── Sales Budget
│   ├── Production Budget
│   ├── Materials Budget (Purchase + Usage)
│   ├── Labour Budget
│   ├── Overhead Budgets (Factory/Admin/Selling)
│   ├── Cash Budget
│   ├── Capital Expenditure Budget
│   └── Master Budget (Summary of all above)
│
└── By FLEXIBILITY
    ├── Fixed Budget
    └── Flexible Budget
```

---

### 📌 A) Functional Budgets — One by One ⭐

#### 1. Sales Budget (Starting Point!)
> Prepared first because all other budgets depend on it.

```
Sales Budget = Units to be Sold × Selling Price per Unit

| Product | Units | Price | Revenue |
|---------|-------|-------|---------|
| A       | 500   | ₹200  | ₹1,00,000|
| B       | 300   | ₹300  | ₹90,000  |
| TOTAL   |       |       |₹1,90,000 |
```

---

#### 2. Production Budget
> Based on Sales Budget ± Stock changes.

```
Production Budget (units) = Sales Units
                           + Desired Closing Stock (F.G.)
                           − Opening Stock (F.G.)
```

**Example:**
```
Sales units required        = 500
Add: Desired Closing Stock  = 100
Less: Opening Stock         = (80)
Production Required         = 520 units
```

---

#### 3. Materials Budget
```
Materials Required = Production units × Material per unit

Purchase Budget = Material Required
                + Desired Closing Material Stock
                − Opening Material Stock
```

---

#### 4. Labour Budget
```
Labour Hours Required = Production units × Standard Hours per unit
Labour Cost = Labour Hours × Wage Rate per hour
```

---

#### 5. Cash Budget ⭐⭐

> Shows **expected cash inflows and outflows** for each period. Helps detect cash surpluses or deficits in advance.

```
CASH BUDGET FORMAT:

                        Jan ₹    Feb ₹    Mar ₹
OPENING BALANCE           XX       XX       XX
ADD: Receipts
  Cash Sales              XX       XX       XX
  Collections (Debtors)   XX       XX       XX
  Loans received          XX        -        -
TOTAL INFLOWS (A)         XX       XX       XX
─────────────────────────────────────────────
LESS: Payments
  Raw Materials           XX       XX       XX
  Labour                  XX       XX       XX
  Overheads               XX       XX       XX
  Capital Expenditure      -       XX        -
  Loan repayment          XX        -        -
TOTAL OUTFLOWS (B)        XX       XX       XX
─────────────────────────────────────────────
CLOSING BALANCE (A−B)     XX       XX       XX
```

> 💼 **BugZero Example:**
> BugZero expects ₹10L in January (3 contracts paid), but must pay:
> - ₹3L salaries, ₹1L server bills, ₹2L software licenses
> Cash Budget helps them see if they have enough to pay a ₹5L advance for new office rent in February!

---

#### 6. Master Budget

> **Master Budget** = The **summary budget** that brings together all functional budgets into:
> 1. **Budgeted Profit & Loss Account**
> 2. **Budgeted Balance Sheet**
> 3. **Cash Flow Statement**

It gives the **overall financial picture** of the organization for the budget period.

---

### 📌 B) Fixed Budget vs Flexible Budget ⭐⭐

| Feature | Fixed Budget | Flexible Budget |
|---------|-------------|-----------------|
| **Prepared for** | ONE level of activity | MULTIPLE activity levels |
| **Rigidity** | Rigid — doesn't change | Flexible — adjusts with output |
| **Usefulness** | Limited — outdated if output changes | More realistic and useful |
| **Cost behavior** | Ignores fixed/variable split | Recognizes cost behavior |
| **Variance analysis** | Misleading when actual ≠ budgeted | Meaningful comparison |
| **Best for** | Stable, predictable operations | Variable/uncertain operations |

---

### 📊 Solved Example: Fixed vs Flexible Budget

**Fixed Budget at 100% capacity:**
- Output: 1,000 units
- Variable Cost: ₹30/unit → ₹30,000
- Fixed Cost: ₹20,000
- Total Cost: ₹50,000

**Actual output: 800 units. Actual total cost: ₹45,000**

```
FIXED BUDGET COMPARISON (Misleading):
  Budgeted Cost = ₹50,000
  Actual Cost   = ₹45,000
  Variance      = ₹5,000 Favourable ← Seems good!

But this is WRONG — output also fell by 200 units!

FLEXIBLE BUDGET COMPARISON (Correct):
  Flexible Budget for 800 units:
    Variable Cost = 800 × ₹30 = ₹24,000
    Fixed Cost    = ₹20,000 (unchanged)
    Flex Budget   = ₹44,000

  Actual Cost = ₹45,000
  True Variance = ₹45,000 − ₹44,000 = ₹1,000 Adverse ← True picture!
```

> 🧠 **Key Insight:** Flexible Budget adjusts for actual output level → gives a **fair comparison**.

---

## 7.5 Zero-Based Budgeting (ZBB) ⭐⭐

> **Zero-Based Budgeting (ZBB)** = A budgeting method where **every expense must be justified from scratch** for each new period, starting from a **zero base** — regardless of what was spent in previous years.

### 📌 Traditional Budgeting vs ZBB

| Feature | Traditional Budgeting | Zero-Based Budgeting |
|---------|----------------------|----------------------|
| **Starting Point** | Last year's budget + % increase | ZERO (start fresh) |
| **Justification** | Only changes justified | Every rupee justified |
| **Approach** | Incremental | Fundamental review |
| **Time required** | Less | More (detailed) |
| **Wastage** | Carries forward old inefficiencies | Eliminates wasteful spending |
| **Best for** | Stable organizations | Cost reduction, startups |

---

### 📌 Steps in ZBB ⭐

```
Step 1: Identify Decision Units
        (Each department/activity is a decision unit)
         ↓
Step 2: Create Decision Packages
        (Each unit prepares options: min level, current level, enhanced level)
         ↓
Step 3: Evaluate and Rank Packages
        (Rank by cost-benefit, priority, strategic value)
         ↓
Step 4: Allocate Resources
        (Fund packages from highest to lowest rank until budget runs out)
         ↓
Step 5: Prepare Final Budget
```

---

### ✅ Advantages of ZBB

| Advantage | Explanation |
|-----------|-------------|
| **Eliminates wasteful spending** | No "carry-over" of past inefficiencies |
| **Focuses on value** | Every rupee must justify its existence |
| **Encourages innovation** | Managers think creatively about costs |
| **Better resource allocation** | Resources go where they're most needed |
| **Motivates managers** | Forces involvement and justification |
| **Detects outdated activities** | Removes programs that no longer add value |

### ❌ Limitations of ZBB

| Limitation | Explanation |
|-----------|-------------|
| **Time-consuming** | Requires massive detailed analysis |
| **Expensive** | High cost to implement |
| **Requires skilled staff** | Managers need training |
| **Risk of politics** | Powerful managers may protect their budgets |
| **Short-term focus** | May neglect long-term strategic investments |
| **Not practical yearly** | Usually done every 3–5 years, not annually |

> 🧠 **BugZero ZBB Example:**
> Instead of saying "We spent ₹5L on QA tools last year, so budget ₹5.5L this year" → ZBB says: "Justify EVERY tool. Do we still need Selenium license? Jira? Postman? Which ones are actually being used? Drop the rest!"
> Result: BugZero finds ₹1.2L in tools no one uses and eliminates them! 🎉

---

## 📝 Summary

```
┌──────────────────────────────────────────────────────────────┐
│                    CHAPTER 7 SNAPSHOT                        │
├──────────────────────────────────────────────────────────────┤
│ BUDGET = Pre-determined financial plan for future period     │
│ BUDGETARY CONTROL = Plan → Execute → Compare → Correct       │
│                                                              │
│ STEPS: Objectives → PBF → Functional Budgets → Master        │
│        → Execute → Compare → Correct                         │
│                                                              │
│ PRINCIPAL BUDGET FACTOR = The key constraint                 │
│ (Usually Sales Demand, Labour, Material, or Cash)            │
│                                                              │
│ PRODUCTION BUDGET = Sales + Closing Stock − Opening Stock    │
│                                                              │
│ FIXED BUDGET   → One level, rigid                            │
│ FLEXIBLE BUDGET → Multiple levels, adjusts to actual output  │
│ (Flexible Budget = Better for variance analysis!)            │
│                                                              │
│ ZBB = Start from ZERO, justify every expense                 │
│ Advantage: No waste | Limitation: Time-consuming             │
└──────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. What is a Budget? Define Budgetary Control. State its objectives/steps.
> 2. What is the **Principal Budget Factor**? Give examples.
> 3. Distinguish between **Fixed and Flexible Budget** (table + example)
> 4. **Prepare a Cash Budget** from given data ← Numerical!
> 5. **Prepare a Production Budget** and/or **Materials Budget** ← Numerical!
> 6. What is **Zero-Based Budgeting**? State its advantages and limitations.
> 7. Differentiate ZBB from Traditional Budgeting.
> 8. What is a **Master Budget**? What does it consist of?

> [!TIP]
> **Production Budget Formula** = Sales + Closing FG − Opening FG
> **Purchase Budget Formula** = Usage + Closing Material − Opening Material
> These two are the most commonly asked budget numericals!

> [!NOTE]
> **ZBB is theory-heavy** — focus on: definition, steps, advantages vs limitations, and difference from traditional budgeting. This is almost always a theory question, rarely numerical.

---
*📅 Created: 2026-06-29 | Chapter 7 | Management Accounting | DU SOL MBA Sem 2*
