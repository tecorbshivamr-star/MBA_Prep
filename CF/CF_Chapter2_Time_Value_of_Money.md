# 📘 Corporate Finance — Chapter 2: Time Value of Money
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** TVM is highly numerical. Master the core formulas (FV, PV, Annuity, Perpetuity), the Rule of 72, Effective vs Nominal Rate, and be able to solve problems step-by-step. Expect at least 1–2 numerical questions worth 10–15 marks.

---

## 2.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Explain the concept of Time Value of Money and why it matters
- ✅ Draw and interpret time lines for cash flows
- ✅ Calculate Future Value and Present Value of a single cash flow
- ✅ Distinguish between Simple and Compound Interest
- ✅ Apply the Rule of 72 (Doubling Period)
- ✅ Convert between Nominal and Effective interest rates
- ✅ Calculate PV of uneven cash flow series
- ✅ Compute FV and PV of Ordinary Annuity and Annuity Due
- ✅ Calculate PV of a Growing Annuity and a Perpetuity

---

## 2.2 Introduction

### Why Does Money Have Time Value?

**A rupee today is worth MORE than a rupee tomorrow.** This is the fundamental principle of finance.

Three reasons:

| Reason | Explanation |
|---|---|
| **Preference for Present Consumption** | People prefer to consume now rather than wait |
| **Investment Opportunities** | Money today can be invested to earn returns |
| **Inflation** | Rising prices erode future purchasing power |
| **Uncertainty** | Future cash flows are uncertain; present cash is certain |

> 📌 *TVM is the foundation of Capital Budgeting, Valuation, and all financial decision-making.*

---

## 2.3 Time Lines and Notation

A **Time Line** is a visual tool to represent cash flows at different points in time.

```
Period:   0         1         2         3         n
          │─────────│─────────│─────────│─── ... ─│
Cash Flow: CF₀      CF₁       CF₂       CF₃       CFₙ
```

- **Period 0** = Today (Present)
- **Positive values** = Cash inflows (receipts)
- **Negative values** = Cash outflows (payments)

### Standard Notation:

| Symbol | Meaning |
|---|---|
| **PV** | Present Value (value today) |
| **FV** | Future Value (value at end of period n) |
| **k or r** | Interest rate / Discount rate per period |
| **n** | Number of periods |
| **PMT or A** | Annuity payment (equal periodic cash flow) |
| **FVIF(k,n)** | Future Value Interest Factor = (1+k)ⁿ |
| **PVIF(k,n)** | Present Value Interest Factor = 1/(1+k)ⁿ |
| **FVIFA(k,n)** | FV Interest Factor of Annuity |
| **PVIFA(k,n)** | PV Interest Factor of Annuity |

---

## 2.4 Future Value of a Single Cash Flow

**Concept**: If you invest PV today at rate k for n periods, how much will you have at the end?

### Compound Interest Formula:

```
FV = PV × (1 + k)ⁿ

FV = PV × FVIF(k, n)

Where: FVIF(k, n) = (1 + k)ⁿ
```

> **Compounding** = earning interest on interest (interest is reinvested each period).

### Example:
> Invest ₹10,000 at 10% p.a. for 3 years.

```
FV = 10,000 × (1.10)³
   = 10,000 × 1.331
   = ₹13,310
```

**Year-by-year breakdown:**

| Year | Opening Balance | Interest (10%) | Closing Balance |
|---|---|---|---|
| 1 | ₹10,000 | ₹1,000 | ₹11,000 |
| 2 | ₹11,000 | ₹1,100 | ₹12,100 |
| 3 | ₹12,100 | ₹1,210 | ₹13,310 |

---

## 2.5 Simple Interest

**Simple Interest** = Interest calculated only on the **original principal** (no compounding).

```
Simple Interest (SI) = P × r × n

FV (Simple Interest) = P + SI = P × (1 + r × n)
```

### Simple vs. Compound Interest Comparison:

| Feature | Simple Interest | Compound Interest |
|---|---|---|
| **Base for Interest** | Original Principal only | Principal + Accumulated Interest |
| **Growth** | Linear | Exponential |
| **Formula** | FV = P(1 + rn) | FV = P(1 + r)ⁿ |
| **Use** | Short-term loans, trade credit | Long-term investments, loans |

### Example:
> ₹10,000 at 10% for 3 years:
- **Simple Interest**: FV = 10,000 × (1 + 0.10 × 3) = ₹13,000
- **Compound Interest**: FV = 10,000 × (1.10)³ = ₹13,310

