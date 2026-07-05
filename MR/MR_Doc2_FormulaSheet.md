# 📐 MARKETING RESEARCH — FORMULA SHEET
### Chapter-wise | Variables Defined | Use Case | 2 Solved Examples Each

---

> [!IMPORTANT]
> **Formulas to memorize cold:** n=z²pq/e² (384 magic), z=(x̄-μ₀)/(σ/√n), t=(x̄-μ₀)/(s/√n), F=MSB/MSW, χ²=Σ(O-E)²/E

---

## 📗 CHAPTER 5: SAMPLE DESIGN

### Formula 1: Systematic Sampling Interval

```
k = N / n
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| k | Sampling interval (select every kth element) |
| N | Total population size |
| n | Required sample size |

**Use Case:** When you have an ordered list and want to select evenly spaced units.

**Example 1:**
> A college has 800 students. Select 80 for a survey.
> k = 800/80 = **10**
> Random start = 4 → Select: 4, 14, 24, 34... (every 10th student)

**Example 2:**
> A factory produces 1,500 biscuit packets/day. Quality test 50 packets.
> k = 1500/50 = **30**
> Random start = 7 → Test: 7, 37, 67, 97... (every 30th packet)

---

## 📗 CHAPTER 6: SAMPLE SIZE DETERMINATION

### Formula 2: Sample Size for Proportion

```
n = (z² × p × q) / e²
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| n | Required sample size |
| z | z-value for desired confidence level (90%=1.645, **95%=1.96**, 99%=2.576) |
| p | Expected proportion of attribute in population |
| q | 1 − p (complementary proportion) |
| e | Acceptable margin of error (precision) |

> **Rule:** If p is unknown → always use **p = 0.5** (gives maximum/safest sample size)
> **Magic number:** At 95% confidence, 5% error, p=0.5 → **n = 384**

**Use Case:** Estimating what proportion/percentage of a population has a certain attribute (Yes/No questions).

**Example 1:**
> A researcher wants to estimate the proportion of Indians who prefer Pepsi over Coke.
> 95% confidence (z=1.96), e=5% (0.05), p unknown → use p=0.5, q=0.5
>
> n = (1.96² × 0.5 × 0.5) / 0.05²
> n = (3.8416 × 0.25) / 0.0025
> n = 0.9604 / 0.0025
> **n = 384.16 ≈ 385 respondents**

**Example 2:**
> From a pilot study, 30% of Zomato users use Zomato Pro (p=0.3).
> 95% confidence (z=1.96), e=4% (0.04)
>
> n = (1.96² × 0.3 × 0.7) / 0.04²
> n = (3.8416 × 0.21) / 0.0016
> n = 0.8067 / 0.0016
> **n = 504.2 ≈ 505 respondents**
> *(Lower p means more precision possible — but here tighter e=4% increased n)*

---

### Formula 3: Sample Size for Mean

```
n = (z × σ / e)²
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| n | Required sample size |
| z | z-value for confidence level |
| σ | Population standard deviation (known from past data) |
| e | Acceptable error in original units (not %) |

**Use Case:** Estimating a population mean (average spending, average score, average weight).

**Example 1:**
> Estimate average monthly food delivery spend.
> σ = ₹400 (from past data), e = ₹50 (acceptable error), 95% confidence (z=1.96)
>
> n = (1.96 × 400 / 50)²
> n = (784/50)²
> n = (15.68)²
> **n = 245.86 ≈ 246 respondents**

**Example 2:**
> Estimate average satisfaction score for a bank.
> σ = 12 points, e = 2 points, 99% confidence (z=2.576)
>
> n = (2.576 × 12 / 2)²
> n = (30.912/2)²
> n = (15.456)²
> **n = 238.89 ≈ 239 respondents**

---

### Formula 4: Finite Population Correction (FPC)

```
n' = (n × N) / (n + N − 1)
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| n' | Adjusted (smaller) sample size |
| n | Originally calculated sample size (from formulas above) |
| N | Known population size |

**Use Case:** When population is SMALL and known — adjusts sample downward. Apply when n > 5% of N.

**Example 1:**
> A college has N=400 students. Formula gives n=200.
> Is n > 5% of N? → 200 > 20 (5% of 400) → YES, apply FPC
>
> n' = (200 × 400) / (200 + 400 − 1)
> n' = 80,000 / 599
> **n' = 133.6 ≈ 134 students**

