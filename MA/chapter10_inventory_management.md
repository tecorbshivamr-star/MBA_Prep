# 📘 Chapter 10: Inventory Management
### Management Accounting | DU SOL | 2nd Semester
> 📖 **Mix of Theory + Numericals — Store Ledger questions are exam favourites!**

---

## 🎯 Learning Objectives
- Understand **Inventory Management** and why it matters
- Know all **costs associated** with holding inventory
- Learn **inventory control techniques**: ABC, VED, FSN, HML, GOLF, SDE
- Apply **EOQ** formula (recap from Ch. 2)
- Prepare **Store Ledgers** under FIFO, LIFO, and Weighted Average methods

---

## 10.2 Introduction

> Every business holds stock — raw materials, WIP, or finished goods. **Too much inventory = money locked up. Too little = production stops.**
> Inventory Management = Finding the **right balance**.

> 🧠 **BugZero Analogy:**
> BugZero needs USB testing dongles, server RAM, and software licenses in stock.
> - **Too much stock**: ₹2L locked in dongles nobody uses → opportunity cost
> - **Too little stock**: Project starts, no dongles available → testing delayed → client angry!
> **Inventory Management = having exactly the right amount, at the right time.**

---

## 10.3 Inventory Management

> **Inventory Management** = The systematic process of **ordering, storing, using, and replenishing** a company's inventory to ensure smooth operations while minimizing costs.

### 📌 Types of Inventory

| Type | Description | BugZero Example |
|------|-------------|----------------|
| **Raw Material** | Inputs not yet processed | USB dongles, server components |
| **Work-in-Progress (WIP)** | Partially processed/tested items | Projects currently being tested |
| **Finished Goods** | Completed, ready to deliver | Finalized test reports ready for clients |
| **Maintenance, Repair & Operating (MRO)** | Consumables for operations | Printer paper, cables, cleaning supplies |

### 📌 Objectives of Inventory Management
1. Ensure **uninterrupted supply** of materials for production
2. **Minimize investment** in inventory (reduce holding costs)
3. Prevent **stock-outs** (no production stoppages)
4. Prevent **excess stock** (avoid wastage and obsolescence)
5. Maintain **accurate inventory records**
6. Reduce **material handling and storage costs**

---

## 10.4 Costs Associated with Inventory ⭐⭐

### 1. 🛒 Ordering Cost (Procurement Cost)

> Costs incurred **each time an order is placed**, regardless of order size.

```
Examples: Cost of preparing purchase order, administrative expenses,
          inspection cost, transport/freight charges per order
```

```
Total Ordering Cost = Number of Orders × Cost per Order
Number of Orders    = Annual Demand / Order Quantity
```

**Relationship:** More orders placed → Higher ordering cost ↑

---

### 2. 📦 Carrying Cost (Holding Cost)

> Costs incurred to **hold and store** inventory.

```
Examples: Warehouse rent, insurance on stock, cost of capital tied up,
          obsolescence risk, deterioration, stores staff salary
```

```
Total Carrying Cost = Average Stock × Carrying Cost per unit per year
Average Stock       = Order Quantity / 2 (assuming uniform usage)
```

**Relationship:** Larger order quantity → More stock held → Higher carrying cost ↑

---

### 3. ⚠️ Stock-out Cost (Shortage Cost)

> Costs incurred when inventory **runs out** and demand cannot be met.

```
Examples: Lost sales, emergency purchases at higher prices,
          production downtime, customer dissatisfaction, lost goodwill
```

**Relationship:** Lower safety stock → Higher risk of stock-out → Higher stock-out cost ↑

---

### 4. 💰 Purchase Cost

> The **actual price paid** for the item × quantity purchased.

```
Total Purchase Cost = Units Purchased × Price per Unit
```

May decrease with **bulk discounts** (quantity discounts).

---

### 📌 The Trade-Off (Total Cost Curve)

```
Cost ↑
      │           Total Cost = Ordering + Carrying
      │          ╲           /
      │            ╲       /
      │   Carrying   ╲   / Ordering Cost
      │   Cost         ╳
      │              / ╲ ← EOQ (Minimum Total Cost)
      └─────────────────────────── Order Qty →
```

> **EOQ = The order quantity where Ordering Cost = Carrying Cost → Total Cost is MINIMUM**

---

## 10.5 Techniques of Inventory Management ⭐⭐⭐

