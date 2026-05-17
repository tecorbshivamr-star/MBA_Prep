# 📗 DMO CHAPTER 1: Linear Programming (LP)
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

A factory makes **two products** — Chairs and Tables. Both use **limited** wood and labour. The manager wants to know: **How many chairs and how many tables should I make to earn maximum profit?**

This is a **Linear Programming** problem. LP helps find the **BEST (optimal) decision** when you have:
- A goal to maximize or minimize (profit, cost)
- Limited resources (raw material, labour, machine hours)
- Choices about how to use those resources

Real life LP uses:
- Airlines deciding how many seats to allocate to each fare class
- Reliance deciding which refinery products to produce in what quantities
- Army deciding how to allocate resources to different missions

---

## 🔵 WHAT IS LINEAR PROGRAMMING?

**Definition:**
Linear Programming (LP) is a mathematical optimization technique used to find the best outcome (maximum profit or minimum cost) in a mathematical model whose requirements are represented by **linear relationships**.

**Why "Linear"?** Because all equations are straight lines (no x², no √x — just x multiplied by a constant).

---

## 🔵 KEY CONDITIONS FOR LP

For a problem to be solvable by LP, four conditions must hold:

| Condition | Meaning | Example |
|-----------|---------|---------|
| **Linearity** | All relationships are linear | Profit = 5x₁ + 4x₂ (not 5x₁²) |
| **Certainty** | All parameters (profit, resource use) are known and fixed | Profit per chair = ₹5 always |
| **Proportionality** | Resource use is proportional to production | Making 2 chairs uses 2× resources of 1 chair |
| **Non-negativity** | Decision variables must be ≥ 0 | Cannot produce negative chairs |
| **Divisibility** | Variables can take fractional values (in LP) | Can produce 2.5 chairs (Integer LP handles this separately) |

---

## 🔵 LP TERMINOLOGY

| Term | Definition | Example |
|------|-----------|---------|
| **Decision Variables** | What we are deciding (unknowns) | x₁ = chairs, x₂ = tables |
| **Objective Function** | What we want to maximize or minimize | Maximize Z = 5x₁ + 4x₂ |
| **Constraints** | Limitations on resources | 2x₁ + 4x₂ ≤ 40 (wood available) |
| **Non-negativity Constraints** | Variables must be ≥ 0 | x₁ ≥ 0, x₂ ≥ 0 |
| **Feasible Region** | All solutions that satisfy ALL constraints | The shaded area on graph |
| **Optimal Solution** | Best feasible solution (highest/lowest Z) | Corner point giving max Z |
| **Feasible Solution** | Any solution satisfying all constraints | Multiple solutions exist |

---

## 🔵 LP FORMULATION — STEP BY STEP ⭐

### The 4-Step Formulation Process:

**Step 1: Identify Decision Variables**
What are we deciding how many of?

**Step 2: Write the Objective Function**
What is the goal? (Maximize profit OR Minimize cost)

**Step 3: Write the Constraints**
What are the resource limitations?

**Step 4: State Non-negativity Constraints**
All variables ≥ 0

---

### WORKED EXAMPLE — Furniture Factory:

**Problem:**
A furniture maker produces Chairs (C) and Tables (T).
- Chair: ₹300 profit, requires 2 hrs wood cutting + 4 hrs assembly
- Table: ₹500 profit, requires 3 hrs wood cutting + 2 hrs assembly
- Available: 120 hrs wood cutting, 160 hrs assembly per week
- Demand constraint: Max 40 tables per week
- Find: Optimal production mix for maximum profit

**Step 1 — Decision Variables:**
```
x₁ = Number of Chairs produced per week
x₂ = Number of Tables produced per week
```

**Step 2 — Objective Function:**
```
Maximize Z = 300x₁ + 500x₂
```

**Step 3 — Constraints:**
```
Wood cutting:  2x₁ + 3x₂ ≤ 120    [wood cutting hours]
Assembly:      4x₁ + 2x₂ ≤ 160    [assembly hours]
Table demand:  x₂ ≤ 40             [maximum tables]
```

**Step 4 — Non-negativity:**
```
x₁ ≥ 0, x₂ ≥ 0
```

**Complete LP Model:**
```
Maximize Z = 300x₁ + 500x₂
Subject to:
    2x₁ + 3x₂ ≤ 120
    4x₁ + 2x₂ ≤ 160
    x₂ ≤ 40
    x₁, x₂ ≥ 0
```

---

## 🔵 GRAPHICAL METHOD (For 2 Variables)

### Steps:

**Step 1:** Convert each inequality constraint to equality → Plot as straight line

**Step 2:** Determine which side of each line is feasible (satisfies ≤)

**Step 3:** Identify the Feasible Region (intersection of all constraints)

