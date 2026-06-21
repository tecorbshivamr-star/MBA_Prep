# 📘 EEB — Chapter 4: IS-LM Model
### *Exam-Ready Notes | MBA SEM 2*

---

> **🎯 Exam Strategy:** The IS-LM model is one of the most diagram-heavy chapters. Focus on **drawing both curves correctly**, understanding **shifts vs movements**, and the **policy effects**. Expect a diagram-based question for sure.

---

## 4.1 Learning Objectives

- ✅ Explain the Keynesian framework and why it differs from Classical economics
- ✅ Derive and understand the IS curve (Goods Market)
- ✅ Derive and understand the LM curve (Money Market)
- ✅ Determine short-run equilibrium in the IS-LM model
- ✅ Analyze the effect of Fiscal Policy on the IS curve
- ✅ Analyze the effect of Monetary Policy on the LM curve
- ✅ Understand the interaction between monetary and fiscal policy

---

## 4.2 Introduction

### What is the IS-LM Model?

The **IS-LM Model** (John Hicks, 1937 — based on Keynes' General Theory) shows how the **Goods Market** and **Money Market** interact simultaneously to determine the economy's **short-run equilibrium** — specifically, the equilibrium **output (Y)** and **interest rate (r)**.

| Curve | Stands For | Market it Represents |
|---|---|---|
| **IS** | Investment = Saving | **Goods Market** equilibrium |
| **LM** | Liquidity preference = Money supply | **Money Market** equilibrium |

> 📌 *"IS-LM is the workhorse model of short-run macroeconomics — it shows how fiscal and monetary policies work."*

**Both curves together → Determine (Y*, r*) simultaneously**

---

## 4.3 Keynesian Framework

### Classical vs Keynesian — Key Differences

| Feature | **Classical Economics** | **Keynesian Economics** |
|---|---|---|
| **Time Horizon** | Long run | Short run |
| **Prices & Wages** | Flexible (adjust instantly) | Sticky/Rigid (slow to adjust) |
| **Markets** | Always clear (equilibrium) | Can be in disequilibrium |
| **Unemployment** | Only voluntary, temporary | Involuntary unemployment possible |
| **Role of Government** | Minimal — "invisible hand" works | Active — government must intervene |
| **Demand** | Supply creates its own demand (Say's Law) | Demand determines output |

### Keynesian Core Ideas

**1. Aggregate Demand Drives Output (Short Run)**
- In the short run, **demand = production** — firms produce what is demanded
- If demand falls → Output falls → Unemployment rises

**2. Wages and Prices are Sticky**
- Workers resist wage cuts → Unemployment can persist
- Firms don't cut prices immediately → Markets don't self-correct quickly

**3. Government Intervention is Necessary**
- Economy can get stuck in a recession; government must stimulate demand
- Fiscal policy (G↑ or T↓) or Monetary policy (Ms↑) can restore full employment

### The Keynesian Cross (Foundation of IS Curve)

**Planned Expenditure:**
```
E = C + I + G
C = C₀ + c(Y − T)       [Consumption Function]
```
Where:
- **C₀** = Autonomous consumption
- **c** = MPC (Marginal Propensity to Consume, 0 < c < 1)
- **Y − T** = Disposable Income

**Equilibrium Condition:**
```
Y = E  →  Output = Planned Expenditure
Y = C₀ + c(Y − T) + I + G
Y(1 − c) = C₀ − cT + I + G
Y = [1/(1−c)] × (C₀ + I + G − cT)
```

**The Multiplier:**
```
Multiplier (k) = 1 / (1 − MPC) = 1 / MPS
```

| MPC | Multiplier |
|---|---|
| 0.5 | 2 |
| 0.75 | 4 |
| 0.8 | 5 |
| 0.9 | 10 |

> **Example**: MPC = 0.8, ΔG = ₹100 crore → ΔY = 5 × 100 = **₹500 crore**

---

## 4.4 The IS and LM Curves

### 🔵 THE IS CURVE — Goods Market Equilibrium

**Definition**: The IS curve shows all combinations of **interest rate (r)** and **output (Y)** for which the **Goods Market is in equilibrium** (Investment = Saving, or equivalently, Y = C + I + G + NX).

#### Why IS Curve Slopes Downward?

```
↓ r  →  ↓ cost of borrowing  →  ↑ Investment (I)  →  ↑ Aggregate Demand  →  ↑ Y
```

**Higher interest rate → Lower investment → Lower output**
**Lower interest rate → Higher investment → Higher output**

```
Interest Rate (r)
     │
   r₁│ • A (high r, low Y)
     │   \
   r₂│    • B (low r, high Y)
     │     \
     │      \  IS Curve
     └────────────────────► Output (Y)
         Y₁   Y₂
```

#### IS Curve Equation:
```
Y = [1/(1−c)] × (C₀ + I₀ − b×r + G − cT)

Where:
- b = sensitivity of investment to interest rate
- I = I₀ − b×r  (Investment falls as r rises)
```

**Slope of IS**: `Δr/ΔY = −(1−c)/b`
- Flatter IS when: MPC is high (large multiplier) OR investment is very sensitive to interest rates

---

#### What SHIFTS the IS Curve?

| Shift Direction | Cause |
|---|---|
| **IS shifts RIGHT (↑Y at every r)** | ↑G, ↓T, ↑Autonomous Consumption, ↑Investment confidence, ↑Exports |
| **IS shifts LEFT (↓Y at every r)** | ↓G, ↑T, ↓Consumer confidence, ↓Investment, ↑Imports |

```
        r
        │
        │    IS₁  IS₂
        │   \    \
        │    \    \   → Fiscal Expansion shifts IS RIGHT
        │     \    \
        └──────────────► Y
```

> **Movement ALONG IS** = Change in interest rate (r changes, same IS curve)
> **SHIFT of IS** = Change in fiscal policy, consumer/investor confidence, exports

---

### 🔴 THE LM CURVE — Money Market Equilibrium

**Definition**: The LM curve shows all combinations of **interest rate (r)** and **output (Y)** for which the **Money Market is in equilibrium** (Money Demand = Money Supply).

#### Money Demand (Liquidity Preference — Keynes)

People hold money for three reasons:
1. **Transactions Demand** → Proportional to income (↑Y → ↑money needed for transactions)
2. **Precautionary Demand** → Buffer for unexpected expenses (also ↑ with Y)
3. **Speculative Demand** → Inversely related to interest rate (↑r → ↓money held as cash, prefer bonds)

```
Money Demand: Md = kY − hr

Where:
- k = sensitivity of money demand to income
- h = sensitivity of money demand to interest rate
```

**Money Market Equilibrium:**
```
Ms/P = kY − hr   (Real Money Supply = Real Money Demand)

Solving for r:
r = (k/h)Y − (1/h)(Ms/P)
```

#### Why LM Curve Slopes Upward?

```
↑ Y  →  ↑ Transactions demand for money  →  ↑ r to restore money market equilibrium
```

**Higher output → More money demand → Higher interest rate to equilibrate money market**

```
Interest Rate (r)
     │           / LM Curve
   r₂│        • B (high Y, high r)
     │      /
   r₁│   • A (low Y, low r)
     │  /
     └────────────────────► Output (Y)
       Y₁     Y₂
```

#### LM Curve Equation:
```
r = (k/h)Y − (1/h)(Ms/P)
```

**Slope of LM**: `Δr/ΔY = k/h`
- Steeper LM when: Money demand very sensitive to income (k large) OR very insensitive to interest rate (h small)

---

#### What SHIFTS the LM Curve?

| Shift Direction | Cause |
|---|---|
| **LM shifts RIGHT/DOWN (↓r at every Y)** | ↑ Money Supply (Ms↑), ↓ Price Level (P↓) |
| **LM shifts LEFT/UP (↑r at every Y)** | ↓ Money Supply (Ms↓), ↑ Price Level (P↑) |

```
        r
        │
        │  LM₁ LM₂
        │  /  /
        │ /  /    → Monetary Expansion shifts LM RIGHT
        │/  /
        └──────────────► Y
```

> **Movement ALONG LM** = Change in income/output
> **SHIFT of LM** = Change in money supply or price level

---

### 6 IS-LM Curve Cases (Key Section 4.4)

| Case | Situation | Result |
|---|---|---|
| **1. Normal IS-LM** | Both curves have normal slopes | Standard equilibrium |
| **2. Liquidity Trap (LM horizontal)** | Interest rate at zero lower bound; money demand perfectly elastic | Monetary policy ineffective; Fiscal policy fully effective |
| **3. Classical Case (LM vertical)** | Money demand insensitive to r; Quantity Theory holds | Fiscal policy ineffective (full crowding out); Monetary policy effective |
| **4. Investment Trap (IS vertical)** | Investment perfectly insensitive to r | Monetary policy ineffective; Fiscal policy fully effective |
| **5. Flat IS** | High MPC, highly interest-sensitive investment | Large fiscal multiplier, large monetary effect |
| **6. Steep IS** | Low MPC, investment insensitive to r | Small multiplier, small monetary effect |

---

### 🔑 Special Case: Liquidity Trap

**Definition**: When interest rates are so low (near zero) that everyone expects them to rise → People hold cash instead of bonds → Money demand becomes **perfectly elastic**.

```
r
│
│ ─────────────────── LM (horizontal at very low r)
│
└──────────────────────────► Y
```

**Implication**:
- ↑ Money Supply → No further fall in r (already at zero) → No boost to investment → **Monetary policy fails**
- ↑ G → Full multiplier effect (no crowding out) → **Fiscal policy fully effective**
- **Real-world examples**: Japan (1990s–2000s), USA after 2008 Financial Crisis, COVID-era

---

## 4.5 Short-Run Equilibrium in IS-LM

### Finding Equilibrium

Equilibrium is where **IS = LM** simultaneously:
- Goods market is in equilibrium
- Money market is in equilibrium
- Gives unique **(Y*, r*)** pair

```
        r
        │          LM
        │         /
        │        /
      r*│ ─────•  ← Equilibrium (Y*, r*)
        │     /\
        │    /  \
        │   /    IS
        └─────────────────────► Y
                Y*
```

**Solving Mathematically:**

IS: `Y = A − b×r` (where A = autonomous spending multiplier)
LM: `r = (k/h)Y − Ms/(h×P)`

Substitute LM into IS → Solve for Y* and r*

---

### What Changes Equilibrium?

| Policy Action | IS/LM Affected | Effect on Y* | Effect on r* |
|---|---|---|---|
| ↑ Government Spending (G) | IS shifts Right | ↑ | ↑ |
| ↑ Taxes (T) | IS shifts Left | ↓ | ↓ |
| ↑ Money Supply (Ms) | LM shifts Right | ↑ | ↓ |
| ↓ Money Supply (Ms) | LM shifts Left | ↓ | ↑ |

---

## 4.6 Effect of Fiscal Policy on the IS Curve

### Expansionary Fiscal Policy (↑G or ↓T)

**Mechanism:**
```
↑G → ↑Aggregate Demand → IS shifts RIGHT → ↑Y and ↑r
```

**Diagram:**
```
        r
        │          LM
        │         /
      r₂│ ───────• B (new equilibrium)
        │       /|
      r₁│ ─────• |A (old equilibrium)
        │     /| |
        │    / IS₁ IS₂
        └──────────────────► Y
              Y₁ Y₂
```

- Output rises from Y₁ to Y₂
- Interest rate rises from r₁ to r₂
- **But Y₂ < what Keynesian Cross predicts** — Why? **Crowding Out!**

---

### Crowding Out Effect

**Definition**: When government spending raises interest rates, which **reduces private investment**, partially offsetting the initial fiscal stimulus.

```
↑G → IS shifts right → ↑Y → ↑Money demand → ↑r → ↓Private Investment
                                                    → Partially offsets ↑G
```

**Degree of Crowding Out depends on:**

| Condition | Crowding Out | Reason |
|---|---|---|
| **Steep LM** (inelastic money demand) | **High** | Small Ms increase causes big r rise |
| **Flat LM** (elastic money demand / Liquidity Trap) | **Zero** | r doesn't rise; no reduction in I |
| **Steep IS** (investment insensitive to r) | **Low** | Even if r rises, I doesn't fall much |
| **Flat IS** (investment very sensitive to r) | **High** | Small r rise causes big fall in I |

**Full Crowding Out** (Classical Case — Vertical LM):
- Every ₹1 of G replaces exactly ₹1 of private investment
- No net effect on Y → Fiscal policy completely ineffective

---

### Contractionary Fiscal Policy (↓G or ↑T)

```
↓G or ↑T → ↓AD → IS shifts LEFT → ↓Y and ↓r
```
- Used to **cool an overheating economy** (combat inflation)

---

### Tax Multiplier vs Government Spending Multiplier

```
Government Spending Multiplier = 1 / (1 − MPC)

Tax Multiplier = −MPC / (1 − MPC)
```

> Note: Tax multiplier is smaller (in absolute value) than spending multiplier because ↑T first reduces consumption by MPC × ΔT (not by full ΔT).

**Balanced Budget Multiplier = 1**
If ΔG = ΔT (equal increase in both), net multiplier = 1 (not zero!)

---

## 4.7 Effect of Monetary Policy on LM Curve

### Expansionary Monetary Policy (↑Ms — "Easy Money")

**RBI Tools to Increase Money Supply:**
- ↓ Repo Rate
- ↓ CRR (Cash Reserve Ratio)
- ↓ SLR (Statutory Liquidity Ratio)
- Open Market Operations (RBI buys government securities)

**Mechanism:**
```
↑Ms → ↓r (excess money supply) → LM shifts RIGHT → ↓r and ↑Y
```

**Diagram:**
```
        r
        │      LM₁  LM₂
        │       /   /
      r₁│ ─────• A /
        │      |  /
      r₂│      | • B (new equilibrium)
        │      |/
        │     /  IS
        └──────────────────► Y
              Y₁ Y₂
```

- Interest rate falls from r₁ to r₂ → Cheaper borrowing
- Investment increases → Output rises from Y₁ to Y₂
- **No crowding out** — private investment is stimulated, not displaced

---

### Contractionary Monetary Policy (↓Ms — "Tight Money")

```
↓Ms → ↑r → LM shifts LEFT → ↑r and ↓Y
```
- Used to **fight inflation**
- RBI increases Repo Rate → Banks lend less → Money supply falls

---

### Monetary Policy Effectiveness — When Does It Fail?

| Situation | Why Monetary Policy Fails |
|---|---|
| **Liquidity Trap** | r already at zero floor; ↑Ms doesn't reduce r further |
| **Investment Trap** | Even if r falls, investment doesn't respond (lack of confidence) |
| **Transmission Problem** | Banks don't pass on rate cuts to borrowers (India issue — NPA problem) |
| **Currency Substitution** | People move to foreign currency; domestic money supply ineffective |

---

## 4.8 Interaction Between Monetary and Fiscal Policy

### Policy Mix — Four Combinations

| Fiscal Policy | Monetary Policy | Effect | Example Use |
|---|---|---|---|
| **Expansionary + Expansionary** | ↑G/↓T + ↑Ms | Strong ↑Y; ↑ or stable r (depends on mix) | Deep recession (COVID stimulus) |
| **Contractionary + Contractionary** | ↓G/↑T + ↓Ms | Strong ↓Y; falling r | Severe inflation with overheating |
| **Expansionary Fiscal + Contractionary Monetary** | ↑G + ↓Ms | ↑Y (partial), ↑r sharply | Fiscal stimulus financed without inflation |
| **Contractionary Fiscal + Expansionary Monetary** | ↓G + ↑Ms | Stable Y possible, ↓r | Reduce deficit while supporting growth |

---

### Resolving Crowding Out with Monetary Accommodation

**Problem**: Fiscal expansion (↑G) raises r → Crowds out private investment

**Solution**: Central bank **accommodates** by expanding money supply simultaneously:
```
↑G → IS shifts right → r tends to rise
↑Ms → LM shifts right → r pushed back down
→ Net effect: Y rises significantly, r stays stable
```

**But risk**: Monetizing fiscal deficit → Can cause **inflation**

---

### Policy Coordination in India

| Institution | Policy Tool | Objective |
|---|---|---|
| **Government (Finance Ministry)** | Fiscal Policy (G, T) | Growth, employment, welfare |
| **RBI (Reserve Bank of India)** | Monetary Policy (Ms, repo rate) | Price stability (4% inflation target) |

> **India's Monetary Policy Committee (MPC)** — 6-member body that sets repo rate every 2 months
> **FRBM Act** — Limits fiscal deficit to 3% of GDP to prevent excessive crowding out

---

### The IS-LM in Practice — India Examples

| Event | Policy Response | IS-LM Interpretation |
|---|---|---|
| **COVID-19 (2020)** | ↑G (stimulus), ↓Repo rate | IS + LM both shifted right → cushioned output fall |
| **High Inflation (2022-23)** | RBI raised repo rate 250bps | LM shifted left → ↑r → ↓inflation, slight ↓Y |
| **2008 Global Crisis** | RBI cut rates, govt. stimulus | Expansionary fiscal + monetary mix |
| **Demonetization (2016)** | Sudden ↓Ms | LM shifted sharply left → ↓Y (short term) |

---

## 4.9 Summary

### 🔑 Key Takeaways — Chapter 4

| Topic | What to Remember |
|---|---|
| **Keynesian vs Classical** | Prices sticky in SR; demand drives output; govt. needed |
| **IS Curve** | Downward sloping; Goods market equilibrium; shifts with fiscal policy |
| **LM Curve** | Upward sloping; Money market equilibrium; shifts with monetary policy |
| **Equilibrium** | IS = LM gives (Y*, r*) |
| **Fiscal Policy** | ↑G → IS right → ↑Y, ↑r; crowding out reduces full multiplier effect |
| **Monetary Policy** | ↑Ms → LM right → ↑Y, ↓r; no crowding out |
| **Liquidity Trap** | LM flat → Monetary policy fails; Fiscal fully effective |
| **Classical Case** | LM vertical → Fiscal fails (full crowding out); Monetary effective |
| **Policy Mix** | Best outcomes from coordinated fiscal + monetary policy |

---

### ⚡ Quick Formula Sheet

```
Keynesian Cross:   Y = [1/(1-c)] × (C₀ + I + G − cT)
Multiplier:        k = 1/(1-MPC)
Tax Multiplier:    = -MPC/(1-MPC)

IS Equation:       Y = A − b×r   [downward sloping]
LM Equation:       r = (k/h)Y − Ms/(h×P)   [upward sloping]

Crowding Out:      ↑G → ↑r → ↓I (partial offset)
Full Crowding Out: Vertical LM → ΔG = −ΔI (no ΔY)
Liquidity Trap:    Horizontal LM → Full fiscal multiplier, zero monetary effect
```

---

### 📝 Likely Exam Questions — Chapter 4

1. **What is the IS-LM model? What does each curve represent?**
2. **Explain why the IS curve slopes downward and the LM curve slopes upward.**
3. **What factors shift the IS curve to the right? Draw a diagram.**
4. **What factors shift the LM curve to the right? Draw a diagram.**
5. **Explain short-run equilibrium in the IS-LM model with a diagram.**
6. **What is the Crowding Out Effect? When is it complete and when is it zero?**
7. **Explain the Liquidity Trap. Why does fiscal policy work better than monetary policy in a liquidity trap?**
8. **What is the effect of expansionary fiscal policy on output and interest rates? Draw IS-LM diagram.**
9. **What is the effect of expansionary monetary policy on output and interest rates? Draw IS-LM diagram.**
10. **Distinguish between Classical case and Keynesian case in IS-LM. What are the policy implications?**
11. **What is monetary accommodation? How does it resolve the crowding out problem?**
12. **Explain the policy mix of expansionary fiscal + contractionary monetary policy with a diagram.**

---

*📅 Prepared for: EEB Exam | MBA SEM 2 | June 2026*
*🍀 All the best for your exam!*
