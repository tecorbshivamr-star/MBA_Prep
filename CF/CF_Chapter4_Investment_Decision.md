# 📘 Corporate Finance — Chapter 4: Investment Decision (Capital Budgeting)
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** Capital Budgeting is extremely numerical. Master cash flow estimation (incremental approach), NPV & IRR calculations, and the NPV vs. IRR conflict (ranking reversal). Expect a full capital budgeting numerical (10–15 marks) and theory on NPV superiority over other methods.

---

## 4.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Identify and classify types of capital budgeting decisions
- ✅ Estimate relevant (incremental) cash flows for project evaluation
- ✅ Describe the capital budgeting process step-by-step
- ✅ Apply all evaluation techniques: Payback, ARR, NPV, IRR, MIRR, PI
- ✅ Explain and resolve NPV vs. IRR conflicts
- ✅ Apply the Profitability Index for capital rationing situations

---

## 4.2 Introduction

### What is Capital Budgeting?

**Capital Budgeting** (also called **Investment Appraisal**) is the process of **planning and evaluating long-term investments** in fixed assets — projects whose benefits are expected to be received over multiple future periods.

> 📌 *"Capital Budgeting involves commitment of funds now in anticipation of returns to be received in the future."*

### Why is Capital Budgeting Critical?

| Reason | Explanation |
|---|---|
| **Large Sums Involved** | CAPEX decisions involve significant capital commitment |
| **Long-term Impact** | Affect the firm's competitive position for years/decades |
| **Irreversibility** | Difficult and costly to reverse once committed |
| **Strategic Importance** | Determines future growth, product lines, technology |
| **Risk** | Long time horizons increase uncertainty |

### Capital Budgeting vs. Working Capital Management:

| Feature | **Capital Budgeting** | **Working Capital** |
|---|---|---|
| **Time Horizon** | Long-term (> 1 year) | Short-term (< 1 year) |
| **Assets Involved** | Fixed/Non-current assets | Current assets |
| **Decision Type** | CAPEX | Operational |
| **Reversibility** | Low | High |

---

## 4.3 Types of Capital Budgeting Decision Situations

### Classification 1: By Nature of Decision

| Type | Description | Example |
|---|---|---|
| **Replacement Decisions** | Replace old/worn-out asset with new one | Replace old machine with efficient one |
| **Expansion Decisions** | Add capacity in existing product lines | New production line for existing product |
| **Diversification Decisions** | Enter new product/market/geography | Launch a new product category |
| **Modernisation Decisions** | Upgrade technology to reduce costs | Automate a manual process |
| **Research & Development** | Invest in new technology/product R&D | Pharmaceutical drug research |
| **Mandatory Investments** | Legally required, no profit motive | Pollution control, safety equipment |

---

### Classification 2: By Dependency

| Type | Description |
|---|---|
| **Independent Projects** | Acceptance of one has no effect on the other; evaluated separately |
| **Mutually Exclusive Projects** | Accepting one means rejecting the other (only ONE can be chosen) |
| **Contingent/Dependent Projects** | Acceptance of one requires acceptance of another |
| **Complementary Projects** | Acceptance of one increases cash flows of another |
| **Substitute Projects** | Acceptance of one reduces cash flows of another |

> 📌 **Mutually exclusive** projects are the most common exam scenario — requires **ranking** using NPV/IRR.

---

### Classification 3: By Size / Strategy

| Type | Description |
|---|---|
| **Conventional** | One initial outlay followed by positive cash inflows |
| **Non-Conventional** | Multiple sign changes in cash flows (multiple IRRs possible) |

---

## 4.4 Estimation of Costs and Benefits (Cash Flow Estimation)

### The Golden Rule: **Use INCREMENTAL CASH FLOWS**

> Only consider cash flows that **change because of** the project. Ignore sunk costs; include opportunity costs.

### Key Principles:

