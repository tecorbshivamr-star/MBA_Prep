# 📗 DMO CHAPTER 8: Game Theory
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

Imagine Flipkart and Amazon India are deciding their pricing strategy for a sale event:
- If both offer big discounts → Both lose margins
- If only one offers discounts → That one grabs market share; the other loses
- If neither offers discounts → Both maintain margins

Each company's best decision DEPENDS on what the other decides. Neither has full control.

This is **Game Theory** — the mathematical study of strategic interaction between rational players. It helps predict what competitors will do and what you should do in response.

**Game Theory was invented by:** John von Neumann and Oskar Morgenstern (1944); further developed by John Nash (Nobel Prize 1994).

---

## 🔵 WHAT IS GAME THEORY?

**Definition:**
Game Theory is a branch of mathematics and economics that studies strategic decision-making in situations where the outcome of one player's choice depends on the choices of other players.

**Game theory applies when:**
- At least two players (competitors, firms, countries)
- Each player's outcome depends on ALL players' decisions
- Players are rational (act in their own best interest)
- Each player knows the possible strategies and outcomes

---

## 🔵 KEY TERMINOLOGY

| Term | Definition |
|------|-----------|
| **Player** | Decision maker in the game (firm, person, country) |
| **Strategy** | Complete plan of action a player will follow |
| **Payoff** | Outcome (gain or loss) for a player from a strategy combination |
| **Payoff Matrix** | Table showing payoffs for all strategy combinations |
| **Zero-Sum Game** | One player's gain = other player's loss (total = zero) |
| **Non-Zero-Sum Game** | Gains and losses don't cancel out (cooperative benefit possible) |
| **Pure Strategy** | Player always plays the same strategy |
| **Mixed Strategy** | Player randomizes between strategies using probabilities |
| **Saddle Point** | Pure strategy equilibrium (both players' optimal strategies coincide) |
| **Nash Equilibrium** | No player wants to unilaterally change strategy |

---

## 🔵 TWO-PERSON ZERO-SUM GAME ⭐ Most Tested

**Zero-Sum Game:** Whatever Player A gains, Player B loses. Total payoff always = 0.

**Payoff Matrix Convention:**
- Rows = Player A's strategies
- Columns = Player B's strategies
- Values = Player A's payoff (Player B's payoff = negative of this)

---

## 🔵 PURE STRATEGY — SADDLE POINT ⭐

