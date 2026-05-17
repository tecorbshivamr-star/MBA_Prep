# 📗 DMO CHAPTER 3: Queuing Theory
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

You're at an SBI bank. Customers keep arriving. The teller serves them one by one. Sometimes the queue is long. Sometimes nobody is waiting.

**Questions the bank manager asks:**
- How long will a customer wait on average?
- How many people will be in the queue on average?
- How busy will the teller be?
- Should we open a second teller window?

**Queuing Theory** (also called Waiting Line Theory) provides mathematical answers to these exact questions.

Every service business — banks, hospitals, call centres, restaurants, toll booths, petrol stations — uses queuing theory to balance service quality vs. cost.

---

## 🔵 WHAT IS QUEUING THEORY?

**Definition:**
Queuing Theory is the mathematical study of waiting lines (queues). It helps managers determine the optimal number of service facilities (servers) by analyzing the relationship between arrival rates, service rates, waiting times, and queue lengths.

**The Core Trade-off:**
```
More servers → Less waiting time → HIGHER COST
Fewer servers → More waiting time → LOWER COST (but unhappy customers)

Optimal: Minimize Total Cost = Service Cost + Waiting Cost
```

---

## 🔵 COMPONENTS OF A QUEUING SYSTEM

Every queuing system has:

### 1. Arrival Process
- **Arrival Rate (λ):** Average number of customers arriving per unit time
- **Distribution:** Usually Poisson distribution (random arrivals)
- Poisson: Most real-world arrivals are well-approximated by Poisson distribution

### 2. Queue (Waiting Line)
- **Queue Discipline:** Rule deciding who is served next
  - FCFS/FIFO (First Come First Served) — most common
  - LCFS/LIFO (Last Come First Served) — like a stack
  - SIRO (Service in Random Order)
  - Priority (VIP customers first)
- **Queue Length:** Maximum number allowed in the system (finite or infinite)
- **Calling Population:** Total population of potential customers (finite or infinite)

### 3. Service Mechanism
- **Service Rate (μ):** Average number of customers served per unit time
- **Service Time Distribution:** Usually Exponential distribution
- **Number of Servers (c):** Number of parallel service channels

---

## 🔵 KENDALL'S NOTATION

Queuing models are described using Kendall's notation: **A/B/c/K/N/D**

| Symbol | Meaning |
|--------|---------|
| A | Arrival time distribution |
| B | Service time distribution |
| c | Number of servers |
| K | System capacity (max customers, default = ∞) |
| N | Calling population size (default = ∞) |
| D | Queue discipline (default = FCFS) |

**Key Distributions:**
- **M** = Markovian (Poisson arrivals / Exponential service)
- **D** = Deterministic (fixed times)
- **G** = General (any distribution)

**Most Common Models:**
- **M/M/1** — Single server, Poisson arrivals, Exponential service ← Most important for exam
- **M/M/c** — Multiple servers, Poisson arrivals, Exponential service
- **M/D/1** — Single server, fixed service time
- **M/G/1** — Single server, general service time

---

## 🔵 THE M/M/1 MODEL — COMPLETE ANALYSIS ⭐ Most Tested

### Assumptions:
1. Arrivals follow Poisson distribution with rate λ
2. Service times follow Exponential distribution with rate μ
3. Single server (one service channel)
4. First Come First Served (FCFS)
5. Infinite queue capacity
6. Infinite calling population

### The Traffic Intensity (Utilization Factor):
```
ρ = λ/μ
```
- **ρ < 1:** System is STABLE (server not overwhelmed) — queue doesn't grow infinitely
- **ρ ≥ 1:** System is UNSTABLE (queue grows without bound) — add more servers!
- **ρ = Server utilization** (fraction of time server is busy)

---

### THE 5 KEY M/M/1 FORMULAS ⭐ Memorize These!

```
ρ = λ/μ                        [Traffic intensity / Server utilization]

Lq = λ²/[μ(μ-λ)]             [Average number of customers IN QUEUE]

L  = λ/(μ-λ)                  [Average number of customers IN SYSTEM]

Wq = λ/[μ(μ-λ)]              [Average waiting time IN QUEUE]

W  = 1/(μ-λ)                  [Average time IN SYSTEM (queue + service)]
```

