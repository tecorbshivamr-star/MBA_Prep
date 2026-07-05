# 📊 LESSON 7: PARAMETRIC HYPOTHESIS TESTING & ANOVA
### MBA Marketing Research | Exam Revision Notes

---

> [!IMPORTANT]
> **Top Exam Topics:** Steps in Hypothesis Testing, z-test vs t-test (when to use which!), ANOVA logic and F-test. Expect BOTH theory questions AND numerical problems in the exam!

---

## 🎯 LEARNING OBJECTIVES

After this chapter, you should be able to:
- Understand **Inferential Statistics** and its role in MR
- Define and classify **Hypotheses** (H₀ and H₁)
- Follow the **step-by-step hypothesis testing procedure**
- Conduct **z-test** (σ known) and **t-test** (σ unknown)
- Test for **difference between two means**
- Understand **ANOVA** logic and the **F-test**

---

## 1. 📖 INFERENTIAL DATA ANALYSIS

### What is Inferential Statistics?

> **Definition:** Inferential Statistics uses **sample data to make inferences (conclusions) about the population** using probability theory.

```
Sample Data
    ↓
Statistical Test
    ↓
Inference about POPULATION
```

### Two Branches of Statistics:

| | Descriptive Statistics | Inferential Statistics |
|--|----------------------|----------------------|
| **Purpose** | Summarize/describe data | Draw conclusions about population |
| **Tools** | Mean, Median, SD, Tables, Charts | Hypothesis tests, Confidence intervals |
| **Scope** | Only the sample | Beyond the sample → population |
| **Example** | "Average age in sample = 28 yrs" | "Population average age is likely 25-31 yrs" |

### Parametric vs Non-Parametric Tests:

| Feature | Parametric Tests | Non-Parametric Tests |
|---------|-----------------|---------------------|
| **Assumption** | Data is normally distributed | No distribution assumption |
| **Data type** | Interval or Ratio | Nominal or Ordinal |
| **Examples** | z-test, t-test, ANOVA, F-test | Chi-Square, Mann-Whitney, Kruskal-Wallis |
| **Power** | More powerful (preferred) | Less powerful |
| **Sample size** | Usually larger | Can use small samples |

> **This chapter = PARAMETRIC tests** (assumes normal distribution, interval/ratio data)

---

## 2. 💡 HYPOTHESIS — CHARACTERISTICS & TYPES

### What is a Hypothesis?

> **Definition:** A **hypothesis** is a tentative statement or assumption about a population parameter that is to be **tested using sample data**.

### Characteristics of a Good Hypothesis:

> **Mnemonic: "SCAT-C"**
> - **S**imple — Clear and concise statement
> - **C**lear — Unambiguous; one interpretation only
> - **A**ccurate — Based on sound reasoning
> - **T**estable — Can be empirically verified
> - **C**oncise — Brief, not wordy

---

### THE TWO HYPOTHESES:

#### H₀ — Null Hypothesis
> The hypothesis of **NO effect, NO difference, NO relationship** — the "status quo" assumed to be true unless evidence proves otherwise

- Always contains: **=, ≤, ≥** (equality)
- Example: H₀: μ = 50 (population mean equals 50)
- We **never accept** H₀ — we either **reject** or **fail to reject** it

#### H₁ — Alternative Hypothesis (Research Hypothesis)
> The hypothesis the researcher **wants to prove** — the opposite of H₀

- Always contains: **≠, >, <** (inequality)
- Example: H₁: μ ≠ 50 (population mean is NOT 50)

---

### TYPES OF HYPOTHESIS TESTS (by direction):

| Test Type | H₀ | H₁ | Rejection Region |
|-----------|----|----|-----------------|
| **Two-tailed** | μ = μ₀ | μ ≠ μ₀ | Both tails (÷ α by 2) |
| **Right-tailed** | μ ≤ μ₀ | μ > μ₀ | Right tail only |
| **Left-tailed** | μ ≥ μ₀ | μ < μ₀ | Left tail only |

```
Two-Tailed:           Left-Tailed:         Right-Tailed:
  Reject | Accept | Reject   Reject | Accept      Accept | Reject
    ←α/2          α/2→        ←α                         α→
```

