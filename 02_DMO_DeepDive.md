# 📘 DEEP DIVE: Decision Modelling and Optimization
### MBA 2nd Semester | DU SOL | Subject 10
**Prepared in IIM Format | Quantitative Methods for Managerial Decision Making**

---

> **How to Use:** This is a quantitative subject. Focus on understanding the **logic** of each model, learn the **formulas**, and practice with the **worked examples**. Every chapter has real-life applications — connect models to business problems.

---

## 📌 CHAPTER 1: Model Building for Optimization & Distribution and Network Models

### 1.1 What is a Model?

**Definition:**
A model is a simplified mathematical representation of a real-world system or problem used to analyze, understand, and optimize decisions.

**Types of Models:**
| Type | Description | Example |
|------|-------------|---------|
| **Physical** | Scaled-down replica | Prototype of a new product |
| **Schematic** | Diagram or flowchart | Process flow in a factory |
| **Mathematical** | Equations and formulas | Linear programming for production mix |

---

### 1.2 Linear Programming (LP) — The Foundation

**Definition:**
Linear Programming is a mathematical technique for optimizing (maximizing or minimizing) a linear objective function subject to a set of linear constraints.

**Standard Form:**
```
Maximize (or Minimize):  Z = c₁x₁ + c₂x₂ + ... + cₙxₙ
Subject to:              a₁₁x₁ + a₁₂x₂ ≤ b₁
                         a₂₁x₁ + a₂₂x₂ ≤ b₂
                         x₁, x₂ ≥ 0
```

**Key Terms:**
- **Objective Function:** The quantity to be optimized (profit, cost, time)
- **Decision Variables:** The unknowns we are solving for (x₁, x₂)
- **Constraints:** Limitations on resources (time, material, capacity)
- **Feasible Region:** Set of all points satisfying all constraints
- **Optimal Solution:** Point in feasible region giving best objective value

**Worked Example — Production Mix Problem:**
A company makes two products A and B.
- Profit: A = ₹5/unit, B = ₹4/unit
- Machine hours: A needs 2 hrs, B needs 1 hr; Total available = 40 hrs
- Labour hours: A needs 1 hr, B needs 2 hrs; Total available = 40 hrs

```
Maximize: Z = 5x₁ + 4x₂
Subject to: 2x₁ + x₂ ≤ 40  (Machine)
            x₁ + 2x₂ ≤ 40  (Labour)
            x₁, x₂ ≥ 0
```
**Solution via Corner Points:**
Corner points of feasible region: (0,0), (20,0), (0,20), (13.3, 13.3)
- Z at (13.3, 13.3) = 5(13.3) + 4(13.3) = 66.5 + 53.3 = **₹119.6 (Maximum)**

---

### 1.3 Transportation Model

**Definition:**
The Transportation Model is a special LP used to determine the most cost-effective way to transport goods from multiple sources (supply points) to multiple destinations (demand points).

**Structure:**
- **Supply:** Amount available at each source
- **Demand:** Amount required at each destination
- **Cost Matrix:** Cost of shipping one unit from each source to each destination

**Methods to Find Initial Solution:**
1. **North-West Corner Method** — Start top-left, allocate as much as possible
2. **Least Cost Method (LCM)** — Start with cheapest cell first
3. **Vogel's Approximation Method (VAM)** — Most accurate initial solution; uses opportunity costs

**Optimality Test:** Modified Distribution (MODI) Method / Stepping Stone Method

**Real-life Application:**
Indian Railways uses transportation models to allocate goods wagons from depots to loading stations minimizing empty running costs.

---

### 1.4 Assignment Model

**Definition:**
The Assignment Model allocates n jobs to n machines (or workers to tasks) on a one-to-one basis to minimize total cost or time.

**Hungarian Algorithm Steps:**
1. Row reduction (subtract row minimum from each row)
2. Column reduction (subtract column minimum from each column)
3. Cover all zeros with minimum number of lines
4. If lines = n → optimal; else adjust and repeat