### 📌 A) ABC Analysis ⭐ (Covered in Ch. 2 — Quick Recap)

| Class | % of Items | % of Value | Control |
|-------|-----------|-----------|---------|
| **A** | 10% | 70-80% | **Tight** — frequent review, close monitoring |
| **B** | 20% | 15-20% | **Moderate** |
| **C** | 70% | 5-10% | **Loose** — bulk ordering, periodic review |

---

### 📌 B) VED Analysis ⭐⭐ (NEW — Exam Favourite!)

> **VED** = Classification based on **criticality/essentiality** of the item to operations.

| Class | Full Form | Meaning | Example at BugZero |
|-------|----------|---------|-------------------|
| **V** | **Vital** | Without this, operations STOP completely | Selenium testing framework license |
| **E** | **Essential** | Operations severely hampered without it | Postman API testing tool |
| **D** | **Desirable** | Useful but operations can continue without it | Adobe Acrobat for reports |

> 🔑 **Use VED for**: Manufacturing & IT firms where certain materials/tools are mission-critical.
> V items → **Stock maintained at all times, even if expensive**

---

### 📌 C) FSN Analysis ⭐⭐

> **FSN** = Classification based on **movement/usage rate** of items.

| Class | Full Form | Meaning | Action |
|-------|----------|---------|--------|
| **F** | **Fast Moving** | Consumed quickly, high turnover | Order frequently, keep adequate stock |
| **S** | **Slow Moving** | Consumed slowly, low turnover | Review regularly, avoid overstocking |
| **N** | **Non-Moving** | Not consumed at all (dead stock) | Dispose of, write off, or return |

> 💼 **BugZero Example:**
> - **F**: USB Type-C cables (used daily) → Order frequently
> - **S**: HDMI adapters (used occasionally) → Monitor carefully
> - **N**: Old CD-ROM drive (nobody uses it) → Dispose of it!

---

### 📌 D) HML Analysis

> **HML** = Classification based on **unit price** of the item (similar to ABC but by price, not total value).

| Class | Full Form | Meaning |
|-------|----------|---------|
| **H** | **High** | High unit price items |
| **M** | **Medium** | Medium unit price items |
| **L** | **Low** | Low unit price items |

> Used for **controlling purchasing authority** — high-value items require senior approval.

---

### 📌 E) GOLF Analysis

> **GOLF** = Classification based on **source of supply**.

| Class | Full Form | Meaning |
|-------|----------|---------|
| **G** | **Government** | Obtained from govt sources (controlled materials) |
| **O** | **Ordinary** | Obtained from open market |
| **L** | **Local** | Obtained locally |
| **F** | **Foreign** | Imported materials |

> Helps in **lead time planning** — foreign items need longer lead times, import procedures.

---

### 📌 F) SDE Analysis

> **SDE** = Classification based on **availability/difficulty in procurement**.

| Class | Full Form | Meaning |
|-------|----------|---------|
| **S** | **Scarce** | Rare items, difficult to get, need high safety stock |
| **D** | **Difficult** | Available but takes time, need moderate safety stock |
| **E** | **Easy** | Easily available, no need for large safety stock |

---

### 📌 Combining Analyses

In practice, companies combine two analyses for better control:
- **ABC + VED**: Most powerful combination
  - A+V items = Most critical → Tightest control
  - C+D items = Low value + Desirable → Least attention

---

## 10.6 Economic Order Quantity (EOQ) ⭐⭐

> (Covered in detail in Chapter 2 — Quick Reference)

```
         ┌────────────────┐
EOQ =   │   2 × A × O   │
         │  ───────────   │
         │       C        │
         └────────────────┘

A = Annual Demand (units)
O = Ordering Cost per order (₹)
C = Carrying Cost per unit per year (₹)
```

### 📊 Solved Example
Annual demand = 8,000 units. Ordering cost = ₹125. Carrying cost = ₹2/unit/year.

```
EOQ = √(2 × 8,000 × 125 / 2)
    = √(20,00,000 / 2)
    = √10,00,000
    = 1,000 units

No. of orders per year = 8,000 / 1,000 = 8 orders
Total Ordering Cost    = 8 × ₹125 = ₹1,000
Average Stock          = 1,000 / 2 = 500 units
Total Carrying Cost    = 500 × ₹2 = ₹1,000
Total Inventory Cost   = ₹1,000 + ₹1,000 = ₹2,000 (Minimum!) ✅
```

---

## 10.7 Just-in-Time (JIT)