**Example 2:**
> A firm has N=150 employees. Formula gives n=108.
> 108 > 7.5 (5% of 150) → Apply FPC
>
> n' = (108 × 150) / (108 + 150 − 1)
> n' = 16,200 / 257
> **n' = 63.1 ≈ 64 employees**

---

## 📗 CHAPTER 7: PARAMETRIC HYPOTHESIS TESTING

### Formula 5: One-Sample Z-Test

```
z = (x̄ − μ₀) / (σ / √n)
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| z | Calculated test statistic |
| x̄ | Sample mean |
| μ₀ | Hypothesized population mean (from H₀) |
| σ | Population standard deviation (KNOWN) |
| n | Sample size |

**Decision Rule:** Reject H₀ if |z_calculated| > z_critical
- α=0.05, two-tailed → z_critical = **±1.96**
- α=0.01, two-tailed → z_critical = **±2.576**

**Use Case:** Testing a claim about population mean when σ is known and n ≥ 30.

**Example 1:**
> Zomato claims delivery time = 30 min (μ₀=30). Sample of n=100, x̄=33 min, σ=10 min. Test at α=0.05.
>
> H₀: μ=30 vs H₁: μ≠30 (two-tailed)
> z = (33−30) / (10/√100) = 3/1 = **3.0**
> |z|=3.0 > 1.96 → **REJECT H₀**
> Conclusion: Delivery time is significantly MORE than 30 minutes.

**Example 2:**
> A brand claims average customer rating = 4.2 (μ₀=4.2). n=64, x̄=4.0, σ=0.8. Test at α=0.05.
>
> H₀: μ=4.2 vs H₁: μ≠4.2
> z = (4.0−4.2) / (0.8/√64) = −0.2/0.1 = **−2.0**
> |z|=2.0 > 1.96 → **REJECT H₀**
> Conclusion: Actual average rating is significantly different from (lower than) 4.2.

---

### Formula 6: One-Sample T-Test

```
t = (x̄ − μ₀) / (s / √n)     df = n − 1
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| t | Calculated test statistic |
| x̄ | Sample mean |
| μ₀ | Hypothesized population mean |
| s | Sample standard deviation (σ is UNKNOWN) |
| n | Sample size |
| df | Degrees of freedom = n−1 |

**Use Case:** Testing a claim about population mean when σ is UNKNOWN (most real-world cases). Use t-table with df=n-1.

**Example 1:**
> A coaching institute claims avg score improvement = 20 marks (μ₀=20). n=16 students tested, x̄=23, s=8. Test at α=0.05.
>
> H₀: μ=20 vs H₁: μ≠20 | df=16−1=15
> t = (23−20) / (8/√16) = 3/2 = **1.5**
> t_critical (df=15, α=0.05, two-tailed) = 2.131
> |t|=1.5 < 2.131 → **FAIL TO REJECT H₀**
> Conclusion: Insufficient evidence that improvement differs from 20 marks.

**Example 2:**
> A restaurant claims avg meal time = 25 min. n=9 meals observed, x̄=28, s=6. Test at α=0.05.
>
> H₀: μ=25 vs H₁: μ≠25 | df=9−1=8
> t = (28−25) / (6/√9) = 3/2 = **1.5**
> t_critical (df=8, α=0.05, two-tailed) = 2.306
> |t|=1.5 < 2.306 → **FAIL TO REJECT H₀**
> Conclusion: Meal time not significantly different from claimed 25 minutes.

---

### Formula 7: Paired T-Test