**Real-life Example:** Assigning sales representatives to territories to minimize travel costs.

---

### 1.5 Network Models

**Definition:**
Network Models represent problems as a network of nodes (points) and arcs (connections) to optimize flow, path, or span.

**Key Network Models:**

| Model | Goal | Example |
|-------|------|---------|
| **Shortest Path** | Find minimum distance path | Google Maps routing |
| **Maximum Flow** | Maximize flow through a network | Pipeline, internet traffic |
| **Minimum Spanning Tree** | Connect all nodes at minimum total cost | Telecom cable laying, railway networks |

**Dijkstra's Algorithm** — Used for shortest path problem.

**Real-life Application:** Amazon's warehouse-to-customer delivery routing uses shortest path algorithms to minimize delivery time.

---

## 📌 CHAPTER 2: Multicriteria Decision Models

### 2.1 What is a Multicriteria Decision?

**Definition:**
Multicriteria Decision Making (MCDM) involves selecting the best alternative from a set of options when there are multiple, often conflicting criteria to evaluate.

**Example:** Selecting a vendor — criteria include price, quality, delivery speed, and reliability. No single vendor excels on all dimensions.

---

### 2.2 Goal Programming

**Definition:**
Goal Programming is an extension of LP that allows optimization of multiple objectives simultaneously. Instead of a single objective, it tries to achieve multiple "goals" and minimizes the deviation from these goals.

**Key Concept — Deviational Variables:**
- **d⁻ (Under-achievement):** How much below the goal we are
- **d⁺ (Over-achievement):** How much above the goal we are

**Example:**
A company has two goals:
- Goal 1: Achieve profit of at least ₹10,000
- Goal 2: Keep labour hours ≤ 200

```
Minimize: d₁⁻ + d₂⁺
Subject to: Profit constraint + d₁⁻ - d₁⁺ = 10,000
            Labour constraint + d₂⁻ - d₂⁺ = 200
```

---

### 2.3 Analytic Hierarchy Process (AHP)

**Definition:**
AHP (developed by Thomas Saaty) is a structured technique for organizing and analyzing complex decisions with multiple criteria using pairwise comparisons.

**Steps:**
1. Define the decision goal
2. Identify criteria and alternatives
3. Make pairwise comparisons (1-9 scale: 1=Equal, 9=Extremely preferred)
4. Calculate priority weights (Eigenvector method)
5. Check Consistency Ratio (CR < 0.10 = acceptable)
6. Calculate overall ranking of alternatives

**Saaty's Scale:**
| Value | Meaning |
|-------|---------|
| 1 | Equal importance |
| 3 | Moderate importance |
| 5 | Strong importance |
| 7 | Very strong importance |
| 9 | Extreme importance |

**Real-life Example:** The Government of India uses AHP-like frameworks for evaluating infrastructure project bids — weighing cost, technical capability, timeline, and past experience.

---

## 📌 CHAPTER 3: Waiting Line Models (Queuing Theory)

### 3.1 What is a Waiting Line (Queue)?

**Definition:**
Queuing Theory is the mathematical study of waiting lines (queues) to analyze and design systems that serve customers efficiently.

**Why it matters in business:**
- Too few servers → Long queues → Customer dissatisfaction
- Too many servers → Idle capacity → Increased cost
- **Goal:** Optimal balance between service cost and waiting cost

---

### 3.2 Components of a Queuing System

| Component | Description | Example |
|-----------|-------------|---------|
| **Arrival Process** | How customers arrive | Random (Poisson distribution) |
| **Service Process** | How long service takes | Exponential distribution |
| **Number of Servers** | Single or multiple channels | Bank tellers |
| **Queue Discipline** | Order of service | FCFS (First Come First Served) |
| **Queue Capacity** | Max customers in system | Finite or Infinite |

