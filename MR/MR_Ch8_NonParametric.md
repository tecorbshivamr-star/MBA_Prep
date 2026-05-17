# 📗 MR CHAPTER 8: Non-Parametric Tests
### Subject: Marketing Research | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

In Chapter 7, we used **Parametric Tests** (like t-tests and ANOVA). These are very powerful, but they have strict rules. The data *must* be high quality (Interval/Ratio numbers like Sales in ₹), and it *must* follow a perfect bell-curve shape (Normal Distribution).

But what if you do a survey and just ask people for their Gender (Male/Female) and their favorite Color (Red/Blue)? You can't calculate the "average" of Male and Female! The data is just categories.

When the strict mathematical rules are broken, you cannot use Parametric tests. You must switch to **Non-Parametric Tests**. They are less powerful, but they work on any type of messy, categorical, or ranked data.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. When to use Non-Parametric Tests?
- When your data is **Nominal** (Categories: Male/Female, Delhi/Mumbai) or **Ordinal** (Ranks: 1st, 2nd, 3rd).
- When your sample size is extremely small (e.g., n = 10).
- When your data does not form a normal bell curve (e.g., it is heavily skewed).

### 2. The Chi-Square Test (χ²)
This is the most famous non-parametric test. It checks if two categorical variables are connected.
- *Example:* Is there a connection between Gender (Male/Female) and choosing to buy a Sports Car (Yes/No)?
- It compares the **Observed** numbers (what actually happened in your survey) against the **Expected** numbers (what should have happened if gender had absolutely zero effect on buying a sports car). 

### 3. Alternative Tests Matchup
If you break the rules of a parametric test, you use its non-parametric twin:
- Instead of an Independent t-test → Use **Mann-Whitney U Test**
- Instead of a Paired t-test → Use **Wilcoxon Signed Rank Test**
- Instead of One-Way ANOVA → Use **Kruskal-Wallis Test**

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. What are Non-Parametric tests? In what situations are they preferred over Parametric tests? Explain the application of the Chi-Square test of independence. (15 Marks)

**1. Definition of Non-Parametric Tests:**
Non-parametric tests (often called "distribution-free" tests) are statistical procedures that do not rely on the restrictive assumptions required by parametric tests. Specifically, they do not assume that the data is drawn from a normally distributed population, nor do they require the data to be measured at the interval or ratio level.

**2. Situations Preferred Over Parametric Tests:**
A researcher should actively choose a non-parametric test under the following conditions:
*   **Measurement Level:** The data collected is only nominal (categorical labels like brand names) or ordinal (rankings). Parametric tests cannot compute the mean of categorical data.
*   **Violation of Assumptions:** The population data is heavily skewed or contains extreme outliers, severely violating the assumption of normality required by t-tests or ANOVA.
*   **Small Sample Size:** The sample size is too small (e.g., n < 30) to rely on the Central Limit Theorem to assume a normal distribution.
*   **Simplicity:** They are generally easier to compute manually and simpler to explain to non-technical management.

**3. The Chi-Square (χ²) Test of Independence:**
The Chi-Square test is arguably the most widely used non-parametric test in marketing research. It is used exclusively for cross-tabulated nominal data to determine if there is a statistically significant association (dependence) between two categorical variables.

*   **Application Example:** A marketer wants to know if a consumer's geographic region (North, South, East, West) influences their preference for three different coffee brands (Brand A, B, C). Both variables are nominal.
*   **The Hypotheses:**
    *   *Null Hypothesis (H₀):* There is NO association between Region and Brand Preference (they are independent).
    *   *Alternative Hypothesis (H₁):* There IS an association between Region and Brand Preference.
*   **The Methodology:**
    1.  The researcher creates a contingency table (cross-tabulation) recording the *Observed Frequencies* (O) from the survey data.
    2.  The researcher calculates the *Expected Frequencies* (E) for each cell — which is the mathematical probability of what the cell should look like if H₀ were absolutely true.
    3.  The formula $\chi^2 = \sum \frac{(O - E)^2}{E}$ is applied. 
    4.  If the difference between what was Observed and what was Expected is massively large, the resulting $\chi^2$ value will exceed the critical table value, leading the researcher to reject the Null Hypothesis and conclude that region strongly influences coffee preference.

**Conclusion:**
While non-parametric tests lack the deep statistical power of their parametric counterparts (meaning they are slightly less likely to detect a subtle difference if one genuinely exists), they are essential, robust tools that save researchers when dealing with real-world, non-ideal data.