> (Covered in detail in Chapter 8 — Quick Reference)

```
Key Idea: Order/Produce ONLY what is needed, WHEN needed
Result: Near-zero inventory → Eliminates carrying cost
Risk: Any supply disruption = production halt
```

**JIT vs Traditional Inventory:**

| Feature | Traditional | JIT |
|---------|------------|-----|
| Stock Level | High safety stock | Minimal/Zero |
| Order Size | Large batch | Small, frequent |
| Supplier Relation | Multiple suppliers | Few, trusted partners |
| Focus | Avoid stock-out | Eliminate waste |

---

## 10.8 Methods of Inventory Valuation ⭐⭐⭐

When materials are **issued from stores to production**, what price do we use? Three main methods:

---

### 📌 Method 1: FIFO (First In, First Out) ⭐⭐⭐

> **FIFO** = The items that came in **first** are assumed to be issued/used **first**.
> **Closing stock = valued at most recent (latest) prices**

```
Issue price = Oldest stock price first → then next oldest → and so on
```

**Impact in Rising Prices:**
- Issues at LOWER prices → Lower COGS → HIGHER Profit → MORE tax
- Closing stock at HIGHER (current) prices → Accurate balance sheet

---

### 📌 Method 2: LIFO (Last In, First Out) ⭐⭐

> **LIFO** = The items that came in **last** are assumed to be issued/used **first**.
> **Closing stock = valued at oldest prices**

```
Issue price = Most recent stock first → then next recent → and so on
```

**Impact in Rising Prices:**
- Issues at HIGHER prices → Higher COGS → LOWER Profit → LESS tax
- Closing stock at LOWER (old) prices → Understated balance sheet
- **NOT accepted under Ind AS / IFRS** (but can be asked in exams!)

---

### 📌 Method 3: Weighted Average Price ⭐⭐⭐

> **WAP** = A new average price is calculated **each time a new receipt comes in**.
> All issues use this average price until the next receipt.

```
Weighted Average Price = Total Value of Stock in Hand
                        ─────────────────────────────
                         Total Units in Hand
```

**Impact:** Smooths out price fluctuations. Between FIFO and LIFO for profit.

---

## 10.9 📊 Solved Practical Questions

### 🔢 Store Ledger Numerical

**Transactions for BugZero's USB Dongles:**

| Date | Particulars | Units | Rate (₹) |
|------|------------|-------|----------|
| Apr 1 | Opening Stock | 100 | ₹20 |
| Apr 5 | Received | 200 | ₹22 |
| Apr 10 | Issued | 150 | — |
| Apr 15 | Received | 100 | ₹25 |
| Apr 20 | Issued | 180 | — |
| Apr 30 | Closing Stock | ? | ? |

---

### ✅ FIFO Method

```
Apr 1: Opening = 100 units @ ₹20 = ₹2,000

Apr 5: Receipt = 200 @ ₹22 → Stock: 100@₹20 + 200@₹22

Apr 10: Issue 150 units (FIFO: oldest first)
  → Issue all 100 @ ₹20 = ₹2,000
  → Issue 50 @ ₹22 = ₹1,100
  → Total Issue value = ₹3,100
  → Remaining: 150 @ ₹22 = ₹3,300

Apr 15: Receipt 100 @ ₹25 → Stock: 150@₹22 + 100@₹25

Apr 20: Issue 180 units (FIFO: oldest first)
  → Issue all 150 @ ₹22 = ₹3,300
  → Issue 30 @ ₹25 = ₹750
  → Total Issue value = ₹4,050
  → Remaining: 70 @ ₹25

CLOSING STOCK (FIFO) = 70 units × ₹25 = ₹1,750
Total Issues = ₹3,100 + ₹4,050 = ₹7,150
```

---

### ✅ LIFO Method

```
Apr 1: Opening = 100 units @ ₹20 = ₹2,000

Apr 5: Receipt = 200 @ ₹22 → Stock: 100@₹20 + 200@₹22

Apr 10: Issue 150 units (LIFO: newest first)
  → Issue all 150 from 200 @ ₹22 = ₹3,300
  → Remaining: 100@₹20 + 50@₹22

Apr 15: Receipt 100 @ ₹25 → Stock: 100@₹20 + 50@₹22 + 100@₹25

Apr 20: Issue 180 units (LIFO: newest first)
  → Issue all 100 @ ₹25 = ₹2,500
  → Issue all 50 @ ₹22 = ₹1,100
  → Issue 30 @ ₹20 = ₹600
  → Total Issue value = ₹4,200
  → Remaining: 70 @ ₹20

CLOSING STOCK (LIFO) = 70 units × ₹20 = ₹1,400
Total Issues = ₹3,300 + ₹4,200 = ₹7,500
```