| Principle | Explanation |
|---|---|
| **Incremental Basis** | Only consider changes in cash flows caused by the project |
| **After-Tax Basis** | All cash flows must be on an after-tax basis |
| **Cash Flow ≠ Profit** | Use cash flows (not accounting profit); add back depreciation |
| **Ignore Sunk Costs** | Past costs already incurred — irrelevant to future decisions |
| **Include Opportunity Costs** | Foregone cash flows from alternative use must be included |
| **Include Side Effects** | Cannibalisation of existing products must be factored in |
| **Working Capital** | Changes in NWC are cash outflows (beginning) and inflows (end) |

---

### Three Components of Project Cash Flows:

```
PROJECT CASH FLOWS
│
├── 1. INITIAL INVESTMENT (t=0)
│       └── Outflow at start of project
│
├── 2. OPERATING CASH FLOWS (t=1 to n)
│       └── Annual net inflows during project life
│
└── 3. TERMINAL CASH FLOW (t=n)
        └── Cash flows at end of project life
```

---

### Component 1: Initial Investment Outlay (t = 0)

```
Initial Investment =
  Cost of new asset (purchase price)
+ Installation / commissioning costs
+ Increase in Net Working Capital (NWC)
− Salvage value of old asset (if replacement)
± Tax on gain/loss on sale of old asset
```

**Tax on Sale of Old Asset:**
```
If Sale Price > Book Value → Capital Gain → Pay Tax on Gain
If Sale Price < Book Value → Capital Loss → Tax Saving (negative outflow)
If Sale Price = Book Value → No tax effect

Tax on Gain = (Sale Price − Book Value) × Tax Rate
```

#### Example — Replacement Decision:
> New machine cost: ₹10,00,000. Old machine book value: ₹2,00,000, sold for ₹3,00,000. Tax = 30%. Additional NWC required: ₹50,000.

```
Cost of new machine              = ₹10,00,000
Less: Sale proceeds of old       = ₹ 3,00,000
Less: Tax saved on old sale gain = -(3,00,000 − 2,00,000) × 30% = −₹30,000  [Tax payable, so add back]
Add: Tax on gain                 = +₹30,000
Add: Additional NWC              = ₹   50,000
─────────────────────────────────────────────
Initial Investment               = ₹ 7,80,000
```

---

### Component 2: Operating Cash Flows (t = 1 to n)

**Two methods to calculate:**

#### Method A: Cash Flow from Operations
```
Operating CF = (Revenue − Operating Costs) × (1 − Tax) + Depreciation × Tax

Or equivalently:
Operating CF = EBIT × (1 − t) + Depreciation
             = Net Operating Profit After Tax (NOPAT) + Depreciation
```

#### Method B: From Net Profit
```
Operating CF = Net Profit After Tax + Depreciation
             = EAT + Depreciation
```

> 💡 **Depreciation is added back** because it is a **non-cash charge** — it reduces taxable profit (gives tax shield) but does not involve actual cash outflow.

**Depreciation Tax Shield:**
```
Tax Shield on Depreciation = Depreciation × Tax Rate

After-tax cost of Depreciation = Depreciation × (1 − Tax Rate)
```

#### Example:
> Revenue = ₹5,00,000; Operating Costs = ₹2,00,000; Depreciation = ₹1,00,000; Tax = 30%.

```
EBIT = 5,00,000 − 2,00,000 − 1,00,000 = ₹2,00,000
EBT  = ₹2,00,000 (no interest, all-equity)
Tax  = 2,00,000 × 30% = ₹60,000
EAT  = ₹1,40,000

Operating CF = EAT + Depreciation = 1,40,000 + 1,00,000 = ₹2,40,000

Check: (Revenue − Costs)(1−t) + Dep×t
     = 3,00,000 × 0.70 + 1,00,000 × 0.30
     = 2,10,000 + 30,000 = ₹2,40,000 ✓
```

---

### Component 3: Terminal Cash Flow (at t = n)

```
Terminal Cash Flow =
  Salvage Value of new asset
± Tax on gain/loss on disposal
+ Recovery of Net Working Capital
```

---

## 4.5 Process of Capital Budgeting

