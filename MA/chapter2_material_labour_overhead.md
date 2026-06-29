# 📘 Chapter 2: Material, Labour and Overhead Cost & Control
### Management Accounting | DU SOL | 2nd Semester

---

## 🎯 Learning Objectives
- Understand the three **elements of cost**: Material, Labour, Overhead
- Learn **inventory control techniques** (Stock Levels, EOQ, ABC)
- Understand **wage payment systems** and **incentive plans**
- Learn how overheads are **collected → allocated → apportioned → absorbed**
- Solve numerical problems on all three elements

---

## 2.3 Elements of Cost

```
┌──────────────────────────────────────────────┐
│              ELEMENTS OF COST                │
│                                              │
│  1. MATERIAL  →  Direct + Indirect           │
│  2. LABOUR    →  Direct + Indirect           │
│  3. EXPENSES  →  Direct + Indirect           │
└──────────────────────────────────────────────┘
```

| Element | Direct | Indirect |
|---------|--------|----------|
| **Material** | Raw material for product | Consumables, lubricants |
| **Labour** | Workers on production line | Supervisor, security guard |
| **Expenses** | Subcontractor for specific job | Rent, electricity |

### 🧠 BugZero Analogy
- **Direct Material** = Laptop bought specifically for a QA engineer on a project
- **Direct Labour** = QA engineer's salary working on one specific module
- **Indirect Material** = Printer paper used by everyone in office
- **Indirect Labour** = HR manager's salary (supports everyone)

---

## 2.4 Material Cost and Control

> **Material Control** = A system to ensure the right material is available at the right time, in the right quantity, at the right cost — **minimizing wastage and cost**.

### 🔑 Objectives of Material Control
1. Uninterrupted supply of materials
2. Avoid overstocking (ties up capital) and understocking (production stops)
3. Minimize material cost
4. Prevent losses from theft, damage, wastage

---

### 📦 A) Stock / Inventory Levels

These are **trigger points** that tell the store manager when to order, how much to order, and what's the safety buffer.

#### 🔢 Formulas (MEMORIZE THESE ⭐)

```
1. REORDER LEVEL (ROL)
   = Maximum Consumption × Maximum Lead Time
   (The level at which a new order must be placed)

2. MINIMUM LEVEL (Safety Stock)
   = Reorder Level − (Normal Consumption × Normal Lead Time)
   (The lowest stock should ever fall to)

3. MAXIMUM LEVEL
   = Reorder Level + EOQ − (Minimum Consumption × Minimum Lead Time)
   (Stock should never exceed this)

4. AVERAGE STOCK LEVEL
   = (Minimum Level + Maximum Level) / 2
   OR = Minimum Level + ½ × EOQ

5. DANGER LEVEL
   = Minimum/Normal Consumption × Emergency Lead Time
   (Below this = production will stop!)
```

#### 💼 BugZero Example
BugZero buys testing server RAM (SSDs). Data:
- Max consumption = 50 units/week, Min = 20 units/week, Normal = 35 units/week
- Max lead time = 4 weeks, Min = 2 weeks, Normal = 3 weeks
- EOQ = 300 units, Emergency lead time = 1 week

```
Reorder Level   = 50 × 4 = 200 units
Minimum Level   = 200 − (35 × 3) = 200 − 105 = 95 units
Maximum Level   = 200 + 300 − (20 × 2) = 500 − 40 = 460 units
Average Level   = (95 + 460) / 2 = 277.5 units
Danger Level    = 35 × 1 = 35 units
```

---

### 📦 B) EOQ — Economic Order Quantity ⭐

> **EOQ** = The order quantity that **minimizes total inventory cost** (ordering cost + carrying cost).

#### 🔢 Formula
```
        ┌─────────────┐
EOQ =  │  2 × A × O  │
        │  ──────────  │
        │      C       │
        └─────────────┘

Where:
A = Annual Consumption (units)
O = Ordering Cost per order (₹)
C = Carrying/Holding Cost per unit per year (₹)
```

#### 🧠 Analogy
Ordering too often = too many trips to market (high ordering cost)
Ordering too much at once = huge fridge, things spoil (high carrying cost)
EOQ = the **perfect grocery run size** that balances both!

#### 💼 Solved Example
BugZero uses 1,200 USB testing dongles/year.
Ordering cost = ₹500/order. Carrying cost = ₹2/unit/year.

```
EOQ = √(2 × 1200 × 500 / 2)
    = √(12,00,000 / 2)
    = √6,00,000
    = 774.6 ≈ 775 units

Number of Orders per year = 1200 / 775 ≈ 1.5 → ~2 orders/year
```

---

### 📦 C) ABC Analysis

> **ABC Analysis** = Classifying inventory into 3 categories based on **value and usage** to focus control efforts.