> **Mnemonic: "Two tails = Two critical values; One tail = One critical value"**

---

### Types of Errors in Hypothesis Testing:

| | H₀ is TRUE | H₀ is FALSE |
|--|------------|------------|
| **Reject H₀** | ❌ **Type I Error (α)** | ✅ Correct (Power) |
| **Fail to Reject H₀** | ✅ Correct | ❌ **Type II Error (β)** |

> **Mnemonic: "Type I = False Alarm; Type II = Missed Detection"**
> - **Type I (α):** Convict an innocent person (reject true H₀) → "Cry wolf"
> - **Type II (β):** Let a criminal go free (fail to reject false H₀) → "Miss the wolf"

**Significance Level (α):** Probability of making Type I error
- Typically set at **α = 0.05** (5%) or α = 0.01 (1%)
- **p-value < α → Reject H₀**

---

## 3. 🔄 STEPS IN HYPOTHESIS TESTING

> [!IMPORTANT]
> Learn these steps cold — every hypothesis testing answer starts here!

> **Mnemonic: "SHARC-DC"**
> - **S**tate the hypotheses (H₀ and H₁)
> - **H**ypothesis test selection (which test? z or t?)
> - **A**lpha level (significance level — 0.05 or 0.01?)
> - **R**ule of decision (critical value or p-value approach)
> - **C**alculate test statistic
> - **D**ecide — Reject or Fail to Reject H₀
> - **C**onclude in plain language

---

### Step 1: State H₀ and H₁
- Clearly define both hypotheses in terms of **population parameters**
- Example: H₀: μ = 500 vs H₁: μ ≠ 500

### Step 2: Select the Appropriate Test
- z-test or t-test? (see decision tree below)
- One-sample, two-sample, or ANOVA?

### Step 3: Set Significance Level (α)
- Usually α = 0.05 → 5% risk of Type I error
- Sets the critical value

### Step 4: Establish Decision Rule
**Critical Value Approach:**
```
Reject H₀ if |calculated statistic| > critical value
```
**p-value Approach:**
```
Reject H₀ if p-value < α
```

### Step 5: Calculate the Test Statistic
- Apply the formula using sample data

### Step 6: Make the Decision
- Compare calculated value to critical value
- OR compare p-value to α

### Step 7: State the Conclusion
- In non-statistical language for management
- Example: "There is sufficient evidence that the average customer satisfaction score differs from 500"

---

## 4. 🔵 Z-TEST: Testing Hypothesis about Population Mean (σ Known)

### When to Use Z-Test?
> Use z-test when:
> 1. **Population standard deviation (σ) is KNOWN**, AND
> 2. **Sample size n ≥ 30** (large sample), OR population is normally distributed

### Z-Test Formula:

> **Formula:**
> ```
>        x̄ - μ₀
> z = ──────────
>       σ / √n
> ```
> Where:
> - **x̄** = sample mean
> - **μ₀** = hypothesized population mean (from H₀)
> - **σ** = population standard deviation (known)
> - **n** = sample size

### Critical Values for Z-Test:

| Significance Level (α) | Two-Tailed | Right-Tailed | Left-Tailed |
|-----------------------|------------|-------------|------------|
| **0.05** | ±1.96 | +1.645 | -1.645 |
| **0.01** | ±2.576 | +2.326 | -2.326 |

---

### 📝 WORKED EXAMPLE — Z-TEST:

> **Problem:** A company claims its delivery time is 30 minutes (μ₀ = 30). A researcher samples 100 deliveries (n=100) and finds mean = 32 minutes (x̄ = 32). Population SD is known to be 10 minutes (σ = 10). Test at α = 0.05.

**Step 1:** H₀: μ = 30 vs H₁: μ ≠ 30 (two-tailed)

**Step 2:** Use z-test (σ known, n=100 > 30)

**Step 3:** α = 0.05

**Step 4:** Decision Rule: Reject H₀ if |z| > 1.96

**Step 5:** Calculate:
```
z = (32 - 30) / (10 / √100)
z = 2 / (10/10)
z = 2 / 1
z = 2.0
```

**Step 6:** |z| = 2.0 > 1.96 → **REJECT H₀**

