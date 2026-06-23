# 📘 Corporate Finance — Chapter 3: Cost of Capital
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** Cost of Capital is a formula-heavy chapter. Master the specific cost formulas (Kd, Kp, Ke, Kr), the three methods for Cost of Equity (CAPM, DDM, Bond Yield Plus), and WACC calculation using both Book Value and Market Value weights. Expect a WACC numerical worth 10–15 marks.

---

## 3.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Define Cost of Capital and explain its significance
- ✅ Classify costs of capital across different dimensions
- ✅ Calculate the cost of debt (Kd), preference shares (Kp), equity (Ke), and retained earnings (Kr)
- ✅ Compute Weighted Average Cost of Capital (WACC)
- ✅ Distinguish between Book Value and Market Value weights
- ✅ Understand international dimensions and factors affecting cost of capital globally

---

## 3.2 Introduction

### What is Cost of Capital?

**Cost of Capital** is the **minimum rate of return** that a firm must earn on its investments to satisfy its investors (debt holders, preference shareholders, and equity shareholders) and maintain the market value of its shares.

> 📌 *"Cost of Capital is the rate of return the firm must earn on its investments to keep its market value unchanged."* — Solomon Ezra

### Why is Cost of Capital Important?

| Application | Role of Cost of Capital |
|---|---|
| **Capital Budgeting** | Used as the **hurdle rate / discount rate** to evaluate projects (Accept if IRR > WACC, or NPV > 0) |
| **Capital Structure** | Optimal mix minimises WACC, maximising firm value |
| **Performance Evaluation** | EVA (Economic Value Added) = NOPAT − (Capital × WACC) |
| **Dividend Policy** | Retained earnings have an opportunity cost = Ke |
| **Firm Valuation** | Free cash flows discounted at WACC to get firm value |

### Key Assumptions:
1. Firm's business risk is unchanged (same risk class investments)
2. Firm's financial risk is unchanged (same capital structure)
3. Dividends grow at constant rate (for DDM approach)

---

## 3.3 Various Classifications of Costs of Capital

### Classification 1: Explicit vs. Implicit Cost

| Type | Definition | Example |
|---|---|---|
| **Explicit Cost** | The actual contractual rate paid to suppliers of funds | Interest on debt, dividend on preference shares |
| **Implicit Cost** | Opportunity cost — return foregone on the next best alternative | Cost of retained earnings (what shareholders could earn elsewhere) |

> 📌 **Explicit costs** appear in the income statement; **Implicit costs** do not — but they are real economic costs.

---

### Classification 2: Historical vs. Future Cost

| Type | Definition | Use |
|---|---|---|
| **Historical Cost** | Cost incurred in the past when funds were raised | Reference / comparison only |
| **Future Cost** | Expected cost of raising new funds | **Relevant for decision-making** |

> ⚠️ **Always use Future (Marginal) Costs** for financial decisions — past costs are sunk costs.

---

### Classification 3: Specific vs. Composite (Overall) Cost

| Type | Definition | Formula |
|---|---|---|
| **Specific Cost** | Cost of each individual source of capital separately | Kd, Kp, Ke, Kr |
| **Composite / Overall Cost** | Weighted average of all specific costs | **WACC** |

---

### Classification 4: Average vs. Marginal Cost

| Type | Definition | Use |
|---|---|---|
| **Average Cost** | Weighted average cost of all existing capital | Evaluating existing assets |
| **Marginal Cost** | Cost of raising **one additional rupee** of new capital | **Relevant for new investment decisions** |

> 💡 **Marginal Cost of Capital (MCC)** rises as more funds are raised due to **flotation costs** and **market saturation**.

---

### Summary Classification Table

| Dimension | Types |
|---|---|
| By Nature | Explicit vs. Implicit |
| By Time | Historical vs. Future |
| By Source | Specific (Kd, Kp, Ke, Kr) vs. Composite (WACC) |
| By Volume | Average vs. Marginal |

---

## 3.4 Measurement of Specific Costs of Capital

### A. Cost of Debt (Kd)

**Definition**: The after-tax cost of raising funds through debt (loans, debentures, bonds).

> Interest on debt is **tax-deductible** → Tax Shield → reduces effective cost.

#### Formula — After-tax Cost of Debt:

```
Kd (after-tax) = Kd (before-tax) × (1 − Tax Rate)

Or more precisely:
Kd = [I × (1 − t)] / NP

Where:
  I  = Annual interest payment
  t  = Corporate tax rate
  NP = Net proceeds from debt (issue price − flotation costs)
```

#### For Redeemable Debt (Approximation Formula):

```
Kd = [I(1−t) + (RV − NP)/n] / [(RV + NP)/2]

Where:
  I  = Annual interest
  t  = Tax rate
  RV = Redemption value (face value at maturity)
  NP = Net proceeds
  n  = Years to maturity
```

#### Example:
> 10% Debentures, Face Value ₹1,000, issued at ₹950 (net proceeds), redeemable at ₹1,000 after 5 years. Tax rate = 30%.

```
I(1−t) = 100 × 0.70 = ₹70
(RV − NP)/n = (1,000 − 950)/5 = ₹10
(RV + NP)/2 = (1,000 + 950)/2 = ₹975

Kd = (70 + 10) / 975 = 80/975 = 8.21%
```

#### For Irredeemable (Perpetual) Debt:
```
Kd = I(1−t) / NP
```

---

### B. Cost of Preference Shares (Kp)

**Definition**: The rate of return required by preference shareholders.

> Note: Preference dividends are **NOT tax-deductible** (paid from after-tax profits).

#### For Irredeemable Preference Shares:
```
Kp = D / NP

Where:
  D  = Annual preference dividend
  NP = Net proceeds (issue price − flotation costs)
```

#### For Redeemable Preference Shares (Approximation):
```
Kp = [D + (RV − NP)/n] / [(RV + NP)/2]

Where:
  D  = Annual dividend
  RV = Redemption value
  NP = Net proceeds
  n  = Number of years to redemption
```

#### Example:
> 12% Preference Shares, Face Value ₹100, issued at ₹95 (net), redeemable at ₹100 after 10 years.

```
D = ₹12
(RV − NP)/n = (100 − 95)/10 = ₹0.50
(RV + NP)/2 = (100 + 95)/2 = ₹97.50

Kp = (12 + 0.50) / 97.50 = 12.50/97.50 = 12.82%
```

> ⚠️ **Key Difference** from Kd: No tax adjustment for Kp since dividends are paid from post-tax profits.

---

### C. Cost of Equity (Ke)

**Definition**: The minimum rate of return required by equity shareholders on their investment.

> This is the **most difficult** cost to estimate — equity has no contractual obligation.

Three main approaches:

---

#### Approach 1: Dividend Discount Model (DDM) / Gordon's Model

##### (i) Zero Growth (Constant Dividend):
```
Ke = D / P₀

Where:
  D  = Constant annual dividend
  P₀ = Current market price of equity share
```

##### (ii) Constant Growth (Gordon Growth Model):
```
Ke = D₁ / P₀ + g

Where:
  D₁ = Dividend expected at end of Year 1 = D₀ × (1+g)
  P₀ = Current market price
  g  = Constant dividend growth rate (sustainable growth rate)
  g  = ROE × Retention Ratio (ploughback ratio)
```

##### Example:
> Share price = ₹100, D₀ = ₹5, growth rate = 6%.

```
D₁ = 5 × 1.06 = ₹5.30
Ke = 5.30/100 + 0.06 = 0.053 + 0.06 = 11.3%
```

**Limitations of DDM:**
- Assumes constant growth — unrealistic for many firms
- Cannot be used for non-dividend-paying companies
- Sensitive to growth rate (g) estimate

---

#### Approach 2: Capital Asset Pricing Model (CAPM)

```
Ke = Rf + β × (Rm − Rf)

Where:
  Rf        = Risk-free rate (e.g., G-Sec yield)
  β (Beta)  = Systematic risk of the stock
  Rm        = Expected market return
  (Rm − Rf) = Market Risk Premium (MRP)
```

**Interpretation of Beta:**

| Beta Value | Interpretation |
|---|---|
| β = 0 | Risk-free asset (e.g., T-Bill) |
| β = 1 | Moves exactly with market |
| β > 1 | More volatile than market (aggressive stock) |
| β < 1 | Less volatile than market (defensive stock) |
| β < 0 | Moves opposite to market (rare; e.g., Gold) |

