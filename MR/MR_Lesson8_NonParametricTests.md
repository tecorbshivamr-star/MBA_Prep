# 📉 LESSON 8: NON-PARAMETRIC TESTS
### MBA Marketing Research | Exam Revision Notes

---

> [!IMPORTANT]
> **Top Exam Topics:** Chi-Square test (most important!), When to use which non-parametric test, Parametric vs Non-Parametric comparison. Learn the "WHEN TO USE" for each test — examiners love this!

---

## 🎯 LEARNING OBJECTIVES

After this chapter, you should be able to:
- Understand when to use **Non-Parametric Tests** vs Parametric Tests
- Conduct and interpret the **Chi-Square Test** (goodness of fit + independence)
- Apply the **Sign Test** for paired data
- Use the **Mann-Whitney U Test** for two independent groups
- Apply the **Wilcoxon Signed-Rank Test** for paired data
- Use the **Kruskal-Wallis Test** for three or more groups

---

## 1. 📖 INTRODUCTION — WHY NON-PARAMETRIC TESTS?

### What are Non-Parametric Tests?

> **Definition:** Non-Parametric (or Distribution-Free) tests are statistical tests that make **NO assumption about the population distribution** (especially normality).

### When to Use Non-Parametric Tests:

> **Mnemonic: "SONS"**
> - **S**mall sample size (n < 30)
> - **O**rdinal or Nominal data (not interval/ratio)
> - **N**on-normal distribution (skewed data)
> - **S**uspect outliers distorting results

---

### Parametric vs Non-Parametric — Master Comparison:

| Feature | Parametric | Non-Parametric |
|---------|-----------|----------------|
| **Distribution assumption** | Normal distribution required | None (distribution-free) |
| **Data type** | Interval / Ratio | Nominal / Ordinal (any) |
| **Sample size** | Usually large (n ≥ 30) | Small samples OK |
| **Statistical power** | Higher (preferred if assumptions met) | Lower |
| **Examples** | z-test, t-test, ANOVA | Chi-square, Mann-Whitney, Kruskal-Wallis |
| **Measures** | Mean, SD | Median, Ranks |

---

### Non-Parametric Test Selection Map:

```
How many groups?
│
├── ONE group
│   ├── Comparing to expected distribution → Chi-Square Goodness of Fit
│   └── Paired before-after (small n) → Sign Test OR Wilcoxon Signed-Rank
│
├── TWO groups
│   ├── Independent samples → Mann-Whitney U Test
│   └── Paired/Related samples → Sign Test or Wilcoxon Signed-Rank Test
│
└── THREE or MORE groups
    └── Independent samples → Kruskal-Wallis Test
```

> **Mnemonic: "CSMWK"** — *"Can Students Master Work-hard Knowledge?"*
> - **C**hi-Square
> - **S**ign Test
> - **M**ann-Whitney U
> - **W**ilcoxon Signed-Rank
> - **K**ruskal-Wallis

---

## 2. 📊 CHI-SQUARE TEST (χ²) ← MOST IMPORTANT!

> **Definition:** A non-parametric test used to examine relationships between **categorical variables** or to test if observed frequencies match expected frequencies.

### Two Applications:

| Type | Tests | Example |
|------|-------|---------|
| **Chi-Square Goodness of Fit** | Does observed distribution match expected? | Is brand preference equally distributed? |
| **Chi-Square Test of Independence** | Are two categorical variables related? | Is gender related to brand preference? |

---

### A. Chi-Square Goodness of Fit Test

**Use when:** Testing if one categorical variable follows an expected distribution

**Hypotheses:**
- H₀: Observed frequencies = Expected frequencies (no significant difference)
- H₁: Observed ≠ Expected (significant difference exists)

**Formula:**
```
χ² = Σ [(O - E)² / E]

Where:
O = Observed frequency
E = Expected frequency
df = k - 1 (k = number of categories)
```

**Worked Example:**
> A researcher wants to test if 4 cola brands are equally preferred.
> 200 people surveyed. Expected if equal = 200/4 = 50 each.

| Brand | Observed (O) | Expected (E) | (O-E)² / E |
|-------|-------------|-------------|------------|
| Pepsi | 70 | 50 | 8.0 |
| Coke | 60 | 50 | 2.0 |
| Thums Up | 50 | 50 | 0.0 |
| Sprite | 20 | 50 | 18.0 |
| **Total** | **200** | **200** | **χ²=28.0** |

