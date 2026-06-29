# 📘 Chapter 3: Job, Batch and Contract Costing
### Management Accounting | DU SOL | 2nd Semester

---

## 🎯 Learning Objectives
- Understand **Job Costing** — what it is, how it works, pros and cons
- Learn **Batch Costing** and how batch size is determined
- Understand **Contract Costing** — its special terms and profit calculation
- Compare all three methods clearly
- Solve numerical problems on contract costing

---

## 3.1 Introduction

Different industries produce different types of products/services. The method of **costing varies** based on the nature of production:

| Production Type | Costing Method |
|----------------|----------------|
| Custom/unique jobs | **Job Costing** |
| Identical units in groups | **Batch Costing** |
| Large, long-term construction work | **Contract Costing** |
| Continuous mass production | Process Costing (Ch.4) |

> 🧠 **BugZero Analogy:**
> - Building a **custom QA dashboard** for one client = **Job Costing**
> - Deploying the **same test suite** for 100 similar apps = **Batch Costing**
> - Winning a **₹50L 2-year contract** to automate testing for a bank = **Contract Costing**

---

## 3.2 Job Costing

> **Job Costing** = A method where costs are collected and accumulated **separately for each job or order**, which is carried out according to customer specifications.

### 📌 Features of Job Costing
1. Each job is **unique** — done to customer's specification
2. Each job has a **separate Job Cost Card/Sheet**
3. Production is **against specific orders**, not for stock
4. Costs are tracked **job-by-job**
5. Used in: Printing presses, Engineering workshops, Interior design, Custom software development

---

### 📋 Job Cost Sheet Format

```
┌─────────────────────────────────────────────────────────────┐
│                    JOB COST SHEET                           │
│  Job No.: ____  Customer: ____  Date Started: ____         │
├─────────────────────────────────────────────────────────────┤
│  PARTICULARS                                      ₹         │
├─────────────────────────────────────────────────────────────┤
│  A. DIRECT MATERIAL                                         │
│     Material issued to job                      XX,XXX      │
│                                                             │
│  B. DIRECT LABOUR                                           │
│     Hours × Rate per hour                       XX,XXX      │
│                                                             │
│  C. DIRECT EXPENSES                                         │
│     Subcontractor / special tools               XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  PRIME COST (A+B+C)                             XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  D. FACTORY OVERHEAD                                        │
│     (OAR × Machine/Labour hours)                XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  WORKS COST                                     XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  E. ADMIN OVERHEAD (% of Works Cost)            XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  COST OF PRODUCTION                             XX,XXX      │
├─────────────────────────────────────────────────────────────┤
│  F. SELLING & DIST. OVERHEAD                   XX,XXX       │
├─────────────────────────────────────────────────────────────┤
│  TOTAL COST / COST OF JOB                      XX,XXX       │
│  PROFIT (as agreed)                            XX,XXX       │
│  SELLING PRICE / INVOICE PRICE                 XX,XXX       │
└─────────────────────────────────────────────────────────────┘
```

---

### ✅ Advantages of Job Costing

| Advantage | Explanation |
|-----------|-------------|
| **Accurate Cost** | Cost of each job known precisely |
| **Profitability Analysis** | Profit/loss per job easily identified |
| **Customer Billing** | Exact cost basis for invoicing |
| **Cost Control** | Actual vs estimated cost compared per job |
| **Quotation Aid** | Helps in quoting future similar jobs |
| **Accountability** | Each job has a responsible person |

### ❌ Limitations of Job Costing

| Limitation | Explanation |
|-----------|-------------|
| **Expensive** | Maintaining separate records for every job is costly |
| **Clerical Work** | Extensive paperwork and documentation |
| **No Standardization** | Each job is different — hard to compare |
| **Historical** | Costs known only after completion |
| **Overhead Allocation** | Arbitrary, may distort job cost |

> 💼 **BugZero Example:**
> BugZero gets a job to do **security testing of a fintech app** for ₹2L.
> They track every engineer's hour, every tool used, every bug reported separately.
> At end: Total cost = ₹1.4L → Profit = ₹60,000 on this job ✅

