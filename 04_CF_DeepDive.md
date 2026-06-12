# 📘 DEEP DIVE: Corporate Finance
### MBA 2nd Semester | DU SOL | Subject 12
**Prepared in IIM Format | Finance for Strategic Decision Making**

---

> **How to Use:** Corporate Finance is heavily formula-based. Understand the **logic** behind each formula first, then memorize it. Every concept connects — TVM feeds into NPV, which feeds into Capital Budgeting, which drives Capital Structure decisions.

---

## 📌 CHAPTER 1: Financial Management — An Overview

### 1.1 Definition

**Financial Management** is the planning, organizing, directing, and controlling of financial activities — specifically the procurement and utilization of funds — to achieve organizational objectives.

**Three Core Decisions in Financial Management:**

| Decision | Question Asked | Tool Used |
|----------|---------------|-----------|
| **Investment Decision** | Where to invest funds? | Capital Budgeting (NPV, IRR) |
| **Financing Decision** | How to raise funds? | Capital Structure (Debt vs Equity) |
| **Dividend Decision** | How much to return to shareholders? | Dividend Policy |

---

### 1.2 Goal of Financial Management

**Traditional Goal:** Profit Maximization
- Simple but flawed: ignores timing, risk, and shareholder value

**Modern Goal: Shareholder Wealth Maximization (SWM)**
```
Shareholder Wealth = Share Price × Number of Shares Outstanding
```
- Considers time value of money
- Considers risk
- Long-term perspective
- Aligns management with shareholder interests

**Agency Problem:**
- Separation of ownership (shareholders) and control (managers)
- Managers may pursue their own interests (perks, empire building) at shareholders' expense
- **Solution:** Stock options, monitoring, corporate governance (SEBI regulations in India)

---

### 1.3 Functions of Financial Manager

1. **Financial Planning:** Forecasting cash flows, budgeting
2. **Capital Budgeting:** Evaluating long-term investments
3. **Capital Structure:** Deciding optimal debt-equity mix
4. **Working Capital Management:** Managing day-to-day liquidity
5. **Dividend Policy:** Deciding retention vs distribution

---

### 1.4 Financial Markets in India

| Market | Instruments | Regulator |
|--------|-------------|-----------|
| Money Market | T-Bills, Commercial Paper, CDs | RBI |
| Capital Market — Equity | Shares, BSE, NSE | SEBI |
| Capital Market — Debt | Bonds, Debentures | SEBI |
| Derivatives Market | Futures, Options | SEBI |
| Forex Market | Currency trading | RBI |

---

## 📌 CHAPTER 2: Time Value of Money (TVM)

### 2.1 The Core Concept

**"A rupee today is worth more than a rupee tomorrow."**

**Reasons:**
1. **Opportunity Cost:** Money today can be invested to earn returns
2. **Inflation:** Future money has lower purchasing power
3. **Risk:** Future receipts are uncertain

---

### 2.2 Key TVM Concepts and Formulas

**Future Value (FV) — Compounding:**
```
FV = PV × (1 + r)ⁿ
```
*"How much will ₹1,000 grow to in 5 years at 10%?"*

**Present Value (PV) — Discounting:**
```
PV = FV / (1 + r)ⁿ = FV × [1/(1+r)ⁿ]
```
*"What is ₹1,000 received 5 years later worth today?"*

**The Discount Factor:** `DF = 1/(1+r)ⁿ`

---

### 2.3 Annuity and Perpetuity

**Annuity:** Equal cash flows for a fixed number of periods

**Present Value of Annuity (PVA):**
```
PVA = CF × [1 - (1+r)⁻ⁿ] / r
```

**Future Value of Annuity (FVA):**
```
FVA = CF × [(1+r)ⁿ - 1] / r
```

**Perpetuity:** Equal cash flows FOREVER
```
PV of Perpetuity = CF / r
```

**Growing Perpetuity (Gordon Growth Model):**
```
PV = CF / (r - g)    where g = constant growth rate, r > g
```

---

### 2.4 Worked Examples

**Example 1 — FV:**
Invest ₹10,000 at 12% p.a. for 3 years (compounded annually):
```
FV = 10,000 × (1.12)³ = 10,000 × 1.4049 = ₹14,049
```

**Example 2 — PV:**
You will receive ₹50,000 in 4 years. Discount rate = 10%:
```
PV = 50,000 / (1.10)⁴ = 50,000 / 1.4641 = ₹34,151
```