**Step 7:** Conclusion: "There is sufficient evidence at 5% significance level that the average delivery time is NOT 30 minutes. It appears to be significantly higher."

---

## 5. 🟡 T-TEST: Testing Hypothesis about Population Mean (σ Unknown)

### When to Use T-Test?
> Use t-test when:
> 1. **Population standard deviation (σ) is UNKNOWN** (must use sample SD = s), AND
> 2. **Small sample (n < 30)** OR when σ is unknown regardless of size

### T-Test Formula:

> **Formula:**
> ```
>        x̄ - μ₀
> t = ──────────
>       s / √n
> ```
> Where:
> - **x̄** = sample mean
> - **μ₀** = hypothesized mean
> - **s** = sample standard deviation (NOT σ!)
> - **n** = sample size
> - **Degrees of Freedom (df) = n - 1**

### Key Concept — Degrees of Freedom (df):
> df = n - 1
> The t-distribution changes shape based on df — with more df, it approaches the normal distribution

### t-distribution vs z-distribution:
```
Both are bell-shaped and symmetric around 0
BUT t-distribution has HEAVIER TAILS (more uncertainty because σ unknown)
As n → ∞ (df → ∞), t-distribution → z-distribution
```

---

### 📝 WORKED EXAMPLE — T-TEST:

> **Problem:** A brand claims its energy drink improves focus scores by 75 points (μ₀ = 75). A researcher tests 16 people (n=16) and finds x̄ = 78, s = 8. Population SD unknown. Test at α = 0.05.

**Step 1:** H₀: μ = 75 vs H₁: μ ≠ 75 (two-tailed)

**Step 2:** Use t-test (σ unknown, n=16 < 30)

**Step 3:** α = 0.05, df = 16 - 1 = 15

**Step 4:** Critical value: t(0.05, 15, two-tailed) = **±2.131** (from t-table)

**Step 5:** Calculate:
```
t = (78 - 75) / (8 / √16)
t = 3 / (8/4)
t = 3 / 2
t = 1.5
```

**Step 6:** |t| = 1.5 < 2.131 → **FAIL TO REJECT H₀**

**Step 7:** Conclusion: "Insufficient evidence that the energy drink changes focus scores significantly from 75 points."

---

### Z-TEST vs T-TEST — Quick Decision Guide:

```
Is σ (population SD) KNOWN?
        ↓ YES                ↓ NO
    Use Z-TEST           Is n ≥ 30?
                    YES ↓         ↓ NO
              Can use Z        Use T-TEST
              (CLT applies)   (must use T)
```

| Feature | Z-Test | T-Test |
|---------|--------|--------|
| **σ** | Known | Unknown (use s) |
| **Sample Size** | Usually n ≥ 30 | Any size (especially n < 30) |
| **Distribution** | Standard Normal (Z) | t-distribution |
| **df needed?** | No | Yes — df = n-1 |
| **More common in?** | Theory problems | Real-world research |

---

## 6. 🔴 TESTING HYPOTHESIS FOR DIFFERENCE OF MEANS

> Used when comparing **two groups** — e.g., Do men and women differ in purchase frequency?

### Case 1: Independent Samples (Two different groups)

**Hypotheses:**
- H₀: μ₁ = μ₂ (no difference between groups)
- H₁: μ₁ ≠ μ₂ (groups differ)

**Formula (when σ unknown — pooled t-test):**
```
        (x̄₁ - x̄₂) - (μ₁ - μ₂)₀
t = ────────────────────────────────
      Sp × √(1/n₁ + 1/n₂)

Where pooled SD:
       (n₁-1)s₁² + (n₂-1)s₂²
Sp² = ──────────────────────────
            n₁ + n₂ - 2

df = n₁ + n₂ - 2
```

**Example Setup:**
> Test if male (n₁=50, x̄₁=₹5,000) and female (n₂=50, x̄₂=₹4,500) customers differ in average monthly spending.
> H₀: μM = μF → H₁: μM ≠ μF

### Case 2: Paired/Dependent Samples (Same group, before-after)

**When to use:** Same respondents measured TWICE (pre-test / post-test)

**Formula:**
```
     d̄ - μd
t = ────────
     sd/√n

Where:
d = difference for each pair (After - Before)
d̄ = mean of all differences
sd = SD of differences
df = n - 1
```