---

### 3.3 Kendall's Notation: A/B/C/D/E

- **A** = Arrival distribution (M = Markovian/Poisson, D = Deterministic)
- **B** = Service distribution (M = Exponential, D = Deterministic)
- **C** = Number of servers
- **D** = System capacity (default = ∞)
- **E** = Population size (default = ∞)

Most common model: **M/M/1** — Single server, Poisson arrivals, Exponential service

---

### 3.4 M/M/1 Queue Formulas

**Given:**
- λ = Arrival rate (customers per hour)
- μ = Service rate (customers per hour)
- ρ = λ/μ = Traffic intensity (must be < 1 for stable system)

**Key Performance Measures:**

| Measure | Formula | Meaning |
|---------|---------|---------|
| **Lq** | λ²/μ(μ-λ) | Avg customers waiting in queue |
| **L** | λ/(μ-λ) | Avg customers in system |
| **Wq** | λ/μ(μ-λ) | Avg waiting time in queue |
| **W** | 1/(μ-λ) | Avg time in system |
| **P₀** | 1 - ρ | Probability system is idle |
| **Pₙ** | (1-ρ)ρⁿ | Probability of n customers in system |

**Worked Example:**
A bank has 1 teller. Customers arrive at λ = 10/hr. Service rate μ = 15/hr.
- ρ = 10/15 = 0.667
- L = 10/(15-10) = **2 customers** in system
- W = 1/(15-10) = **0.2 hrs = 12 minutes** in system
- Lq = (10²)/(15×5) = **1.33 customers** waiting
- Wq = 10/(15×5) = **0.133 hrs = 8 minutes** waiting

---

### 3.5 Real-Life Applications

| Situation | Queuing Model Used |
|-----------|-------------------|
| Bank teller counters | M/M/s (multi-server) |
| Call centre staffing | M/M/s with finite capacity |
| Hospital emergency rooms | Priority queuing |
| Airport check-in | M/M/s |
| UPI transaction processing | M/D/1 |

**Case Study — Domino's Pizza "30 Minutes or Free" Guarantee:**
Domino's modeled its delivery operations using queuing theory. By analyzing arrival rates (orders), service times (preparation + delivery), and traffic patterns, they optimized store locations and staffing to reliably meet the 30-minute guarantee. This became their core competitive strategy.

---

## 📌 CHAPTER 4: Simulation

### 4.1 What is Simulation?

**Definition:**
Simulation is the process of building a mathematical or computer model of a real system and conducting experiments on it to understand system behavior or evaluate alternative strategies without disturbing the real system.

**When to Use Simulation:**
- System is too complex for analytical solution
- Real-world experimentation is expensive or dangerous
- Need to test "what-if" scenarios

---

### 4.2 Monte Carlo Simulation

**Definition:**
Monte Carlo Simulation uses random numbers to simulate probabilistic events and approximate complex outcomes.

**Steps:**
1. Identify the probability distribution of the variable
2. Set up cumulative probability intervals
3. Generate random numbers
4. Map random numbers to variable values
5. Repeat for N iterations
6. Analyze results

**Worked Example — Inventory Demand Simulation:**

| Demand/Day | Probability | Cumulative Probability | Random Number Range |
|------------|-------------|----------------------|---------------------|
| 10 | 0.20 | 0.20 | 00-19 |
| 20 | 0.35 | 0.55 | 20-54 |
| 30 | 0.30 | 0.85 | 55-84 |
| 40 | 0.15 | 1.00 | 85-99 |

If Random Number = 67 → Demand = 30 units

---

### 4.3 Applications of Simulation

| Application | Use |
|-------------|-----|
| Financial Modeling | Monte Carlo for option pricing (Black-Scholes) |
| Supply Chain | Testing inventory policies |
| Manufacturing | Evaluating production line changes |
| Healthcare | Modeling patient flow in hospitals |
| Traffic | NHAI uses simulation for highway design |