> 💡 **Compound interest always gives a HIGHER FV** than simple interest (for n > 1).

---

## 2.6 Doubling Period (Rule of 72)

**Question**: How many years does it take to **double** your money at a given interest rate?

### Rule of 72 (Approximate):

```
Doubling Period (n) ≈ 72 / r

Where r = interest rate in percentage
```

### Rule of 69 (More Accurate for Continuous Compounding):

```
Doubling Period ≈ 69 / r  (or more precisely: ln(2)/r = 0.693/r)
```

### Examples:

| Interest Rate | Rule of 72 | Actual Years |
|---|---|---|
| 6% | 72/6 = 12 years | 11.9 years |
| 9% | 72/9 = 8 years | 8.04 years |
| 12% | 72/12 = 6 years | 6.12 years |
| 18% | 72/18 = 4 years | 4.19 years |
| 24% | 72/24 = 3 years | 3.22 years |

> 📌 **Exam tip**: Use Rule of 72 for quick approximations. For exact answers, use: n = ln(2) / ln(1+k)

### Exact Formula for Doubling Period:
```
2 = (1 + k)ⁿ
n = ln(2) / ln(1 + k)
```

---

## 2.7 Effective versus Nominal Rate

### Nominal Rate (Annual Percentage Rate — APR)
The **stated** interest rate before adjusting for compounding frequency.

### Effective Annual Rate (EAR / EFF%)
The **actual** rate earned/paid per year, accounting for within-year compounding.

### Formula:

```
EAR = (1 + k_nom / m)^m − 1

Where:
  k_nom = Nominal annual rate
  m     = Number of compounding periods per year
```

### Compounding Frequency Table:

| Compounding | m | EAR at 12% Nominal |
|---|---|---|
| Annual | 1 | 12.00% |
| Semi-annual | 2 | 12.36% |
| Quarterly | 4 | 12.55% |
| Monthly | 12 | 12.68% |
| Daily | 365 | 12.75% |
| Continuous | ∞ | e^0.12 − 1 = 12.75% |

### Continuous Compounding:
```
EAR = e^(k_nom) − 1
FV  = PV × e^(k × n)
```

### Example:
> Bank A offers 12% compounded monthly. Bank B offers 12.5% compounded annually. Which is better?

```
EAR (Bank A) = (1 + 0.12/12)^12 − 1 = (1.01)^12 − 1 = 12.68%
EAR (Bank B) = 12.50%

∴ Bank A is better (12.68% > 12.50%)
```

> ⚠️ **Always compare using EAR**, not nominal rates, when compounding frequencies differ.

### Converting Nominal to Effective (Key Exam Formula):
```
EAR = (1 + k_nom/m)^m − 1

Reverse: k_nom = m × [(1 + EAR)^(1/m) − 1]
```

---

## 2.8 Present Value of a Single Cash Flow

**Concept**: What is a future cash flow worth **today**? (Reverse of FV)

**Discounting** = bringing future value back to present.

### Formula:

```
PV = FV / (1 + k)ⁿ

PV = FV × PVIF(k, n)

Where: PVIF(k, n) = 1 / (1 + k)ⁿ
```

### Example:
> You will receive ₹13,310 after 3 years. Discount rate = 10%. What is its PV?

```
PV = 13,310 / (1.10)³
   = 13,310 / 1.331
   = ₹10,000
```

### Key Relationships:

| Variable Increases | Effect on PV |
|---|---|
| Discount rate (k) ↑ | PV ↓ (inverse relationship) |
| Time period (n) ↑ | PV ↓ (farther away = worth less today) |
| Future cash flow ↑ | PV ↑ (direct relationship) |

---

## 2.9 Present Value of an Uneven Series

When cash flows **differ each period**, discount each cash flow separately and sum them up.

### Formula:

```
PV = CF₁/(1+k)¹ + CF₂/(1+k)² + CF₃/(1+k)³ + ... + CFₙ/(1+k)ⁿ

PV = Σ [CFₜ / (1+k)ᵗ]  for t = 1 to n
```

### Example:
> Discount rate = 10%. Cash flows: Year 1: ₹1,000 | Year 2: ₹2,000 | Year 3: ₹3,000

| Year | Cash Flow | PVIF (10%, n) | PV |
|---|---|---|---|
| 1 | ₹1,000 | 1/1.10 = 0.909 | ₹909 |
| 2 | ₹2,000 | 1/1.21 = 0.826 | ₹1,652 |
| 3 | ₹3,000 | 1/1.331 = 0.751 | ₹2,253 |
| **Total PV** | | | **₹4,814** |