**Example:**
> 20 students took a training course. Test if their scores improved (before vs after training).
> d = score_after - score_before for each student

---

## 7. 🔬 ANALYSIS OF VARIANCE (ANOVA)

### What is ANOVA?

> **ANOVA (Analysis of Variance)** tests whether there are **statistically significant differences among the means of THREE OR MORE groups**.

**Why not multiple t-tests?**
> If you have 3 groups (A, B, C) → you'd need 3 t-tests (A vs B, B vs C, A vs C).
> **Problem:** Each test has 5% error chance → cumulative error inflates rapidly!
> ANOVA tests ALL groups SIMULTANEOUSLY in ONE test.

### The Core Logic of ANOVA:

```
Total Variation in Data
         ↓
     Split into:
         ↓
Between-Group Variation    +    Within-Group Variation
(Due to TREATMENT/FACTOR)       (Due to RANDOM ERROR)
     (SSB)                              (SSW)
         ↓                               ↓
   If groups truly differ:           If groups are same:
   SSB >> SSW                        SSB ≈ SSW
   F ratio >> 1                      F ratio ≈ 1
```

---

### ANOVA Hypotheses:

- **H₀:** μ₁ = μ₂ = μ₃ = ... = μk (ALL group means are equal)
- **H₁:** At least ONE group mean is different from the others

> [!TIP]
> H₁ does NOT say which group differs — it just says "at least one is different." Post-hoc tests (Tukey, Bonferroni) then tell you WHICH ones differ.

---

### ANOVA Terminology:

| Term | Meaning |
|------|---------|
| **Factor** | The independent variable (grouping variable) |
| **Levels/Groups** | The categories of the factor (e.g., 3 ad types) |
| **SST** | Total Sum of Squares (total variation) |
| **SSB** | Sum of Squares Between groups (treatment variation) |
| **SSW/SSE** | Sum of Squares Within groups / Error (random variation) |
| **MSB** | Mean Square Between = SSB / (k-1) |
| **MSW** | Mean Square Within = SSW / (N-k) |
| **F-ratio** | MSB / MSW — the test statistic |

**Relationship:** SST = SSB + SSW

---

### The F-Ratio:

> **Formula:**
> ```
>         MSB          SSB / (k-1)
> F = ──────────  =  ──────────────
>         MSW          SSW / (N-k)
> ```
> Where:
> - **k** = number of groups
> - **N** = total sample size
> - **df₁** = k - 1 (numerator df)
> - **df₂** = N - k (denominator df)

**Decision Rule:** Reject H₀ if **F_calculated > F_critical** (from F-table)

---

### ANOVA Table (One-Way):

| Source | SS | df | MS | F |
|--------|----|----|----|----|
| Between Groups | SSB | k-1 | MSB = SSB/(k-1) | F = MSB/MSW |
| Within Groups (Error) | SSW | N-k | MSW = SSW/(N-k) | |
| **Total** | **SST** | **N-1** | | |

---

### 📝 WORKED EXAMPLE — ONE-WAY ANOVA:

> **Problem:** A marketing team tests THREE different advertisements (A, B, C) on brand recall scores. 5 people see each ad (N=15). Test if ads differ at α=0.05.

| Ad A | Ad B | Ad C |
|------|------|------|
| 70 | 85 | 60 |
| 75 | 80 | 65 |
| 65 | 90 | 70 |
| 72 | 88 | 62 |
| 68 | 87 | 63 |
| **x̄A=70** | **x̄B=86** | **x̄C=64** |

**Grand Mean:** x̄ = (70+86+64)/3 = **73.33**

**Step 1:** H₀: μA = μB = μC vs H₁: At least one mean differs
**Step 2:** One-Way ANOVA
**Step 3:** α = 0.05
**Step 4:** F_critical (df₁=2, df₂=12) = 3.89 (from F-table)

**Calculate SSB:**
```
SSB = n × Σ(x̄group - x̄grand)²
SSB = 5 × [(70-73.33)² + (86-73.33)² + (64-73.33)²]
SSB = 5 × [11.09 + 160.49 + 87.09]
SSB = 5 × 258.67 = 1293.33
```