**Example 3 — Loan EMI (Annuity):**
Home loan of ₹30 lakh at 9% p.a. for 20 years. Monthly rate = 9/12 = 0.75%:
```
EMI = P × r(1+r)ⁿ / [(1+r)ⁿ - 1]
    = 30,00,000 × 0.0075 × (1.0075)²⁴⁰ / [(1.0075)²⁴⁰ - 1]
    = ₹26,992/month
```

---

### 2.5 Real-Life Application — India

**SIP (Systematic Investment Plan) — Mutual Funds:**
Invest ₹5,000/month in mutual fund at 12% p.a. for 20 years:
```
FV = 5,000 × [(1.01)²⁴⁰ - 1] / 0.01 = ₹49.96 lakh
```
Total invested = ₹12 lakh; Total returns = ₹49.96 lakh → Power of compounding!

---

## 📌 CHAPTER 3: Cost of Capital

### 3.1 What is Cost of Capital?

**Definition:**
Cost of Capital is the minimum rate of return that a company must earn on its investments to satisfy its investors (both debt and equity holders). It is the **hurdle rate** for capital budgeting decisions.

**If Project Return > Cost of Capital → Accept (creates value)**
**If Project Return < Cost of Capital → Reject (destroys value)**

---

### 3.2 Component Costs

**Cost of Debt (Kd):**
```
Kd (pre-tax) = Annual Interest / Net Proceeds
Kd (after-tax) = Kd(pre-tax) × (1 - Tax Rate)
```
*Interest is tax-deductible → after-tax cost of debt is lower.*

**Example:** Bond with 10% coupon, ₹1,000 face value, tax rate 30%:
```
Kd(after-tax) = 10% × (1 - 0.30) = 7%
```

**Cost of Preference Share (Kp):**
```
Kp = Dividend / Net Issue Price
```
*No tax benefit (dividends not tax-deductible)*

**Cost of Equity (Ke) — Three Methods:**

**Method 1: Dividend Growth Model (Gordon Model):**
```
Ke = (D₁ / P₀) + g
```
Where: D₁ = Expected dividend next year, P₀ = Current stock price, g = growth rate

**Method 2: CAPM (Capital Asset Pricing Model):**
```
Ke = Rf + β(Rm - Rf)
```
Where: Rf = Risk-free rate, β = Beta (systematic risk), Rm = Market return, (Rm-Rf) = Market risk premium

**Method 3: Earnings Yield Method:**
```
Ke = EPS / Market Price per Share
```

---

### 3.3 WACC — Weighted Average Cost of Capital

**Definition:**
WACC is the average cost of all capital components, weighted by their proportion in the firm's capital structure.

```
WACC = Wd × Kd(1-T) + Wp × Kp + We × Ke
```
Where: Wd, Wp, We = weights of debt, preference, equity
(Weights should be based on **market values**, not book values)

**Worked Example:**
| Source | Amount (₹ Cr) | Cost | Weight |
|--------|--------------|------|--------|
| Debt | 400 | 7% (after-tax) | 0.40 |
| Equity | 600 | 14% | 0.60 |
| **Total** | **1000** | | **1.00** |

```
WACC = 0.40 × 7% + 0.60 × 14% = 2.8% + 8.4% = 11.2%
```
This company must earn at least **11.2%** on any new investment.

---

### 3.4 CAPM — Capital Asset Pricing Model

**Beta (β):**
- β = 1: Stock moves exactly with market
- β > 1: More volatile than market (aggressive stock)
- β < 1: Less volatile than market (defensive stock)
- β = 0: No market risk (T-bills)

**India CAPM Example (Reliance Industries):**
- Rf = 7% (10-yr Govt Bond yield)
- β(Reliance) = 0.95
- Rm = 13% (Nifty 50 long-run return)
- Market Risk Premium = 13% - 7% = 6%

```
Ke = 7% + 0.95 × 6% = 7% + 5.7% = 12.7%
```

---

## 📌 CHAPTER 4: Investment Decisions (Capital Budgeting)

### 4.1 What is Capital Budgeting?

**Definition:**
Capital Budgeting is the process of planning and managing a firm's long-term investments — decisions about whether to invest in projects, machinery, products, or acquisitions.

**Types of Capital Budgeting Decisions:**
- Replacement decisions (upgrade old machinery)
- Expansion decisions (new plant)
- New product decisions (launch new product line)
- Mandatory decisions (environmental compliance)

---

### 4.2 Capital Budgeting Techniques

#### A. Payback Period (PBP)