```
CAPITAL BUDGETING PROCESS
│
├── Step 1: IDENTIFICATION of investment opportunities
│           (Strategic planning, R&D, market research)
│
├── Step 2: DEVELOPMENT of project proposals
│           (Feasibility studies, project reports)
│
├── Step 3: EVALUATION of proposals
│           (Apply Payback, ARR, NPV, IRR, PI techniques)
│
├── Step 4: SELECTION of projects
│           (Based on evaluation results + strategic fit)
│           (Subject to capital rationing if applicable)
│
├── Step 5: IMPLEMENTATION
│           (Procurement, construction, commissioning)
│
└── Step 6: POST-COMPLETION AUDIT / REVIEW
            (Compare actual vs projected cash flows)
            (Learn from variances for future decisions)
```

---

## 4.6 Evaluation Techniques

### Overview of All Techniques:

| Technique | Type | Uses TVM? | Uses Cash Flows? | Decision Rule |
|---|---|---|---|---|
| **Payback Period** | Non-discounting | ❌ | ✅ | PBP < Target |
| **Discounted Payback** | Discounting | ✅ | ✅ | DPBP < Target |
| **ARR** | Non-discounting | ❌ | ❌ (uses profit) | ARR > Target |
| **NPV** | Discounting | ✅ | ✅ | NPV > 0 |
| **IRR** | Discounting | ✅ | ✅ | IRR > WACC |
| **MIRR** | Discounting | ✅ | ✅ | MIRR > WACC |
| **PI** | Discounting | ✅ | ✅ | PI > 1 |

---

### Technique 1: Payback Period (PBP)

**Definition**: Time required to **recover the initial investment** from the project's cash inflows.

#### For Even Cash Flows:
```
PBP = Initial Investment / Annual Cash Flow
```

#### For Uneven Cash Flows:
```
PBP = Year before full recovery + (Unrecovered amount / CF in next year)
```

#### Example:
> Investment = ₹5,00,000. Cash Flows: Y1=₹1,50,000; Y2=₹2,00,000; Y3=₹2,50,000; Y4=₹1,00,000.

| Year | CF | Cumulative CF |
|---|---|---|
| 1 | 1,50,000 | 1,50,000 |
| 2 | 2,00,000 | 3,50,000 |
| 3 | 2,50,000 | 6,00,000 |

```
Unrecovered after Y2 = 5,00,000 − 3,50,000 = 1,50,000
PBP = 2 + (1,50,000 / 2,50,000) = 2 + 0.60 = 2.6 years
```

**Merits:**
- Simple to calculate and understand
- Good for liquidity-focused firms
- Useful as risk proxy (shorter = less risk)

**Demerits:**
- Ignores TVM
- Ignores cash flows after payback period
- No consideration of profitability
- Arbitrary cutoff period

---

### Technique 2: Discounted Payback Period (DPBP)

Uses **discounted (PV)** cash flows instead of nominal cash flows.

```
DPBP = Year before full recovery + (Unrecovered PV amount / PV of CF in next year)
```

> Corrects TVM issue of PBP but still ignores cash flows beyond the DPBP. Always > PBP.

---

### Technique 3: Accounting Rate of Return (ARR)

**Definition**: Average annual profit as a percentage of investment.

```
ARR = (Average Annual Net Profit After Tax / Average Investment) × 100

Average Investment = (Initial Investment + Salvage Value) / 2

OR: ARR = (Average Annual Net Profit / Initial Investment) × 100
```

**Decision Rule**: Accept if ARR > Required/Target Rate; For mutually exclusive: choose highest ARR.

**Merits:** Simple; uses readily available accounting data; considers full project life.

**Demerits:** Uses profit not cash flows; ignores TVM; uses average (masks fluctuations).

---

### Technique 4: Net Present Value (NPV) ✅ **(Most Important)**

**Definition**: The difference between the present value of all future cash inflows and the initial investment, discounted at the cost of capital (WACC).

```
NPV = Σ [CFt / (1+k)ᵗ] − Initial Investment

NPV = PV of Inflows − PV of Outflows

Decision Rule:
  NPV > 0 → Accept (project adds value)
  NPV < 0 → Reject (project destroys value)
  NPV = 0 → Indifferent (just earns required return)

For Mutually Exclusive: Choose project with HIGHEST positive NPV
```