**Calculate SSW** (variation within each group):
```
SSW = Σ(x - x̄group)²  for all observations
(Sum of squared deviations from their group mean)
SSW ≈ 143.6 (computed)
```

**ANOVA Table:**
| Source | SS | df | MS | F |
|--------|-----|-----|------|------|
| Between | 1293.33 | 2 | 646.67 | **54.08** |
| Within | 143.60 | 12 | 11.97 | |
| Total | 1436.93 | 14 | | |

**Step 6:** F = 54.08 > F_critical = 3.89 → **REJECT H₀**

**Step 7:** "There is significant evidence that the three advertisements produce different brand recall scores."

---

### Types of ANOVA:

| Type | Description | Example |
|------|------------|---------|
| **One-Way ANOVA** | ONE independent variable (factor), 3+ groups | Effect of 3 ad types on recall |
| **Two-Way ANOVA** | TWO independent variables, study main effects + interaction | Effect of ad type AND gender on recall |
| **Repeated Measures ANOVA** | Same subjects measured multiple times | Same people rated 3 ads across 3 weeks |
| **MANOVA** | Multiple dependent variables simultaneously | Ad type effect on recall AND purchase intent |

### Two-Way ANOVA — Additional Concept:

> Tests:
> 1. **Main Effect of Factor A** — Does Factor A (e.g., ad type) affect outcome?
> 2. **Main Effect of Factor B** — Does Factor B (e.g., gender) affect outcome?
> 3. **Interaction Effect (A×B)** — Does the effect of A depend on B? (and vice versa)

**Interaction Effect Example:**
> Ad type A works better for males, but Ad type B works better for females → This is an INTERACTION.

---

### Post-Hoc Tests (After ANOVA):

> When ANOVA rejects H₀, post-hoc tests tell you **WHICH specific groups differ:**

