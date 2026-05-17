# 📗 DMO CHAPTER 2: Transportation Problem
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

Imagine **Amul** has **3 dairy plants** (in Anand, Mehsana, Valsad) and **4 distribution centres** (in Mumbai, Delhi, Chennai, Kolkata).

Each plant can supply a fixed quantity of milk per day. Each distribution centre needs a fixed quantity. Transporting milk from each plant to each city costs different amounts per litre.

**Question:** From which plant should milk be sent to which city, and how much, to **minimize total transport cost?**

That's the **Transportation Problem** — allocating supply to meet demand at minimum cost.

---

## 🔵 WHAT IS THE TRANSPORTATION PROBLEM?

**Definition:**
The Transportation Problem is a special type of Linear Programming problem concerned with finding the **minimum cost plan** for distributing a commodity from a number of **supply sources** (origins) to a number of **demand destinations** (destinations).

**Key Features:**
- Multiple supply points (factories, warehouses)
- Multiple demand points (cities, customers)
- Transportation cost between each supply-demand pair
- Fixed supply at each source
- Fixed demand at each destination
- Goal: Minimize total transportation cost

---

## 🔵 STRUCTURE OF A TRANSPORTATION PROBLEM

### The Transportation Table (Matrix):

|  | D1 | D2 | D3 | Supply |
|--|----|----|----|----|
| **S1** | C₁₁ | C₁₂ | C₁₃ | a₁ |
| **S2** | C₂₁ | C₂₂ | C₂₃ | a₂ |
| **S3** | C₃₁ | C₃₂ | C₃₃ | a₃ |
| **Demand** | b₁ | b₂ | b₃ | |

Where:
- S1, S2, S3 = Supply sources (factories)
- D1, D2, D3 = Demand destinations (cities)
- Cᵢⱼ = Cost per unit to transport from source i to destination j
- aᵢ = Supply available at source i
- bⱼ = Demand required at destination j

---

## 🔵 BALANCED vs UNBALANCED

| Type | Condition | Action |
|------|-----------|--------|
| **Balanced** | Total Supply = Total Demand | Solve directly |
| **Unbalanced (Excess Supply)** | Total Supply > Total Demand | Add dummy destination; cost = 0 |
| **Unbalanced (Excess Demand)** | Total Supply < Total Demand | Add dummy source; cost = 0 |

**Why balance?** The methods require supply = demand to work properly.

---

## 🔵 WORKED EXAMPLE — Full Problem

**Problem:** A company has 3 plants (P1, P2, P3) and 4 warehouses (W1, W2, W3, W4).

**Cost Matrix (₹ per unit):**

| | W1 | W2 | W3 | W4 | **Supply** |
|--|----|----|----|----|-------|
| **P1** | 2 | 3 | 1 | 5 | 30 |
| **P2** | 7 | 3 | 4 | 6 | 40 |
| **P3** | 4 | 6 | 7 | 2 | 20 |
| **Demand** | 20 | 30 | 20 | 20 | **90/90** ✓ |

**Balanced:** Total Supply = 90 = Total Demand ✓

---

## 🔵 METHOD 1: NORTH-WEST CORNER METHOD (NWCM)

### Rules:
1. Start at the **top-left (north-west) cell**
2. Allocate as much as possible = min(supply of row, demand of column)
3. Reduce supply and demand by the allocated amount
4. Move **right** if column demand is satisfied; move **down** if row supply is exhausted; move **diagonally** if both
5. Repeat until all supply and demand are met

### NWCM Solution:

**Step 1:** Cell P1-W1: min(30, 20) = 20 → Allocate 20
- P1 supply: 30-20=10; W1 demand: 20-20=0 → Move right

**Step 2:** Cell P1-W2: min(10, 30) = 10 → Allocate 10
- P1 supply: 10-10=0; W2 demand: 30-10=20 → Move down

**Step 3:** Cell P2-W2: min(40, 20) = 20 → Allocate 20
- P2 supply: 40-20=20; W2 demand: 20-20=0 → Move right

**Step 4:** Cell P2-W3: min(20, 20) = 20 → Allocate 20
- P2 supply: 20-20=0; W3 demand: 20-20=0 → Move diagonally

**Step 5:** Cell P3-W4: min(20, 20) = 20 → Allocate 20
- Done!

**NWCM Allocation Table:**

| | W1 | W2 | W3 | W4 | Supply |
|--|----|----|----|----|-------|
| **P1** | **20** | **10** | — | — | 30 ✓ |
| **P2** | — | **20** | **20** | — | 40 ✓ |
| **P3** | — | — | — | **20** | 20 ✓ |
| **Demand** | 20✓ | 30✓ | 20✓ | 20✓ | |