**Case Study — Flipkart Big Billion Days:**
Flipkart uses simulation models to test server load, warehouse throughput, and logistics capacity before its annual Big Billion Days sale. By running millions of simulated transactions, they identify bottlenecks and scale resources appropriately — preventing the embarrassing crashes of 2014.

---

## 📌 CHAPTER 5: Decision-Making under Uncertainty

### 5.1 Decision Theory Framework

**Types of Decision Environments:**

| Environment | What is Known | Example |
|-------------|---------------|---------|
| **Certainty** | Outcomes known with certainty | Buying government bonds |
| **Risk** | Probability of outcomes known | Insurance pricing |
| **Uncertainty** | Probabilities unknown | Launching new product in unknown market |

---

### 5.2 Decision Criteria under Uncertainty

**Given:** A payoff table with alternatives (rows) and states of nature (columns)

| Alternative | State 1 (Good) | State 2 (Average) | State 3 (Bad) |
|-------------|---------------|------------------|--------------|
| A (Expand) | 200 | 100 | -50 |
| B (Maintain) | 100 | 100 | 60 |
| C (Contract) | 40 | 40 | 40 |

**1. Maximax Criterion (Optimistic — Best of Best):**
Choose the alternative with the maximum of maximum payoffs.
- Max of A = 200, B = 100, C = 40 → **Choose A**

**2. Maximin Criterion (Pessimistic — Best of Worst):**
Choose the alternative with the maximum of minimum payoffs.
- Min of A = -50, B = 60, C = 40 → **Choose B** (maximum of minimums = 60)

**3. Minimax Regret Criterion (Savage Criterion):**
Minimize the maximum "regret" (opportunity loss).
- Calculate regret = Best payoff in that state - Actual payoff
- Choose alternative with minimum of maximum regrets

**4. Hurwicz Criterion (Coefficient of Optimism — α):**
H = α × Maximum payoff + (1-α) × Minimum payoff
- If α = 0.6 for Alternative A: H = 0.6(200) + 0.4(-50) = 120 - 20 = **100**

**5. Laplace Criterion (Equal Probability):**
Assume all states equally likely; choose highest average payoff.
- Average A = (200+100-50)/3 = 83.3
- Average B = (100+100+60)/3 = 86.7 → **Choose B**

---

### 5.3 Decision Tree Analysis

**Definition:**
A Decision Tree is a graphical representation of sequential decisions and their possible outcomes, used to evaluate complex multi-stage decisions.

**Symbols:**
- **□ Square node** = Decision node (we choose)
- **○ Circle node** = Chance node (nature chooses)
- **→ Branch** = Alternative or outcome

**Key Calculation — Expected Monetary Value (EMV):**
EMV = Σ (Probability × Payoff) for each branch

**Real-life Example:** Pharma companies use decision trees to decide whether to invest in clinical trials (high cost, uncertain outcome) vs. licensing existing drugs.

---

## 📌 CHAPTER 6: Project Scheduling (PERT & CPM)

### 6.1 Overview

**CPM (Critical Path Method):** Deterministic — activity times are known with certainty. Used in construction projects.

**PERT (Program Evaluation and Review Technique):** Probabilistic — activity times are uncertain. Used in R&D, software projects.

---

### 6.2 Key Concepts

| Term | Definition |
|------|------------|
| **Activity** | A specific task in the project |
| **Event/Node** | Start or end of an activity |
| **Network Diagram** | AOA (Activity on Arrow) or AON (Activity on Node) |
| **Critical Path** | Longest path through network = Minimum project duration |
| **Slack/Float** | Extra time available for non-critical activities |
| **EST** | Earliest Start Time |
| **LFT** | Latest Finish Time |

**Critical Path:** All activities on this path have **Zero Slack**. Delay in any critical activity delays the entire project.

---

### 6.3 PERT Time Estimates