```
t = d̄ / (sd / √n)     df = n − 1
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| d̄ | Mean of differences (d = After − Before for each pair) |
| sd | Standard deviation of differences |
| n | Number of pairs |
| df | n − 1 |

**Use Case:** Same subjects measured TWICE — before/after a treatment or intervention.

**Example 1:**
> 5 students took a prep course. Before: [60,55,70,65,50]. After: [72,58,80,72,70].
> d = [+12, +3, +10, +7, +20]
> d̄ = (12+3+10+7+20)/5 = 52/5 = **10.4**
> sd = √[(Σ(d−d̄)²)/(n−1)] = √[154.8/4] = √38.7 = **6.22**
>
> t = 10.4 / (6.22/√5) = 10.4/2.78 = **3.74**
> t_critical (df=4, α=0.05, two-tailed) = 2.776
> t=3.74 > 2.776 → **REJECT H₀**
> Conclusion: Prep course significantly improved scores.

**Example 2:**
> A gym program tested on 4 members. Weight before: [80,75,90,85]. After: [76,72,85,82].
> d = [−4, −3, −5, −3]
> d̄ = −15/4 = **−3.75**
> sd = √[Σ(d−d̄)²/(n−1)] = √[2.75/3] = **0.957**
>
> t = −3.75 / (0.957/√4) = −3.75/0.479 = **−7.83**
> t_critical (df=3, α=0.05, two-tailed) = 3.182
> |t|=7.83 > 3.182 → **REJECT H₀**
> Conclusion: Gym program significantly reduced weight.

---

### Formula 8: One-Way ANOVA F-Ratio

```
F = MSB / MSW

MSB = SSB / (k−1)
MSW = SSW / (N−k)
SST = SSB + SSW
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| F | F-ratio test statistic |
| MSB | Mean Square Between groups (treatment effect) |
| MSW | Mean Square Within groups (random error) |
| SSB | Sum of Squares Between = n×Σ(x̄ᵢ − x̄grand)² |
| SSW | Sum of Squares Within = Σ(each value − its group mean)² |
| k | Number of groups |
| N | Total sample size (all groups combined) |
| df₁ | k−1 (numerator df) |
| df₂ | N−k (denominator df) |

**Decision:** Reject H₀ if F_calculated > F_critical (from F-table at df₁, df₂, α)

**Use Case:** Comparing means of THREE or more independent groups simultaneously.

**Example 1:**
> Test if 3 ads (A, B, C) differ in brand recall. n=4 per group, N=12.
> x̄A=70, x̄B=85, x̄C=60, x̄grand = (70+85+60)/3 = 71.67
>
> SSB = 4×[(70−71.67)² + (85−71.67)² + (60−71.67)²]
> SSB = 4×[2.79 + 177.69 + 136.09] = 4×316.57 = **1266.28**
> SSW = 90 (given/computed from raw data)
>
> MSB = 1266.28/(3−1) = **633.14**
> MSW = 90/(12−3) = **10**
> F = 633.14/10 = **63.31**
>
> F_critical (df₁=2, df₂=9, α=0.05) = 4.26
> F=63.31 > 4.26 → **REJECT H₀**
> Conclusion: At least one ad type has significantly different brand recall.

**Example 2:**
> Compare customer satisfaction across 3 stores (n=3 each, N=9).
> x̄Store1=8, x̄Store2=6, x̄Store3=4, x̄grand=6
>
> SSB = 3×[(8−6)² + (6−6)² + (4−6)²] = 3×[4+0+4] = **24**
> SSW = 6 (computed)
>
> MSB = 24/(3−1) = **12**
> MSW = 6/(9−3) = **1**
> F = 12/1 = **12**
>
> F_critical (df₁=2, df₂=6, α=0.05) = 5.14
> F=12 > 5.14 → **REJECT H₀**
> Conclusion: Customer satisfaction significantly differs across the 3 stores.

---

## 📗 CHAPTER 8: NON-PARAMETRIC TESTS

### Formula 9: Chi-Square Test