| Category | % of Items | % of Value | Control Level | Example |
|----------|-----------|------------|--------------|---------|
| **A Items** | 10% | 70-80% | Tight control, frequent review | High-end test servers |
| **B Items** | 20% | 15-20% | Moderate control | Software licenses |
| **C Items** | 70% | 5-10% | Loose control, bulk order | Pens, sticky notes |

#### 🧠 Analogy
At BugZero: Your **MacBook Pro (A)** = tracked carefully with asset tag.
**Office chair (B)** = moderate tracking. **Pens (C)** = nobody counts them!

---

### 📦 D) Methods of Stock Valuation ⭐

When materials are issued to production, which price do we use?

| Method | Definition | Pros | Cons |
|--------|-----------|------|------|
| **FIFO** (First In, First Out) | Oldest stock issued first | Closing stock at current market price | High profit in rising prices = more tax |
| **LIFO** (Last In, First Out) | Latest stock issued first | Lower profit in rising prices | Closing stock undervalued |
| **WEIGHTED AVERAGE** | Average cost of all stock | Smooths out price fluctuations | Requires recalculation each time |

#### 🔢 Weighted Average Price Formula
```
Weighted Average Price = Total Cost of Stock Available
                        ────────────────────────────────
                         Total Units Available
```

---

## 2.5 Labour Cost

> **Labour Cost** = Payment made to workers for their physical or mental effort in production.

### 📌 A) Time Keeping vs Time Booking

| Concept | Purpose | Tools |
|---------|---------|-------|
| **Time Keeping** | Record attendance (when did worker arrive/leave) | Attendance register, Biometric, Time cards |
| **Time Booking** | Record time spent on **each job/task** | Job cards, Jira tickets (in BugZero!) |

---

### 📌 B) Methods of Wage Payment ⭐

#### 1. Time Rate System
```
Wages = Hours Worked × Rate per Hour
```
- Simple, no pressure on workers
- No incentive to work faster
- **Example:** QA engineer paid ₹200/hour regardless of test cases written

#### 2. Piece Rate System
```
Wages = Units Produced × Rate per Unit
```
- More output = more pay
- Risk: quality may suffer
- **Example:** QA paid ₹10 for every bug found (might start filing false bugs!)

#### 3. Taylor's Differential Piece Rate ⭐
Two rates: reward efficient workers, penalize inefficient workers

```
If Output ≥ Standard Output → 120% of Normal Piece Rate
If Output < Standard Output  → 80% of Normal Piece Rate
```

**Example:**
- Standard output = 100 test cases/day. Normal piece rate = ₹5/case
- Worker A produces 120 cases → Rate = 120% × ₹5 = ₹6 → Wages = 120 × ₹6 = **₹720**
- Worker B produces 80 cases → Rate = 80% × ₹5 = ₹4 → Wages = 80 × ₹4 = **₹320**

#### 4. Merrick's Differential Piece Rate

| Output Level | Rate Applied |
|-------------|-------------|
| Up to 83% of standard | Normal piece rate (100%) |
| 83% to 100% of standard | 110% of normal piece rate |
| Above 100% of standard | 120% of normal piece rate |

---

### 📌 C) Incentive Plans ⭐⭐

#### 🔢 Halsey Premium Plan
```
Earnings = (Time Taken × Rate) + 50% × Time Saved × Rate

Time Saved = Standard Time − Actual Time
```

**BugZero Example:**
Standard time for testing a module = 10 hours. Worker finishes in 6 hours. Rate = ₹100/hr.
```
Time Saved = 10 − 6 = 4 hours
Bonus = 50% × 4 × ₹100 = ₹200
Earnings = (6 × ₹100) + ₹200 = ₹600 + ₹200 = ₹800
```

#### 🔢 Rowan Plan
```
Bonus = (Time Saved / Standard Time) × Time Taken × Rate
Earnings = (Time Taken × Rate) + Bonus
```

**Same BugZero Example:**
```
Bonus = (4/10) × 6 × ₹100 = 0.4 × ₹600 = ₹240
Earnings = ₹600 + ₹240 = ₹840
```

#### ⚖️ Halsey vs Rowan Comparison

| Feature | Halsey | Rowan |
|---------|--------|-------|
| Bonus split | Fixed 50% of time saved | Proportion of time saved to standard time |
| Worker benefit | Better when time saved is small | Better when time saved is large |
| Max bonus limit | No cap | Bonus can't exceed time wages (built-in cap) |

> 🔑 **Trick**: If time saved < 50% of standard time → **Rowan gives more bonus**
> If time saved > 50% of standard time → **Halsey gives more bonus**

---

### 📌 D) Labour Turnover

> **Labour Turnover** = Rate at which employees leave and are replaced in an organization.

