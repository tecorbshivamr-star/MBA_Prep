# 📗 DMO CHAPTER 4: Simulation
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

You want to know: "If I open a new restaurant, how much will I earn?" You can't open it and find out (too risky and expensive). Instead, you **simulate** it — pretend to run the restaurant thousands of times on paper (or computer), using probabilities for how many customers come, what they order, etc.

This is **Simulation** — creating an artificial model of reality and running experiments on it.

**Famous Simulations:**
- Flight simulators (train pilots without crashing real planes)
- Nuclear bomb tests (too dangerous to do physically)
- Weather forecasting (simulate atmosphere)
- Business: "What if demand drops 30% next quarter?"

---

## 🔵 WHAT IS SIMULATION?

**Definition:**
Simulation is a technique that involves building a mathematical or logical model of a real system and then conducting experiments on that model to understand the behavior of the system or evaluate strategies for its operation.

**Why Simulate Instead of Solving Mathematically?**

| Situation | Use Simulation When... |
|-----------|----------------------|
| Too complex for LP/queuing | Multiple random variables interact |
| Real experiments too costly | Can't build a factory just to test |
| Need to test many scenarios | What-if analysis at low cost |
| System is dynamic over time | Events unfold over time |
| Risk too high for real experiment | Drug dosage, aircraft design |

---

## 🔵 MONTE CARLO SIMULATION ⭐ Most Important for MBA Exams

**Origin:** Named after the Monte Carlo casino in Monaco — because of the use of random numbers (like rolling dice).

**Core Idea:** Use **random numbers** to represent probabilistic events and simulate what might happen many times. Analyze the results statistically.

---

## 🔵 STEPS IN MONTE CARLO SIMULATION

```
Step 1: Define the Problem
         ↓
Step 2: Identify the probability distribution of each uncertain variable
         ↓
Step 3: Build cumulative probability distribution
         ↓
Step 4: Assign random number ranges to each value
         ↓
Step 5: Generate random numbers
         ↓
Step 6: Simulate the system (map random numbers to values)
         ↓
Step 7: Analyze results and draw conclusions
```

---

## 🔵 WORKED EXAMPLE — Demand Simulation ⭐

**Problem:**
A sweet shop at Connaught Place records daily demand for gulab jamun boxes over 200 days:

| Demand (boxes) | Days Observed | Probability |
|---------------|--------------|-------------|
| 0 | 20 | 0.10 |
| 1 | 40 | 0.20 |
| 2 | 60 | 0.30 |
| 3 | 50 | 0.25 |
| 4 | 30 | 0.15 |
| **Total** | **200** | **1.00** |

Each box sells for ₹100; costs ₹60. Unsold boxes are wasted. The shop currently stocks 2 boxes/day. Simulate 10 days using the following random numbers: **52, 37, 82, 14, 95, 26, 78, 44, 61, 09**

---

**Step 1 — Build Cumulative Probability Distribution:**

| Demand | Probability | Cumulative Probability |
|--------|-------------|----------------------|
| 0 | 0.10 | 0.10 |
| 1 | 0.20 | 0.30 |
| 2 | 0.30 | 0.60 |
| 3 | 0.25 | 0.85 |
| 4 | 0.15 | 1.00 |

**Step 2 — Assign Random Number Ranges (2-digit, 00-99):**

| Demand | Probability | Cumulative | Random Number Range |
|--------|-------------|------------|-------------------|
| 0 | 0.10 | 0.10 | 00 – 09 |
| 1 | 0.20 | 0.30 | 10 – 29 |
| 2 | 0.30 | 0.60 | 30 – 59 |
| 3 | 0.25 | 0.85 | 60 – 84 |
| 4 | 0.15 | 1.00 | 85 – 99 |

**Rule for Random Number Assignment:**
- If cumulative probability goes from 0 to 0.10, assign RN range 00 to 09 (10 numbers = 10% of 00-99)
- Range width = Probability × 100

**Step 3 — Simulate 10 Days (Stock = 2 boxes/day):**

| Day | Random Number | Demand | Sales (min(demand,2)) | Revenue | Cost | Waste | Profit |
|-----|--------------|--------|----------------------|---------|------|-------|--------|
| 1 | 52 | 2 | 2 | 200 | 120 | 0 | 80 |
| 2 | 37 | 2 | 2 | 200 | 120 | 0 | 80 |
| 3 | 82 | 3 | 2 | 200 | 120 | 0 | 80 |
| 4 | 14 | 1 | 1 | 100 | 120 | 1×60=60 | -80 |
| 5 | 95 | 4 | 2 | 200 | 120 | 0 | 80 |
| 6 | 26 | 1 | 1 | 100 | 120 | 1×60=60 | -80 |
| 7 | 78 | 3 | 2 | 200 | 120 | 0 | 80 |
| 8 | 44 | 2 | 2 | 200 | 120 | 0 | 80 |
| 9 | 61 | 3 | 2 | 200 | 120 | 0 | 80 |
| 10 | 09 | 0 | 0 | 0 | 120 | 2×60=120 | -240 |
| **Total** | | | | **₹1,600** | **₹1,200** | **₹240** | **₹160** |