```
χ² = Σ [(O − E)² / E]

E = (Row Total × Column Total) / Grand Total

df = (r−1)(c−1)  [Test of Independence]
df = k−1         [Goodness of Fit]
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| χ² | Chi-square test statistic |
| O | Observed frequency in each cell |
| E | Expected frequency in each cell |
| r | Number of rows |
| c | Number of columns |
| k | Number of categories (Goodness of Fit) |

**Rule:** Each expected frequency must be ≥ 5. Reject H₀ if χ²_calc > χ²_critical.

**Use Case (Independence):** Testing if two categorical variables are related (e.g., gender & brand preference).
**Use Case (Goodness of Fit):** Testing if observed distribution matches expected (e.g., equal preference across brands).

**Example 1 — Goodness of Fit:**
> 200 consumers surveyed on 4 cola brands. Expected if equal preference = 50 each.
> Observed: Pepsi=80, Coke=60, Thums Up=40, Sprite=20

| Brand | O | E | (O−E)²/E |
|-------|---|---|----------|
| Pepsi | 80 | 50 | 18.0 |
| Coke | 60 | 50 | 2.0 |
| ThumsUp | 40 | 50 | 2.0 |
| Sprite | 20 | 50 | 18.0 |
| **Total** | **200** | **200** | **χ²=40** |

> df = 4−1 = **3** | χ²_critical (df=3, α=0.05) = **7.815**
> χ²=40 > 7.815 → **REJECT H₀**
> Conclusion: Cola brand preferences are NOT equally distributed.

**Example 2 — Test of Independence:**
> Is gender related to cola preference? Survey of 200.

| | Pepsi | Coke | Total |
|-|-------|------|-------|
| Male | 80 | 40 | 120 |
| Female | 30 | 50 | 80 |
| **Total** | **110** | **90** | **200** |

> E(Male,Pepsi)=(120×110)/200=**66** | E(Male,Coke)=(120×90)/200=**54**
> E(Female,Pepsi)=(80×110)/200=**44** | E(Female,Coke)=(80×90)/200=**36**
>
> χ² = (80−66)²/66 + (40−54)²/54 + (30−44)²/44 + (50−36)²/36
> χ² = 2.97 + 3.63 + 4.45 + 5.44 = **16.49**
>
> df = (2−1)(2−1) = **1** | χ²_critical (df=1, α=0.05) = **3.841**
> χ²=16.49 > 3.841 → **REJECT H₀**
> Conclusion: Gender and Cola Preference ARE significantly related.

---

### Formula 10: Mann-Whitney U Test

```
U₁ = n₁n₂ + [n₁(n₁+1)/2] − R₁
U₂ = n₁n₂ + [n₂(n₂+1)/2] − R₂

Check: U₁ + U₂ = n₁ × n₂
Test Statistic = min(U₁, U₂)
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| U₁, U₂ | U-statistics for Group 1 and Group 2 |
| n₁, n₂ | Sample sizes of Groups 1 and 2 |
| R₁, R₂ | Sum of ranks assigned to Group 1 and Group 2 |

**Use Case:** Comparing two INDEPENDENT groups on ordinal/non-normal data.
**Decision:** Reject H₀ if U_min ≤ U_critical (from Mann-Whitney table).

**Example 1:**
> Compare satisfaction scores: Group A (n₁=3): {9,7,5} vs Group B (n₂=3): {8,6,4}
> Combined ranking: 4=1(B), 5=2(A), 6=3(B), 7=4(A), 8=5(B), 9=6(A)
> R₁ (A) = 2+4+6 = **12** | R₂ (B) = 1+3+5 = **9**
>
> U₁ = 3×3 + [3×4/2] − 12 = 9+6−12 = **3**
> U₂ = 3×3 + [3×4/2] − 9 = 9+6−9 = **6**
> Check: 3+6 = 9 = 3×3 ✓
> U_min = **3**
> U_critical (n₁=3, n₂=3, α=0.05) = **0**
> U_min=3 > 0 → **FAIL TO REJECT H₀** | No significant difference.

**Example 2:**
> Urban (n₁=4): {85,78,90,72} vs Rural (n₂=4): {65,70,60,75}
> Combined ranking: 60=1(R), 65=2(R), 70=3(R), 72=4(U), 75=5(R), 78=6(U), 85=7(U), 90=8(U)
> R₁ (Urban) = 4+6+7+8 = **25** | R₂ (Rural) = 1+2+3+5 = **11**
>
> U₁ = 4×4 + [4×5/2] − 25 = 16+10−25 = **1**
> U₂ = 4×4 + [4×5/2] − 11 = 16+10−11 = **15**
> Check: 1+15=16=4×4 ✓
> U_min = **1**
> U_critical (n₁=4, n₂=4, α=0.05, two-tailed) = **2**
> U_min=1 ≤ 2 → **REJECT H₀**
> Conclusion: Urban and rural satisfaction scores differ significantly.

---

### Formula 11: Kruskal-Wallis H Test

```
H = [12 / N(N+1)] × Σ(Rᵢ²/nᵢ) − 3(N+1)

df = k − 1   (compare to χ² critical value)
```