---

## 2.10 Relationship Between FVIF(k,n) and PVIF(k,n)

These two factors are **reciprocals** of each other:

```
FVIF(k, n) = (1 + k)ⁿ

PVIF(k, n) = 1 / (1 + k)ⁿ = 1 / FVIF(k, n)

∴  FVIF(k, n) × PVIF(k, n) = 1
```

| FVIF(k,n) | PVIF(k,n) |
|---|---|
| Future Value Interest Factor | Present Value Interest Factor |
| Used to find FV given PV | Used to find PV given FV |
| Always > 1 (for k > 0) | Always < 1 (for k > 0) |
| Increases with k and n | Decreases with k and n |

> 📌 **Practical Use**: If FVIF(10%, 5) = 1.6105, then PVIF(10%, 5) = 1/1.6105 = 0.6209

---

## 2.11 Shorter Discounting / Compounding Period

When compounding occurs **more frequently than annually**, adjust k and n:

```
Adjusted Rate per Period  = k / m
Adjusted Number of Periods = n × m

FV = PV × (1 + k/m)^(n×m)
PV = FV / (1 + k/m)^(n×m)

Where m = compounding frequency per year
```

### Example:
> ₹5,000 invested at 12% p.a. compounded quarterly for 2 years.

```
k/m = 12%/4 = 3% per quarter
n×m = 2 × 4 = 8 quarters

FV = 5,000 × (1.03)^8
   = 5,000 × 1.2668
   = ₹6,334
```

### Comparison of FV at Different Compounding Frequencies (₹1,000 at 12% for 1 year):

| Compounding | FV |
|---|---|
| Annual | ₹1,120.00 |
| Semi-annual | ₹1,123.60 |
| Quarterly | ₹1,125.51 |
| Monthly | ₹1,126.83 |
| Daily | ₹1,127.47 |

> 💡 **More frequent compounding = Higher FV** (and lower PV for discounting).

---

## 2.12 Annuity

An **Annuity** is a series of **equal cash flows** at **regular intervals** for a **fixed period**.

### Types of Annuity:

| Type | Cash Flow Timing | Example |
|---|---|---|
| **Ordinary Annuity** (Annuity-in-Arrears) | End of each period | Loan EMIs, bond coupons |
| **Annuity Due** (Annuity-in-Advance) | Beginning of each period | Insurance premiums, lease payments |

---

### A. Future Value of Ordinary Annuity

```
FVA = A × FVIFA(k, n)

FVIFA(k, n) = [(1 + k)ⁿ − 1] / k
```

### Example:
> Deposit ₹1,000 at end of each year for 3 years at 10% p.a.

```
FVIFA(10%, 3) = [(1.10)³ − 1] / 0.10
              = [1.331 − 1] / 0.10
              = 0.331 / 0.10 = 3.31

FVA = 1,000 × 3.31 = ₹3,310
```

---

### B. Present Value of Ordinary Annuity

```
PVA = A × PVIFA(k, n)

PVIFA(k, n) = [1 − 1/(1+k)ⁿ] / k  =  [1 − PVIF(k,n)] / k
```

### Example:
> Receive ₹1,000 at end of each year for 3 years. Discount rate = 10%.

```
PVIFA(10%, 3) = [1 − 1/(1.10)³] / 0.10
              = [1 − 0.7513] / 0.10
              = 0.2487 / 0.10 = 2.487

PVA = 1,000 × 2.487 = ₹2,487
```

---

### C. Annuity Due — Adjustment

Since each payment occurs **one period earlier**, multiply the ordinary annuity result by **(1 + k)**:

```
FVA (Due) = FVA (Ordinary) × (1 + k)
PVA (Due) = PVA (Ordinary) × (1 + k)
```

> 📌 **Annuity Due is ALWAYS larger than Ordinary Annuity** — because each cash flow earns/discounts one extra period.

### Example:
> Same as above but payments at beginning of year:
```
PVA (Due) = 2,487 × 1.10 = ₹2,736
FVA (Due) = 3,310 × 1.10 = ₹3,641
```

---

### D. Finding Annuity Payment (A) — Loan Amortisation

Given PV (loan amount), find the EMI:

```
A = PV / PVIFA(k, n)   [Ordinary Annuity]
```

### Example:
> Home loan of ₹10,00,000 at 9% p.a. for 20 years. Find annual payment.

```
PVIFA(9%, 20) = [1 − (1.09)^-20] / 0.09 = 9.1285

A = 10,00,000 / 9.1285 = ₹1,09,546 per year
```

---

