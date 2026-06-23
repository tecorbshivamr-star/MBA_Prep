# 📘 Corporate Finance — Chapter 5: Risk Analysis in Capital Budgeting
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** Focus on Sensitivity Analysis (most tested), Scenario Analysis, RADR vs. Certainty Equivalent comparison, and Decision Tree Analysis (draw the tree!). Expect theory + a small numerical on sensitivity or decision tree.

---

## 5.1 Learning Objectives

By the end of this chapter, you should be able to:

- ✅ Define Risk and distinguish it from Uncertainty
- ✅ Identify and classify the sources of risk in capital budgeting
- ✅ Conduct and interpret Sensitivity Analysis
- ✅ Apply Scenario Analysis and Simulation (Monte Carlo)
- ✅ Use Risk-Adjusted Discount Rate (RADR) and Certainty Equivalent (CE) methods
- ✅ Construct and solve Decision Trees for sequential investment decisions

---

## 5.2 Introduction

### Why Risk Analysis in Capital Budgeting?

Standard capital budgeting (NPV, IRR) assumes **certainty** of future cash flows — but in reality, cash flows are **uncertain and variable**.

> 📌 *"All capital investment decisions involve some degree of risk — the future is never perfectly predictable."*

**Risk analysis helps:**
- Identify which variables most affect project viability
- Quantify the range of possible outcomes
- Adjust the decision-making process for risk
- Avoid overconfident project selection

---

## 5.3 Definition of Risk

### Risk vs. Uncertainty

| Feature | **Risk** | **Uncertainty** |
|---|---|---|
| **Definition** | Variability in outcomes where **probabilities are known** | Variability where **probabilities cannot be assigned** |
| **Measurability** | Quantifiable (using probability distributions) | Not quantifiable |
| **Example** | Probability of rain = 60% | Revolutionary new technology — no historical data |
| **Framework** | Use Expected Value, SD, Variance | Use scenario/qualitative judgment |

> 📌 *Knight (1921)*: Distinguished risk (measurable) from uncertainty (unmeasurable).

---

### Measures of Risk:

| Measure | Formula | Interpretation |
|---|---|---|
| **Expected Value (EV)** | EV = Σ (Pᵢ × CFᵢ) | Probability-weighted average outcome |
| **Variance (σ²)** | σ² = Σ Pᵢ × (CFᵢ − EV)² | Average squared deviation from mean |
| **Standard Deviation (σ)** | σ = √Variance | Absolute measure of risk (same units as CF) |
| **Coefficient of Variation (CV)** | CV = σ / EV | Relative risk per unit of return; used to compare projects of different scales |

> 💡 **CV is the best measure for comparing risk across projects with different expected values.**

#### Example:
> Project A: EV = ₹10,000, σ = ₹2,000 → CV = 0.20
> Project B: EV = ₹50,000, σ = ₹8,000 → CV = 0.16

```
Project B has lower CV (0.16 < 0.20) → Less risky per unit of return → Prefer B
```

---

### Types of Risk in Capital Budgeting:

| Type | Definition |
|---|---|
| **Stand-alone Risk** | Risk of a project in isolation (ignoring diversification) |
| **Corporate / Firm Risk** | Contribution of the project to the firm's total risk |
| **Market / Systematic Risk** | Contribution to market risk (measured by project Beta) |

> For a diversified investor, only **market (systematic) risk** matters. But for managers and concentrated owners, **firm risk** also matters.

---

## 5.4 Sources of Risk

### Project-Specific Sources:

| Source | Explanation |
|---|---|
| **Estimation Risk** | Error in estimating cash flows, life, salvage value |
| **Technology Risk** | Risk that technology becomes obsolete faster than expected |
| **Completion Risk** | Risk of project delays, cost overruns during implementation |
| **Operating Risk** | Variability in operating costs (labor, raw material price changes) |
| **Market / Demand Risk** | Uncertainty in demand for the project's output |

### Firm-Level Sources:

| Source | Explanation |
|---|---|
| **Business Risk** | Variability in firm's EBIT due to operating leverage (fixed costs) |
| **Financial Risk** | Variability due to use of debt (financial leverage) |
| **Management Risk** | Poor decision-making, governance failures |

### Market-Level Sources:

| Source | Explanation |
|---|---|
| **Systematic Risk** | Economy-wide risks: recession, inflation, interest rate changes |
| **Regulatory Risk** | Change in government policy, taxes, environmental laws |
| **Country Risk** | Political instability, currency inconvertibility |

---

## 5.5 Sensitivity Analysis

### Definition

**Sensitivity Analysis** examines how **NPV (or IRR) changes** when **one variable at a time** is changed from its base case value, holding all other variables constant.

> Also called **"What-if" Analysis** or **"Ceteris Paribus" Analysis**

### Purpose:
- Identify which variables are most **critical** (have greatest impact on NPV)
- Focus management attention on key assumptions
- Reveal the project's **vulnerability** to specific risks

---

### Steps in Sensitivity Analysis:

```
Step 1: Establish the BASE CASE
        → Calculate NPV using most likely estimates of all variables

Step 2: Identify KEY VARIABLES
        → Sales volume, selling price, variable cost, fixed cost,
           project life, salvage value, discount rate

Step 3: Change ONE variable at a time
        → Typically: ±10%, ±20% or set pessimistic/optimistic values

Step 4: Recalculate NPV for each change

Step 5: Measure Sensitivity
        → % change in NPV / % change in variable

Step 6: RANK variables by impact on NPV
        → Most sensitive variable = most critical risk factor
```

---

### Sensitivity Analysis — Full Numerical Example:

> **Base Case** (WACC = 10%):
> - Sales Volume: 10,000 units/yr
> - Selling Price: ₹50/unit
> - Variable Cost: ₹30/unit
> - Fixed Cost: ₹50,000/yr
> - Project Life: 5 years
> - Initial Investment: ₹2,00,000

**Base Case Annual CF:**
```
Revenue        = 10,000 × 50 = ₹5,00,000
Variable Cost  = 10,000 × 30 = ₹3,00,000
Fixed Cost     =              ₹   50,000
─────────────────────────────────────────
EBITDA         =              ₹1,50,000
(Assume no depreciation/tax for simplicity)

PV of CFs (Annuity 5 yrs, 10%) = 1,50,000 × 3.791 = ₹5,68,650
Base Case NPV = 5,68,650 − 2,00,000 = ₹3,68,650
```

**Sensitivity Table (10% adverse change in each variable):**

| Variable | Change | New Annual CF | New NPV | Change in NPV | % Change in NPV |
|---|---|---|---|---|---|
| Base Case | — | ₹1,50,000 | ₹3,68,650 | — | — |
| Sales Volume | −10% (9,000 units) | ₹1,30,000 | ₹2,92,830 | −75,820 | **−20.6%** |
| Selling Price | −10% (₹45) | ₹1,00,000 | ₹1,79,100 | −1,89,550 | **−51.4%** |
| Variable Cost | +10% (₹33) | ₹1,20,000 | ₹2,54,920 | −1,13,730 | **−30.8%** |
| Fixed Cost | +10% (₹55,000) | ₹1,45,000 | ₹3,49,695 | −18,955 | **−5.1%** |

> **Conclusion**: Selling Price is most critical (−51.4% NPV change) → Management must protect pricing power. Fixed Cost is least sensitive.

---

### Sensitivity Graph (Spider Diagram / Tornado Chart):

```
% Change in NPV
      │
 +50% │     ╱  Selling Price (steepest slope = most sensitive)
      │    ╱
      │   ╱  Variable Cost
      │  ╱
      │ ╱  Sales Volume
      │╱  
──────┼──────────────────────────────► % Change in Variable
      │╲  Fixed Cost (flattest = least sensitive)
      │ ╲
 -50% │  ╲

Steeper slope = More sensitive = Higher risk factor
```

---

### Limitations of Sensitivity Analysis:

| Limitation | Explanation |
|---|---|
| **One variable at a time** | Does not consider simultaneous changes in multiple variables |
| **No probability** | Does not assign likelihood to each scenario |
| **Ignores correlations** | Variables are often correlated (e.g., price and volume) |
| **Subjectivity** | Range of variation chosen is subjective |

---

## 5.6 Methods to Adjust Risk in Capital Budgeting

### Method 1: Scenario Analysis

**Definition**: Examines NPV under **three distinct scenarios** — Pessimistic, Base (Most Likely), and Optimistic — where **multiple variables change simultaneously**.