##### Example:
> Rf = 7%, Rm = 13%, β = 1.2

```
Ke = 7% + 1.2 × (13% − 7%)
   = 7% + 1.2 × 6%
   = 7% + 7.2%
   = 14.2%
```

**Advantages of CAPM:**
- Considers systematic (market) risk explicitly
- Widely used in practice
- Works even for non-dividend-paying firms

**Limitations:**
- Beta is historical; may not predict future
- Assumes single-factor model
- Requires estimation of market risk premium

---

#### Approach 3: Bond Yield Plus Risk Premium

A simpler approach: add an equity risk premium to the firm's own debt cost.

```
Ke = Kd (pre-tax) + Equity Risk Premium

Equity Risk Premium typically ranges from 3% to 5%
```

##### Example:
> Company's pre-tax bond yield = 10%, Equity Risk Premium = 4%
```
Ke = 10% + 4% = 14%
```

> 📌 This is a rough-and-ready approach, used when DDM or CAPM data is unavailable.

---

### D. Cost of Retained Earnings (Kr)

**Definition**: The opportunity cost to existing equity shareholders — the return they **forgo** by not receiving dividends (which they could invest elsewhere).

> Retained earnings are **NOT free**. They have an implicit opportunity cost = Ke.

```
Kr = Ke   (in most frameworks)

OR using DDM:
Kr = D₁ / P₀ + g   [same as Ke using Gordon's model]

OR using CAPM:
Kr = Rf + β(Rm − Rf)   [same as CAPM-based Ke]
```

**Why Kr is slightly less than Ke for new equity:**
- New equity involves **flotation costs** (underwriting, legal fees)
- Retained earnings have **no flotation costs**

```
Ke (New Equity) = D₁ / [P₀ × (1 − f)] + g

Where f = flotation cost as a % of issue price
```

---

### Specific Costs Summary Table

| Source | Formula | Tax Effect |
|---|---|---|
| **Debt (Kd)** | [I(1−t) + (RV−NP)/n] / [(RV+NP)/2] | ✅ Tax shield |
| **Preference (Kp)** | [D + (RV−NP)/n] / [(RV+NP)/2] | ❌ No tax shield |
| **Equity (Ke) — DDM** | D₁/P₀ + g | ❌ No deduction |
| **Equity (Ke) — CAPM** | Rf + β(Rm − Rf) | ❌ No deduction |
| **Retained Earnings (Kr)** | Same as Ke (no flotation cost) | ❌ No deduction |

---

## 3.5 Calculation of Weighted Average Cost of Capital (WACC)

### Definition

**WACC** is the overall cost of capital of the firm, calculated as the **weighted average of the costs of all individual sources of capital**, where weights represent the proportion of each source in the total capital structure.

```
WACC = Kd × Wd + Kp × Wp + Ke × We + Kr × Wr

Where:
  W = Weight (proportion) of each source in total capital
  Wd + Wp + We + Wr = 1 (weights sum to 1)
```

Or in expanded form:

```
WACC = [Kd(1−t) × D/V] + [Kp × P/V] + [Ke × E/V]

Where V = D + P + E (Total firm value)
```

---

### Step-by-Step WACC Calculation:

**Step 1**: Identify each source of capital and its amount
**Step 2**: Calculate the specific cost of each source (Kd, Kp, Ke, Kr)
**Step 3**: Calculate weights (either Book Value or Market Value)
**Step 4**: Multiply each cost by its weight
**Step 5**: Sum up all weighted costs → WACC

---

### Comprehensive WACC Example:

> **Capital Structure:**
> - 10% Debentures: ₹40,00,000 (Tax = 30%, Net Proceeds = ₹38,00,000, redeemable at par in 5 years)
> - 12% Preference Shares: ₹20,00,000 (Net Proceeds = ₹19,00,000, redeemable at par in 10 years)
> - Equity Shares: ₹40,00,000 (Market Price = ₹50, D₁ = ₹4, g = 6%)

**Step 1: Cost of Debt**
```
I(1−t) = 10% × 1,000 × 0.70 = ₹70
(RV−NP)/n = (1,000 − 950)/5 = ₹10 [per ₹1,000 debenture]
(RV+NP)/2 = (1,000+950)/2 = ₹975
Kd = (70+10)/975 = 8.21%
```