- df = 4 - 1 = **3**
- χ²_critical (df=3, α=0.05) = **7.815**
- χ² = 28.0 > 7.815 → **REJECT H₀**
- **Conclusion:** Brand preferences are NOT equally distributed.

---

### B. Chi-Square Test of Independence

**Use when:** Testing association/relationship between TWO categorical variables

**Hypotheses:**
- H₀: Variable A and Variable B are INDEPENDENT (no relationship)
- H₁: Variable A and Variable B are DEPENDENT (relationship exists)

**Formula:**
```
χ² = Σ [(O - E)² / E]

Expected frequency for each cell:
E = (Row Total × Column Total) / Grand Total

df = (r - 1)(c - 1)
Where r = rows, c = columns
```

**Worked Example:**
> Test if Gender is related to Cola Preference at α=0.05

**Observed Table:**
| | Pepsi | Coke | Total |
|-|-------|------|-------|
| **Male** | 80 | 40 | 120 |
| **Female** | 30 | 50 | 80 |
| **Total** | 110 | 90 | 200 |

**Expected Frequencies:**
- E(Male, Pepsi) = (120 × 110) / 200 = **66**
- E(Male, Coke) = (120 × 90) / 200 = **54**
- E(Female, Pepsi) = (80 × 110) / 200 = **44**
- E(Female, Coke) = (80 × 90) / 200 = **36**

**Chi-Square Calculation:**
```
χ² = (80-66)²/66 + (40-54)²/54 + (30-44)²/44 + (50-36)²/36
χ² = 2.97 + 3.63 + 4.45 + 5.44
χ² = 16.49
```

- df = (2-1)(2-1) = **1**
- χ²_critical (df=1, α=0.05) = **3.841**
- χ² = 16.49 > 3.841 → **REJECT H₀**
- **Conclusion:** Gender and Cola Preference are significantly related (NOT independent)

### Assumptions of Chi-Square:
1. Data is **categorical** (nominal/ordinal)
2. Observations are **independent**
3. Expected frequency in each cell ≥ **5** (if not, merge categories)
4. Sample size should be **adequate**

### Chi-Square Critical Values (Common):
| df | α = 0.05 | α = 0.01 |
|----|---------|---------|
| 1 | 3.841 | 6.635 |
| 2 | 5.991 | 9.210 |
| 3 | 7.815 | 11.345 |
| 4 | 9.488 | 13.277 |

---

## 3. ✅ SIGN TEST

> **Definition:** The simplest non-parametric test for **paired data** — only uses the **DIRECTION (sign)** of differences (+/-), ignoring magnitude.

### When to Use:
- Two **related/paired samples** (before-after measurements)
- Ordinal data or small sample
- Non-normal distribution
- **Non-parametric alternative to Paired t-test**

### How It Works:
1. Calculate difference: D = After - Before for each pair
2. Record only the **SIGN** (+, -, or 0)
3. Ignore zero differences (tied pairs)
4. Count: n₊ (positives), n₋ (negatives)
5. Test statistic = smaller of n₊ or n₋

**Hypotheses:**
- H₀: P(+) = P(-) = 0.5 (no systematic difference)
- H₁: P(+) ≠ P(-) (systematic difference exists)

**Decision Rule (Small Sample):**
- Compare smaller count to **Sign Test Critical Table**
- If test statistic ≤ critical value → Reject H₀

**Worked Example:**
> Test if training improved employee scores (n=10 pairs):

| Employee | Before | After | Sign |
|----------|--------|-------|------|
| 1 | 60 | 75 | + |
| 2 | 55 | 50 | − |
| 3 | 70 | 80 | + |
| 4 | 65 | 65 | 0 (ignore) |
| 5 | 50 | 70 | + |
| 6 | 72 | 78 | + |
| 7 | 68 | 65 | − |
| 8 | 58 | 72 | + |
| 9 | 62 | 80 | + |
| 10 | 74 | 70 | − |

- n₊ = 6, n₋ = 3 (ignore the 0)
- n = 9 (effective pairs), test stat = min(6,3) = **3**
- At α=0.05, critical value for n=9 = **1** (from Sign test table)
- 3 > 1 → **Fail to Reject H₀**