**Definition:** Time required to recover the initial investment from cash inflows.

```
PBP = Initial Investment / Annual Cash Inflow (for equal cash flows)
```

**For unequal cash flows:** Cumulate until investment recovered.

**Decision Rule:** Accept if PBP < Target period; Reject otherwise.

**Limitations:** Ignores time value of money; Ignores cash flows after payback.

---

#### B. Net Present Value (NPV) — MOST IMPORTANT

**Definition:**
NPV is the difference between the present value of all cash inflows and the present value of all cash outflows (initial investment).

```
NPV = Σ [CFt / (1+WACC)ᵗ] - Initial Investment
    = PV of inflows - PV of outflows
```

**Decision Rule:**
- **NPV > 0 → Accept** (project creates value)
- **NPV < 0 → Reject** (project destroys value)
- **NPV = 0 → Indifferent** (earns exactly the cost of capital)

**Worked Example:**
Project cost = ₹1,00,000. Cash flows: Year 1 = ₹40,000; Year 2 = ₹50,000; Year 3 = ₹30,000. WACC = 10%.

| Year | CF | PV Factor @10% | PV of CF |
|------|-----|----------------|---------|
| 1 | 40,000 | 0.909 | 36,360 |
| 2 | 50,000 | 0.826 | 41,300 |
| 3 | 30,000 | 0.751 | 22,530 |
| **Total PV** | | | **1,00,190** |

```
NPV = 1,00,190 - 1,00,000 = ₹190 → Positive → ACCEPT
```

---

#### C. Internal Rate of Return (IRR)

**Definition:**
IRR is the discount rate at which NPV = 0. It is the project's own rate of return.

```
0 = Σ [CFt / (1+IRR)ᵗ] - Initial Investment
```

**Decision Rule:**
- **IRR > WACC → Accept**
- **IRR < WACC → Reject**
- **IRR = WACC → Indifferent**

**IRR Calculation (Interpolation):**
```
IRR = r₁ + [NPV₁ / (NPV₁ - NPV₂)] × (r₂ - r₁)
```
Where r₁ and r₂ are two trial rates with positive and negative NPVs.

---

#### D. Profitability Index (PI)

```
PI = PV of Future Cash Inflows / Initial Investment
   = 1 + (NPV / Initial Investment)
```

**Decision Rule:** Accept if PI > 1 (equivalent to NPV > 0)
**Use:** When capital is rationed (rank projects by PI)

---

### 4.3 NPV vs IRR — Which is Better?

| Criterion | NPV | IRR |
|-----------|-----|-----|
| Measure | Absolute value created (₹) | Rate of return (%) |
| Reinvestment assumption | At WACC (realistic) | At IRR (often unrealistic) |
| Multiple solutions | No | Possible (non-conventional CFs) |
| Capital rationing | Not directly useful | Not directly useful (use PI) |
| **Preferred method** | **YES — academically superior** | Good for communication |

**Golden Rule: When NPV and IRR conflict → Trust NPV.**

---

### 4.4 Case Study — Tata Steel's Corus Acquisition (2007)

**Background:** Tata Steel acquired Corus (Anglo-Dutch steelmaker) for $12.1 billion — India's largest M&A deal at the time.

**Capital Budgeting Analysis (simplified):**
- Initial outlay: $12.1 billion
- Expected synergies: Cost savings + Revenue gains
- WACC used: ~10-11% (blended India-UK cost)
- NPV projection: Positive based on steel demand forecasts

**Reality:**
- 2008 global financial crisis → Steel demand collapsed
- Corus became a drag on Tata Steel balance sheet
- By 2015, Tata Steel was trying to sell Corus's European plants