**Total Cost (NWCM):**
```
= 20×2 + 10×3 + 20×3 + 20×4 + 20×2
= 40 + 30 + 60 + 80 + 40
= ₹250
```

**Limitation of NWCM:** Completely ignores costs! Just a mechanical starting point. Usually gives high initial cost.

---

## 🔵 METHOD 2: LEAST COST METHOD (LCM) / MATRIX MINIMA

### Rules:
1. Find the **cell with the lowest cost** in the entire table
2. Allocate as much as possible to that cell
3. Cross out (eliminate) the row or column that is exhausted
4. Repeat from remaining cells

### LCM Solution:

**Step 1:** Lowest cost = P1-W3 (cost=1). Allocate min(30,20) = 20
- P1 supply: 30-20=10; W3 demand: 20-20=0 → Cross out W3

**Step 2:** Next lowest in remaining = P1-W1 (cost=2). Allocate min(10,20) = 10
- P1 supply: 10-10=0; W1 demand: 20-10=10 → Cross out P1

**Step 3:** Next lowest = P3-W4 (cost=2). Allocate min(20,20) = 20
- P3 supply: 20-20=0; W4 demand: 20-20=0 → Cross out P3 and W4

**Step 4:** Now only P2 remains with demand at W1=10, W2=30.
- Allocate P2-W1: min(40,10) = 10 → W1 done; P2 supply: 40-10=30
- Allocate P2-W2: min(30,30) = 30 → Done!

**LCM Allocation Table:**

| | W1 | W2 | W3 | W4 | Supply |
|--|----|----|----|----|-------|
| **P1** | **10** | — | **20** | — | 30 ✓ |
| **P2** | **10** | **30** | — | — | 40 ✓ |
| **P3** | — | — | — | **20** | 20 ✓ |
| **Demand** | 20✓ | 30✓ | 20✓ | 20✓ | |

**Total Cost (LCM):**
```
= 10×2 + 20×1 + 10×7 + 30×3 + 20×2
= 20 + 20 + 70 + 90 + 40
= ₹240
```

Better than NWCM (₹250)! LCM considers costs and gives a better initial solution.

---

## 🔵 METHOD 3: VOGEL'S APPROXIMATION METHOD (VAM) ⭐ Best Initial Solution

VAM is the most accurate initial solution method. It considers the "penalty" for not using the cheapest route.

### Rules:
1. For each **row**, calculate the penalty = difference between **1st and 2nd lowest cost** in that row
2. For each **column**, calculate the penalty = difference between 1st and 2nd lowest cost in that column
3. Select the row or column with the **highest penalty**
4. In that row/column, allocate as much as possible to the **cheapest cell**
5. Cross out satisfied row/column and repeat

### VAM Solution:

**Step 1 — Calculate Row and Column Penalties:**

| | W1 | W2 | W3 | W4 | Supply | **Row Penalty** |
|--|----|----|----|----|-------|-----------|
| **P1** | 2 | 3 | 1 | 5 | 30 | 3-1 = **2** |
| **P2** | 7 | 3 | 4 | 6 | 40 | 4-3 = **1** |
| **P3** | 4 | 6 | 7 | 2 | 20 | 4-2 = **2** |
| **Demand** | 20 | 30 | 20 | 20 | | |
| **Col Penalty** | 4-2=**2** | 3-3=**0** | 4-1=**3**← | 5-2=**3**← | | |

Highest penalty = 3 (tied between W3 and W4)

**Select W3 (Column 3, penalty=3):** Cheapest in W3 = P1 (cost=1)
Allocate min(30,20) = 20 to P1-W3
- P1 supply: 30-20=10; W3 eliminated

**Step 2 — Recalculate without W3:**

| | W1 | W2 | W4 | Supply | **Row Penalty** |
|--|----|----|----|----|-----------|
| **P1** | 2 | 3 | 5 | 10 | 3-2 = **1** |
| **P2** | 7 | 3 | 6 | 40 | 6-3 = **3** |
| **P3** | 4 | 6 | 2 | 20 | 4-2 = **2** |
| **Demand** | 20 | 30 | 20 | | |
| **Col Penalty** | 4-2=**2** | 3-3=**0** | 5-2=**3**← | | |

Highest penalty = 3 (tied P2 row and W4 col)

**Select W4 (penalty=3):** Cheapest in W4 = P3 (cost=2)
Allocate min(20,20) = 20 to P3-W4
- P3 supply: 0; W4 eliminated; cross out P3

**Step 3 — Recalculate without W3, W4, P3:**