**Limitation:** Sign test **wastes information** — ignores HOW MUCH things changed. Wilcoxon signed-rank test is more powerful.

---

## 4. 🔵 MANN-WHITNEY U TEST

> **Definition:** A non-parametric test to compare **two independent groups** — tests whether one group's values tend to be higher/lower than the other.

### When to Use:
- Two **independent samples**
- Ordinal data OR non-normal distributions
- **Non-parametric alternative to Independent Samples t-test**

### How It Works:
1. **Combine** both samples and **rank all values** together (1 = smallest)
2. **Sum the ranks** for each group (R₁ and R₂)
3. Calculate U statistics:

**Formula:**
```
U₁ = n₁n₂ + [n₁(n₁+1)/2] - R₁
U₂ = n₁n₂ + [n₂(n₂+1)/2] - R₂

Check: U₁ + U₂ = n₁ × n₂

Test Statistic = Minimum of U₁ and U₂
```

**Hypotheses:**
- H₀: The two populations have the same distribution (medians are equal)
- H₁: The populations differ (one tends to have higher values)

**Decision:** Compare U_min to **Mann-Whitney critical value table**
- If U_calculated ≤ U_critical → Reject H₀

**Worked Example (Small n):**
> Compare satisfaction scores: Group A (n₁=4): {7, 5, 9, 3} and Group B (n₂=4): {6, 8, 4, 10}

**Combined Ranking:**
| Value | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|-------|---|---|---|---|---|---|---|----|
| Rank | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
| Group | A | B | A | B | A | B | A | B |

- R₁ (Group A ranks) = 1+3+5+7 = **16**
- R₂ (Group B ranks) = 2+4+6+8 = **20**

```
U₁ = 4×4 + [4×5/2] - 16 = 16 + 10 - 16 = 10
U₂ = 4×4 + [4×5/2] - 20 = 16 + 10 - 20 = 6
U_min = 6
```

- U_critical (n₁=4, n₂=4, α=0.05, two-tailed) = **2**
- U = 6 > 2 → **Fail to Reject H₀**
- No significant difference between groups.

### For Large Samples (n > 20):
> Convert U to z-score:
```
z = [U - (n₁n₂/2)] / √[n₁n₂(n₁+n₂+1)/12]
```
Then use standard z-table for decision.

---

## 5. 🟡 WILCOXON SIGNED-RANK TEST

> **Definition:** A non-parametric test for **paired/related samples** that uses **both the sign AND the magnitude (rank)** of differences — more powerful than the Sign Test.

### When to Use:
- Two **related/paired samples** (same subjects, before-after)
- Ordinal or non-normal data
- **Non-parametric alternative to Paired t-test** (MORE POWERFUL than Sign Test)

### How It Works:
1. Calculate **D = After - Before** for each pair
2. **Ignore D = 0** (ties)
3. **Rank the ABSOLUTE values** of differences |D| (smallest = rank 1)
4. Assign signs (+/-) back to ranks
5. Calculate **W₊** (sum of positive ranks) and **W₋** (sum of negative ranks)
6. Test statistic **T = Minimum of W₊ and W₋**

**Decision:** Compare T to Wilcoxon critical value table
- If T ≤ T_critical → Reject H₀

**Worked Example:**
> 7 employees trained. Before/After scores:

| Emp | Before | After | D | |D| | Rank | Signed Rank |
|-----|--------|-------|---|-----|------|-------------|
| 1 | 60 | 72 | +12 | 12 | 5 | +5 |
| 2 | 55 | 50 | −5 | 5 | 2 | −2 |
| 3 | 70 | 85 | +15 | 15 | 7 | +7 |
| 4 | 65 | 72 | +7 | 7 | 3 | +3 |
| 5 | 50 | 40 | −10 | 10 | 4 | −4 |
| 6 | 72 | 85 | +13 | 13 | 6 | +6 |
| 7 | 68 | 69 | +1 | 1 | 1 | +1 |

- **W₊** = 5+7+3+6+1 = **22**
- **W₋** = 2+4 = **6**
- **T = min(22, 6) = 6**
- T_critical (n=7, α=0.05, two-tailed) = **2**
- T = 6 > 2 → **Fail to Reject H₀** at 5% (just barely)

### Sign Test vs Wilcoxon:

| Feature | Sign Test | Wilcoxon Signed-Rank |
|---------|-----------|---------------------|
| Uses | Only +/- direction | Direction AND magnitude |
| Power | Lower | Higher (more sensitive) |
| Data | Any paired data | Interval-level differences needed |
| Complexity | Very simple | Moderate |
| When preferred | Quick/simple check | More accurate conclusion |

---

## 6. 🔴 KRUSKAL-WALLIS TEST

> **Definition:** A non-parametric test to compare **THREE or more independent groups** — tests if at least one group has a different distribution/median.

### When to Use:
- **3 or more independent groups**
- Ordinal data or non-normal distributions
- **Non-parametric alternative to One-Way ANOVA**

### How It Works:
1. **Combine** all groups and **rank all values** together
2. **Sum ranks** for each group (R₁, R₂, R₃...)
3. Calculate **H-statistic**:

**Formula:**
```
         12            Rᵢ²
H = ─────────── × Σ ──────  −  3(N+1)
      N(N+1)          nᵢ

Where:
N = Total sample size (all groups combined)
nᵢ = Sample size of group i
Rᵢ = Sum of ranks for group i
```

**Hypotheses:**
- H₀: All groups have the same distribution/median
- H₁: At least one group has a different distribution

**Decision:** Compare H to **Chi-Square critical value** with df = k-1
- If H > χ²_critical → Reject H₀

**Worked Example:**
> Compare customer satisfaction across 3 stores (n=3 each):
- Store A: {8, 6, 4}
- Store B: {7, 9, 5}
- Store C: {3, 2, 1}

**All values ranked (N=9):**
| Value | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|-------|---|---|---|---|---|---|---|---|---|
| Rank | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
| Group | C | C | C | A | B | A | B | A | B |

- R_A = 4+6+8 = **18**
- R_B = 5+7+9 = **21**
- R_C = 1+2+3 = **6**

```
H = [12/(9×10)] × [(18²/3) + (21²/3) + (6²/3)] − 3(10)
H = [12/90] × [108 + 147 + 12] − 30
H = 0.1333 × 267 − 30
H = 35.6 − 30
H = 5.6
```

- df = k-1 = 3-1 = **2**
- χ²_critical (df=2, α=0.05) = **5.991**
- H = 5.6 < 5.991 → **Fail to Reject H₀** (barely)

> [!TIP]
> **Key fact:** Kruskal-Wallis uses the **Chi-Square distribution** for its critical values (df = k-1). This is commonly asked!

---

## 7. 🔗 ALL TESTS — MEGA COMPARISON TABLE

| Test | Parametric Equivalent | Groups | Sample Type | Data | Test Stat |
|------|--------------------|--------|------------|------|-----------|
| **Chi-Square** | — | Any | Independent | Nominal | χ² |
| **Sign Test** | Paired t-test | 2 | Paired/Related | Any | Smaller of n₊/n₋ |
| **Mann-Whitney U** | Independent t-test | 2 | Independent | Ordinal+ | U |
| **Wilcoxon Signed-Rank** | Paired t-test | 2 | Paired/Related | Ordinal+ | T (min of W₊/W₋) |
| **Kruskal-Wallis** | One-Way ANOVA | 3+ | Independent | Ordinal+ | H (uses χ² dist.) |

---

## 8. ⚡ ADVANTAGES & DISADVANTAGES OF NON-PARAMETRIC TESTS

### Advantages:
> **Mnemonic: "SNORE"**
> - **S**mall samples work fine
> - **N**o normality assumption needed
> - **O**rdinal/Nominal data usable
> - **R**obust to outliers
> - **E**asy to compute (ranking-based)

### Disadvantages:
> **Mnemonic: "WILD"**
> - **W**eaker statistical power (than parametric)
> - **I**gnores data precision (uses ranks not values)
> - **L**ess efficient — needs larger sample for same power as parametric
> - **D**ifficult to handle ties in rankings

---

## 🧠 MASTER MNEMONIC SHEET — LESSON 8