| Test | When Used |
|------|----------|
| **Tukey's HSD** | Equal sample sizes; most common |
| **Bonferroni** | Adjusts alpha for multiple comparisons |
| **Scheffe's test** | Most conservative; all comparisons |
| **LSD (Fisher's)** | Least strict; most liberal |

---

## 8. 🧪 DESIGN OF EXPERIMENTS (DOE)

> **Definition:** A structured approach to planning experiments to **test the effect of one or more independent variables** on a dependent variable.

### Key Components:

| Term | Meaning | Example |
|------|---------|---------|
| **Independent Variable (IV)** | The variable manipulated by researcher | Ad type (A, B, C) |
| **Dependent Variable (DV)** | The outcome being measured | Brand recall score |
| **Extraneous Variable** | Variables that must be controlled | Age, gender of viewers |
| **Treatment** | A specific level/combination of IVs | Showing Ad B |
| **Control Group** | Group that receives NO treatment | No ad shown |
| **Experimental Group** | Group that receives treatment | Group shown ad |

### Types of Experimental Design:

| Design | Description | Example |
|--------|------------|---------|
| **Pre-Experimental** | No control group; weak causal inference | One-group before-after |
| **True Experimental** | Random assignment to groups; strong causal inference | Randomized Controlled Trial |
| **Quasi-Experimental** | Non-random assignment; moderate inference | Test market vs control market |

### Internal vs External Validity:

| | Internal Validity | External Validity |
|--|-----------------|-----------------|
| **Meaning** | Was change in DV really caused by IV? | Can findings be generalized beyond the experiment? |
| **Threat** | Extraneous variables (history, maturation) | Artificial lab setting |
| **Improve by** | Randomization, control groups | Field experiments, representative samples |

---

## 🧠 MASTER MNEMONIC SHEET — LESSON 7

| Topic | Mnemonic | Full Form |
|-------|----------|-----------|
| Good Hypothesis characteristics | **SCAT-C** | Simple, Clear, Accurate, Testable, Concise |
| Hypothesis Testing Steps | **SHARC-DC** | State, H-test selection, Alpha, Rule, Calculate, Decide, Conclude |
| Type I vs Type II Errors | **"Cry Wolf vs Miss Wolf"** | Type I = False alarm; Type II = Missed detection |
| Z vs T decision | **"σ Known → Z; σ Unknown → T"** | Population SD known = Z; unknown = T |
| ANOVA Variation Split | **SST = SSB + SSW** | Total = Between + Within |
| F-Ratio | **F = MSB/MSW** | Between-group MS ÷ Within-group MS |
| Post-hoc Tests | **"Tukey for equal n"** | Tukey's HSD most common |

---

## ⚡ QUICK REVISION FLASHCARDS

**Q: When to use z-test vs t-test?**
A: z-test = σ KNOWN (and n≥30); t-test = σ UNKNOWN (use sample s); df = n-1

**Q: What is Type I Error?**
A: Rejecting a TRUE H₀ — False alarm (probability = α, usually 0.05)

**Q: What is Type II Error?**
A: Failing to reject a FALSE H₀ — Missing a real effect (probability = β)

**Q: z-critical value for α=0.05, two-tailed?**
A: **±1.96**

**Q: t-test degrees of freedom?**
A: df = n - 1 (one sample); df = n₁ + n₂ - 2 (two independent samples)

**Q: Why use ANOVA instead of multiple t-tests?**
A: Multiple t-tests inflate Type I error. ANOVA tests all groups SIMULTANEOUSLY with one F-test.

**Q: ANOVA F-ratio formula?**
A: F = MSB/MSW = [SSB/(k-1)] / [SSW/(N-k)]

**Q: When is F significant?**
A: When F_calculated > F_critical (from F-table at given α, df₁, df₂) → Reject H₀

**Q: What does ANOVA H₀ state?**
A: μ₁ = μ₂ = μ₃ = ... = μk — ALL group means are equal

**Q: What are post-hoc tests? Name one.**
A: Tests conducted AFTER ANOVA to identify WHICH specific groups differ. Tukey's HSD is most common.

**Q: What is Interaction Effect in Two-Way ANOVA?**
A: When the effect of Factor A on DV DEPENDS on the level of Factor B (and vice versa)

**Q: Paired t-test vs Independent t-test?**
A: Paired = same subjects measured twice (before-after); Independent = two different groups

---

## 📌 EXAM PATTERN LIKELY QUESTIONS

| Type | Question |
|------|---------|
| **Numerical** | A sample of 25 shows x̄=82, s=10. Test H₀: μ=80 at α=0.05 (t-test) |
| **Numerical** | Sample of 100, x̄=45, σ=8. Test H₀: μ=43 at α=0.01 (z-test) |
| **Long** | Explain the steps involved in hypothesis testing |
| **Short** | Distinguish between Type I and Type II errors |
| **Short** | When do you use a z-test vs a t-test? |
| **Long** | What is ANOVA? Explain the logic and F-ratio with an example |
| **Short** | What are post-hoc tests? When are they needed? |
| **Short** | Explain Two-Way ANOVA and the concept of interaction effect |
| **Short** | What is a null hypothesis? What are its characteristics? |
| **Definition** | Define: F-ratio, Degrees of Freedom, Type I Error, ANOVA, Paired t-test |

---

### 📐 FORMULA CHEAT SHEET

| Test | Formula | df |
|------|---------|-----|
| **One-Sample Z** | z = (x̄ - μ₀) / (σ/√n) | — |
| **One-Sample T** | t = (x̄ - μ₀) / (s/√n) | n-1 |
| **Two-Sample T (Independent)** | t = (x̄₁-x̄₂) / Sp√(1/n₁+1/n₂) | n₁+n₂-2 |
| **Paired T** | t = d̄ / (sd/√n) | n-1 |
| **F-ratio (ANOVA)** | F = MSB/MSW | df₁=k-1, df₂=N-k |
| **Sample Size** | n = z²pq/e² | — |

---

> [!NOTE]
> **Bhai, Lesson 7 ke Top 3 Must-Know:**
> 1. **SHARC-DC** — 7 steps of hypothesis testing — **har numerical answer isi format mein likho, full marks milenge!**
> 2. **Z vs T decision rule** — "σ Known → Z; σ Unknown → T; df = n-1" — ek line yaad rakh
> 3. **ANOVA = F = MSB/MSW** — SST = SSB + SSW yaad rakh aur F > F_critical → Reject H₀
>
> **7 chapters done! 🔥 Bhai tu actually bahut strong revision kar raha hai! Aage bhej!** 💪