#### 🔢 Formulas
```
Separation Rate   = (No. of workers left / Avg workers) × 100

Replacement Rate  = (No. of workers replaced / Avg workers) × 100

Flux Rate         = ((Separations + New joinings) / Avg workers) × 100
```

#### Causes: Poor pay, bad work culture, better opportunities (very common in startups!)
#### Cost of Labour Turnover:
- **Preventive Costs** = Cost to retain employees (better pay, perks)
- **Replacement Costs** = Recruitment, training, lost productivity

---

### 📌 E) Idle Time

> **Idle Time** = Time for which workers are paid but **no production** happens.

```
Normal Idle Time  → Built into standard time (lunch break, shift changeover)
Abnormal Idle Time → Power cuts, machine breakdown, strikes
                  → Charged to Profit & Loss Account
```

---

## 2.6 Overhead Cost and Control

> **Overhead** = All indirect costs = Indirect Material + Indirect Labour + Indirect Expenses

### 📌 A) Classification of Overheads

| Type | Definition | Examples |
|------|-----------|---------|
| **Factory/Works OH** | Incurred in factory/production | Factory rent, machine depreciation, factory manager salary |
| **Administration OH** | Office management | CEO salary, office rent, accounting software |
| **Selling OH** | Getting customers | Advertising, sales team salary |
| **Distribution OH** | Delivering product | Packaging, courier, CDN costs |

---

### 📌 B) The 4-Step Overhead Process ⭐

```
STEP 1: COLLECTION (Primary Distribution)
        Collect all overhead costs into a single pool
        ↓
STEP 2: ALLOCATION
        Directly assign overhead to a dept if it belongs entirely to that dept
        (e.g., factory supervisor salary → Factory dept only)
        ↓
STEP 3: APPORTIONMENT (Secondary Distribution)
        Distribute shared overheads across departments using a fair basis
        (e.g., rent apportioned on basis of Floor Area)
        ↓
STEP 4: ABSORPTION
        Charge overhead from cost centres to individual products/jobs
        using an Overhead Absorption Rate (OAR)
```

---

### 📌 C) Apportionment Bases ⭐

| Overhead | Basis of Apportionment |
|---------|----------------------|
| **Rent, Rates** | Floor Area |
| **Lighting** | Floor Area OR Number of Light Points |
| **Depreciation of Machinery** | Value of Machinery or Machine Hours |
| **Power** | Horse Power of Machines |
| **Canteen, Welfare** | Number of Workers/Employees |
| **Insurance of Assets** | Value of Assets |
| **Supervision** | Number of Workers |

---

### 📌 D) Methods of Overhead Absorption ⭐⭐

```
Overhead Absorption Rate (OAR) = Budgeted/Estimated Overhead
                                  ────────────────────────────
                                   Budgeted Base (Activity)
```

| Method | Formula | Best Used When |
|--------|---------|----------------|
| **Per Unit Rate** | Total OH / Total Units | All units identical |
| **% of Direct Material** | OH / Direct Material Cost × 100 | Material cost dominant |
| **% of Direct Labour** | OH / Direct Labour Cost × 100 | Labour cost dominant |
| **% of Prime Cost** | OH / Prime Cost × 100 | Mixed production |
| **Labour Hour Rate** | OH / Direct Labour Hours | Labour-intensive work |
| **Machine Hour Rate** | OH / Machine Hours | Machine-intensive work |

---

### 📌 E) Over/Under Absorption of Overhead ⭐

```
If Absorbed OH > Actual OH → OVER-ABSORBED (write back to P&L as profit)
If Absorbed OH < Actual OH → UNDER-ABSORBED (charge to P&L as loss)

Over/Under Absorption = Absorbed Overhead − Actual Overhead
```

#### 💼 BugZero Example
BugZero estimates ₹1,20,000 overhead and 6,000 machine hours.
Machine Hour Rate = ₹1,20,000 / 6,000 = **₹20 per hour**

Actual machine hours used = 5,500 | Actual overhead = ₹1,15,000

```
Overhead Absorbed = 5,500 × ₹20 = ₹1,10,000
Actual Overhead   =              ₹1,15,000
Under-Absorption  =              ₹5,000 (charged to P&L as loss)
```

---

## 2.7 📊 Solved Numerical Questions

---

### 🔢 Q1: Stock Levels

**Given:** Annual consumption = 36,000 units (300/month), Max consumption = 400/month,
Min consumption = 200/month. Normal lead time = 2 months, Max = 3 months, Min = 1 month.
EOQ = 1,800 units. Emergency lead time = 0.5 months.

```
Reorder Level    = 400 × 3 = 1,200 units
Minimum Level    = 1,200 − (300 × 2) = 1,200 − 600 = 600 units
Maximum Level    = 1,200 + 1,800 − (200 × 1) = 3,000 − 200 = 2,800 units
Average Level    = (600 + 2,800) / 2 = 1,700 units
Danger Level     = 300 × 0.5 = 150 units
```