| | W1 | W2 | Supply | **Row Penalty** |
|--|----|----|-------|-----------|
| **P1** | 2 | 3 | 10 | 3-2=**1** |
| **P2** | 7 | 3 | 40 | 7-3=**4**← |
| **Demand** | 20 | 30 | | |
| **Col Penalty** | 7-2=**5**← | 3-3=**0** | | |

Highest penalty = 5 (W1 column)

**Select W1 (penalty=5):** Cheapest in W1 = P1 (cost=2)
Allocate min(10,20) = 10 to P1-W1
- P1 supply: 0; W1 demand: 10 remaining; cross out P1

**Step 4 — Only P2 remains; W1 demand=10, W2 demand=30:**
Allocate 10 to P2-W1, 30 to P2-W2

**VAM Allocation Table:**

| | W1 | W2 | W3 | W4 | Supply |
|--|----|----|----|----|-------|
| **P1** | **10** | — | **20** | — | 30 ✓ |
| **P2** | **10** | **30** | — | — | 40 ✓ |
| **P3** | — | — | — | **20** | 20 ✓ |
| **Demand** | 20✓ | 30✓ | 20✓ | 20✓ | |

**Total Cost (VAM):**
```
= 10×2 + 20×1 + 10×7 + 30×3 + 20×2
= 20 + 20 + 70 + 90 + 40
= ₹240
```

Same as LCM in this case. VAM often achieves optimal or near-optimal initial solution.

---

## 🔵 NUMBER OF BASIC VARIABLES (ALLOCATIONS) — DEGENERACY

**Rule:** A valid (non-degenerate) transportation solution must have exactly:
```
Number of allocations = m + n - 1
Where: m = number of rows (sources), n = number of columns (destinations)
```

In our example: m=3, n=4 → Allocations needed = 3+4-1 = **6**

Our VAM solution has 5 allocations → **DEGENERATE!**

**Handling Degeneracy:** Add a small quantity ε (epsilon, nearly zero) to any unoccupied independent cell to make the number of allocations = m+n-1.

---

## 🔵 OPTIMALITY TEST — MODI METHOD (U-V Method)

After getting an initial solution, we must check if it is optimal (can't be improved).

**MODI (Modified Distribution) Method Steps:**

1. Assign u values (for rows) and v values (for columns) such that for each occupied cell: **uᵢ + vⱼ = cᵢⱼ**
2. Set u₁ = 0 (arbitrary start)
3. Solve for all u and v values
4. Calculate opportunity cost for each **unoccupied** cell: **dᵢⱼ = cᵢⱼ - uᵢ - vⱼ**
5. If all dᵢⱼ ≥ 0 → OPTIMAL (no improvement possible)
6. If any dᵢⱼ < 0 → NOT optimal; bring that cell into solution (loop adjustment)

---

## 🔵 COMPARISON OF INITIAL SOLUTION METHODS

| Method | Considers Costs? | Quality | Complexity |
|--------|-----------------|---------|-----------|
| **NWCM** | NO | Poor (highest cost) | Easiest |
| **LCM** | YES (directly) | Good | Moderate |
| **VAM** | YES (penalties) | Best (closest to optimal) | Harder |

**Best Practice for Exam:**
- Always use VAM for initial solution (unless question specifies otherwise)
- Then test with MODI for optimality

---

## 🔴 EXAM-READY CONTENT

### Quick Exam Template for Transportation Problem:

```
Step 1: Check if balanced (ΣSupply = ΣDemand). If not, add dummy.
Step 2: Apply VAM to get initial basic feasible solution.
Step 3: Calculate total cost = Σ(allocation × cost)
Step 4: Check allocations = m+n-1 (degeneracy check)
Step 5: Apply MODI to test optimality
Step 6: If optimal, report solution. If not, improve.
```

### Key Points to Write in Any Exam Answer:
1. Draw the transportation table clearly with all costs
2. Show penalty calculation for each row and column (VAM)
3. Show allocation table clearly
4. Calculate total cost step by step
5. Check degeneracy (m+n-1 rule)

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Transportation Problem | Allocate supply to demand at minimum transportation cost |
| Balanced | Total supply = Total demand |
| NWCM | Start top-left; fill mechanically; ignores costs |
| LCM | Allocate to cheapest cell first; considers costs |
| VAM | Calculate penalties; allocate to min-cost in max-penalty row/col; best initial solution |
| Basic Variables | Cells with allocations (must be m+n-1) |
| Non-Basic Variables | Unoccupied cells (candidates for entry) |
| Degeneracy | Fewer than m+n-1 allocations; fix with ε |
| MODI Method | Optimality test using u-v values and opportunity costs |
| Shadow Price | Opportunity cost of non-basic cell in MODI |
| Dummy | Row or column with zero costs added to balance supply/demand |

---

*Chapter 2 Complete | DMO | MBA 2nd Semester, DU SOL*