### Quick Derivations (helpful for exams):
```
L = Lq + ρ          [System = Queue + In-service]
W = Wq + 1/μ        [System time = Queue time + Service time]
Lq = λ × Wq         [Little's Law applied to queue]
L  = λ × W          [Little's Law applied to system]
```

---

## 🔵 LITTLE'S LAW ⭐

**John D.C. Little's Law (1961):**
```
L = λ × W
```
This simple but powerful relationship states:
- L = Average number of customers in the system
- λ = Average arrival rate
- W = Average time a customer spends in the system

**It applies to ANY stable queuing system** — regardless of arrival distribution, service distribution, or number of servers!

**Also:**
```
Lq = λ × Wq
```
(Average in queue = Arrival rate × Average wait in queue)

---

## 🔵 WORKED EXAMPLE — M/M/1 ⭐

**Problem:** Customers arrive at an SBI ATM at an average rate of **18 per hour**. The ATM serves customers at an average rate of **24 per hour**. Assume Poisson arrivals and exponential service times.

**Calculate:**
1. Server utilization (ρ)
2. Average number in queue (Lq)
3. Average number in system (L)
4. Average waiting time in queue (Wq)
5. Average time in system (W)
6. Probability that no customer is in the system (P₀)

**Solution:**

**Given:**
```
λ = 18 customers/hour
μ = 24 customers/hour
```

**Check stability:** ρ = λ/μ = 18/24 = 0.75 < 1 ✓ (System is stable)

**Step 1 — Traffic Intensity:**
```
ρ = λ/μ = 18/24 = 0.75 = 75%
(ATM is busy 75% of the time)
```

**Step 2 — Lq (Average in Queue):**
```
Lq = λ²/[μ(μ-λ)]
   = (18)²/[24 × (24-18)]
   = 324/[24 × 6]
   = 324/144
   = 2.25 customers
```

**Step 3 — L (Average in System):**
```
L = λ/(μ-λ)
  = 18/(24-18)
  = 18/6
  = 3 customers
```
OR: L = Lq + ρ = 2.25 + 0.75 = 3 ✓

**Step 4 — Wq (Average Wait in Queue):**
```
Wq = λ/[μ(μ-λ)]
   = 18/[24 × (24-18)]
   = 18/[24×6]
   = 18/144
   = 0.125 hours = 7.5 minutes
```

**Step 5 — W (Average Time in System):**
```
W = 1/(μ-λ)
  = 1/(24-18)
  = 1/6 hours
  = 10 minutes
```
OR: W = Wq + 1/μ = 7.5 + 1/24 × 60 = 7.5 + 2.5 = 10 minutes ✓

**Step 6 — P₀ (Probability of empty system):**
```
P₀ = 1 - ρ = 1 - 0.75 = 0.25
(25% chance the ATM is idle)
```

**Summary Table:**

| Measure | Value | Interpretation |
|---------|-------|---------------|
| ρ | 0.75 | ATM busy 75% of time |
| Lq | 2.25 | Average 2.25 customers waiting |
| L | 3.00 | Average 3 customers in system |
| Wq | 7.5 min | Average 7.5 min wait in queue |
| W | 10 min | Average 10 min total time |
| P₀ | 0.25 | 25% chance ATM idle |

**Managerial Decision:**
Is 7.5 minutes acceptable? If bank's standard is "max 5 min wait" → Need a second ATM.

---

## 🔵 M/M/c MODEL — MULTIPLE SERVERS

When one server is insufficient, we add more.

For M/M/c (c servers):
```
Traffic intensity per server: ρ = λ/(c×μ)   [must be < 1]
```

The formulas for L, Lq, W, Wq in M/M/c are more complex (involve Erlang C formula). For MBA exams, you mostly need to:
1. Understand the concept
2. Know when M/M/c is appropriate
3. Apply if given the formula or table

**Decision Rule for Adding Servers:**
- If Wq (current) > Acceptable wait → Add server
- Compare Total Cost = c × Server Cost + Lq × Waiting Cost
- Choose c that minimizes total cost

---

## 🔵 QUEUE SYSTEM PERFORMANCE MEASURES