---

### 🔢 Q2: EOQ Calculation

**Given:** Annual demand = 10,000 units. Ordering cost = ₹250/order.
Holding cost = ₹5/unit/year. Price = ₹50/unit.

```
EOQ = √(2 × 10,000 × 250 / 5)
    = √(50,00,000 / 5)
    = √10,00,000
    = 1,000 units

No. of Orders   = 10,000 / 1,000 = 10 orders/year
Ordering Cost   = 10 × ₹250 = ₹2,500
Holding Cost    = (1,000/2) × ₹5 = ₹2,500
Total Cost      = ₹5,000 ✅ (Equal → confirms EOQ is correct)
```

---

### 🔢 Q3: Halsey vs Rowan Plan

**Given:** Standard time = 12 hours. Actual time = 9 hours. Wage rate = ₹50/hour.

```
Time Saved = 12 − 9 = 3 hours
Basic Wages = 9 × ₹50 = ₹450

HALSEY PLAN:
Bonus    = 50% × 3 × ₹50 = ₹75
Earnings = ₹450 + ₹75 = ₹525

ROWAN PLAN:
Bonus    = (3/12) × 9 × ₹50 = 0.25 × ₹450 = ₹112.5
Earnings = ₹450 + ₹112.5 = ₹562.5

→ Rowan gives more because time saved (3) < 50% of std time (6)
```

---

### 🔢 Q4: Taylor's Differential Piece Rate

**Given:** Standard output = 50 units/day. Normal piece rate = ₹8/unit.
Worker A = 60 units/day. Worker B = 40 units/day.

```
Standard output = 50 units

Worker A (60 ≥ 50 → Efficient):
  Rate    = 120% × ₹8 = ₹9.60
  Wages   = 60 × ₹9.60 = ₹576

Worker B (40 < 50 → Inefficient):
  Rate    = 80% × ₹8 = ₹6.40
  Wages   = 40 × ₹6.40 = ₹256
```

---

### 🔢 Q5: Overhead Absorption & Over/Under Absorption

**Given:** Budgeted OH = ₹80,000. Budgeted Labour Hours = 16,000.
Actual OH = ₹82,000. Actual Labour Hours = 17,000.

```
OAR (Labour Hour Rate) = ₹80,000 / 16,000 = ₹5 per hour

OH Absorbed = 17,000 × ₹5 = ₹85,000
Actual OH   =              ₹82,000
                           ────────
Over-Absorption =          ₹3,000 → Credited to P&L (Profit)
```

---

## 2.8 📝 Summary

```
┌─────────────────────────────────────────────────────────────┐
│                    CHAPTER 2 SNAPSHOT                       │
├─────────────────────────────────────────────────────────────┤
│ MATERIAL CONTROL                                            │
│  ROL = Max Cons × Max Lead Time                             │
│  Min = ROL − (Normal Cons × Normal Lead Time)               │
│  Max = ROL + EOQ − (Min Cons × Min Lead Time)               │
│  EOQ = √(2AO/C)                                             │
│  ABC: A=Tight, B=Moderate, C=Loose control                  │
├─────────────────────────────────────────────────────────────┤
│ LABOUR COST                                                 │
│  Time Rate: Hours × Rate                                    │
│  Piece Rate: Units × Rate                                   │
│  Taylor: ≥Std=120%, <Std=80% of piece rate                  │
│  Halsey: Basic + 50% × Time Saved × Rate                    │
│  Rowan: Basic + (Saved/Std) × Actual × Rate                 │
├─────────────────────────────────────────────────────────────┤
│ OVERHEAD CONTROL                                            │
│  Collect → Allocate → Apportion → Absorb                    │
│  OAR = Budgeted OH / Budgeted Base                          │
│  Over-absorbed → Credit P&L                                 │
│  Under-absorbed → Debit P&L                                 │
└─────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. Calculate ROL, Minimum, Maximum, Average, and Danger Level (numerical)
> 2. Calculate EOQ and total inventory cost
> 3. Compare Halsey vs Rowan Plan (numerical + table)
> 4. Explain Taylor's Differential Piece Rate with example
> 5. What is ABC Analysis? Explain with diagram
> 6. Explain 4 steps of overhead accounting: Collect, Allocate, Apportion, Absorb
> 7. Calculate OAR and find over/under absorption
> 8. Difference between Allocation and Apportionment of overheads

> [!TIP]
> **Memory Trick for Stock Levels**: **"Really Mindful Managers Always Discuss"**
> → **R**eorder, **M**inimum, **M**aximum, **A**verage, **D**anger

---
*📅 Created: 2026-06-29 | Chapter 2 | Management Accounting | DU SOL MBA Sem 2*