---

## 3.3 Batch Costing

> **Batch Costing** = A form of job costing where instead of costing a **single unit**, costs are collected for a **batch (group) of identical units**, and then cost per unit is calculated.

```
Cost per Unit = Total Cost of Batch / Number of Units in Batch
```

### 📌 Features of Batch Costing
1. A batch = group of **identical, similar products**
2. Each batch gets a **Batch Cost Sheet** (like job cost sheet)
3. Cost per unit = Total batch cost ÷ Units in batch
4. Used in: Pharmaceuticals, Bakeries, Electronics, Spare parts manufacturing

### 📌 Determining Optimum Batch Size
Same concept as **EOQ** — balance between setup cost and carrying cost:

```
         ┌──────────────────────┐
Batch  = │  2 × D × S           │
 Size    │  ─────────────────   │
(EBQ)    │  C                   │
         └──────────────────────┘

Where:
D = Annual Demand (units)
S = Setting-up / Batch Setup Cost (₹)
C = Carrying Cost per unit per year (₹)
```

> 💼 **BugZero Example:**
> BugZero creates **100 identical USB testing dongles** for internal use.
> Total batch cost = ₹50,000 → Cost per dongle = ₹50,000 / 100 = **₹500 each**

---

## 3.4 Difference: Job Costing vs Batch Costing

| Feature | Job Costing | Batch Costing |
|---------|------------|---------------|
| **Unit** | Single unique job | Group of identical units |
| **Customer** | Made to specific order | May be for stock or order |
| **Cost Unit** | Each job | Each batch (then per unit) |
| **Identity** | Each job differs | All units in batch are same |
| **Industries** | Printing, construction, IT consulting | Pharma, bakery, electronics |
| **Similarity** | Both use a Cost Sheet, both are forms of specific order costing |

---

## 3.5 Contract Costing

> **Contract Costing** = A method of costing for **large, long-term contracts** (usually construction/civil works) that span **more than one accounting year**, carried out at the **customer's site**.

Also called: **Terminal Costing** or **Long-term Job Costing**

### 📌 Features of Contract Costing
1. Work done at the **contractee's (client's) site**
2. Contracts are **long-term** — often 2–5 years
3. Contract price is **fixed in advance**
4. A **separate account** is maintained for each contract
5. Contractor bears the **risk of cost overrun**
6. Used in: Civil construction, shipbuilding, large IT infrastructure projects

> 💼 **BugZero Example:**
> BugZero wins a **₹1 Crore, 2-year contract** to build and implement an end-to-end automated testing platform for State Bank. Work happens at the bank's premises. BugZero tracks every cost month by month for this contract.

---

## 3.6 Difference: Job Costing vs Contract Costing