**When does a pure strategy solution exist?**
When there is a **Saddle Point** — an entry in the payoff matrix that is simultaneously:
- The MINIMUM of its ROW (Player A can't do worse by changing, IF this is minimum of row)
- The MAXIMUM of its COLUMN (Player B can't do better by changing)

**Finding Saddle Point:**

**Step 1:** Find the MINIMUM value in each row (Row Minima)
**Step 2:** Find the MAXIMUM among these Row Minima → This is **MAXIMIN** (Player A's optimal)
**Step 3:** Find the MAXIMUM value in each column (Column Maxima)
**Step 4:** Find the MINIMUM among these Column Maxima → This is **MINIMAX** (Player B's optimal)
**Step 5:** If Maximin = Minimax → **Saddle Point exists!** This value = **Value of the Game**

---

### WORKED EXAMPLE 1 — Pure Strategy:

**Payoff Matrix (Player A's gains):**

| | B1 | B2 | B3 | **Row Min** |
|--|----|----|----|----|
| **A1** | 4 | 6 | 3 | **3** |
| **A2** | 7 | 5 | 2 | **2** |
| **A3** | 3 | 8 | 6 | **3** |
| **Col Max** | 7 | 8 | **6** | |

**Maximin (Player A):** Max of Row Minima = max(3, 2, 3) = **3** (rows A1 or A3)

**Minimax (Player B):** Min of Column Maxima = min(7, 8, 6) = **6** (column B3)

**Maximin ≠ Minimax (3 ≠ 6)** → NO Saddle Point → Must use Mixed Strategy

---

### WORKED EXAMPLE 2 — Pure Strategy (with Saddle Point):

| | B1 | B2 | B3 | **Row Min** |
|--|----|----|----|----|
| **A1** | 3 | 7 | 2 | **2** |
| **A2** | 5 | 6 | 4 | **4** ← **Maximin** |
| **A3** | 2 | 8 | 3 | **2** |
| **Col Max** | 5 | 8 | **4** ← **Minimax** | |

**Maximin = 4; Minimax = 4 → EQUAL! Saddle Point Exists!**

**Saddle Point:** A2, B3 (value = 4)

**Optimal Strategy:** Player A always plays A2; Player B always plays B3
**Value of Game = 4** (Player A always gains 4; Player B always loses 4)

---

## 🔵 MIXED STRATEGY — 2×2 GAME ⭐

When no saddle point exists, both players should **randomize** between strategies to prevent the opponent from predicting and exploiting their play.

**For a 2×2 game:** Let Player A play A1 with probability p and A2 with probability (1-p)

**Finding Optimal Mixed Strategy:**

**Principle:** Player A should choose p such that Player B is indifferent between B1 and B2.
(If B is indifferent, B can't exploit A's strategy)

### WORKED EXAMPLE — Mixed Strategy:

**Payoff Matrix (2×2, no saddle point):**

| | B1 | B2 |
|--|----|----|
| **A1** | 4 | 2 |
| **A2** | 1 | 5 |

**Check for Saddle Point:**
Row minima: Row 1 → min(4,2)=2; Row 2 → min(1,5)=1 → Maximin = 2
Column maxima: Col 1 → max(4,1)=4; Col 2 → max(2,5)=5 → Minimax = 4
2 ≠ 4 → **No Saddle Point → Mixed Strategy**

---

**Finding Player A's Optimal Probabilities:**

Let A play A1 with probability p, A2 with probability (1-p).

Player A makes B indifferent:
```
Expected payoff to A when B plays B1 = 4p + 1(1-p) = 3p + 1
Expected payoff to A when B plays B2 = 2p + 5(1-p) = -3p + 5
```
Set equal:
```
3p + 1 = -3p + 5
6p = 4
p = 2/3
1-p = 1/3
```

**Player A:** Play A1 with probability 2/3; play A2 with probability 1/3

**Value of Game:**
```
V = 3p + 1 = 3(2/3) + 1 = 2 + 1 = 3
```
OR: V = -3p + 5 = -3(2/3) + 5 = -2 + 5 = 3 ✓

---

**Finding Player B's Optimal Probabilities:**

Let B play B1 with probability q, B2 with probability (1-q).

Player B makes A indifferent:
```
Expected payoff when A plays A1 = 4q + 2(1-q) = 2q + 2
Expected payoff when A plays A2 = 1q + 5(1-q) = -4q + 5
```
Set equal:
```
2q + 2 = -4q + 5
6q = 3
q = 1/2
1-q = 1/2
```

**Player B:** Play B1 with probability 1/2; play B2 with probability 1/2

**Summary:**
```
Player A: p(A1) = 2/3, p(A2) = 1/3
Player B: p(B1) = 1/2, p(B2) = 1/2
Value of Game = 3
```

---

## 🔵 DOMINANCE PRINCIPLE ⭐

**Dominance** simplifies games by eliminating strategies that are always worse than another.

**Rule:**
- A strategy is **dominated** if there exists another strategy that gives BETTER (or equal) payoff in ALL situations
- Dominated strategies can be DELETED from the matrix
- Repeat until matrix is small enough to solve

**For Player A:** Delete rows where another row is always ≥ (A prefers higher payoffs)
**For Player B:** Delete columns where another column is always ≤ (B prefers lower payoffs, wants to minimize A's gain)

### Dominance Example:

| | B1 | B2 | B3 |
|--|----|----|-----|
| **A1** | 3 | 5 | 7 |
| **A2** | 5 | 6 | 4 |
| **A3** | 1 | 4 | 3 |

**Check A3 vs A1:** A1=[3,5,7] vs A3=[1,4,3] → A1 > A3 in all columns → A3 dominated by A1 → Delete A3

**Remaining:**
| | B1 | B2 | B3 |
|--|----|----|-----|
| **A1** | 3 | 5 | 7 |
| **A2** | 5 | 6 | 4 |

**Check B1 vs B2:** B prefers lower values for A (B1=[3,5] vs B2=[5,6]) → B1 ≤ B2 in both rows → B2 dominated by B1 for B → Delete B2

**Remaining:**
| | B1 | B3 |
|--|----|----|
| **A1** | 3 | 7 |
| **A2** | 5 | 4 |

Now solve this 2×2 game using mixed or pure strategy!

---

## 🔵 NASH EQUILIBRIUM ⭐

**Definition (John Nash, 1950):**
A Nash Equilibrium is a set of strategies, one for each player, such that **no player can benefit by unilaterally changing their own strategy**, given the strategies of other players.

**Saddle Point = Nash Equilibrium in pure strategies**
**Mixed strategy solution = Nash Equilibrium in mixed strategies**

**Key Property:** At Nash Equilibrium, no one has an incentive to deviate.

---

## 🔵 THE PRISONER'S DILEMMA ⭐ Classic Example

**Scenario:** Two suspects (A and B) are arrested. Police have limited evidence. They're questioned separately with no communication. Each can Confess or Deny.

**Payoff Matrix (Years in prison — lower is better for each):**

| | B: Deny | B: Confess |
|--|---------|-----------|
| **A: Deny** | A=1, B=1 | A=10, B=0 |
| **A: Confess** | A=0, B=10 | A=5, B=5 |

**Analysis:**
- If B Denies: A's best response → Confess (0 years < 1 year)
- If B Confesses: A's best response → Confess (5 years < 10 years)
- **Confess is A's DOMINANT STRATEGY** (regardless of B's choice)
- Same analysis for B → Confess is B's dominant strategy

**Nash Equilibrium:** Both Confess → Both get 5 years

**The Dilemma:** If both Denied, both get only 1 year (much better!). But neither trusts the other to cooperate → Both defect → Worse outcome for both.

**Business Application:**
- Two companies both advertising aggressively → Both spend money but neither gains market share
- If both reduced advertising → Both save money; similar market shares
- But neither trusts the other to stop → Both keep advertising → Prisoner's Dilemma!

India Example: Airtel and Jio price wars — both cutting prices damages both companies' profits, but neither can stop unilaterally.

---

## 🔵 NON-ZERO-SUM GAMES

In real business, games are often **non-zero-sum** — one firm's gain doesn't necessarily come from another's loss.

**Example:** Standard-setting competition
- Both Apple and Android want their platform to become the standard
- If they cooperate → Market grows → Both benefit
- If they compete aggressively → Market fragments → Both lose customers

**Cooperative Game Theory:** Studies how players can form coalitions to achieve better outcomes together.

---

## 🔵 BUSINESS APPLICATIONS OF GAME THEORY

| Application | Game | Insight |
|-------------|------|---------|
| **Price wars** | Prisoner's Dilemma | Both firms lose from price war; need credible commitment to not cut |
| **Bidding/Auctions** | Winner's Curse | Highest bidder often overbids; need to adjust strategy |
| **Entry deterrence** | Chicken Game | Incumbent threatens to compete aggressively if entrant comes in |
| **Salary negotiation** | Bargaining Game | BATNA strength determines outcome |
| **R&D racing** | Coordination Game | Who sets the standard wins the market |
| **OPEC oil production** | Cartel Game | Mutual interest to restrict; individual interest to cheat |

---

## 🔴 EXAM-READY CONTENT

### Complete Exam Solving Template:

```
STEP 1: Draw/State the Payoff Matrix

STEP 2: Find Row Minima and Column Maxima

STEP 3: Check Maximin vs Minimax:
  - If Maximin = Minimax → Pure Strategy (Saddle Point)
    → Optimal strategies and Value of Game = Saddle Point value

  - If Maximin ≠ Minimax → Mixed Strategy needed

STEP 4 (Mixed, 2×2): 
  Find p using: E(A against B1) = E(A against B2)
  Find q using: E(B against A1) = E(B against A2)
  Value of Game V = either equation at optimal p

STEP 5: Apply Dominance to reduce matrix if needed (before Steps 2-4)

STEP 6: State final optimal strategies and game value clearly
```

---

### Exam Tip — Quick Check for Saddle Point:

> **Saddle Point = entry that is simultaneously the smallest in its row AND the largest in its column**

Look for this entry directly — saves calculation time!

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Game Theory | Mathematics of strategic interaction between rational players |
| Zero-Sum Game | One's gain = other's loss; total always zero |
| Payoff Matrix | Table of outcomes for all strategy combinations |
| Pure Strategy | Always play the same strategy |
| Mixed Strategy | Randomize between strategies with probabilities |
| Saddle Point | Entry = Row minimum AND Column maximum; pure strategy equilibrium |
| Maximin | Player A's criterion: maximize the minimum payoff |
| Minimax | Player B's criterion: minimize the maximum payoff to A |
| Value of Game (V) | Expected payoff at equilibrium |
| Nash Equilibrium | No player benefits by unilaterally changing strategy |
| Dominant Strategy | Best strategy regardless of opponent's choice |
| Prisoner's Dilemma | Both players defect to Nash Equilibrium; both would benefit from cooperation |

---

## ✅ ALL 8 DMO CHAPTERS COMPLETE!

### DMO File Index:
| Chapter | File |
|---------|------|
| Ch 1: Linear Programming | DMO_Ch1_LinearProgramming.md |
| Ch 2: Transportation Problem | DMO_Ch2_TransportationProblem.md |
| Ch 3: Queuing Theory | DMO_Ch3_QueuingTheory.md |
| Ch 4: Simulation | DMO_Ch4_Simulation.md |
| Ch 5: PERT & CPM | DMO_Ch5_PERT_CPM.md |
| Ch 6: Decision Theory | DMO_Ch6_DecisionTheory.md |
| Ch 7: Markov Chains | DMO_Ch7_MarkovChains.md |
| Ch 8: Game Theory | DMO_Ch8_GameTheory.md |

---

*Chapter 8 Complete | DMO | MBA 2nd Semester, DU SOL*
