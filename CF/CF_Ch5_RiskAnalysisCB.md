# 📗 CF CHAPTER 5: Risk Analysis in Capital Budgeting
### Subject: Corporate Finance | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

In Chapter 4, we calculated NPV assuming we knew *exactly* how much cash the project would generate over the next 5 years. 
But wait—nobody can predict the future! 
What if raw material costs suddenly double? What if sales are 20% lower than expected? What if a pandemic hits?

**Risk Analysis** is the process of stress-testing our Capital Budgeting decisions to see what happens to our project if things go wrong.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

How do we measure and adjust for this uncertainty?

### 1. Sensitivity Analysis (The "What-If" Test)
- You change **one variable at a time** (e.g., change ONLY the sales price, keeping everything else constant) and see how it affects the NPV.
- It tells management which variable the project is most "sensitive" to. If a 5% drop in selling price turns the NPV negative, management knows they must lock in selling prices with contracts.

### 2. Scenario Analysis
- Instead of changing one variable, you change several variables to create different "Scenarios."
- Usually three: **Best Case (Optimistic)**, **Base Case (Expected)**, and **Worst Case (Pessimistic)**.
- You calculate the NPV for all three to see the range of possible outcomes.

### 3. Risk-Adjusted Discount Rate (RADR)
- If a project is very risky (like launching a totally untested new product), the normal WACC isn't a high enough hurdle.
- You artificially increase the discount rate. 
- **Rule:** Higher Risk = Higher Discount Rate = Lower NPV. It makes risky projects harder to accept.

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. Explain the various methods used for incorporating risk into Capital Budgeting decisions. Distinguish between Sensitivity Analysis and Scenario Analysis. (15 Marks)

**1. Introduction to Risk in Capital Budgeting:**
Risk in capital budgeting refers to the variability of expected future cash flows. Since capital expenditures are large, irreversible, and long-term, incorporating risk is essential to prevent value destruction. 

**2. Methods for Incorporating Risk:**

*   **A. Risk-Adjusted Discount Rate (RADR):**
    This method adjusts the denominator in the NPV formula. For projects with above-average risk, a risk premium is added to the firm's cost of capital (WACC). 
    *Formula:* $RADR = Risk-Free Rate + Risk Premium$
    *Impact:* A higher discount rate heavily penalizes future cash flows, resulting in a lower NPV, thereby enforcing stricter acceptance criteria for risky projects.

*   **B. Certainty Equivalent (CE) Approach:**
    This method adjusts the numerator (the cash flows) rather than the discount rate. The uncertain expected cash flows are multiplied by a Certainty Equivalent Coefficient (α), which ranges from 0 to 1. (1 = completely certain, 0.5 = highly uncertain). The adjusted, "certain" cash flows are then discounted at the risk-free rate.

*   **C. Monte Carlo Simulation:**
    A highly advanced, computer-driven technique that assigns probability distributions to all key variables (price, cost, volume). The computer runs thousands of simulations to generate a probability distribution of the project's NPV, giving management the exact probability (e.g., 15%) that the project will have a negative NPV.

**3. Distinction: Sensitivity vs. Scenario Analysis:**

| Basis of Difference | Sensitivity Analysis | Scenario Analysis |
|---------------------|----------------------|-------------------|
| **Variables Changed** | Changes **only ONE variable** at a time (e.g., only sales volume) while holding all others constant. | Changes **MULTIPLE variables** simultaneously to reflect a cohesive state of the world. |
| **Objective** | Identifies the single most critical "weak link" in the project. | Provides a holistic view of the project under different macro-conditions (Optimistic, Base, Pessimistic). |
| **Realism** | Less realistic (in the real world, variables are correlated; if price drops, volume usually rises). | Highly realistic (captures the correlation between variables during a downturn or boom). |

**Conclusion:**
While no mathematical model can eliminate risk, using a combination of RADR for discounting and Scenario Analysis for forecasting equips the financial manager to make resilient, informed investment decisions under uncertainty.