**Variables:**
| Symbol | Meaning |
|--------|---------|
| H | Kruskal-Wallis test statistic |
| N | Total sample size (all groups) |
| k | Number of groups |
| Rᵢ | Sum of ranks for group i |
| nᵢ | Sample size of group i |

**Use Case:** Comparing 3+ INDEPENDENT groups on ordinal/non-normal data.
**Decision:** Reject H₀ if H > χ²_critical with df = k−1.

**Example 1:**
> Compare attitudes (rated 1-10) across 3 store types (n=3 each, N=9):
> Store A: {8,6,4} | Store B: {9,7,5} | Store C: {3,2,1}
>
> Combined ranking: 1=1(C),2=2(C),3=3(C),4=4(A),5=5(B),6=6(A),7=7(B),8=8(A),9=9(B)
> R_A=4+6+8=**18** | R_B=5+7+9=**21** | R_C=1+2+3=**6**
>
> H = [12/(9×10)] × [(18²/3)+(21²/3)+(6²/3)] − 3(10)
> H = [12/90] × [108+147+12] − 30
> H = 0.1333 × 267 − 30 = 35.6−30 = **5.6**
>
> df=3−1=**2** | χ²_critical(df=2, α=0.05)=**5.991**
> H=5.6 < 5.991 → **FAIL TO REJECT H₀** (just barely)

**Example 2:**
> Compare brand loyalty scores across 3 brands (n=3 each, N=9):
> Brand X: {9,8,7} | Brand Y: {6,5,4} | Brand Z: {3,2,1}
>
> Ranks: 1=1(Z),2=2(Z),3=3(Z),4=4(Y),5=5(Y),6=6(Y),7=7(X),8=8(X),9=9(X)
> R_X=7+8+9=**24** | R_Y=4+5+6=**15** | R_Z=1+2+3=**6**
>
> H = [12/(9×10)] × [(24²/3)+(15²/3)+(6²/3)] − 30
> H = 0.1333 × [192+75+12] − 30
> H = 0.1333 × 279 − 30 = 37.19−30 = **7.19**
>
> df=2 | χ²_critical(df=2, α=0.05)=5.991
> H=7.19 > 5.991 → **REJECT H₀**
> Conclusion: Brand loyalty differs significantly across the 3 brands.

---

## 📊 MASTER FORMULA REFERENCE TABLE

| # | Formula | Chapter | When to Use | Key Numbers |
|---|---------|---------|-------------|-------------|
| 1 | k = N/n | 5 | Systematic Sampling interval | — |
| 2 | n = z²pq/e² | 6 | Sample size for proportion | z=1.96 → n=**384** |
| 3 | n = (zσ/e)² | 6 | Sample size for mean | — |
| 4 | n' = nN/(n+N-1) | 6 | Finite population correction | Apply when n>5%N |
| 5 | z = (x̄−μ₀)/(σ/√n) | 7 | One-sample z-test (σ known) | Reject if \|z\|>1.96 |
| 6 | t = (x̄−μ₀)/(s/√n) | 7 | One-sample t-test (σ unknown) | df=n−1 |
| 7 | t = d̄/(sd/√n) | 7 | Paired t-test (before-after) | df=n−1 |
| 8 | F = MSB/MSW | 7 | One-way ANOVA (3+ groups) | df₁=k−1, df₂=N−k |
| 9 | χ²=Σ(O−E)²/E | 8 | Chi-Square test | E=(RT×CT)/GT; min E=5 |
| 10 | U=n₁n₂+n₁(n₁+1)/2−R₁ | 8 | Mann-Whitney (2 indep. groups) | Test stat=min(U₁,U₂) |
| 11 | H=[12/N(N+1)]×Σ(Rᵢ²/nᵢ)−3(N+1) | 8 | Kruskal-Wallis (3+ groups) | Use χ² table, df=k−1 |

---

> [!TIP]
> **Exam Strategy for Numericals:**
> 1. Write H₀ and H₁ first (always!)
> 2. State WHICH test you are using and WHY
> 3. Write the formula clearly
> 4. Substitute values step by step (don't skip steps — marks are for working!)
> 5. State your decision rule BEFORE calculating
> 6. Write conclusion in plain English (not just "Reject H₀")