```
Scenarios:
  Pessimistic = All key variables take their worst values simultaneously
  Base Case   = Most likely values (as per base case)
  Optimistic  = All key variables take their best values simultaneously
```

#### Example:

| Scenario | Probability | NPV |
|---|---|---|
| Pessimistic | 0.25 | −₹50,000 |
| Base Case | 0.50 | ₹1,00,000 |
| Optimistic | 0.25 | ₹2,50,000 |

```
Expected NPV = 0.25×(−50,000) + 0.50×(1,00,000) + 0.25×(2,50,000)
             = −12,500 + 50,000 + 62,500
             = ₹1,00,000

Variance = 0.25×(−50,000−1,00,000)² + 0.50×(0)² + 0.25×(2,50,000−1,00,000)²
         = 0.25×(22,500,000,000) + 0 + 0.25×(22,500,000,000)
         = ₹11,250,000,000

σ = √11,250,000,000 = ₹1,06,066

CV = 1,06,066 / 1,00,000 = 1.06  (relatively high risk)
```

**Advantage over Sensitivity Analysis**: Multiple variables change simultaneously — more realistic.

**Limitation**: Only 3 discrete scenarios; ignores the full distribution of outcomes.

---

### Method 2: Simulation Analysis (Monte Carlo)

**Definition**: Uses computer-generated **random sampling** from probability distributions of each key variable to generate **thousands of possible NPV outcomes**.

```
MONTE CARLO SIMULATION STEPS:
│
├── Step 1: Specify probability distribution for each uncertain variable
│           (Sales volume: Normal; Price: Triangular; Cost: Uniform)
│
├── Step 2: Randomly sample one value for each variable
│           (Computer picks values based on their distributions)
│
├── Step 3: Calculate NPV using sampled values
│
├── Step 4: Repeat Steps 2-3 many times (1,000 to 10,000 iterations)
│
└── Step 5: Plot distribution of all NPVs
            → Mean NPV, Standard Deviation, Probability (NPV < 0)
```

**Output:** A full **probability distribution** of NPV outcomes.

```
Probability
     │        ╭───╮
     │       ╱     ╲
     │      ╱       ╲
     │─────╱─────────╲────────────► NPV
     │   ◄─►           ◄─►
     │  NPV<0           NPV>0

P(NPV < 0) = Area to the left of zero = Probability of loss
```

**Advantages:**
- Considers correlations between variables
- Generates full probability distribution (not just 3 scenarios)
- Most comprehensive risk analysis tool

**Limitations:**
- Requires significant data and computing power
- Results depend on assumed probability distributions
- Complex to communicate to non-specialists

---

### Method 3: Risk-Adjusted Discount Rate (RADR)

**Definition**: Adjust the discount rate upward to reflect project risk. Higher risk → Higher discount rate → Lower NPV → Higher hurdle to clear.

```
RADR = Risk-Free Rate + Risk Premium for the project

NPV (Risk-Adjusted) = Σ [CFt / (1 + RADR)ᵗ] − Initial Investment
```

**Risk Premium Classification:**

| Project Type | Risk Level | RADR Adjustment |
|---|---|---|
| Replacement (same business) | Low | WACC + 0–2% |
| Expansion (existing business) | Moderate | WACC + 2–4% |
| New Product / Market | High | WACC + 4–6% |
| R&D / Speculative | Very High | WACC + 6%+ |

#### Example:
> WACC = 12%. Base project NPV at 12% = ₹80,000.
> Project is a new product launch → RADR = 12% + 5% = 17%.
> Recalculated NPV at 17% = ₹35,000. Still positive → Accept.

**Merits of RADR:**
- Simple to apply
- Intuitive — higher risk deserves higher return
- Widely used in practice

**Demerits of RADR:**
- Risk premium is subjective (no standard formula)
- Assumes risk increases at constant rate with time (compounds over years)
- Does not distinguish between types of risk

---

### Method 4: Certainty Equivalent (CE) Approach

**Definition**: Convert risky cash flows to their **certain equivalents** (smaller, but guaranteed amounts) and then discount at the **risk-free rate**.

```
CE Cash Flow = α × Risky Cash Flow

Where:
  α (alpha) = Certainty Equivalent Coefficient (0 < α ≤ 1)
  α = 1     → Certainty (no risk)
  α → 0     → Extremely risky

NPV (CE) = Σ [αt × CFt / (1 + Rf)ᵗ] − Initial Investment
```

