# 📗 DMO CHAPTER 7: Markov Chains
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

In the Indian telecom market, every month some Airtel customers switch to Jio, some Jio customers switch to Airtel, and others stay with their current provider.

Questions a telecom company asks:
- If a customer is with Airtel today, what's the probability they'll still be with Airtel next month?
- In the long run, what market share will each company have?
- Will market shares ever stabilize?

**Markov Chains** answer these questions. They model systems where the future state depends ONLY on the current state — not on how you got there.

---

## 🔵 WHAT IS A MARKOV CHAIN?

**Definition:**
A Markov Chain is a mathematical system that undergoes transitions from one state to another according to certain probabilistic rules. The key property is:

**The Markov Property:**
> The future state depends ONLY on the current state — NOT on the history of past states.

**Example:**
- Customer is with Airtel TODAY → Probability of switching TOMORROW depends only on being with Airtel today
- It doesn't matter if they were with Jio 3 months ago, or always with Airtel
- Past history is irrelevant — only the CURRENT state matters

This is called the **"memoryless" property**.

---

## 🔵 KEY COMPONENTS

| Component | Definition | Example |
|-----------|-----------|---------|
| **States** | Possible conditions the system can be in | {Airtel, Jio, Vi} |
| **Transition Probabilities** | Probability of moving from one state to another | P(Airtel→Jio) = 0.20 |
| **Transition Matrix (P)** | Matrix of all transition probabilities | 3×3 matrix for 3 brands |
| **State Vector (π)** | Current probability distribution across states | [0.40, 0.45, 0.15] = market shares |
| **Initial State Vector (π₀)** | State vector at time 0 | Today's market shares |

---

## 🔵 THE TRANSITION MATRIX ⭐

**Rules for Transition Matrix:**
1. Each element Pᵢⱼ = probability of moving FROM state i TO state j
2. Each ROW must sum to 1.0 (you must go somewhere!)
3. All elements must be ≥ 0

**Brand Switching Example:**

**Monthly Brand Switching Probabilities:**

| From\To | Airtel | Jio | Vi |
|---------|--------|-----|----|
| **Airtel** | 0.70 | 0.20 | 0.10 |
| **Jio** | 0.15 | 0.75 | 0.10 |
| **Vi** | 0.25 | 0.30 | 0.45 |

**Reading the Matrix:**
- An Airtel customer stays with Airtel: 70% probability
- An Airtel customer switches to Jio: 20% probability
- An Airtel customer switches to Vi: 10% probability
- ✓ Row sum: 0.70+0.20+0.10 = 1.00

---

## 🔵 STATE VECTOR AND TRANSITIONS

**Current State Vector (π₀):** Market shares today
```
π₀ = [Airtel: 0.40, Jio: 0.45, Vi: 0.15]
```

**After 1 Period (π₁):**
```
π₁ = π₀ × P
```

**Calculating π₁:**
```
Airtel next month = 0.40(0.70) + 0.45(0.15) + 0.15(0.25)
= 0.280 + 0.0675 + 0.0375 = 0.385

Jio next month = 0.40(0.20) + 0.45(0.75) + 0.15(0.30)
= 0.080 + 0.3375 + 0.0450 = 0.4625

Vi next month = 0.40(0.10) + 0.45(0.10) + 0.15(0.45)
= 0.040 + 0.0450 + 0.0675 = 0.1525

π₁ = [0.385, 0.4625, 0.1525]
```
**Check: 0.385 + 0.4625 + 0.1525 = 1.00 ✓**

**Interpretation:** After 1 month, Airtel's market share drops from 40% → 38.5%; Jio rises from 45% → 46.25%.

**After n Periods:**
```
πₙ = π₀ × Pⁿ
```

---

## 🔵 STEADY-STATE (EQUILIBRIUM) PROBABILITIES ⭐ Most Important

Over time, most Markov Chains settle into a **steady state** — probabilities stop changing from period to period.

**Definition:**
Steady-state probabilities (π*) are the long-run probabilities of being in each state, independent of the initial state.

**Property:**
```
π* = π* × P
```
(After one transition, distribution remains the same)

**Also:** Σπᵢ* = 1

---

### Solving for Steady State — 2 State Example:

**Simpler Example — Customer Retention:**

A subscription service (like Hotstar). Monthly transitions:
- Subscriber stays: 0.80; Cancels: 0.20
- Cancelled customer returns: 0.10; Stays cancelled: 0.90

**Transition Matrix:**
```
P = | 0.80  0.20 |   (from Subscriber)
    | 0.10  0.90 |   (from Cancelled)
```

**Let π* = [π₁, π₂] where π₁ = steady-state fraction of subscribers**

**Equations (from π* = π* × P):**
```
π₁ = π₁(0.80) + π₂(0.10)   ... (1)
π₂ = π₁(0.20) + π₂(0.90)   ... (2)
π₁ + π₂ = 1                  ... (3)
```

**From equation (1):**
```
π₁ = 0.80π₁ + 0.10π₂
π₁ - 0.80π₁ = 0.10π₂
0.20π₁ = 0.10π₂
π₂ = 2π₁
```