PERT uses three time estimates:
- **Optimistic time (a):** Best-case scenario
- **Most Likely time (m):** Most probable
- **Pessimistic time (b):** Worst-case scenario

**Expected Time:** `te = (a + 4m + b) / 6`

**Variance:** `σ² = [(b - a) / 6]²`

**Worked Example:**
Activity: a=2, m=5, b=8
- te = (2 + 4×5 + 8)/6 = (2+20+8)/6 = **30/6 = 5 weeks**
- σ² = [(8-2)/6]² = [1]² = **1**

---

### 6.4 Real-Life Application

**Case Study — Delhi Metro Rail Corporation (DMRC):**
DMRC used CPM/PERT extensively for Phase 1-4 planning.
- Network of 1000+ activities (tunneling, station construction, track laying, electrification)
- Critical path identified across 8 years of construction
- Crashing (time-cost tradeoff) used to meet 2010 Commonwealth Games deadline
- DMRC's Phase 1 completion 3 months AHEAD of schedule — credited to rigorous CPM use

---

## 📌 CHAPTER 7: Markov Processes

### 7.1 What is a Markov Process?

**Definition:**
A Markov Process (or Markov Chain) is a stochastic process where the future state depends ONLY on the current state, not on the history of past states. This is called the **Markovian Property** or **Memoryless Property**.

**"The future is independent of the past given the present."**

---

### 7.2 Key Concepts

