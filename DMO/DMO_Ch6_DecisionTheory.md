# 📗 DMO CHAPTER 6: Decision Theory
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

A startup founder is deciding whether to:
- **Option A:** Launch a new product
- **Option B:** Improve existing product
- **Option C:** Enter a new market

The outcome depends on what the economy does — **Boom, Stable, or Recession** — which she can't control.

If she could predict the future perfectly → Easy choice. But she can't. So she uses **Decision Theory** — a structured way to choose the BEST option given uncertainty.

---

## 🔵 DECISION ENVIRONMENTS

| Environment | Knowledge Level | Example |
|------------|----------------|---------|
| **Certainty** | Know exactly what outcome each action produces | Investing in fixed deposit at guaranteed 6% |
| **Risk** | Know the probability of each outcome | Coin flip — 50% heads, 50% tails |
| **Uncertainty** | Don't even know probabilities | Launching a product in a brand new market |

---

## 🔵 KEY TERMS

| Term | Definition |
|------|-----------|
| **Alternative** | A course of action available to decision maker |
| **State of Nature** | Future condition beyond decision maker's control |
| **Payoff** | Outcome (profit, cost) for each combination of alternative + state of nature |
| **Payoff Matrix** | Table showing all payoffs for all combinations |

---

## 🔵 PAYOFF MATRIX (Standard Format)

**Example:** A company is deciding between three strategies with three possible market conditions:

| Alternative | Boom | Stable | Recession |
|------------|------|--------|-----------|
| **Product Launch** | 80 | 30 | -30 |
| **Product Improvement** | 50 | 45 | 20 |
| **New Market Entry** | 100 | 20 | -50 |

*(Values in ₹ lakhs profit)*

---

## 🔵 DECISION MAKING UNDER UNCERTAINTY ⭐

When probabilities are NOT known. Five classical criteria:

---

### Criterion 1: MAXIMAX (Optimist / "Go Big") ⭐

**Rule:** Choose the alternative with the **maximum of all maximum payoffs**

**Logic:** "I am optimistic — assume the BEST state of nature will occur"

**Step 1 — Find Maximum Payoff for each alternative:**
| Alternative | Maximum Payoff |
|------------|---------------|
| Product Launch | 80 |
| Product Improvement | 50 |
| **New Market Entry** | **100 ← Maximum** |

**Decision: New Market Entry (Maximum payoff = 100)**

**Criticism:** Ignores worst-case outcomes. Very risky approach.

---

### Criterion 2: MAXIMIN (Pessimist / "Play Safe") ⭐

**Rule:** Choose the alternative with the **maximum of all minimum payoffs**

**Logic:** "Assume the WORST state will occur; choose what's best in the worst case"

**Step 1 — Find Minimum Payoff for each alternative:**
| Alternative | Minimum Payoff |
|------------|---------------|
| Product Launch | -30 |
| **Product Improvement** | **20 ← Maximum of minimums** |
| New Market Entry | -50 |

**Decision: Product Improvement (Maximum of minimum = 20)**

**Criticism:** Too conservative; ignores upside.

---

### Criterion 3: MINIMAX REGRET (Opportunity Loss) ⭐

**Rule:** Minimize the maximum "regret" (opportunity loss)

**Logic:** "I want to minimize the maximum amount I'll regret not choosing the better option"

**Step 1 — Build Regret Matrix:**
For each state of nature, find the best payoff. Regret = Best payoff in that state − Each payoff.

**Best payoff in each state:**
- Boom: max(80, 50, 100) = 100 (New Market Entry)
- Stable: max(30, 45, 20) = 45 (Product Improvement)
- Recession: max(-30, 20, -50) = 20 (Product Improvement)

**Regret Matrix:**
| Alternative | Boom | Stable | Recession | Max Regret |
|------------|------|--------|-----------|-----------|
| Product Launch | 100-80=20 | 45-30=15 | 20-(-30)=50 | **50** |
| **Product Improvement** | 100-50=50 | 45-45=0 | 20-20=0 | **50** |
| New Market Entry | 100-100=0 | 45-20=25 | 20-(-50)=70 | **70** |

**Decision: Product Launch OR Product Improvement (both have minimum max regret = 50)**

Tie! In case of tie, use secondary criterion or prefer more conservative option.