**Step 4:** Find corner points (vertices) of the feasible region

**Step 5:** Calculate Z at each corner point

**Step 6:** Corner point with highest Z (for maximization) = OPTIMAL SOLUTION

---

### Solving the Furniture Example:

**Step 1 — Plot constraint lines:**

For **2x₁ + 3x₂ = 120:**
- Set x₁ = 0: x₂ = 40 → Point (0, 40)
- Set x₂ = 0: x₁ = 60 → Point (60, 0)
- Draw line through (0,40) and (60,0)

For **4x₁ + 2x₂ = 160:**
- Set x₁ = 0: x₂ = 80 → Point (0, 80)
- Set x₂ = 0: x₁ = 40 → Point (40, 0)
- Draw line through (0,80) and (40,0)

For **x₂ = 40:**
- Horizontal line at x₂ = 40

**Step 2 — Find corner points of feasible region:**

Corner points are intersections of constraint boundaries:

**Corner A (0, 0):** Origin
```
Z = 300(0) + 500(0) = ₹0
```

**Corner B (40, 0):** Intersection of x-axis and assembly constraint
```
Z = 300(40) + 500(0) = ₹12,000
```

**Corner C — Intersection of wood cutting and assembly:**
Solve simultaneously:
```
2x₁ + 3x₂ = 120  →  Multiply by 2:  4x₁ + 6x₂ = 240
4x₁ + 2x₂ = 160
Subtract:  4x₂ = 80 → x₂ = 20
Substitute: 2x₁ + 3(20) = 120 → 2x₁ = 60 → x₁ = 30
Corner C = (30, 20)
Z = 300(30) + 500(20) = 9,000 + 10,000 = ₹19,000
```

**Corner D — Intersection of wood cutting and table demand (x₂=40):**
```
2x₁ + 3(40) = 120 → 2x₁ = 0 → x₁ = 0
Corner D = (0, 40)
Z = 300(0) + 500(40) = ₹20,000
```

**But check: Is (0,40) feasible for assembly constraint?**
```
4(0) + 2(40) = 80 ≤ 160 ✓
```
Yes, feasible!

**Summary of Corner Points:**

| Corner | x₁ (Chairs) | x₂ (Tables) | Z (Profit) |
|--------|------------|------------|-----------|
| A | 0 | 0 | ₹0 |
| B | 40 | 0 | ₹12,000 |
| **C** | **30** | **20** | **₹19,000** |
| **D** | **0** | **40** | **₹20,000** ← OPTIMAL |

**OPTIMAL SOLUTION:**
Produce **0 Chairs and 40 Tables** → Maximum Profit = **₹20,000/week**

---

## 🔵 SIMPLEX METHOD (For Multiple Variables)

The Graphical Method only works for 2 variables. The Simplex Method handles many variables algebraically.

**Key Concepts:**

**Slack Variable:** Added to convert ≤ inequality to equality
```
2x₁ + 3x₂ ≤ 120  becomes  2x₁ + 3x₂ + s₁ = 120
(s₁ = unused wood cutting capacity = "slack")
```

**Basic Feasible Solution (BFS):** A corner point solution in algebraic form

**Pivot Operation:** Mathematical operation to move from one corner point to a better one

**Entering Variable:** Variable that enters the basis (enters the solution)

**Leaving Variable:** Variable that leaves the basis

**Optimality Condition:** Z row coefficients all ≥ 0 (for maximization) → No further improvement possible

> **MBA Exam Note:** For most MBA exams, you need to UNDERSTAND the logic of Simplex, not necessarily execute 5 iterations by hand. Focus on graphical method for 2-variable problems.

---

## 🔵 SPECIAL CASES IN LP

| Case | Description | How to Identify |
|------|-------------|----------------|
| **Infeasibility** | No solution satisfies all constraints | Feasible region is EMPTY (constraints contradict each other) |
| **Unboundedness** | Objective can be increased infinitely | Feasible region has no boundary in the direction of improvement |
| **Multiple Optima** | Two or more optimal solutions with same Z | Objective function line is parallel to a constraint line |
| **Degeneracy** | More than one constraint passes through same corner point | Corner point determined by 3+ constraints (in 2D) |

---

## 🔵 SENSITIVITY ANALYSIS & SHADOW PRICE ⭐

After solving LP, managers want to know: **"What if something changes?"**

### Ranging (Sensitivity Analysis):
- How much can objective function coefficients change before optimal solution changes?
- How much can RHS of constraints change before optimal basis changes?

### Shadow Price (Dual Value): ⭐ Most Asked
**Definition:** The increase in the optimal objective function value per unit increase in the RHS of a binding constraint.