## 2.13 Relationship Between FVIFA(k,n) and PVIFA(k,n)

These are related but **NOT simple reciprocals** (unlike FVIF and PVIF):

```
FVIFA(k, n) = PVIFA(k, n) × FVIF(k, n)

Or:  PVIFA(k, n) = FVIFA(k, n) / FVIF(k, n) = FVIFA(k, n) × PVIF(k, n)
```

**Intuition**: The FV of an annuity equals the PV of the annuity compounded forward for n periods.

```
FVA = PVA × (1 + k)ⁿ
```

| Factor | Formula | Use |
|---|---|---|
| FVIFA(k,n) | [(1+k)ⁿ − 1] / k | Find FV of annuity given A |
| PVIFA(k,n) | [1 − (1+k)^−ⁿ] / k | Find PV of annuity given A |
| Relationship | FVIFA = PVIFA × (1+k)ⁿ | Convert between them |

---

## 2.14 Present Value of a Growing Annuity

A **Growing Annuity** is a finite series of cash flows that **grow at a constant rate (g)** each period.

### Formula:

```
PV of Growing Annuity = A × [1 − ((1+g)/(1+k))ⁿ] / (k − g)

Where:
  A = First period cash flow
  g = Constant growth rate per period
  k = Discount rate
  n = Number of periods
  Condition: k ≠ g
```

### Example:
> First year salary = ₹5,00,000, growing at 5% p.a. for 10 years. Discount rate = 12%.

```
PV = 5,00,000 × [1 − (1.05/1.12)^10] / (0.12 − 0.05)
   = 5,00,000 × [1 − (0.9375)^10] / 0.07
   = 5,00,000 × [1 − 0.5168] / 0.07
   = 5,00,000 × 6.9029
   = ₹34,51,450
```

> 📌 **Special Case**: If g = 0, the growing annuity formula reduces to the ordinary annuity formula (PVIFA).

---

## 2.15 Present Value of a Perpetuity

A **Perpetuity** is an annuity that continues **forever** (infinite cash flows).

### Types:

#### A. Level (Constant) Perpetuity:
Cash flow is the same every period, forever.

```
PV of Perpetuity = A / k

Where:
  A = Constant annual cash flow
  k = Discount rate
```

### Example:
> Preference share pays ₹100 dividend forever. Required return = 8%.

```
PV = 100 / 0.08 = ₹1,250
```

---

#### B. Growing Perpetuity (Gordon Growth Model):
Cash flow grows at constant rate g forever.

```
PV of Growing Perpetuity = A / (k − g)

Condition: k > g  (otherwise PV → ∞)
```

### Example:
> Dividend next year = ₹5, growing at 3% forever. Required return = 10%.

```
PV = 5 / (0.10 − 0.03) = 5 / 0.07 = ₹71.43
```

> 📌 **This is the foundation of the Dividend Discount Model (DDM)** used for stock valuation.

---

### Summary of All PV Formulas:

| Cash Flow Type | Formula |
|---|---|
| **Single CF** | PV = FV × [1/(1+k)ⁿ] |
| **Ordinary Annuity** | PV = A × [1 − (1+k)^−ⁿ] / k |
| **Annuity Due** | PV = A × [1 − (1+k)^−ⁿ] / k × (1+k) |
| **Growing Annuity** | PV = A × [1 − ((1+g)/(1+k))ⁿ] / (k−g) |
| **Level Perpetuity** | PV = A / k |
| **Growing Perpetuity** | PV = A / (k−g) |

---

## 2.16 Important Steps to Solve TVM Problems

Follow this systematic approach for any TVM problem:

```
STEP 1: Draw a Time Line
         → Identify periods, cash flows, direction (in/out)

STEP 2: Identify the Given Variables
         → What is known? (PV, FV, k, n, A, g)
         → What is to be found?

STEP 3: Check Compounding Frequency
         → If m > 1: Adjust k → k/m and n → n×m

STEP 4: Identify the Cash Flow Pattern
         → Single CF? Annuity? Uneven series? Perpetuity?

STEP 5: Select the Correct Formula
         → Apply appropriate formula or factor table

STEP 6: Calculate
         → Show all steps clearly in exam

STEP 7: Sanity Check
         → FV > PV? (for positive k) ✔
         → PV of Perpetuity reasonable? ✔
```

### Common Mistakes to Avoid:

| Mistake | Correct Approach |
|---|---|
| Using nominal rate when compounding > 1x/year | Adjust: k/m and n×m |
| Using ordinary annuity formula for annuity due | Multiply by (1+k) |
| Confusing EAR and nominal rate | Compare using EAR only |
| Not drawing time line first | Always draw time line — prevents errors |
| Double-counting PV of annuity | PVIFA already accounts for all periods |