---

### Criterion 4: LAPLACE (Equal Probability / "Balanced")

**Rule:** Assign equal probability to all states; choose alternative with highest average payoff

**Logic:** "Since I don't know probabilities, assume all states equally likely"

With 3 states: P = 1/3 each

| Alternative | Average = (Boom + Stable + Recession)/3 |
|------------|----------------------------------------|
| Product Launch | (80+30-30)/3 = 80/3 = 26.67 |
| **Product Improvement** | **(50+45+20)/3 = 115/3 = 38.33 ← Highest** |
| New Market Entry | (100+20-50)/3 = 70/3 = 23.33 |

**Decision: Product Improvement (Average = 38.33)**

---

### Criterion 5: HURWICZ (Optimism-Pessimism Index, α)

**Rule:** Weighted average of best and worst payoffs using α (optimism coefficient)

**Formula:**
```
H = α × (Maximum Payoff) + (1-α) × (Minimum Payoff)
Choose alternative with highest H
```

Where α = 0 → Pure pessimism (Maximin); α = 1 → Pure optimism (Maximax)

**If α = 0.6:**

| Alternative | H = 0.6×Max + 0.4×Min |
|------------|----------------------|
| Product Launch | 0.6(80) + 0.4(-30) = 48 - 12 = 36 |
| **Product Improvement** | **0.6(50) + 0.4(20) = 30 + 8 = 38 ← Highest** |
| New Market Entry | 0.6(100) + 0.4(-50) = 60 - 20 = 40 |

Wait — New Market Entry = 40 > 38, so **Decision: New Market Entry**

---

### Decision Criteria Summary:

| Criterion | Type | Decision |
|-----------|------|---------|
| Maximax | Optimist | New Market Entry |
| Maximin | Pessimist | Product Improvement |
| Minimax Regret | Balanced | Product Launch/Improvement |
| Laplace | Neutral | Product Improvement |
| Hurwicz (α=0.6) | Semi-optimist | New Market Entry |

---

## 🔵 DECISION MAKING UNDER RISK — EMV ⭐

When probabilities ARE known.

**Expected Monetary Value (EMV):**
```
EMV = Σ [Probability(i) × Payoff(i)]
Choose alternative with MAXIMUM EMV (for profit)
or MINIMUM EMV (for cost)
```

**Example:** Probabilities: Boom=0.30, Stable=0.50, Recession=0.20

**EMV Calculation:**
| Alternative | EMV |
|------------|-----|
| Product Launch | 0.30(80)+0.50(30)+0.20(-30) = 24+15-6 = **₹33 lakhs** |
| **Product Improvement** | **0.30(50)+0.50(45)+0.20(20) = 15+22.5+4 = ₹41.5 lakhs ← Maximum** |
| New Market Entry | 0.30(100)+0.50(20)+0.20(-50) = 30+10-10 = **₹30 lakhs** |

**Decision: Product Improvement (EMV = ₹41.5 lakhs)**

---

## 🔵 EXPECTED VALUE OF PERFECT INFORMATION (EVPI) ⭐

**What is EVPI?**
The maximum amount a decision maker should pay to obtain PERFECT information about which state of nature will occur.

**Formula:**
```
EVPI = EMV(with Perfect Information) - EMV(best without PI)
```

**Step 1 — Calculate EMV with Perfect Information:**
Under perfect information, you always make the BEST choice for each state:
- If you know Boom → Choose New Market Entry (payoff=100)
- If you know Stable → Choose Product Improvement (payoff=45)
- If you know Recession → Choose Product Improvement (payoff=20)

```
EMV(PI) = 0.30(100) + 0.50(45) + 0.20(20)
        = 30 + 22.5 + 4
        = ₹56.5 lakhs
```

**Step 2 — EMV without PI (best EMV from above):**
```
Best EMV = ₹41.5 (Product Improvement)
```

**Step 3 — EVPI:**
```
EVPI = 56.5 - 41.5 = ₹15 lakhs
```

**Interpretation:** The decision maker should pay AT MOST ₹15 lakhs for a perfect market forecast. If a research firm charges ₹10 lakhs → Worth buying. If charges ₹20 lakhs → Not worth it.

---

## 🔵 DECISION TREES ⭐