| Measure | Symbol | What It Tells You |
|---------|--------|------------------|
| Traffic Intensity | ρ | How busy the server is |
| Avg customers in queue | Lq | Queue buildup |
| Avg customers in system | L | Overall congestion |
| Avg wait in queue | Wq | Customer wait experience |
| Avg time in system | W | Total customer experience time |
| Prob. of empty system | P₀ | Idle time |
| Prob. of n in system | Pₙ | Probability distribution of queue size |

**Pₙ Formula (M/M/1):**
```
Pₙ = (1-ρ) × ρⁿ
```
Example: Prob. of exactly 3 customers in system = (1-0.75) × 0.75³ = 0.25 × 0.422 = 0.105 (10.5%)

---

## 🔵 COST OPTIMIZATION IN QUEUING

**Total Cost Model:**
```
Total Cost = Server Cost + Waiting Cost
TC = c × Cs + L × Cw

Where:
c = number of servers
Cs = cost per server per unit time
Cw = cost per customer per unit time waiting (lost goodwill, productivity)
```

**Example:**
- One teller: TC = 1×₹500 + 3×₹200 = ₹500 + ₹600 = **₹1,100/hour**
- Two tellers: L drops to 1.5; TC = 2×₹500 + 1.5×₹200 = ₹1,000 + ₹300 = **₹1,300/hour**
→ One teller is cheaper here. But if Cw (waiting cost) is higher, two tellers might win.

---

## 🔵 REAL-WORLD APPLICATIONS IN INDIA

| Application | Setting | Decision |
|-------------|---------|---------|
| **Bank teller optimization** | HDFC Bank branches | How many tellers needed per shift |
| **Call centre staffing** | Airtel, Jio customer care | How many agents per hour |
| **Airport check-in** | IndiGo, Air India | How many check-in counters to open |
| **Hospital OPD** | AIIMS, Apollo | Doctor appointments schedule |
| **Toll booth design** | NHAI toll plazas | How many lanes to keep open |
| **Petrol pump** | HPCL, BPCL pumps | How many pumps per station |
| **E-commerce server load** | Flipkart Big Billion Day | Server capacity to handle peak traffic |

---

## 🔴 EXAM-READY CONTENT

### Standard Exam Template:

```
Given: λ = ___ per hour; μ = ___ per hour
Step 1: Check stability: ρ = λ/μ = ___ (must be < 1)
Step 2: Lq = λ²/[μ(μ-λ)] = ___
Step 3: L = λ/(μ-λ) = ___     OR L = Lq + ρ
Step 4: Wq = Lq/λ = ___       OR Wq = λ/[μ(μ-λ)]
Step 5: W = L/λ = ___          OR W = 1/(μ-λ)
Step 6: P₀ = 1-ρ = ___
Step 7: Interpret each result in context
```

### Practice Problem:
**A hospital emergency ward receives patients at the rate of 6 per hour. A doctor can examine 10 patients per hour. Find all M/M/1 performance measures.**

**Solution:**
```
λ = 6/hr; μ = 10/hr
ρ = 6/10 = 0.60
Lq = 36/[10×4] = 36/40 = 0.90 patients
L  = 6/4 = 1.5 patients
Wq = 6/[10×4] = 6/40 = 0.15 hrs = 9 minutes
W  = 1/4 = 0.25 hrs = 15 minutes
P₀ = 1-0.6 = 0.40 (40% chance no patient waiting)
```

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| Queuing Theory | Mathematics of waiting lines and service systems |
| λ (Lambda) | Arrival rate — customers per unit time |
| μ (Mu) | Service rate — customers served per unit time |
| ρ (Rho) | Traffic intensity = λ/μ; server utilization |
| Lq | Average number of customers waiting in QUEUE |
| L | Average number of customers in SYSTEM (queue + service) |
| Wq | Average waiting time in QUEUE |
| W | Average time in SYSTEM (queue + service) |
| M/M/1 | Poisson arrivals / Exponential service / Single server |
| Little's Law | L = λ × W (universal queuing relationship) |
| P₀ | Probability system is empty = 1-ρ |
| FCFS | First Come First Served — standard queue discipline |

---

*Chapter 3 Complete | DMO | MBA 2nd Semester, DU SOL*