**Notes:**
- Revenue = Sales × ₹100
- Cost = Stock (2) × ₹60 = ₹120 per day (whether sold or not)
- Waste = Unsold boxes × ₹60
- Profit = Revenue - Cost (total cost including waste)

**Results:**
- Average daily profit = ₹160/10 = **₹16/day**
- Average demand simulated = (2+2+3+1+4+1+3+2+3+0)/10 = **2.1 boxes/day**

**Managerial Insight:**
Should the shop stock 3 boxes instead? Simulate again with stock=3:
- On days when demand=3 or 4, more sales (higher profit)
- On days when demand=0 or 1, more waste (higher loss)
- Simulation reveals which stock level gives higher average profit

**This is exactly how simulation helps — compare multiple strategies easily!**

---

## 🔵 RANDOM NUMBER GENERATION

In exams, random numbers are GIVEN to you. In practice, computers generate them.

**Types of Random Numbers:**
- **True Random Numbers:** Generated from physical processes (radioactive decay, thermal noise)
- **Pseudo-Random Numbers:** Computer-generated sequences that appear random but repeat (for simulation purposes, this is fine)

**Random Number Table:** A pre-generated table of random digits used in manual simulation exercises.

---

## 🔵 ADVANTAGES OF SIMULATION

| Advantage | Explanation |
|-----------|-------------|
| **Handles complexity** | Can model systems too complex for analytical methods |
| **Safe experimentation** | Test strategies without real-world risk |
| **Flexibility** | Any distribution, any system |
| **What-if analysis** | Easily test multiple scenarios |
| **Visual and intuitive** | Results easier to understand than abstract math |
| **Time compression** | Simulate 5 years in minutes |

---

## 🔵 LIMITATIONS OF SIMULATION

| Limitation | Explanation |
|-----------|-------------|
| **Not optimal** | Finds good solutions but doesn't guarantee the BEST solution |
| **Time and cost** | Complex simulations require significant effort to build |
| **Model validity** | Garbage in, garbage out — model must match reality |
| **Interpretation** | Large amounts of output data can be hard to interpret |
| **No cause-effect** | Shows WHAT happens; doesn't always explain WHY |

---

## 🔵 TYPES OF SIMULATION

| Type | Description | Example |
|------|-------------|---------|
| **Monte Carlo** | Uses random numbers for static probabilistic problems | Demand estimation, stock analysis |
| **Discrete Event Simulation** | Models system as sequence of events in time | Factory workflow, queuing systems |
| **Continuous Simulation** | System changes continuously over time | Chemical plant, ecological models |
| **System Dynamics** | Feedback loops and stock-flow relationships | Urban growth, epidemic spread |
| **Agent-Based Simulation** | Individual agents with rules interact | Market simulation, traffic flow |

---

## 🔵 SIMULATION IN INDIAN BUSINESS

| Application | Company/Sector | Use |
|------------|---------------|-----|
| **Supply chain stress testing** | Reliance, ITC | "What if supplier X fails? Simulate impact" |
| **Bank stress testing** | RBI mandate | "What if 10% of loans default?" |
| **IPO pricing** | Investment banks | Simulate share price scenarios |
| **Manufacturing capacity** | Tata Motors | Simulate plant throughput under different demand |
| **Portfolio risk** | Mutual funds | Monte Carlo for Value at Risk (VaR) |
| **COVID policy** | Government | Simulate epidemic spread under different interventions |

---

## 🔴 EXAM-READY CONTENT

### Standard Exam Answer Template for Monte Carlo Simulation:

```
Step 1: State the probability distribution from given data
Step 2: Calculate cumulative probabilities
Step 3: Assign random number ranges (width = probability × 100)
Step 4: Map each given RN to its corresponding value
Step 5: Calculate output (profit, demand, etc.) for each simulation run
Step 6: Calculate average/total results
Step 7: State managerial conclusion
```

### Common Exam Trap:
- Random number 30 → Belongs to range that STARTS at 30 (not 29)
- Always use: if cumulative prob = 0.30, then range goes UP TO but NOT INCLUDING the next starting number
- Range for demand=2 (if cum prob goes 0.30 to 0.60) → RN range 30 to 59

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Simulation | Artificial experiment on a model of a real system |
| Monte Carlo | Simulation technique using random numbers for probabilistic variables |
| Random Number (RN) | Number drawn from uniform distribution used to represent random events |
| Cumulative Probability | Running total of probabilities up to each value |
| RN Range | Group of random numbers assigned to represent each outcome |
| What-if Analysis | Testing different scenarios in simulation |
| Discrete Event Simulation | Models system as sequence of timed events |

---

*Chapter 4 Complete | DMO | MBA 2nd Semester, DU SOL*