A Decision Tree is a graphical representation of a multi-stage decision problem. Better than a payoff matrix when decisions are sequential (one decision leads to another).

**Symbols:**
- **□ (Square):** Decision node — decision maker chooses
- **○ (Circle):** Chance node — nature chooses (with probabilities)
- **→ (Branches):** Alternatives or states of nature

**Solving Direction:** Always solve from RIGHT to LEFT (fold back)

---

### DECISION TREE WORKED EXAMPLE:

**Problem:**
A pharmaceutical company can either:
1. Conduct clinical trials (costs ₹50 lakhs): 70% chance drug is effective (value ₹300 lakhs); 30% chance fails (value ₹0)
2. Launch without trials (saves ₹50 lakhs): 40% chance drug is effective (₹200 lakhs revenue); 60% chance fails and faces liability (₹-100 lakhs)

**Draw Tree and Solve:**

```
                        70% → Effective: 300 - 50 = 250
□ Decision ─── Conduct trials ─ ○
                        30% → Fails: 0 - 50 = -50

              └── Launch without ─ ○
                        40% → Effective: 200
                        60% → Fails: -100
```

**Step 1 — Calculate EMV at each chance node (right to left):**

**Chance Node 1 (Trials):**
```
EMV = 0.70(250) + 0.30(-50)
    = 175 - 15
    = ₹160 lakhs
```

**Chance Node 2 (No trials):**
```
EMV = 0.40(200) + 0.60(-100)
    = 80 - 60
    = ₹20 lakhs
```

**Step 2 — Decision at Decision Node:**
- Conduct trials: EMV = ₹160 lakhs
- Launch without trials: EMV = ₹20 lakhs

**Decision: Conduct Clinical Trials (EMV = ₹160 lakhs)**

---

### Multi-Stage Decision Tree:

In real problems, decisions are often sequential:
1. Should we do market research?
2. Based on research results, should we launch?

This creates a tree with MULTIPLE decision and chance nodes. Always solve right-to-left.

---

## 🔵 COMPARISON TABLE

| Method | Environment | When to Use |
|--------|------------|-------------|
| Maximax | Uncertainty | Optimistic manager; high-growth mindset |
| Maximin | Uncertainty | Risk-averse; conservative; startup with limited cash |
| Minimax Regret | Uncertainty | Balanced; concerned about post-decision regret |
| Laplace | Uncertainty | No information about probabilities |
| Hurwicz | Uncertainty | Know your risk attitude (α) |
| EMV | Risk | Probabilities are known; simple one-stage |
| Decision Tree | Risk | Sequential decisions; probabilities known |
| EVPI | Risk | Decide whether to buy market research |

---

## 🔴 EXAM-READY CONTENT

### Full 10-Mark Problem Template:

```
Step 1: Build payoff matrix from problem data
Step 2: Apply all required criteria (as asked):
  - Maximax: Max of each row max
  - Maximin: Max of each row min
  - Minimax Regret: Build regret matrix; take row max; choose min
  - Laplace: Calculate row average
  - Hurwicz: H = α×Max + (1-α)×Min
Step 3: EMV (if probabilities given):
  EMV = Σ P(i) × Payoff(i) for each alternative
Step 4: EVPI (if asked):
  EVPI = EMV(PI) - Best EMV
Step 5: Decision Tree (if multi-stage):
  Draw tree → Fold back right to left using EMV
Step 6: State recommendation clearly
```

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Decision under Certainty | Know exactly what will happen |
| Decision under Risk | Know probabilities of outcomes |
| Decision under Uncertainty | Don't know probabilities |
| Maximax | Optimist — pick best best-case |
| Maximin | Pessimist — pick best worst-case |
| Minimax Regret | Minimize maximum opportunity loss |
| Laplace | Equal probabilities to all states |
| Hurwicz | Weighted optimism-pessimism index |
| EMV | Expected Monetary Value = Σ P(i)×Payoff(i) |
| EVPI | Max worth paying for perfect information |
| Decision Tree | Sequential decisions shown as tree; solve right-to-left |
| Decision Node □ | You choose |
| Chance Node ○ | Nature chooses (with probability) |

---

*Chapter 6 Complete | DMO | MBA 2nd Semester, DU SOL*
