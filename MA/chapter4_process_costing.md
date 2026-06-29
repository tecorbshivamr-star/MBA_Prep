# 📘 Chapter 4: Process Costing
### Management Accounting | DU SOL | 2nd Semester

---

## 🎯 Learning Objectives
- Understand what **Process Costing** is and where it's used
- Calculate **Normal Loss, Abnormal Loss, and Abnormal Gain**
- Prepare a **Process Account**
- Value **Work-in-Progress** using Equivalent Units
- Differentiate between **Joint Products and By-Products**

---

## 4.2 Introduction

> **Process Costing** = A method of costing where products pass through **multiple stages/processes** and costs are accumulated **for each process**, then averaged over all units produced.

### 📌 Features
1. Production is **continuous** and in **large volumes**
2. Products are **identical/homogeneous**
3. Output of one process = **Input of the next process**
4. Costs collected **process-by-process**
5. Cost per unit = **Total Process Cost ÷ Output Units**

### 📌 Industries
| Industry | Processes |
|---------|-----------|
| Chemical | Mixing → Reaction → Purification → Packing |
| Textile | Spinning → Weaving → Dyeing → Finishing |
| Oil Refinery | Crude → Distillation → Cracking → Blending |
| Paper | Pulping → Bleaching → Rolling → Cutting |

### 🧠 BugZero Analogy
BugZero's **automated testing pipeline** runs in stages:
```
Code Input → [Process 1: Unit Testing] → [Process 2: Integration Testing]
           → [Process 3: UAT] → Final Certified Build (Output)
```
Each process has its own cost (tools, engineer time). Some code is **rejected** at each stage — that's your **process loss**!

---

## 4.3 Wastages: Process Losses ⭐⭐⭐

When raw material goes through a process, some output is **lost**. This loss can be:

```
┌───────────────────────────────────────────────────────┐
│                  PROCESS LOSSES                       │
│                                                       │
│  Input (100 units)                                    │
│       ↓                                               │
│  ┌─── PROCESS ───┐                                    │
│  │               │ → Normal Loss  (expected, planned) │
│  │               │ → Abnormal Loss (more than expected)│
│  │               │ → Abnormal Gain (less loss than exp)│
│  └───────────────┘                                    │
│       ↓                                               │
│  Output (remaining units)                             │
└───────────────────────────────────────────────────────┘
```

---

### 📌 A) Normal Loss ⭐

> **Normal Loss** = The **expected, unavoidable** loss that occurs under normal/efficient operating conditions. It is pre-estimated as a **% of input**.

- Normal loss is **NOT given a cost** (its cost is absorbed by good output)
- If normal loss units have **scrap value** → it reduces the process cost

#### 🔢 Key Formulas:
```
Normal Loss (units) = Normal Loss % × Input units

Cost per unit = (Total Input Cost − Scrap Value of Normal Loss)
                ────────────────────────────────────────────────
                        (Input units − Normal Loss units)
```

### 📌 B) Abnormal Loss ⭐⭐

> **Abnormal Loss** = Loss **over and above** the normal (expected) loss. It is avoidable and unexpected.

- Valued at the **same rate as good output** (Cost per unit)
- Charged to **Abnormal Loss A/c → P&L A/c** (as a loss)

```
Abnormal Loss (units) = Actual Loss − Normal Loss

Value of Abnormal Loss = Abnormal Loss units × Cost per unit
```

### 📌 C) Abnormal Gain ⭐⭐

> **Abnormal Gain** = When **actual loss is LESS than normal loss** — more output than expected. It's a gain!

- Valued at the **same rate as good output**
- Credited to **Abnormal Gain A/c → P&L A/c** (as a gain)
- BUT: Scrap value of the "saved" units must be deducted

```
Abnormal Gain (units) = Normal Loss − Actual Loss

Value of Abnormal Gain = Abnormal Gain units × Cost per unit
```

> 🧠 **BugZero Analogy:**
> - **Normal Loss** = Expecting 10% of code builds to fail QA checks (normal rejection rate)
> - **Abnormal Loss** = 20% fail instead of 10% → extra failures = cost to P&L
> - **Abnormal Gain** = Only 5% fail instead of 10% → better than expected!

---

### 📋 Process Account Format ⭐

```
DR                    PROCESS ACCOUNT                    CR
──────────────────────────────────────────────────────────────
Particulars   Units    ₹   | Particulars      Units    ₹
──────────────────────────────────────────────────────────────
To Materials  1,000  10,000 | By Normal Loss    100    500
To Labour           5,000  | By Abnormal Loss   50  2,375
To Overhead         2,500  | By Output (Next   850 14,625
                           |   Process/F.G.)
──────────────────────────────────────────────────────────────
              1,000  17,500 |                 1,000  17,500
```

---

### 📊 Solved Numerical — All Three Cases

