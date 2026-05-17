# 📗 CF CHAPTER 2: Time Value of Money (TVM)
### Subject: Corporate Finance | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

**The Golden Rule of Finance:** *A Rupee today is worth more than a Rupee tomorrow.*

Why?
1. **Opportunity Cost:** If I have ₹100 today, I can put it in a bank and earn interest. In a year, it will be ₹108. If you give me the ₹100 next year instead, I lose out on that ₹8.
2. **Inflation:** ₹100 today buys a movie ticket. Next year, the ticket might cost ₹110. Your money loses purchasing power.
3. **Risk:** You might promise to give me ₹100 next year, but you might go bankrupt. Having the money *now* is certain.

Therefore, we can never simply add cash flows from different years together. We have to adjust them using the **Time Value of Money**.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. Compounding (Going Forward in Time)
Finding out what money today will be worth in the future.
> **Future Value (FV) = PV × (1 + r)ⁿ**
*(Where PV is Present Value, r is interest rate, n is number of years)*

### 2. Discounting (Going Backward in Time)
Finding out what future money is worth today. This is the most important concept in corporate finance!
> **Present Value (PV) = FV / (1 + r)ⁿ**

### 3. Special Cash Flows
- **Annuity:** A fixed amount of money paid/received every year for a set number of years (e.g., your car loan EMI, or ₹10,000 every year for 5 years).
- **Perpetuity:** A fixed amount of money paid/received every year **FOREVER**. 
  > **PV of Perpetuity = Cash Flow / r**

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. Explain the concepts of Compounding and Discounting. A company promises to pay you ₹50,000 every year for the next 5 years. If your required rate of return is 10%, calculate the Present Value of this annuity. (10 Marks)

**1. Conceptual Explanation:**
*   **Compounding** is the process of calculating the Future Value (FV) of a cash flow or series of cash flows. It operates on the principle of earning "interest on interest." It projects current cash into the future.
*   **Discounting** is the exact opposite. It is the process of determining the Present Value (PV) of a future cash flow. It strips away the interest component to tell us what a future sum is worth in today's terms. It is the foundation of capital budgeting (NPV).

**2. Numerical Solution (Present Value of an Annuity):**
*   **Given:** Cash Flow (CF) = ₹50,000; Rate (r) = 10% or 0.10; Time (n) = 5 years.
*   **Formula:** $PVA = CF \times \frac{1 - (1+r)^{-n}}{r}$
*   **Alternative Method (Using PVAF Table):**
    Present Value of Annuity = Annual Cash Flow × Present Value Annuity Factor (PVAF at 10% for 5 years)
    *(In exams, they often provide tables, or you calculate the factor)*
    PVAF (10%, 5 yrs) = 3.7908
*   **Calculation:**
    PVA = 50,000 × 3.7908 = **₹1,89,540**
*   **Interpretation:** Receiving ₹1,89,540 today is exactly mathematically equivalent to receiving ₹50,000 every year for 5 years, assuming you can invest money at a 10% return.

### Quick Exam Formulas Cheatsheet:
- **Rule of 72:** To find out how long it takes for money to double, divide 72 by the interest rate. (e.g., at 8% interest, money doubles in 72/8 = 9 years).
- **Effective Annual Rate (EAR):** If compounding is semi-annual or quarterly, the actual interest earned is higher than the stated rate.
  $EAR = (1 + \frac{r}{m})^m - 1$ (where m = number of compounding periods per year).