#### Full Numerical Example:
> Project A: Initial investment = ₹1,00,000. Cash Flows: Y1=₹40,000; Y2=₹50,000; Y3=₹30,000; Y4=₹20,000. WACC = 10%.

| Year | CF | PVIF(10%,n) | PV |
|---|---|---|---|
| 1 | 40,000 | 0.909 | 36,360 |
| 2 | 50,000 | 0.826 | 41,300 |
| 3 | 30,000 | 0.751 | 22,530 |
| 4 | 20,000 | 0.683 | 13,660 |
| **Total PV** | | | **1,13,850** |

```
NPV = 1,13,850 − 1,00,000 = ₹13,850 (POSITIVE → ACCEPT ✅)
```

**Why NPV is Superior:**
- Considers TVM
- Considers all cash flows over entire life
- Measures absolute wealth creation in ₹ terms
- Additive: NPV(A+B) = NPV(A) + NPV(B)
- Consistent with shareholder wealth maximisation

---

### Technique 5: Internal Rate of Return (IRR)

**Definition**: The discount rate at which the **NPV of a project equals ZERO** — i.e., the rate at which PV of inflows = Initial investment.

```
0 = Σ [CFt / (1+IRR)ᵗ] − Initial Investment

Decision Rule:
  IRR > WACC (Cost of Capital) → Accept
  IRR < WACC                  → Reject
  IRR = WACC                  → Indifferent

For Mutually Exclusive: Choose project with HIGHEST IRR
  (BUT: Subject to NPV vs. IRR conflict — see Section 4.7)
```

#### Calculation — Interpolation Method:
```
IRR = r₁ + [NPV₁ / (NPV₁ − NPV₂)] × (r₂ − r₁)

Where:
  r₁  = Lower discount rate (where NPV is positive)
  r₂  = Higher discount rate (where NPV is negative)
  NPV₁ = NPV at r₁ (positive)
  NPV₂ = NPV at r₂ (negative)
```

#### Example (using Project A above):
> At 10%: NPV = +₹13,850. Try 20%:

| Year | CF | PVIF(20%,n) | PV |
|---|---|---|---|
| 1 | 40,000 | 0.833 | 33,320 |
| 2 | 50,000 | 0.694 | 34,700 |
| 3 | 30,000 | 0.579 | 17,370 |
| 4 | 20,000 | 0.482 | 9,640 |
| **Total PV** | | | **95,030** |

```
NPV at 20% = 95,030 − 1,00,000 = −₹4,970

IRR = 10 + [13,850 / (13,850 + 4,970)] × (20 − 10)
    = 10 + [13,850 / 18,820] × 10
    = 10 + 0.736 × 10
    = 10 + 7.36
    = 17.36%

IRR = 17.36% > WACC 10% → ACCEPT ✅
```

---

### Technique 6: Modified IRR (MIRR)

**Problem with IRR**: Assumes reinvestment of intermediate cash flows at **IRR itself** — unrealistic when IRR is very high.

**MIRR** assumes intermediate cash flows are **reinvested at WACC** — more realistic.

```
MIRR: PV of costs = PV of [Terminal Value of inflows at WACC] at MIRR

Step 1: Find Terminal Value (FV) of all inflows compounded at WACC
Step 2: Find MIRR such that:
        Initial Investment = TV / (1 + MIRR)ⁿ

        MIRR = (TV / Initial Investment)^(1/n) − 1
```

> MIRR is always between WACC and IRR. Better for projects with non-conventional cash flows.

---

## 4.7 NPV vs. IRR — Conflict and Resolution

### When NPV and IRR Give Same Decision:
- **Independent projects**: Both give same Accept/Reject decision (if IRR > WACC ↔ NPV > 0)
- No conflict for **accept/reject** decisions

### When NPV and IRR Conflict (Mutually Exclusive Projects):
Conflict arises in **ranking** when:

```
NPV Ranks: Project A > Project B
IRR Ranks: Project B > Project A
```

**Causes of Conflict:**