**Given:** Input = 1,000 kg at ₹10/kg. Processing cost = ₹5,000.
Normal Loss = 10%. Scrap value = ₹2/unit.

**Calculate Cost per Unit:**
```
Normal Loss       = 10% × 1,000 = 100 units
Scrap Value of NL = 100 × ₹2   = ₹200
Total Cost        = (1,000 × ₹10) + ₹5,000 = ₹15,000
Net Cost          = ₹15,000 − ₹200 = ₹14,800
Expected Output   = 1,000 − 100 = 900 units
Cost per unit     = ₹14,800 / 900 = ₹16.44/unit
```

---

**CASE 1 — Abnormal Loss:** Actual output = 870 units (Actual loss = 130)
```
Normal Loss  = 100 units
Actual Loss  = 130 units
Abnormal Loss = 130 − 100 = 30 units

Value of Abnormal Loss = 30 × ₹16.44 = ₹493.33
→ Charged to P&L (debit Abnormal Loss A/c)
```

**CASE 2 — Abnormal Gain:** Actual output = 920 units (Actual loss = 80)
```
Normal Loss  = 100 units
Actual Loss  = 80 units
Abnormal Gain = 100 − 80 = 20 units

Value of Abnormal Gain = 20 × ₹16.44 = ₹328.89
Scrap NOT collected (saved): 20 × ₹2 = ₹40 (deducted from gain)
→ Credited to P&L (credit Abnormal Gain A/c)
```

---

## 4.4 Valuation of Work-in-Progress (WIP)

> When a process ends but some units are **not fully complete**, they are called **Work-in-Progress (WIP)**. We convert them to **Equivalent Units** to calculate cost.

> **Equivalent Units** = WIP units expressed as equivalent fully-complete units based on % of completion.

```
Equivalent Units = Actual WIP units × % of Completion
```

### Two Methods of Valuing WIP: ⭐

---

### 📌 Method 1: FIFO Method

> Opening WIP is **completed first**, then fresh input. Old and new costs are kept **separate**.

```
STEP 1: Equivalent Units
= (Opening WIP × % work remaining to complete)
  + Units introduced AND completed in the period
  + (Closing WIP × % completion)

STEP 2: Cost per EU = Current Period Cost / Equivalent Units

STEP 3: Value outputs accordingly
```

---

### 📌 Method 2: Weighted Average Method

> Opening WIP costs are **merged with current period costs**. Simpler to calculate.

```
STEP 1: Equivalent Units
= Units Completed + (Closing WIP × % completion)
  [Opening WIP treated as if started this period]

STEP 2: Cost per EU = (Opening WIP Cost + Current Period Cost)
                      ──────────────────────────────────────────
                                  Equivalent Units

STEP 3: Value outputs accordingly
```

### ⚖️ FIFO vs Weighted Average

| Feature | FIFO | Weighted Average |
|---------|------|-----------------|
| **Opening WIP** | Kept separate from current | Mixed with current costs |
| **Complexity** | More complex | Simpler |
| **Cost accuracy** | More accurate | Less accurate |
| **Common use** | When prices fluctuate | When prices are stable |

---

### 📊 Solved Numerical: Equivalent Production (Weighted Average)

**Given:**
- Opening WIP: 200 units (60% complete), cost ₹3,000
- Input during period: 1,800 units, cost ₹18,000
- Labour & OH: ₹9,000
- Completed output: 1,700 units
- Closing WIP: 300 units (50% complete)

**Weighted Average Method:**

```
STEP 1: Equivalent Units
  Completed output              = 1,700 units (100%)   = 1,700 EU
  Closing WIP                   = 300 × 50%            = 150 EU
  Total Equivalent Units        =                        1,850 EU

STEP 2: Total Cost
  Opening WIP cost              = ₹3,000
  Current Material cost         = ₹18,000
  Labour & OH                   = ₹9,000
  Total                         = ₹30,000

STEP 3: Cost per Equivalent Unit
  = ₹30,000 / 1,850 = ₹16.22 per EU

STEP 4: Valuation
  Completed output = 1,700 × ₹16.22 = ₹27,573
  Closing WIP      = 150 × ₹16.22   = ₹2,433
  Total            = ₹30,006 ≈ ₹30,000 ✅
```

---

## 4.5 Joint Products and By-Products ⭐

### 📌 Joint Products

> **Joint Products** = Two or more products of **significant value** that are produced **simultaneously** from the same raw material up to a **split-off point**.

- Neither is a "main" product — both are important
- Up to split-off: **Joint Costs** (shared)
- After split-off: **Separate costs** (individual)

**Examples:**
| Industry | Joint Products |
|---------|---------------|
| Oil Refinery | Petrol, Diesel, Kerosene, LPG |
| Dairy | Cream, Skim Milk, Butter |
| Meat packing | Beef, Leather, Bone meal |