| Feature | Job Costing | Contract Costing |
|---------|------------|-----------------|
| **Duration** | Short-term (days/weeks) | Long-term (months/years) |
| **Location** | Contractor's factory/office | Contractee's (client's) site |
| **Value** | Relatively small | Very large |
| **Profit** | Taken when job complete | Taken progressively year-by-year |
| **Subcontracting** | Rare | Very common |
| **Accounting** | Simple | Complex (WIP, retention, escalation) |
| **Risk** | Lower | Higher |

---

## 3.7 Special Terms in Contract Costing ⭐⭐

### 1. 📋 Work Certified (Architect's Certificate)
> The **value of work completed** and certified by the architect/engineer as per contract terms.
- Progress payments are made based on Work Certified
- Forms basis of profit calculation

### 2. 📋 Work Uncertified (WIP)
> Work that has been **completed but NOT yet certified** by the architect.
- Appears as **Work-in-Progress** on the Balance Sheet
- Valued at **Cost** (not selling price)

### 3. 💰 Retention Money
> A portion of Work Certified that the **contractee (client) retains** and does NOT pay until the contract is fully complete.

```
Cash Received = Work Certified − Retention Money

Retention % is typically 10%–20% of Work Certified
```

> 🧠 **Analogy:** Like a **security deposit** held by the client until the full job is done and defects are fixed. BugZero completes ₹30L worth of testing work. Client certifies it but retains 10% (₹3L) until final delivery.

### 4. 📈 Escalation Clause
> A clause in the contract allowing the **contract price to be revised** if prices of materials/labour increase beyond a certain level.
- Protects contractor from inflation
- Common in long-term contracts

> 🧠 **Analogy:** Like a **variable rate home loan** — if RBI increases rates, your EMI goes up. Escalation clause protects BugZero if software license costs shoot up during the 2-year contract.

### 5. 💡 Notional Profit
> **Estimated profit** earned on work done to date (not the final profit).

```
Notional Profit = Value of Work Certified − Cost of Work Certified

Cost of Work Certified = Total Cost to Date − Cost of WIP (Uncertified Work)
```

### 6. 🏗️ Contract Account Structure

```
DR                CONTRACT ACCOUNT                CR
─────────────────────────────────────────────────
Materials issued      ₹XX   | Work Certified      ₹XX
Labour                ₹XX   | WIP (uncertified)   ₹XX
Plant/Machinery       ₹XX   | Plant returned      ₹XX
Subcontractor         ₹XX   | Materials returned  ₹XX
OH charged            ₹XX   |
Profit (P&L)          ₹XX   |
─────────────────────────────────────────────────
```

---

## 3.8 Profit on Incomplete Contracts ⭐⭐⭐

> When a contract spans multiple years, we cannot wait until completion to recognize profit. Profit is taken **progressively** based on stage of completion.

### 🔢 Stage of Completion

```
Stage of Completion (%) = (Work Certified / Contract Price) × 100
```

### 🔢 Profit Formula (Most Important ⭐)

```
If Stage < 25% (Very Early):
   Profit credited to P&L = NIL (too uncertain)

If Stage is 25% to 50%:
   Profit = 1/3 × Notional Profit × (Cash Received / Work Certified)

If Stage is 50% to 90%:
   Profit = 2/3 × Notional Profit × (Cash Received / Work Certified)

If Stage > 90% (Near Completion):
   Profit = Estimated Total Profit × (Work Certified / Contract Price)
   OR use engineer's estimate of final profit
```

> 🧠 **Why these rules?**
> The **further along** the contract, the more **certain** the profit. In early stages, things can go wrong — so accountants are **conservative** and recognize less profit.

### 📋 Treatment Summary Table

| % Complete | Profit Recognized | Reason |
|-----------|-------------------|--------|
| < 25% | **Nil** | Too risky, too early |
| 25% – 50% | **1/3** × Notional Profit × Cash/Certified | Some certainty |
| 50% – 90% | **2/3** × Notional Profit × Cash/Certified | Reasonable certainty |
| > 90% | **Full estimated profit** | Near complete |

---

## 3.9 Treatment of Financial Elements in Contract Costing

| Element | Treatment |
|---------|-----------|
| **Materials sent to site** | Debit Contract A/c |
| **Materials returned from site** | Credit Contract A/c |
| **Materials stolen/destroyed** | Debit to P&L (abnormal loss) |
| **Plant purchased for contract** | Debit Contract A/c at cost |
| **Plant depreciation** | Charge to Contract A/c (depreciation amount only) |
| **Plant returned after contract** | Credit Contract A/c at WDV |
| **Subcontractor charges** | Debit Contract A/c |
| **Work Certified** | Credit Contract A/c |
| **Work Uncertified (WIP)** | Credit Contract A/c → B/S as WIP |
| **Profit to P&L** | Credit P&L, balance goes to Reserve |

---

## 3.10 📊 Solved Numerical: Contract Costing

**Problem:** BugZero wins a ₹20,00,000 contract to build a testing platform for a bank.
At year end, the following data is available:

| Item | ₹ |
|------|---|
| Materials sent to site | 5,00,000 |
| Materials returned from site | 20,000 |
| Labour | 3,00,000 |
| Plant (sent to site) | 2,00,000 |
| Plant depreciation for year | 40,000 |
| Overhead charged | 60,000 |
| Work Certified | 12,00,000 |
| Work Uncertified (WIP) | 50,000 |
| Cash received from bank (client) | 10,80,000 |

**Step 1: Prepare Contract Account**
```
DR          CONTRACT ACCOUNT                CR
───────────────────────────────────────────────────────
Materials         5,00,000 | Materials returned   20,000
Labour            3,00,000 | Plant (at WDV)      1,60,000
Plant             2,00,000 |   (2,00,000-40,000)
Depreciation        40,000 | Work Certified     12,00,000
Overhead            60,000 | WIP (Uncertified)     50,000
Profit to P&L    4,30,000 |
                ─────────                    ─────────
                14,30,000                   14,30,000
```

**Step 2: Calculate Notional Profit**
```
Work Certified                 = ₹12,00,000
Cost of Work Certified         = Total Cost − WIP
                               = (5,00,000 − 20,000 + 3,00,000 + 40,000 + 60,000) − 50,000
                               = 8,80,000 − 50,000 = ₹8,30,000

Notional Profit = 12,00,000 − 8,30,000 = ₹3,70,000
```

**Step 3: Determine Stage of Completion**
```
Stage = (12,00,000 / 20,00,000) × 100 = 60%
→ Between 50%–90% → Use 2/3 formula
```

**Step 4: Calculate Profit to be credited to P&L**
```
Profit = 2/3 × Notional Profit × (Cash Received / Work Certified)
       = 2/3 × 3,70,000 × (10,80,000 / 12,00,000)
       = 2/3 × 3,70,000 × 0.9
       = 2/3 × 3,33,000
       = ₹2,22,000 → Credited to P&L

Remaining (₹3,70,000 − ₹2,22,000 = ₹1,48,000) → Transferred to Reserve (WIP Reserve)
```

---

## 📝 Summary

```
┌──────────────────────────────────────────────────────────────┐
│                   CHAPTER 3 SNAPSHOT                         │
├──────────────────────────────────────────────────────────────┤
│ JOB COSTING                                                  │
│  → Unique, custom jobs. Separate cost sheet per job.         │
│  → Cost = DM + DL + DE + Overhead                           │
│                                                              │
│ BATCH COSTING                                                │
│  → Identical units in a group. Cost per unit = Total/Units   │
│  → EBQ = √(2DS/C) to find optimal batch size                │
│                                                              │
│ CONTRACT COSTING                                             │
│  → Long-term, large, at client's site                        │
│  → Key Terms: Work Certified, Uncertified, Retention,        │
│    Escalation Clause, Notional Profit                        │
│  → Profit Rules:                                             │
│     <25%  → Nil                                              │
│     25-50% → 1/3 × NP × (Cash/Certified)                    │
│     50-90% → 2/3 × NP × (Cash/Certified)                    │
│     >90%  → Full estimated profit                            │
└──────────────────────────────────────────────────────────────┘
```

---

## 🔥 Likely Exam Questions

> [!IMPORTANT]
> 1. Define Job Costing. State its advantages and limitations.
> 2. Differentiate between Job Costing and Batch Costing (table).
> 3. Differentiate between Job Costing and Contract Costing (table).
> 4. Explain any 4 special terms used in Contract Costing.
> 5. What is Notional Profit? How is profit recognized on incomplete contracts?
> 6. **Numerical: Prepare Contract Account + Calculate Profit to P&L** ← Most likely!
> 7. What is an Escalation Clause? What is Retention Money?

> [!TIP]
> **Memory Trick for Profit Rules:** Think **"Nothing → 1/3 → 2/3 → Full"**
> as the contract moves from Early → Quarter → Half → Near Done

> [!NOTE]
> **Key difference:** Retention Money = client holds back cash (₹ not yet received).
> WIP/Uncertified = work done but not yet certified (work not yet billed).
> These are two different adjustments — don't mix them up!

---
*📅 Created: 2026-06-29 | Chapter 3 | Management Accounting | DU SOL MBA Sem 2*
