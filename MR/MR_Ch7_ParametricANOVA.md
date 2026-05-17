# 📗 MR CHAPTER 7: Parametric Hypothesis Testing & ANOVA
### Subject: Marketing Research | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

You are the CEO of a supermarket. Your manager claims: *"If we play slow classical music, customers will walk slower and buy 20% more stuff!"*
You run an experiment on 50 customers. They bought 5% more stuff. 

Does this mean the manager's theory is true? Or was it just random luck that those 50 customers happened to buy a little more that day? 

**Hypothesis Testing** is the mathematical lie-detector test. It uses statistics to tell you exactly how likely it is that the manager is right, or if the result was just random chance. 

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. The Two Hypotheses
In every test, you set up a fight between two statements:
- **Null Hypothesis (H₀):** The "Status Quo" or "No Effect." (e.g., *Music has NO effect on sales*). You always assume this is true until proven otherwise.
- **Alternative Hypothesis (H₁):** The researcher's claim. (e.g., *Music INCREASES sales*). 

You run the math. If the probability (p-value) of the result happening by pure chance is less than 5% (p < 0.05), you **Reject the Null Hypothesis**. You proved your theory!

### 2. t-tests (Comparing 1 or 2 things)
- **One-Sample t-test:** Compare your sample to a known national average. (e.g., *Is the average age of our buyers different from 35?*)
- **Independent Samples t-test:** Compare two separate groups. (e.g., *Do Men spend more money than Women?*)
- **Paired Samples t-test:** Compare the *same* group twice. (e.g., *Weighing people BEFORE a diet, and the same people AFTER the diet*).

### 3. ANOVA (Comparing 3 or more things)
What if you have 3 groups? (e.g., *Do customers in Delhi, Mumbai, and Chennai spend different amounts?*) 
You cannot use a t-test. You must use **ANOVA (Analysis of Variance)**. If ANOVA says "Yes, there is a difference," you then use a *Post-Hoc test* to find out exactly which city is the highest.

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. Explain the framework of Hypothesis Testing. What is ANOVA? When is a One-Way ANOVA preferred over a t-test? (15 Marks)

**1. The Framework of Hypothesis Testing:**
Hypothesis testing is a systematic statistical procedure used to make inferences about a population parameter based on sample data. It provides a mathematical basis for decision-making under uncertainty.

**The Sequential Steps:**
*   **Step 1: State the Hypotheses.** Formulate the Null Hypothesis (H₀) which posits no difference/relationship, and the Alternative Hypothesis (H₁) which posits a significant difference/relationship.
*   **Step 2: Choose the Level of Significance (α).** Typically set at 0.05 (5%). This is the maximum acceptable risk of making a Type I Error (rejecting a true Null Hypothesis — a "false positive").
*   **Step 3: Select the Test Statistic.** Choose the appropriate test (z-test, t-test, F-test) based on the sample size, data type, and population variance.
*   **Step 4: Calculate the Test Statistic & P-value.** Use the sample data to compute the mathematical value. 
*   **Step 5: Make the Decision.** If the calculated p-value is less than α (e.g., p = 0.02), reject H₀. If p > α, fail to reject H₀.

**2. Understanding ANOVA (Analysis of Variance):**
ANOVA is a powerful parametric statistical technique used to test if there are statistically significant differences between the means of **three or more** independent populations. 
*   It operates by partitioning the total variance in the data into two components: variance *between* the groups, and variance *within* the groups. 
*   The test statistic is the **F-ratio** (Mean Square Between / Mean Square Within). A high F-ratio indicates that the group means are genuinely different, not just a result of random within-group noise.

**3. Why ANOVA is preferred over t-tests for 3+ groups:**
A common student mistake is assuming that to compare 3 groups (A, B, and C), one could simply run three separate independent t-tests (A vs B, B vs C, A vs C). 
*   **The Problem (Alpha Inflation):** If you set α = 0.05 for one test, you have a 95% chance of being right. If you run three tests on the same data, your chance of not making a Type I error drops to (0.95 × 0.95 × 0.95) = 0.857. This means your actual error rate has skyrocketed from 5% to 14.3%! 
*   **The Solution:** A One-Way ANOVA tests all three groups simultaneously in a single mathematical operation, holding the overall Type I error rate strictly at the designated 5%.

**Conclusion:**
Parametric tests like t-tests and ANOVA form the backbone of quantitative marketing research. However, researchers must ensure the underlying assumptions of these tests (interval/ratio data, normal distribution, homogeneity of variance) are met before relying on their output.