**Step 2: Cost of Preference**
```
D = 12% × 100 = ₹12
(RV−NP)/n = (100−95)/10 = ₹0.50
(RV+NP)/2 = (100+95)/2 = ₹97.50
Kp = (12+0.50)/97.50 = 12.82%
```

**Step 3: Cost of Equity (DDM)**
```
Ke = D₁/P₀ + g = 4/50 + 0.06 = 0.08 + 0.06 = 14%
```

**Step 4: WACC Calculation**

| Source | Amount (₹) | Weight (W) | Specific Cost | W × Cost |
|---|---|---|---|---|
| Debentures | 40,00,000 | 0.40 | 8.21% | 3.28% |
| Preference | 20,00,000 | 0.20 | 12.82% | 2.56% |
| Equity | 40,00,000 | 0.40 | 14.00% | 5.60% |
| **Total** | **1,00,00,000** | **1.00** | | **WACC = 11.44%** |

---

### Book Value vs. Market Value Weights

| Feature | **Book Value (BV) Weights** | **Market Value (MV) Weights** |
|---|---|---|
| **Basis** | Balance sheet (historical cost) | Current market prices |
| **Stability** | More stable over time | Fluctuates with market |
| **Accuracy** | May not reflect true value | Reflects current investor expectations |
| **Preferred for** | Internal analysis, small firms | Investment decisions, DCF valuation |
| **WACC Result** | May understate cost (if equity MV > BV) | More accurate for valuation |

> ✅ **Market Value weights are theoretically preferred** as they reflect the current opportunity cost of capital. Most textbooks and practitioners use MV weights.

---

### Marginal Cost of Capital (MCC) — Break Point Concept

As a firm raises **more and more new capital**, the cost rises due to:
1. **Flotation costs** on new equity issues
2. **Higher interest rates** demanded as debt load increases
3. Market perceives higher risk → demands higher returns

**Break Point (BP)** = point at which a specific source's cost increases:

```
Break Point = Total amount of lower-cost source available / Weight of that source
```

> After the break point, use the higher marginal cost in WACC.

---

## 3.6 International Dimensions to Cost of Capital

When firms operate **globally** or raise capital in **international markets**, the cost of capital is influenced by additional factors:

### Key International Factors:

| Factor | Impact on Cost of Capital |
|---|---|
| **Country Risk / Political Risk** | Higher risk in unstable countries → Higher required return |
| **Exchange Rate Risk** | Currency depreciation increases effective cost of foreign borrowing |
| **Inflation Differential** | Higher domestic inflation → Higher nominal cost (Fisher Effect) |
| **Capital Market Integration** | Global capital markets: Lower cost due to wider investor pool |
| **Tax Treaties** | Double taxation agreements reduce effective tax burden on Kd |
| **LIBOR / SOFR (Global Benchmark Rates)** | International Kd often tied to these + a spread |
| **Regulatory Differences** | Different disclosure and governance standards affect perceived risk |

---

### Fisher Effect (International):

```
(1 + Nominal Rate) = (1 + Real Rate) × (1 + Inflation Rate)

Nominal Rate ≈ Real Rate + Inflation Rate
```

> In high-inflation countries, nominal interest rates are higher → Higher Kd → Higher WACC.

---

### International CAPM (Extended):

```
Ke (Global) = Rf (global) + β_global × (Global MRP) + Country Risk Premium

Where:
  Rf (global) = US T-Bill rate or global risk-free
  Country Risk Premium = Sovereign spread of the country
```

---

### Cross-listing and ADRs/GDRs:

- Firms listed on **multiple stock exchanges** (e.g., BSE + NYSE via ADR) can access **larger investor pools**
- This **reduces cost of equity** through better price discovery and liquidity
- **ADR** (American Depositary Receipt) — Indian firm's shares traded on US exchanges
- **GDR** (Global Depositary Receipt) — traded on European exchanges

---

### Why Global Cost of Capital May Be LOWER:

```
Benefits of Accessing International Markets:
├── Larger investor base → Better risk diversification
├── Access to cheaper debt (lower international rates)
├── Higher liquidity → Lower risk premium
└── Regulatory credibility → Lower perceived risk
```

---

### Risks That Increase International Cost of Capital:

```
Additional Risk Factors (International):
├── Currency Risk (exchange rate fluctuations)
├── Political Risk (government instability, expropriation)
├── Regulatory Risk (changing laws, capital controls)
└── Information Asymmetry (less familiarity with foreign firms)
```

---

## 3.7 Summary

### 🔑 Key Takeaways — Chapter 3

| Concept | Key Point |
|---|---|
| **Cost of Capital** | Minimum return needed to maintain firm value; used as hurdle rate |
| **Explicit vs Implicit** | Explicit = contractual (interest, dividend); Implicit = opportunity cost |
| **Use Future Costs** | Historical costs are irrelevant; use marginal/future costs for decisions |
| **Kd (after-tax)** | Interest × (1−t); tax shield makes debt cheapest source |
| **Kp** | No tax shield; higher than Kd for same coupon rate |
| **Ke (DDM)** | D₁/P₀ + g; requires dividend-paying firm |
| **Ke (CAPM)** | Rf + β(Rm−Rf); best when β is available |
| **Kr** | ≈ Ke; no flotation cost → Kr slightly < Ke (new equity) |
| **WACC** | Weighted average of all specific costs; minimising WACC maximises firm value |
| **MV Weights** | Preferred over BV weights for decision-making |
| **MCC** | Rises as more capital is raised; break point concept |
| **International** | Country risk, FX risk, inflation affect global cost of capital |

---

### ⚡ Master Formula Sheet

```
Cost of Debt (Redeemable):
  Kd = [I(1−t) + (RV−NP)/n] / [(RV+NP)/2]

Cost of Debt (Irredeemable):
  Kd = I(1−t) / NP

Cost of Preference (Redeemable):
  Kp = [D + (RV−NP)/n] / [(RV+NP)/2]

Cost of Preference (Irredeemable):
  Kp = D / NP

Cost of Equity — DDM (Constant Growth):
  Ke = D₁/P₀ + g    where D₁ = D₀(1+g) and g = ROE × b

Cost of Equity — CAPM:
  Ke = Rf + β(Rm − Rf)

Cost of Equity — New Equity (with flotation):
  Ke = D₁ / [P₀(1−f)] + g

Cost of Retained Earnings:
  Kr = Ke  (no flotation cost)

WACC:
  WACC = Σ (Wi × Ki)
  WACC = Kd(1−t)×Wd + Kp×Wp + Ke×We + Kr×Wr

Fisher Effect:
  Nominal Rate = Real Rate + Inflation Rate (approx.)

International CAPM:
  Ke = Rf(global) + β_global × MRP + Country Risk Premium
```

---

### 📝 Likely Exam Questions — Chapter 3

1. **Define Cost of Capital. Why is it important in financial decision-making?**
2. **Distinguish between: (a) Explicit and Implicit Cost, (b) Specific and Composite Cost, (c) Historical and Future Cost.**
3. **How is the after-tax cost of debt calculated? Why does tax rate affect cost of debt but not cost of preference shares?**
4. **Calculate the cost of redeemable debentures given interest rate, issue price, redemption value, and tax rate.** *(Numerical)*
5. **Explain three methods of calculating Cost of Equity. Which method is most reliable?**
6. **Using CAPM, calculate Ke given: Rf = 6%, β = 1.5, Market Return = 14%.** *(Numerical)*
7. **Using Gordon's Growth Model, find Ke given: P₀ = ₹200, D₀ = ₹10, g = 5%.** *(Numerical)*
8. **Why is the cost of retained earnings not zero? How is it estimated?**
9. **What is WACC? How is it calculated? Explain with a complete numerical example.**
10. **Distinguish between Book Value Weights and Market Value Weights in WACC calculation. Which is preferred and why?**
11. **What is Marginal Cost of Capital (MCC)? Explain the break point concept.**
12. **A company has the following capital structure: Equity ₹50L (Ke=14%), Debt ₹30L (Kd=8%), Preference ₹20L (Kp=12%). Calculate WACC.** *(Numerical)*
13. **How do exchange rate risk and country risk affect a firm's international cost of capital?**
14. **Explain how cross-listing (ADR/GDR) can reduce a firm's cost of equity.**
15. **"The cost of debt is lower than the cost of equity." Explain with reasons.** *(Theory)*

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