---

### ✅ Weighted Average Method

```
Apr 1: Stock = 100 @ ₹20 = ₹2,000

Apr 5: Receipt = 200 @ ₹22 = ₹4,400
  New Total: 300 units = ₹6,400
  WAP = ₹6,400 / 300 = ₹21.33/unit

Apr 10: Issue 150 @ ₹21.33 = ₹3,200
  Remaining: 150 units @ ₹21.33 = ₹3,200

Apr 15: Receipt 100 @ ₹25 = ₹2,500
  New Total: 250 units = ₹3,200 + ₹2,500 = ₹5,700
  WAP = ₹5,700 / 250 = ₹22.80/unit

Apr 20: Issue 180 @ ₹22.80 = ₹4,104
  Remaining: 70 units @ ₹22.80 = ₹1,596

CLOSING STOCK (WAP) = 70 units × ₹22.80 = ₹1,596
Total Issues = ₹3,200 + ₹4,104 = ₹7,304
```

---

### 📊 Comparison Summary

| Method | Issues (Cost) | Closing Stock | Profit Effect |
|--------|--------------|--------------|--------------|
| **FIFO** | ₹7,150 (Lower) | ₹1,750 (Higher) | **Highest Profit** |
| **WAP** | ₹7,304 (Middle) | ₹1,596 (Middle) | **Middle Profit** |
| **LIFO** | ₹7,500 (Higher) | ₹1,400 (Lower) | **Lowest Profit** |

> 🔑 **Key Insight (Rising Prices):**
> FIFO → Lower cost of issues → Higher closing stock → Higher profit
> LIFO → Higher cost of issues → Lower closing stock → Lower profit

---

## 10.10 📝 Summary

```
┌──────────────────────────────────────────────────────────────┐
│                    CHAPTER 10 SNAPSHOT                       │
├──────────────────────────────────────────────────────────────┤
│ INVENTORY COSTS                                              │
│  1. Ordering Cost  → Per order, decreases with larger orders │
│  2. Carrying Cost  → Per unit held, increases with stock     │
│  3. Stock-out Cost → Cost of running out                     │
│  4. Purchase Cost  → Price × Quantity                        │
│                                                              │
│ CONTROL TECHNIQUES                                           │
│  ABC → By value (High/Med/Low value)                         │
│  VED → By criticality (Vital/Essential/Desirable)            │
│  FSN → By movement (Fast/Slow/Non-moving)                    │
│  HML → By unit price (High/Medium/Low price)                 │
│  SDE → By availability (Scarce/Difficult/Easy)               │
│                                                              │
│ EOQ = √(2AO/C)  → Minimizes total inventory cost            │
│                                                              │
│ VALUATION METHODS (Rising Prices):                           │
│  FIFO → Lowest issues, Highest closing stock, Highest profit │
│  LIFO → Highest issues, Lowest closing stock, Lowest profit  │
│  WAP  → Middle of both                                       │
└──────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. **Store Ledger numerical under FIFO, LIFO, and Weighted Average** ← Most Likely!
> 2. What is ABC Analysis? How does it differ from VED Analysis?
> 3. Explain **VED Analysis** and **FSN Analysis** with examples
> 4. What are the **costs associated with inventory**? Explain each.
> 5. Calculate **EOQ** and find total inventory cost (numerical)
> 6. Compare FIFO, LIFO, and Weighted Average — which gives highest profit and why?
> 7. What is **SDE Analysis**? Give examples.

> [!TIP]
> **Store Ledger Exam Trick:**
> Always verify: Opening Stock Value + Receipts = Issues + Closing Stock
> (Both in Units and ₹ value — use this to catch errors!)

> [!NOTE]
> **VED vs ABC — Key Difference:**
> ABC = Based on **₹ value** of items (financial importance)
> VED = Based on **operational criticality** (can we function without it?)
> A "C" class item (cheap, low value) could still be "V" (Vital!) — e.g., a ₹2 rubber seal in a machine

---
*📅 Created: 2026-06-29 | Chapter 10 | Management Accounting | DU SOL MBA Sem 2*