**Interpretation:**
- If Shadow Price of wood constraint = ₹150: Getting one more hour of wood cutting would increase maximum profit by ₹150
- A manager can justify paying UP TO ₹150 for one additional hour of wood cutting capacity

**Key Rules:**
- Only BINDING constraints (used fully at optimum) have non-zero shadow prices
- Slack constraints (not fully used) have shadow price = 0
- Shadow price valid only within the ranging interval

**India Application:**
An oil refinery (like HPCL) uses LP to decide how much petrol, diesel, and kerosene to refine from crude oil. Shadow prices tell management how much extra value each additional barrel of crude oil creates — helping justify crude oil purchase decisions.

---

## 🔵 APPLICATIONS OF LP IN INDIA

| Application | Industry | Decision |
|-------------|----------|---------|
| **Product mix** | Manufacturing (Maruti, HUL) | Which products to produce in what quantities |
| **Media planning** | Advertising (HUL, P&G campaigns) | Which media channels to buy for min cost, max reach |
| **Feed mix** | Animal husbandry, NDDB (Amul) | Cheapest feed mix meeting nutritional requirements |
| **Portfolio optimization** | Finance (mutual funds, HDFC MF) | Allocation across assets for max return, min risk |
| **Transportation** | FMCG supply chain | Min cost routing from factories to warehouses |
| **Staff scheduling** | Airlines (IndiGo crew scheduling) | Min cost crew assignment meeting all regulations |

---

## 🔴 EXAM-READY CONTENT

### Full 10-Mark LP Problem:

**Q. A company makes two products P and Q.**
- P: Profit ₹60/unit; requires 2 hrs machine + 1 hr labour
- Q: Profit ₹80/unit; requires 1 hr machine + 3 hrs labour
- Available: 120 machine hours, 150 labour hours per week
- Maximum demand: Q ≤ 60 units
- Formulate and solve graphically. Find optimal solution and maximum profit.

**Ans:**

**Step 1 — Decision Variables:**
```
x₁ = Units of P produced; x₂ = Units of Q produced
```

**Step 2 — Objective Function:**
```
Maximize Z = 60x₁ + 80x₂
```

**Step 3 — Constraints:**
```
Machine: 2x₁ + x₂ ≤ 120
Labour:  x₁ + 3x₂ ≤ 150
Demand:  x₂ ≤ 60
Non-neg: x₁, x₂ ≥ 0
```

**Step 4 — Corner Points:**

Point A (0,0): Z = 0
Point B (60,0): Z = 60(60) + 0 = ₹3,600
Point C — Intersection of Machine and Labour:
```
2x₁ + x₂ = 120 → x₂ = 120-2x₁
x₁ + 3(120-2x₁) = 150
x₁ + 360 - 6x₁ = 150
-5x₁ = -210 → x₁ = 42
x₂ = 120 - 2(42) = 36
Z = 60(42) + 80(36) = 2,520 + 2,880 = ₹5,400
```
Point D — Machine and demand (x₂=60):
```
2x₁ + 60 = 120 → x₁ = 30
Z = 60(30) + 80(60) = 1,800 + 4,800 = ₹6,600
```
Point E (0,50) — Labour and demand intersection:
```
x₁ + 3(60) = 150 → x₁ = -30 (infeasible!) 
So check (0,50) → Labour: 0 + 150 = 150 ✓; Machine: 0+50 = 50 ≤ 120 ✓
Z = 0 + 80(50) = ₹4,000
```
Check (0,60): Machine: 0+60=60 ✓; Labour: 0+180=180>150 ✗ Infeasible!

**Corner Points Summary:**
| Point | x₁ | x₂ | Z |
|-------|----|----|---|
| A | 0 | 0 | ₹0 |
| B | 60 | 0 | ₹3,600 |
| C | 42 | 36 | ₹5,400 |
| **D** | **30** | **60** | **₹6,600 ← MAX** |

**OPTIMAL: Produce 30 units of P and 60 units of Q → Maximum Profit = ₹6,600/week**

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Linear Programming | Optimization technique for linear objective + constraints |
| Decision Variables | The unknowns we are optimizing over |
| Objective Function | Mathematical expression of goal (maximize Z or minimize Z) |
| Constraint | Resource limitation expressed as inequality |
| Feasible Region | Set of all solutions satisfying all constraints |
| Corner Point Theorem | Optimal solution always lies at a corner of feasible region |
| Shadow Price | Value of one additional unit of a binding resource |
| Binding Constraint | Constraint fully used at optimal solution (no slack) |
| Slack Variable | Unused amount of a resource (added to convert ≤ to =) |
| Sensitivity Analysis | Study of how optimal solution changes with parameter changes |

---

*Chapter 1 Complete | DMO | MBA 2nd Semester, DU SOL*