> 🧠 **BugZero Example:** When running a full test suite, BugZero produces simultaneously:
> - A **Test Coverage Report** (sold to client)
> - A **Performance Benchmark Report** (sold separately)
> Both come from the same test run (joint process)!

---

### 📌 By-Products

> **By-Products** = Products of **relatively minor value** produced incidentally alongside the main product.

- Main product = primary objective
- By-product = secondary/incidental output
- **Example:** Sawdust (by-product) when producing timber (main product)

---

### ⚖️ Joint Products vs By-Products

| Feature | Joint Products | By-Products |
|---------|---------------|-------------|
| **Importance** | Both significant | One main, one minor |
| **Value** | Both have substantial value | By-product has low value |
| **Planning** | Both are planned outputs | By-product is incidental |
| **Examples** | Petrol & Diesel | Molasses from sugarcane |

---

### 📌 Methods of Apportioning Joint Costs ⭐

When joint costs must be split between joint products:

| Method | Basis | Formula |
|--------|-------|---------|
| **1. Physical/Weight Basis** | Quantity of output | Joint Cost × (Units of Product / Total Units) |
| **2. Sales Value at Split-off** | Selling price at split-off | Joint Cost × (Sales Value of Product / Total Sales Value) |
| **3. Net Realizable Value (NRV)** | Final sales value minus further processing cost | Joint Cost × (NRV of Product / Total NRV) |
| **4. Average Cost Method** | Treats all units equally | Joint Cost / Total Units |

---

### 📊 Example: Apportionment by Sales Value

**Joint cost = ₹1,00,000. Products A and B at split-off:**

| Product | Units | Price/unit | Sales Value | Apportionment |
|---------|-------|-----------|-------------|---------------|
| A | 500 | ₹150 | ₹75,000 | 75/125 × 1,00,000 = **₹60,000** |
| B | 250 | ₹200 | ₹50,000 | 50/125 × 1,00,000 = **₹40,000** |
| **Total** | | | **₹1,25,000** | **₹1,00,000** |

---

### 📌 Treatment of By-Products (Accounting)

| Method | Treatment |
|--------|-----------|
| **Deduct from Joint Cost** | Sales value of by-product subtracted from total process cost |
| **Credit to P&L** | By-product revenue shown as other income |
| **Separate Costing** | By-product given its own cost and profit calculation |

> **Most commonly used:** Deduct by-product sales value from joint/process cost before calculating cost of main product.

---

## 4.6 📝 Summary

```
┌──────────────────────────────────────────────────────────────┐
│                   CHAPTER 4 SNAPSHOT                         │
├──────────────────────────────────────────────────────────────┤
│ PROCESS COSTING                                              │
│  → Continuous, homogeneous, multi-stage production           │
│  → Cost per unit = Net Cost / Expected Output                │
│                                                              │
│ PROCESS LOSSES                                               │
│  Normal Loss   → Expected, absorbed by good output           │
│  Abnormal Loss → Actual Loss > Normal Loss → Debit P&L       │
│  Abnormal Gain → Actual Loss < Normal Loss → Credit P&L      │
│                                                              │
│ WIP VALUATION                                                │
│  FIFO: Keep old & new costs separate                         │
│  Weighted Avg: Mix old & new costs together                  │
│  Equivalent Units = WIP units × % completion                 │
│                                                              │
│ JOINT PRODUCTS: Both significant, from same raw material     │
│ BY-PRODUCTS: Minor value, incidental to main product         │
│ Joint Cost Split: Physical / Sales Value / NRV method        │
└──────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. **Numerical: Prepare Process Account** with Normal Loss, Abnormal Loss/Gain ← Most Likely!
> 2. What is Normal Loss? How is it different from Abnormal Loss?
> 3. Calculate Equivalent Production using Weighted Average method (numerical)
> 4. Differentiate between Joint Products and By-Products
> 5. Explain methods of apportioning joint costs — with example
> 6. What is process costing? State its features.
> 7. How are by-products treated in accounts?

> [!TIP]
> **Quick formula card for Process Account:**
> - Cost per unit = (Input Cost − NL Scrap Value) ÷ (Input − NL units)
> - Abnormal Loss = Actual Loss − Normal Loss → valued at cost per unit → P&L (Dr)
> - Abnormal Gain = Normal Loss − Actual Loss → valued at cost per unit → P&L (Cr)

> [!NOTE]
> **Don't confuse:** Abnormal Loss → More loss than expected (BAD → Debit P&L)
> Abnormal Gain → Less loss than expected (GOOD → Credit P&L)
> Think: "Abnormal" just means it wasn't planned — could be good OR bad!

---
*📅 Created: 2026-06-29 | Chapter 4 | Management Accounting | DU SOL MBA Sem 2*