| Topic | Mnemonic | Full Form |
|-------|----------|-----------|
| All 5 Non-Parametric Tests | **CSMWK** | Chi-Square, Sign, Mann-Whitney, Wilcoxon, Kruskal-Wallis |
| When to use non-parametric | **SONS** | Small sample, Ordinal data, Non-normal, Suspect outliers |
| Chi-Square Formula | **O & E** | χ² = Σ(O-E)²/E |
| Advantages | **SNORE** | Small, No normality, Ordinal OK, Robust, Easy |
| Disadvantages | **WILD** | Weaker, Ignores precision, Less efficient, Difficult ties |
| Test stat rule | **"Minimum Wins"** | Sign Test, Mann-Whitney, Wilcoxon all use MINIMUM value |

---

## ⚡ QUICK REVISION FLASHCARDS

**Q: What is the non-parametric alternative to independent t-test?**
A: **Mann-Whitney U Test**

**Q: What is the non-parametric alternative to One-Way ANOVA?**
A: **Kruskal-Wallis Test** — uses Chi-Square distribution for critical value

**Q: What is the non-parametric alternative to Paired t-test?**
A: **Wilcoxon Signed-Rank Test** (more powerful) or **Sign Test** (simpler)

**Q: Chi-Square test of independence df formula?**
A: df = (r-1)(c-1) where r=rows, c=columns

**Q: Chi-Square goodness of fit df?**
A: df = k-1 (k = number of categories)

**Q: Minimum expected frequency in Chi-Square?**
A: Each cell must have E ≥ **5**; otherwise merge categories

**Q: Sign Test — what does it ignore?**
A: The **magnitude** (size) of differences — only uses direction (+/-)

**Q: What distribution does Kruskal-Wallis use for critical value?**
A: **Chi-Square distribution** with df = k-1

**Q: Mann-Whitney U check formula?**
A: U₁ + U₂ = n₁ × n₂ (use this to verify your calculation!)

**Q: When to prefer Wilcoxon over Sign Test?**
A: When differences have meaningful magnitude (interval-like) — Wilcoxon is more powerful

---

## 📌 EXAM PATTERN LIKELY QUESTIONS

| Type | Question |
|------|---------|
| **Numerical** | Conduct a Chi-Square test of independence from a 2×2 contingency table |
| **Numerical** | Given paired data, perform Sign Test or Wilcoxon Signed-Rank Test |
| **Long** | Explain Chi-Square test — both goodness of fit and independence |
| **Short** | What is the Mann-Whitney U Test? When is it used? |
| **Short** | Distinguish between Wilcoxon Signed-Rank Test and Sign Test |
| **Short** | What is the Kruskal-Wallis Test? How does it relate to ANOVA? |
| **Short** | What are the advantages and disadvantages of non-parametric tests? |
| **Compare** | Tabulate non-parametric tests and their parametric equivalents |
| **Definition** | Define: Distribution-free test, Null hypothesis, Ranks |
| **Short** | What assumptions must be met for Chi-Square test? |

---

### 📐 FORMULA CHEAT SHEET — LESSON 8

| Test | Key Formula | df / Decision |
|------|------------|--------------|
| **Chi-Square** | χ² = Σ(O-E)²/E | df=(r-1)(c-1) or k-1; Reject if χ²_calc > χ²_critical |
| **Expected Cell Freq** | E = (Row Total × Col Total) / Grand Total | Each E must be ≥ 5 |
| **Mann-Whitney U₁** | U₁ = n₁n₂ + n₁(n₁+1)/2 − R₁ | Reject if U_min ≤ U_critical |
| **Kruskal-Wallis H** | H = [12/N(N+1)] × Σ(Rᵢ²/nᵢ) − 3(N+1) | df=k-1; Compare to χ²_critical |
| **Wilcoxon T** | T = min(W₊, W₋) | Reject if T ≤ T_critical |

---

> [!NOTE]
> **Bhai, Lesson 8 ke Top 3 Must-Know:**
> 1. **Chi-Square** — ye sabse zyada important hai — formula, df, expected frequency ≥5 condition aur ek worked example toh zaroor practice kar
> 2. **CSMWK table** — 5 tests ke parametric equivalents yaad rakh — "Mann-Whitney = t-test substitute, Kruskal-Wallis = ANOVA substitute"
> 3. **"Minimum Wins"** rule — Sign test, Mann-Whitney aur Wilcoxon teeno mein test statistic = **minimum value** — ek trick sabke liye!
>
> **8 chapters done! 🔥 Almost complete! Kuch aur chapters hain toh bhej de bhai!** 💪