> 📌 **α is determined by management's risk preference** — how much certain income they'd accept in exchange for the risky cash flow.

#### Example:
> Risky CF Year 1 = ₹1,00,000; α = 0.80; Rf = 6%.

```
CE Cash Flow = 0.80 × 1,00,000 = ₹80,000
PV = 80,000 / 1.06 = ₹75,472
```

---

### RADR vs. Certainty Equivalent — Key Comparison (Exam Favourite!)

| Feature | **RADR** | **Certainty Equivalent (CE)** |
|---|---|---|
| **Adjustment** | Adjusts the **discount rate** upward | Adjusts the **cash flows** downward |
| **Risk-Free Rate** | Uses risk-adjusted rate | Uses risk-free rate (Rf) |
| **Assumption** | Risk increases uniformly over time | Risk of each period treated separately |
| **Flexibility** | Less flexible (same rate all periods) | More flexible (different α each year) |
| **Theoretical Soundness** | Less rigorous | More rigorous (utility theory based) |
| **Ease of Use** | ✅ Simpler and more widely used | ❌ Requires estimating α (subjective) |
| **Practical Use** | Very common in practice | Less common; more academic |

> 💡 **CE is theoretically superior**; **RADR is practically preferred**.

---

### Method 5: Decision Tree Analysis

**Definition**: A **graphical tool** that maps out all possible **sequential decisions and chance events** along with their probabilities and payoffs.

> Used when capital budgeting involves **multiple stages** and decisions depend on outcomes of earlier stages.

### Key Elements:

| Symbol | Meaning |
|---|---|
| **□ (Square node)** | Decision Node — manager makes a choice |
| **○ (Circle node)** | Chance Node — outcome is uncertain (with probabilities) |
| **→ Branches** | Each possible decision or outcome |
| **Terminal Values** | NPV at the end of each path |

---

### Decision Tree — Full Example:

> **Stage 1**: Invest ₹50,000 in pilot project.
> **After 1 year**: Demand is High (p=0.6) or Low (p=0.4).
>
> **Stage 2** (if Demand is High): Invest ₹2,00,000 in full project → NPV = ₹3,00,000 (p=0.7) or ₹80,000 (p=0.3)
> **Stage 2** (if Demand is Low): Invest ₹2,00,000 → NPV = ₹60,000 (p=0.5) or −₹40,000 (p=0.5). Or Abandon.

```
                        [Success, NPV=3,00,000] p=0.7
                   ╱── ○
     [High]  p=0.6 ─── Invest ₹2L
        ╱              ╲── [Moderate, NPV=80,000] p=0.3
 □ ─── ○
(Pilot)    ╲              ╱── [Moderate, NPV=60,000] p=0.5
     [Low]  p=0.4 ─── Invest ₹2L ─── ○
                   ╲              ╲── [Loss, NPV=−40,000] p=0.5
                    └── Abandon → NPV = 0
```

**Backward Induction (Roll Back Method):**

*Step 1: Calculate EV at each chance node (working backwards)*

```
If High Demand — Invest:
EV = 0.7 × 3,00,000 + 0.3 × 80,000 = 2,10,000 + 24,000 = ₹2,34,000

If Low Demand — Invest:
EV = 0.5 × 60,000 + 0.5 × (−40,000) = 30,000 − 20,000 = ₹10,000

If Low Demand — Abandon:
EV = ₹0 → Choose Abandon (₹0 > ₹10,000... wait: 10,000 > 0 so INVEST)
→ Choose: Invest (₹10,000 > ₹0)
```

*Step 2: Calculate Overall EV at Stage 1*
```
EV = 0.6 × 2,34,000 + 0.4 × 10,000
   = 1,40,400 + 4,000
   = ₹1,44,400

Less: Pilot Investment = −₹50,000
Net Expected NPV = ₹94,400 → POSITIVE → Proceed with Pilot ✅
```

---

### Advantages of Decision Tree Analysis:

| Advantage | Explanation |
|---|---|
| **Sequential decisions** | Handles multi-stage investment decisions explicitly |
| **Visual clarity** | Makes complex decision logic easy to understand |
| **Flexibility** | Can incorporate all possible paths and probabilities |
| **Option value** | Captures value of waiting, abandoning, or expanding |