**Substitute into (3):**
```
π₁ + 2π₁ = 1
3π₁ = 1
π₁ = 1/3 = 0.333
π₂ = 2/3 = 0.667
```

**Steady-State: 33.3% subscribers, 66.7% cancelled (in long run)**

**Managerial Insight:** No matter where you start, the system converges to 33.3% subscriber rate. To improve this, the company must:
- Increase retention rate (0.80 → 0.90) → More stay subscribed
- Increase re-acquisition rate (0.10 → 0.15) → More cancelled return

---

### 3-State Steady-State Solving (Telecom Example):

For the Airtel/Jio/Vi example, solve simultaneously:
```
πA = 0.70πA + 0.15πJ + 0.25πV   ... (A)
πJ = 0.20πA + 0.75πJ + 0.30πV   ... (J)
πV = 0.10πA + 0.10πJ + 0.45πV   ... (V)
πA + πJ + πV = 1                  ... (sum)
```

Replace one equation with the sum equation and solve the 3×3 system. (In exams, this is often given as a 2-state problem; 3-state requires matrix algebra.)

---

## 🔵 TYPES OF STATES

| State Type | Definition | Example |
|-----------|-----------|---------|
| **Transient** | Eventually leaves and never returns | Bankrupt company state |
| **Recurrent/Persistent** | Returns with probability 1 | Regular customer states |
| **Absorbing** | Once entered, cannot leave | Death, bankruptcy |
| **Ergodic** | All states are recurrent + aperiodic | Most business Markov models |

**Absorbing State Example:**
In a loan status Markov chain: Current → 30-days overdue → 60-days overdue → **Written-off (Absorbing)**
Once "Written-off," you never leave that state.

---

## 🔵 FIRST PASSAGE TIME

**Definition:** Expected number of periods to first reach state j, starting from state i.

**Used for:** Expected time for a customer to churn, expected time for a loan to default.

---

## 🔵 APPLICATIONS IN INDIAN BUSINESS

| Application | States | Business Question |
|-------------|--------|------------------|
| **Brand switching** | Brands A, B, C | Long-run market share of each brand |
| **Customer lifetime value** | Active, Lapsed, Churned | Expected revenue over customer lifetime |
| **Credit risk** | Current, 30-day DPD, 60-day DPD, Default | Probability loan defaults |
| **Machine maintenance** | Working, Degraded, Failed | Long-run repair costs |
| **Stock market** | Bull, Neutral, Bear | Expected time in bull/bear market |
| **Employee status** | Employed, On leave, Resigned | Workforce planning |

---

## 🔴 EXAM-READY CONTENT

### Standard 2-State Exam Template:

**Given:** Transition matrix P = | p₁₁  p₁₂ |
                                 | p₂₁  p₂₂ |

**Find steady-state π* = [π₁, π₂]:**

```
Step 1: Write equations: πᵢ = Σ πⱼ × Pⱼᵢ for each state
Step 2: Add constraint: π₁ + π₂ = 1
Step 3: Substitute and solve
Step 4: Interpret: Long-run fraction of time in each state
```

### Full Exam Problem:

**Q:** A two-state Markov chain describes whether a machine is Working (W) or Under Repair (R).
- P(W→W) = 0.90; P(W→R) = 0.10
- P(R→W) = 0.40; P(R→R) = 0.60

**(a) If machine is Working today, find probability it is Working in 2 periods.**
**(b) Find steady-state probabilities.**

**Answer:**

**(a) Two-step transition:**
State vector (starts as Working): π₀ = [1, 0]

Period 1: π₁ = [1×0.90 + 0×0.40, 1×0.10 + 0×0.60] = [0.90, 0.10]

Period 2: π₂ = [0.90×0.90 + 0.10×0.40, 0.90×0.10 + 0.10×0.60]
= [0.81+0.04, 0.09+0.06] = **[0.85, 0.15]**

**P(Working in 2 periods | Working today) = 0.85**

**(b) Steady-state:**
```
πW = 0.90πW + 0.40πR
πW - 0.90πW = 0.40πR
0.10πW = 0.40πR
πR = 0.25πW

πW + πR = 1 → πW + 0.25πW = 1 → 1.25πW = 1 → πW = 0.80
πR = 0.20
```
**Steady state: Machine Working 80% of time; Under Repair 20% of time**

**Interpretation:** In the long run, this machine will be under repair 20% of the time, regardless of its current state. Management should plan maintenance capacity accordingly.

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Markov Chain | Probabilistic system where future depends only on present state |
| Markov Property | Memoryless — only current state determines future |
| States | Possible conditions the system can be in |
| Transition Matrix | Matrix where Pᵢⱼ = probability of i→j |
| State Vector | Probability distribution across all states at a time point |
| Steady-State | Long-run equilibrium probabilities; π* = π* × P |
| Absorbing State | Once entered, cannot leave |
| n-step Transition | πₙ = π₀ × Pⁿ |

---

*Chapter 7 Complete | DMO | MBA 2nd Semester, DU SOL*