| Term | Definition |
|------|------------|
| **State** | Possible condition the system can be in |
| **Transition Probability** | Probability of moving from one state to another |
| **Transition Matrix (P)** | Matrix of all transition probabilities |
| **Steady State** | Long-run equilibrium probabilities (don't change over time) |
| **Absorbing State** | State once entered, cannot be left |

---

### 7.3 Transition Matrix

**Example — Brand Switching:**
Two brands: Brand A and Brand B
```
         Next Period
         A      B
Current  A [0.8  0.2]  = P
Period   B [0.3  0.7]
```
- P(A→A) = 0.8 (80% stay with Brand A)
- P(A→B) = 0.2 (20% switch to Brand B)
- P(B→A) = 0.3 (30% switch to Brand A)
- P(B→B) = 0.7 (70% stay with Brand B)

**Steady State Calculation:**
πA = πA(0.8) + πB(0.3) and πA + πB = 1
Solving: **πA = 0.6, πB = 0.4**
→ In the long run, Brand A holds 60% market share.

---

### 7.4 Business Applications

| Application | Markov Use |
|-------------|------------|
| **Brand Switching** | Predict future market share |
| **Credit Risk** | Track loan from "Current" → "Delinquent" → "Default" |
| **Customer Retention** | Model churn from Active → Inactive → Churned |
| **Machine States** | Working → Degraded → Failed |
| **Insurance** | Actuarial models for health transitions |

**Real-life:** Indian credit rating agencies (CRISIL) use Markov chains to model corporate bond rating transitions (AAA → AA → A → BBB → Default) to price credit risk.

---

## 📌 CHAPTER 8: Theory of Games

### 8.1 What is Game Theory?

**Definition:**
Game Theory is the mathematical study of strategic interactions among rational decision-makers (players) where each player's outcome depends on the actions of others.

> *"Game Theory is the study of how people behave in strategic situations."* — Gregory Mankiw

**Nobel Prize:** John Nash (1994), Harsanyi, Selten — for contributions to Game Theory.

---

### 8.2 Key Concepts

| Term | Definition |
|------|------------|
| **Player** | Decision maker (firm, person, country) |
| **Strategy** | Complete plan of action for all situations |
| **Payoff** | Outcome/reward from a combination of strategies |
| **Zero-Sum Game** | One player's gain = other's loss (total = 0) |
| **Non-Zero Sum** | Both can gain or both can lose |
| **Dominant Strategy** | Best strategy regardless of what opponent does |
| **Saddle Point** | Equilibrium in pure strategy (minimax = maximin) |
| **Nash Equilibrium** | No player can improve payoff by changing strategy alone |

---

### 8.3 Two-Person Zero-Sum Game

**Payoff Matrix (Row player's perspective):**
```
              Column Player
              C1    C2
Row Player R1 [4     2 ]
           R2 [1     6 ]
```

**Maximin (Row player — maximize minimum gain):**
- Min of R1 = 2; Min of R2 = 1 → Maximin = **2** → Choose R1

**Minimax (Column player — minimize maximum loss):**
- Max of C1 = 4; Max of C2 = 6 → Minimax = **4** → Choose C1

**Saddle Point:** If Maximin = Minimax → Pure Strategy Saddle Point
Here: 2 ≠ 4 → No saddle point → Use Mixed Strategy

---

### 8.4 Mixed Strategy

When no saddle point exists, each player randomizes their strategy.

**For 2x2 game:**
```
Payoff Matrix:  [a  b]
                [c  d]
```
Row player's optimal probability p for strategy R1:
`p = (d - c) / [(a - b) - (c - d)]`

---

### 8.5 Prisoner's Dilemma — Classic Case

**Situation:** Two criminals arrested. Cannot communicate.
```
                  Partner Stays Silent   Partner Confesses
You Stay Silent      (-1, -1)              (-10, 0)
You Confess          (0, -10)              (-5, -5)
```
**Nash Equilibrium:** Both confess (dominant strategy for each) → Both get 5 years
**But:** If both stayed silent → Both get only 1 year (better outcome)

**Business Application:** Price wars between airlines (Jet Airways vs. Air India). Each reduces price expecting to gain market share — both end up with lower profits. Cooperation (cartel/price fixing) would be better but is illegal.

---

### 8.6 Applications of Game Theory

| Scenario | Application |
|----------|-------------|
| **Competitive Pricing** | Petrol pump price wars |
| **Auctions** | Spectrum auction (TRAI India) |
| **Negotiation** | Labor-management wage talks |
| **Entry Deterrence** | Reliance Jio's predatory pricing to deter competition |
| **Arms Race** | Nuclear deterrence strategy |
| **Mergers & Acquisitions** | Bidding strategies |

**Case Study — Reliance Jio and Game Theory:**
When Jio entered telecom in 2016, it offered free data and calls for 6 months. This was a dominant strategy:
- If competitors matched → They lose revenue
- If competitors didn't match → Jio captures market
Incumbents (Airtel, Vodafone, Idea) couldn't match long enough → Market consolidated from 12 players to 3.
This is textbook **Game Theory — Entry Deterrence** in action.

---

## MASTER SUMMARY TABLE

| Chapter | Core Topic | Key Tool/Formula | Key Author/Developer |
|---------|-----------|------------------|---------------------|
| 1 | LP & Network Models | Simplex, Transportation, Hungarian, Dijkstra | Dantzig (Simplex) |
| 2 | Multicriteria Decisions | Goal Programming, AHP (Pairwise Matrix) | Thomas Saaty (AHP) |
| 3 | Queuing Theory | M/M/1 formulas: L, Lq, W, Wq | Erlang |
| 4 | Simulation | Monte Carlo Method | Von Neumann |
| 5 | Decision under Uncertainty | Maximax, Maximin, Minimax Regret, Decision Tree | Savage (Minimax Regret) |
| 6 | Project Scheduling | PERT (te formula), CPM, Critical Path | DuPont (CPM), US Navy (PERT) |
| 7 | Markov Processes | Transition Matrix, Steady State (πP=π) | Andrei Markov |
| 8 | Game Theory | Minimax, Saddle Point, Nash Equilibrium | Von Neumann, Nash |

---

*Document prepared for MBA 2nd Semester, DU SOL | Subject: Decision Modelling and Optimization*
*For Academic Use Only*