---

## 2.17 Summary

### 🔑 Key Takeaways — Chapter 2

| Concept | Key Point |
|---|---|
| **TVM Principle** | ₹1 today > ₹1 tomorrow (preference, investment opportunity, inflation) |
| **Compounding** | FV = PV × (1+k)ⁿ — interest earned on interest |
| **Simple Interest** | FV = P(1+rn) — linear growth, no reinvestment |
| **Rule of 72** | Doubling period ≈ 72 / r% |
| **EAR vs Nominal** | EAR = (1 + k_nom/m)^m − 1; always compare via EAR |
| **Discounting** | PV = FV / (1+k)ⁿ — reverse of compounding |
| **Uneven Series** | Discount each CF separately; sum them |
| **FVIF × PVIF = 1** | They are reciprocals |
| **Ordinary Annuity** | Payments at END of period |
| **Annuity Due** | Payments at BEGINNING; multiply by (1+k) |
| **Growing Annuity** | PV = A / (k−g) × [1 − ((1+g)/(1+k))ⁿ] |
| **Level Perpetuity** | PV = A / k |
| **Growing Perpetuity** | PV = A / (k−g) — basis of DDM/stock valuation |

---

### ⚡ Master Formula Sheet

```
Single Cash Flow:
  FV = PV × (1+k)ⁿ           [Compounding]
  PV = FV / (1+k)ⁿ           [Discounting]

FVIF(k,n) = (1+k)ⁿ
PVIF(k,n) = 1/(1+k)ⁿ = 1/FVIF(k,n)

Simple Interest:
  FV = P(1 + r × n)

Rule of 72:
  Doubling Period ≈ 72 / r%

Effective Rate:
  EAR = (1 + k_nom/m)^m − 1
  Continuous: EAR = e^k − 1

Intra-year Compounding:
  FV = PV × (1 + k/m)^(n×m)

Ordinary Annuity:
  FVIFA(k,n) = [(1+k)ⁿ − 1] / k
  PVIFA(k,n) = [1 − (1+k)^−ⁿ] / k
  FVA = A × FVIFA(k,n)
  PVA = A × PVIFA(k,n)

Annuity Due:
  FVA(Due) = FVA × (1+k)
  PVA(Due) = PVA × (1+k)

Annuity Factor Relationship:
  FVIFA = PVIFA × (1+k)ⁿ

Growing Annuity:
  PV = A × [1 − ((1+g)/(1+k))ⁿ] / (k−g)

Level Perpetuity:
  PV = A / k

Growing Perpetuity:
  PV = A / (k−g)   [Gordon Growth Model]

Loan Payment:
  A (EMI) = PV / PVIFA(k,n)
```

---

### 📝 Likely Exam Questions — Chapter 2

1. **What is Time Value of Money? Why does money have time value?**
2. **Distinguish between Simple Interest and Compound Interest with examples.**
3. **What is the Rule of 72? Calculate the doubling period for 8%, 12%, and 15% interest rates.**
4. **Distinguish between Nominal Rate and Effective Annual Rate. Which should be used for comparison and why?**
5. **A sum of ₹20,000 is invested at 10% p.a. compounded quarterly for 3 years. Find FV.** *(Numerical)*
6. **What will be the PV of ₹50,000 receivable after 5 years if discount rate is 12% p.a.?** *(Numerical)*
7. **Calculate the PV of an uneven cash flow stream: Year 1: ₹2,000; Year 2: ₹3,000; Year 3: ₹4,000; at 10% discount rate.** *(Numerical)*
8. **Explain the relationship between FVIF and PVIF. How are they related?**
9. **Distinguish between Ordinary Annuity and Annuity Due. How does the formula differ?**
10. **Calculate the FV and PV of an annuity of ₹5,000 per year for 5 years at 10% p.a.** *(Numerical)*
11. **What is a Perpetuity? How is PV of a perpetuity calculated? Give an example.**
12. **Explain the concept of Growing Perpetuity and its connection to stock valuation (DDM).**
13. **A bank offers 12% nominal rate compounded monthly vs 12.5% compounded annually. Which is better?** *(Numerical)*
14. **What is a Growing Annuity? Write its formula and solve: First income = ₹3,00,000 growing at 6% for 15 years; discount rate = 12%.** *(Numerical)*
15. **Explain the steps to solve TVM problems systematically.** *(Theory + Application)*

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