**Lesson:**
1. NPV analysis is only as good as the assumptions (demand forecasts were over-optimistic)
2. Sensitivity analysis and scenario analysis are critical
3. Synergy estimates in M&A are often inflated (winner's curse)

---

## 📌 CHAPTER 5: Risk Analysis in Capital Budgeting

### 5.1 Why Risk Analysis?

All capital budgeting projections involve uncertainty. Risk analysis quantifies this uncertainty.

**Types of Risk in Capital Budgeting:**
- **Stand-alone risk:** Project risk in isolation
- **Firm risk (corporate risk):** Project's contribution to overall firm risk
- **Market risk (systematic risk):** Project's beta contribution to market risk

---

### 5.2 Techniques for Risk Analysis

**1. Sensitivity Analysis:**
- Change one variable at a time (sales volume, price, cost) and see how NPV changes
- Identifies the most critical variable
- Example: "If sales fall 10%, NPV falls by ₹5 lakh — highly sensitive to sales"

**2. Scenario Analysis:**
- Define 3 scenarios: Optimistic, Base Case, Pessimistic
- Calculate NPV for each scenario
- Expected NPV = Σ (Probability × NPV for each scenario)

**3. Break-Even Analysis:**
- Find the level of sales/output at which NPV = 0
- Break-even point (Accounting): Fixed Costs / (Price - Variable Cost per unit)
- Break-even point (NPV): Level at which NPV just equals zero

**4. Monte Carlo Simulation:**
- Assign probability distributions to all key variables
- Run thousands of simulations → Distribution of NPV outcomes
- Calculate mean NPV and standard deviation

**5. Risk-Adjusted Discount Rate (RADR):**
```
RADR = Risk-free rate + Risk Premium
```
- Higher risk projects → Higher discount rate → Lower NPV → Harder to accept
- Example: New market entry → Add 5% risk premium over WACC

**6. Certainty Equivalent (CE) Method:**
```
Adjusted NPV = CE(CFt) / (1 + Rf)ᵗ
CE(CFt) = α × CFt   where α = certainty equivalent coefficient (0 < α ≤ 1)
```

---

## 📌 CHAPTER 6: Capital Structure Theory

### 6.1 What is Capital Structure?

**Definition:**
Capital Structure refers to the mix of debt and equity financing used by a firm to fund its assets and operations.

```
Capital Structure = Debt (D) + Equity (E)
Debt-to-Equity Ratio = D/E
Debt-to-Total Assets = D/(D+E)
```

**Key Question:** Is there an **optimal capital structure** that minimizes WACC and maximizes firm value?

---

### 6.2 Capital Structure Theories

**Theory 1: Modigliani-Miller (MM) Theorem — Without Taxes (1958)**

**Proposition I:** In a perfect capital market (no taxes, no bankruptcy costs, symmetric information):
```
Firm Value (Levered) = Firm Value (Unlevered)
VL = VU
```
**Capital structure is irrelevant to firm value.**

**Proposition II:** Cost of equity rises with leverage:
```
Ke = K₀ + (K₀ - Kd) × (D/E)
```
The benefit of cheap debt is exactly offset by rising equity cost → WACC unchanged.

---

**Theory 2: MM with Taxes (1963)**

With corporate taxes, interest is tax-deductible → Debt creates a **tax shield**.

```
VL = VU + T × D    (Tax Shield = Tax Rate × Debt)
```

**Implication:** 100% debt financing is optimal (extreme conclusion — unrealistic).

---

**Theory 3: Trade-Off Theory**

**Optimal capital structure** = Balance between:
- **Tax shield benefit** of debt (↑ as D rises)
- **Financial distress costs** (bankruptcy risk ↑ as D rises)

```
VL = VU + PV(Tax Shield) - PV(Financial Distress Costs)
```

**Optimal D/E:** Where marginal tax shield benefit = Marginal financial distress cost.

---

**Theory 4: Pecking Order Theory (Myers & Majluf, 1984)**

Firms prefer financing in this order due to information asymmetry:
1. **Internal funds** (retained earnings) — No signalling issues
2. **Debt** — Less information problem than equity
3. **External equity** — Last resort (signals overvaluation to market)

**India application:** Family-owned firms (Birla, Tata) prefer retained earnings; avoid diluting equity control.

---

**Theory 5: Agency Theory (Jensen & Meckling)**

- **Debt agency costs:** Risk shifting, asset substitution (shareholders take on riskier projects)
- **Equity agency costs:** Managers spend on perks, avoid value-creating but risky projects
- **Optimal structure balances both agency costs**

---

## 📌 CHAPTER 7: Leverage and EBIT-EPS Analysis

### 7.1 Leverage — Definition

**Leverage** refers to the use of fixed costs (operating or financial) to amplify returns. Like a lever — small input, large output (and large losses too).

---

### 7.2 Types of Leverage

**Operating Leverage (OL):**
- Use of **fixed operating costs** (rent, depreciation, salaries)
- Amplifies effect of sales changes on EBIT (Earnings Before Interest and Tax)

```
DOL (Degree of Operating Leverage) = % Change in EBIT / % Change in Sales
                                    = Contribution / EBIT
                                    = (Sales - Variable Costs) / EBIT
```

**Financial Leverage (FL):**
- Use of **fixed financial costs** (interest on debt)
- Amplifies effect of EBIT changes on EPS

```
DFL (Degree of Financial Leverage) = % Change in EPS / % Change in EBIT
                                    = EBIT / (EBIT - Interest)
```

**Combined Leverage (CL):**
```
DCL = DOL × DFL = Contribution / (EBIT - Interest) = Contribution / EBT
```

---

### 7.3 EBIT-EPS Analysis

**Purpose:** Determine which financing plan (all-equity vs. debt-equity mix) gives higher EPS at different levels of EBIT.

**EPS Formula:**
```
EPS = (EBIT - Interest) × (1 - Tax Rate) / Number of Shares
```

**Indifference Point:**
The EBIT level at which EPS is the same under both financing plans:
```
(EBIT - I₁)(1-T)/N₁ = (EBIT - I₂)(1-T)/N₂
```
- **Below indifference point:** Equity financing gives higher EPS
- **Above indifference point:** Debt financing gives higher EPS

**Worked Example:**
Company needs ₹10 lakh. Two options:
- Plan A: 10,000 equity shares @ ₹100
- Plan B: 5,000 shares + ₹5 lakh debt @ 10% interest

Tax rate = 30%

| EBIT | Plan A EPS | Plan B EPS |
|------|-----------|-----------|
| ₹50,000 | (50,000×0.70)/10,000 = **₹3.50** | (50,000-50,000×0.10)(0.70)/5,000 → *negative* |
| ₹1,00,000 | (1,00,000×0.70)/10,000 = **₹7.00** | (1,00,000-5,000)(0.70)/5,000 = **₹13.30** |

→ At higher EBIT, debt financing (Plan B) gives much higher EPS (financial leverage in action).

---

## 📌 CHAPTER 8: Dividend Policy Decisions

### 8.1 What is Dividend Policy?

**Definition:**
Dividend Policy refers to the decisions management makes about how much of the firm's earnings to distribute to shareholders as dividends versus retaining for reinvestment.

**Types of Dividends:**
- **Cash Dividend** — Most common (₹ per share)
- **Stock Dividend (Bonus Shares)** — Additional shares instead of cash
- **Interim Dividend** — Paid during the year
- **Final Dividend** — Declared at year end
- **Special/Extra Dividend** — One-time large payment

---

### 8.2 Dividend Policy Theories

**Theory 1: Dividend Irrelevance — MM (1961)**
In perfect markets, dividend policy doesn't affect firm value. Investors can create "homemade dividends" by selling shares. **Value = NPV of investment decisions, not dividends.**

**Theory 2: Bird-in-Hand Theory (Gordon, Lintner)**
Investors prefer **certain** dividends now over uncertain capital gains later.
Higher dividends → Lower required return → Higher stock price.
"A bird in hand is worth two in the bush."

**Theory 3: Tax Preference Theory**
Capital gains taxed at lower rate (or deferred) than dividends → Investors prefer lower dividends and higher capital gains. Firms should pay lower dividends.

**Theory 4: Signaling Theory**
Dividends signal management's confidence about future earnings.
- Dividend increase → Signal of higher future profits → Stock price rises
- Dividend cut → Signal of financial trouble → Stock price falls

**Theory 5: Clientele Effect**
Different investors have different dividend preferences (tax brackets, income needs). Firms attract a stable "clientele" based on their dividend policy. Changing policy alienates existing shareholders.

---

### 8.3 Walter's and Gordon's Dividend Models

**Walter's Model:**
```
P = (D + (r/Ke)(E-D)) / Ke
```
Where: P = Market price, D = Dividend, E = EPS, r = internal rate of return, Ke = cost of equity

- If r > Ke: Firm should retain all earnings (growth firm)
- If r < Ke: Firm should distribute all earnings (mature firm)
- If r = Ke: Dividend policy irrelevant

**Gordon's Model:**
```
P = E(1-b) / (Ke - br)
```
Where: b = retention ratio, br = growth rate

---

### 8.4 India Dividend Context

| Company | Dividend Policy | Style |
|---------|----------------|-------|
| Coal India | High, stable dividend | Government mandate; PSU |
| TCS | Regular + special dividends | Mature, cash-rich |
| Reliance Industries | Low dividend, high retention | Growth phase |
| Infosys | Progressive dividend policy | Stable growth + buybacks |

**Dividend Distribution Tax (DDT):** India abolished DDT in 2020. Dividends now taxed in hands of shareholders at applicable income tax rate.

---

## 📌 CHAPTER 9: Working Capital Management

### 9.1 What is Working Capital?

**Definition:**
Working Capital is the capital used to finance the day-to-day operations of a business.

```
Gross Working Capital = Total Current Assets
Net Working Capital (NWC) = Current Assets - Current Liabilities
```

**Current Assets:** Cash, Debtors, Inventory, Short-term investments
**Current Liabilities:** Creditors, Short-term loans, Outstanding expenses

---

### 9.2 Operating Cycle

**Definition:**
The Operating Cycle (or Cash Conversion Cycle) is the time it takes for a business to convert raw material purchases into cash receipts from customers.

```
Operating Cycle = Raw Material Storage Period + WIP Period + Finished Goods Period + Debtors Collection Period
Net Operating Cycle = Operating Cycle - Creditors Payment Period
```

**Cash Conversion Cycle (CCC):**
```
CCC = Days Inventory Outstanding (DIO) + Days Sales Outstanding (DSO) - Days Payable Outstanding (DPO)
```

**Ideal:** Shorter CCC = Less working capital needed = More efficient

**Example — Amazon's Negative CCC:**
- Amazon collects from customers immediately (DSO ≈ 0)
- But pays suppliers in ~45-60 days (DPO ≈ 45-60)
- Result: Negative CCC → Suppliers effectively finance Amazon's operations

---

### 9.3 Working Capital Financing Strategies

| Strategy | Description | Risk | Return |
|----------|-------------|------|--------|
| **Conservative** | Finance all assets with long-term funds | Low | Low |
| **Aggressive** | Finance even permanent assets with short-term funds | High | High |
| **Moderate (Hedging)** | Match asset life with liability maturity | Medium | Medium |

---

### 9.4 Key Working Capital Components

**Cash Management:**
- Motives for holding cash: Transaction, Precautionary, Speculative
- **Baumol Model:** Optimal cash balance = √(2 × Annual Cash Need × Transaction Cost / Interest Rate)
- **Miller-Orr Model:** Stochastic cash management (when cash flows uncertain)

**Inventory Management:**
- **EOQ (Economic Order Quantity):** Q* = √(2 × Annual Demand × Ordering Cost / Holding Cost)
- Minimize total inventory cost (ordering cost + holding cost)

**Debtors/Receivables Management:**
- Credit period, credit standards, collection efforts
- Trade-off: Liberal credit → Higher sales but higher bad debts + longer collection period

---

### 9.5 Case Study — Infosys Working Capital Efficiency

**Background:** Infosys, a services company, manages working capital differently from manufacturing companies.

**Key Metrics (FY24):**
- Days Sales Outstanding (DSO): ~67 days (billing to cash collection)
- No inventory (services firm)
- Minimal payables (mainly salaries — monthly)
- Free Cash Flow: ~$2.5 billion annually

**Working Capital Strategy:**
- Strong receivables management (dedicated collections team per client)
- Advance billing for large projects
- Minimal capital tied up in physical assets
- Investment of surplus cash in liquid funds (₹15,000+ crore in liquid investments)

**Lesson:** Working capital management in services firms focuses on receivables and cash. In manufacturing (like Tata Steel), it's dominated by inventory and raw material management.

---

## MASTER SUMMARY TABLE

| Chapter | Core Concept | Key Formula | Key Author |
|---------|-------------|------------|-----------|
| 1 | Financial Management Goals | Shareholder Wealth = Price × Shares | — |
| 2 | Time Value of Money | FV = PV(1+r)ⁿ; PV = FV/(1+r)ⁿ | — |
| 3 | Cost of Capital | WACC = Wd×Kd(1-T) + We×Ke; CAPM | Sharpe, Lintner |
| 4 | Investment Decisions | NPV = ΣCFt/(1+r)ᵗ - I₀ | — |
| 5 | Risk in Capital Budgeting | Sensitivity, Scenario, Monte Carlo | — |
| 6 | Capital Structure | VL = VU + TD (MM with taxes) | Modigliani & Miller |
| 7 | Leverage & EBIT-EPS | DOL, DFL, DCL formulas | — |
| 8 | Dividend Policy | Walter's, Gordon's Model | Walter, Gordon, MM |
| 9 | Working Capital | CCC = DIO + DSO - DPO; EOQ | Baumol, Miller-Orr |

---

*Document prepared for MBA 2nd Semester, DU SOL | Subject: Corporate Finance*
*For Academic Use Only*