| Cause | Explanation |
|---|---|
| **Scale Difference** | One project requires much larger investment |
| **Timing Difference** | Projects have different cash flow timing patterns |
| **Project Life Difference** | Projects have unequal lives |

---

### The Fisher Intersection (Crossover Rate)

At a certain discount rate (**crossover rate**), the NPVs of two projects are equal. Below this rate, one project has higher NPV; above it, the other does.

```
        NPV
         │    Project A
         │   ╱
         │  ╱  
         │ ╱   ╲ Project B
         │╱     ╲
─────────┼────────┼──────► Discount Rate
         0    Crossover  
              Rate (r*)

Below r* → B has higher IRR but A may have higher NPV
Above r* → IRR and NPV agree
```

**Crossover Rate** = IRR of **differential cash flows** (A − B or B − A)

---

### Which Method to Prefer? → **NPV Always Wins** ✅

| Reason | Explanation |
|---|---|
| **Reinvestment Assumption** | NPV assumes reinvestment at WACC (realistic); IRR assumes reinvestment at IRR itself (unrealistic for high IRR projects) |
| **Absolute Value** | NPV measures wealth created in ₹; IRR only gives %. A 50% IRR on ₹1,000 < 20% IRR on ₹1,00,000 |
| **Multiple IRRs** | Non-conventional cash flows can produce multiple IRRs → IRR becomes ambiguous |
| **No IRR** | Some projects (all negative CFs) have no IRR |
| **Additive** | NPV(A+B) = NPV(A) + NPV(B); IRR is not additive |
| **Consistent with Wealth Max** | NPV directly measures value creation for shareholders |

> 📌 **Rule: When NPV and IRR conflict for mutually exclusive projects, ALWAYS choose the project with higher NPV.**

---

### Problem of Multiple IRRs

Occurs with **non-conventional cash flows** (more than one sign change):

```
Example: CF = −1,00,000, +3,00,000, −2,50,000
(Sign changes: −→+ and +→−)

This can produce TWO IRRs → IRR method fails
Solution: Use NPV or MIRR instead
```

---

## 4.8 Profitability Index (PI) Method

### Definition:

**PI** (also called **Benefit-Cost Ratio**) measures the **present value of benefits per rupee of investment**. Used especially in **capital rationing** situations.

```
PI = PV of Future Cash Inflows / Initial Investment

OR: PI = 1 + (NPV / Initial Investment)

Decision Rule:
  PI > 1 → Accept (project creates value)
  PI < 1 → Reject
  PI = 1 → Indifferent

For Mutually Exclusive/Capital Rationing: Rank by PI (highest first)
```

### Example:
> Project A: PV of inflows = ₹1,13,850; Initial Investment = ₹1,00,000.

```
PI = 1,13,850 / 1,00,000 = 1.1385

PI = 1 + (13,850 / 1,00,000) = 1.1385 ✅ Accept
```

---

### When is PI Especially Useful? — Capital Rationing

**Capital Rationing** = Firm has limited capital and cannot fund all positive NPV projects.

**Steps under Capital Rationing:**
1. Calculate PI for each project
2. Rank projects by PI (descending)
3. Select projects in order until budget is exhausted

#### Example:
> Budget = ₹5,00,000. Available projects:

| Project | Investment | NPV | PI | Rank |
|---|---|---|---|---|
| A | 2,00,000 | 60,000 | 1.30 | 1 |
| B | 1,50,000 | 37,500 | 1.25 | 2 |
| C | 2,50,000 | 37,500 | 1.15 | 3 |
| D | 1,00,000 | 10,000 | 1.10 | 4 |

```
Select A (₹2,00,000) + B (₹1,50,000) + D (₹1,00,000) = ₹4,50,000 (within budget)
Total NPV = 60,000 + 37,500 + 10,000 = ₹1,07,500

Note: If we had used NPV ranking: A + C = ₹4,50,000, NPV = 97,500 (LOWER)
PI ranking is BETTER under capital rationing.
```

> ⚠️ **PI may conflict with NPV for mutually exclusive projects** — in that case, always use NPV.

---

### PI vs. NPV Relationship:

```
NPV > 0 ↔ PI > 1
NPV = 0 ↔ PI = 1
NPV < 0 ↔ PI < 1

PI = (NPV + Initial Investment) / Initial Investment
```

---

## 4.9 Summary

### 🔑 Key Takeaways — Chapter 4

| Concept | Key Point |
|---|---|
| **Capital Budgeting** | Long-term investment planning; large, irreversible decisions |
| **Incremental CF** | Only changes in cash flow matter; ignore sunk costs, include opportunity costs |
| **3 CF Components** | Initial outlay (t=0), Operating CFs (t=1 to n), Terminal CF (t=n) |
| **OCF Formula** | EAT + Depreciation = EBIT(1−t) + Depreciation |
| **Depreciation Tax Shield** | Dep × Tax Rate = annual tax saving |
| **Payback Period** | Simple; ignores TVM and post-payback flows |
| **ARR** | Uses profit not cash flows; ignores TVM |
| **NPV** | Best method; measures absolute wealth creation; use WACC as discount rate |
| **IRR** | Rate where NPV=0; accept if IRR > WACC; unrealistic reinvestment assumption |
| **NPV vs. IRR Conflict** | Choose NPV; it directly maximises shareholder wealth |
| **Multiple IRRs** | Non-conventional CFs; use NPV or MIRR instead |
| **MIRR** | Reinvests at WACC; more realistic than IRR |
| **PI** | PV of inflows / Investment; best for capital rationing ranking |
| **Capital Rationing** | Rank by PI to maximise NPV within budget constraint |

---

### ⚡ Master Formula Sheet

```
Initial Investment:
  = Cost of asset + Installation + ΔNWC − Net Salvage of old asset

Operating Cash Flow:
  OCF = EAT + Depreciation
  OCF = EBIT(1−t) + Depreciation
  OCF = (Sales − Costs)(1−t) + Dep × t

Payback Period:
  PBP = Year before recovery + (Unrecovered amount / Next year CF)

ARR:
  ARR = Average Annual Net Profit / Average Investment × 100

NPV:
  NPV = Σ[CFt/(1+k)ᵗ] − I₀

IRR (Interpolation):
  IRR = r₁ + [NPV₁/(NPV₁−NPV₂)] × (r₂−r₁)

MIRR:
  MIRR = (TV / I₀)^(1/n) − 1
  TV = FV of all inflows compounded at WACC

Profitability Index:
  PI = PV of Inflows / Initial Investment
  PI = 1 + (NPV / Initial Investment)

Decision Rules:
  NPV > 0   → Accept
  IRR > WACC → Accept
  PI > 1    → Accept
  PBP < Target → Accept

NPV vs IRR Conflict: ALWAYS choose higher NPV project
Capital Rationing:  ALWAYS rank by PI
```

---

### 📝 Likely Exam Questions — Chapter 4

1. **What is Capital Budgeting? Why is it important? What are its features?**
2. **Classify the types of capital budgeting decisions. Explain each with examples.**
3. **What are incremental cash flows? Why are sunk costs ignored in capital budgeting?**
4. **How is the Initial Investment calculated for a replacement decision?** *(With numerical)*
5. **How is Operating Cash Flow calculated? Distinguish between OCF and Accounting Profit.**
6. **Explain the Payback Period method. What are its merits and limitations?**
7. **What is ARR? How does it differ from NPV? State its limitations.**
8. **Calculate NPV for a project with the following cash flows at WACC = 12%...** *(Full numerical)*
9. **What is IRR? How is it computed using the interpolation method?** *(With numerical)*
10. **Explain the conflict between NPV and IRR for mutually exclusive projects. Which method should be preferred and why?**
11. **What are the problems with IRR? When does a project have multiple IRRs?**
12. **What is MIRR? How does it overcome the limitations of IRR?**
13. **What is the Profitability Index? How is it used in capital rationing?**
14. **A firm has a budget of ₹10,00,000 and 5 projects available. Rank and select using PI.** *(Capital rationing numerical)*
15. **"NPV is the most superior method of capital budgeting." Critically evaluate, comparing it with IRR and Payback Period.**

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