### Limitations:

| Limitation | Explanation |
|---|---|
| **Complexity** | Trees become unmanageable with many stages/branches |
| **Probability estimation** | Assigning probabilities to outcomes is subjective |
| **Single discount rate** | Standard DTA doesn't adjust for risk along each path |

---

### Method 6: Break-Even Analysis (Supplementary)

**Definition**: Identifies the **minimum level of a variable** (sales, price, volume) at which NPV = 0.

```
Break-Even Sales Volume (for NPV = 0):

Set NPV = 0 and solve for the unknown variable

Break-Even Point (Units) = Fixed Costs / (Selling Price − Variable Cost per unit)
                         = Fixed Costs / Contribution Margin per unit
```

> Closely linked to **Sensitivity Analysis** — the break-even value shows how far the base case can fall before the project becomes unviable.

---

## 5.7 Summary

### 🔑 Key Takeaways — Chapter 5

| Concept | Key Point |
|---|---|
| **Risk vs. Uncertainty** | Risk = known probabilities; Uncertainty = unknown probabilities |
| **Stand-alone Risk** | Measured by σ and CV; CV best for cross-project comparison |
| **Sources of Risk** | Project-specific (estimation, technology, market) + Firm-level + Market-level |
| **Sensitivity Analysis** | One variable at a time; identifies most critical variable; no probabilities |
| **Scenario Analysis** | Multiple variables change simultaneously; 3 scenarios with probabilities |
| **Simulation** | Monte Carlo; full probability distribution; most comprehensive |
| **RADR** | Adjusts discount rate; simple, widely used; less flexible |
| **Certainty Equivalent** | Adjusts cash flows; more rigorous; uses Rf; flexible across periods |
| **Decision Tree** | Sequential decisions; backward induction; captures option value |
| **Break-Even** | Minimum variable level for NPV = 0; complements sensitivity |

---

### ⚡ Master Formula Sheet

```
Expected Value:
  EV = Σ (Pᵢ × CFᵢ)

Variance & SD:
  σ² = Σ Pᵢ(CFᵢ − EV)²
  σ  = √σ²

Coefficient of Variation:
  CV = σ / EV   [Lower CV = Less risk per unit of return]

RADR:
  RADR = Risk-Free Rate + Risk Premium
  NPV  = Σ [CFt / (1+RADR)ᵗ] − I₀

Certainty Equivalent:
  CE Cash Flow = α × Risky CF    (0 < α ≤ 1)
  NPV(CE) = Σ [αt × CFt / (1+Rf)ᵗ] − I₀

Sensitivity (% Impact):
  Sensitivity = % Change in NPV / % Change in Variable

Break-Even Volume:
  Q* = Fixed Costs / (P − VC per unit)

Decision Tree: Use Backward Induction
  EV at chance node = Σ (Probability × Payoff)
  At decision node  = Choose branch with highest EV
```

---

### 📝 Likely Exam Questions — Chapter 5

1. **What is Risk in capital budgeting? Distinguish between Risk and Uncertainty.**
2. **What are the sources of risk in capital budgeting decisions? Classify them.**
3. **Define Standard Deviation and Coefficient of Variation. Why is CV preferred for comparing risky projects?**
4. **What is Sensitivity Analysis? Explain its steps with an example.**
5. **Calculate and rank sensitivity for the following project as each variable changes by 10%.** *(Numerical)*
6. **What is Scenario Analysis? How does it differ from Sensitivity Analysis?**
7. **Explain Monte Carlo Simulation as a risk analysis tool. What are its advantages and limitations?**
8. **What is the Risk-Adjusted Discount Rate (RADR) approach? How is the risk premium determined?**
9. **Explain the Certainty Equivalent approach. What is the Certainty Equivalent Coefficient (α)?**
10. **Compare RADR and Certainty Equivalent approaches. Which is theoretically superior and which is practically preferred?**
11. **What is Decision Tree Analysis? Explain with a diagram the decision and chance nodes.**
12. **Draw and solve a Decision Tree for a two-stage investment with given probabilities and payoffs.** *(Numerical)*
13. **What is Break-Even Analysis in the context of capital budgeting?**
14. **"Sensitivity Analysis is the most commonly used tool for risk analysis in capital budgeting." Evaluate this statement critically.**

---

*📅 Prepared for: Corporate Finance Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
