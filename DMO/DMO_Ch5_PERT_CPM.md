# 📗 DMO CHAPTER 5: Project Scheduling — PERT and CPM
### Subject: Decision Modelling & Optimization | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

You're managing construction of a new Reliance Jio office. There are 15 activities:
foundation, walls, roof, electrical, plumbing, painting...

Questions:
- How long will the whole project take?
- Which activities are most critical? (If they are delayed, the whole project delays!)
- Which activities have flexibility? (Can be delayed without affecting deadline?)
- If the project must finish earlier, which activities should be fast-tracked?

**PERT (Program Evaluation and Review Technique)** and **CPM (Critical Path Method)** answer these exact questions. They are the most widely used project management tools in the world.

---

## 🔵 CPM vs. PERT

| Aspect | CPM | PERT |
|--------|-----|------|
| Full Form | Critical Path Method | Program Evaluation and Review Technique |
| Time Estimates | **Single (deterministic)** | **Three estimates (probabilistic)** |
| Focus | Time-cost trade-off (crashing) | Schedule uncertainty and probability |
| Origin | DuPont (1956) — construction/engineering | US Navy (1958) — Polaris missile program |
| Best For | Repetitive projects (clear durations) | R&D, new product development (uncertain durations) |

---

## 🔵 NETWORK DIAGRAM

A project network shows activities and their precedence relationships (what must finish before what).

**Two Types:**
- **AOA (Activity on Arrow):** Activities shown as arrows; events (nodes) represent start/end points
- **AON (Activity on Node):** Activities shown as nodes; arrows show dependencies ← More common in modern software

**For MBA Exams:** AOA is more commonly tested.

**Dummy Activity:** In AOA networks, a dummy activity (dashed arrow, zero duration) is used when:
1. Two activities share the same start and end events (would create duplicate)
2. To show a dependency that cannot be shown without it

---

## 🔵 CPM — COMPLETE WORKED EXAMPLE ⭐

**Problem:** A project has the following activities:

| Activity | Description | Predecessor | Duration (weeks) |
|----------|-------------|------------|-----------------|
| A | Site preparation | None | 3 |
| B | Foundation | A | 5 |
| C | Structural steel | A | 4 |
| D | Roofing | B, C | 3 |
| E | Electrical | B | 6 |
| F | Plumbing | B | 4 |
| G | Interior finish | D, E, F | 5 |

**Step 1 — Draw Network Diagram:**

```
     A(3)      B(5)          E(6)
1 ─────── 2 ─────── 3 ──────────── 5
          │         │               │
          │  C(4)   │ F(4)          │ G(5)
          └─────────4──────────────6──── 7
                    │
                   D(3)
                    └──────────────5
```

(Simplified — actual AOA network needed in exams — draw on paper)

**Step 2 — FORWARD PASS (Calculate Early Start and Early Finish):**

For each event, find the **Earliest Event Time (ET)** = longest path to reach that event.

```
ET(Start) = 0
ET after A: 0 + 3 = 3
ET after B: 3 + 5 = 8
ET after C: 3 + 4 = 7
ET after D: max(ET_B + 5, ET_C + 3) = max(8+5, 7+3) = max(13,10) = 13 ← from B route
Wait — D follows BOTH B and C → D can only start after BOTH B and C complete
ET to start D = max(ET_B, ET_C) = max(8, 7) = 8 → ET_D = 8 + 3 = 11
ET to start E: 8 → ET_E = 8 + 6 = 14
ET to start F: 8 → ET_F = 8 + 4 = 12
ET to start G: max(ET_D, ET_E, ET_F) = max(11, 14, 12) = 14 → ET_G = 14 + 5 = 19
```

**Project Duration = 19 weeks**

**Step 3 — BACKWARD PASS (Calculate Late Start and Late Finish):**

For each event, find the **Latest Event Time (LT)** = latest you can leave without delaying project.

```
LT(End/Event 7) = 19 (= Project Duration)
LT before G: 19 - 5 = 14
LT before E: 14 - 6 = 8
LT before F: 14 - 4 = 10
LT before D: 14 - 3 = 11
LT before B: min(LT_E - 0, LT_F - 0, LT_D - 0) 
  (B must finish in time for E, F, and D to start on time)
  = min(8, 10, 11) = 8
LT before C: 11 - 4 = 7 (must finish in time for D)
LT before A: min(LT_B - 3, LT_C - 4) 
  Wait — LT_A means latest A can finish:
  = min(LT_B, LT_C) = min(8-5, 7-4) = min(3, 3) = 3
  LT(Start) = 3 - 3 = 0 ✓
```

**Step 4 — Calculate FLOAT (Slack) for Each Activity:**

```
Total Float = LT(end event) - ET(start event) - Duration
(OR = Late Start - Early Start = Late Finish - Early Finish)
```

| Activity | Duration | ET(i) | ET(j) | LT(i) | LT(j) | Float |
|----------|---------|-------|-------|-------|-------|-------|
| A | 3 | 0 | 3 | 0 | 3 | 0 |
| B | 5 | 3 | 8 | 3 | 8 | 0 |
| C | 4 | 3 | 7 | 3 | 7 | 0 |
| D | 3 | 8 | 11 | 8 | 11 | 0 |
| E | 6 | 8 | 14 | 8 | 14 | 0 |
| F | 4 | 8 | 12 | 10 | 14 | 2 |
| G | 5 | 14 | 19 | 14 | 19 | 0 |

**Step 5 — Identify Critical Path:**
Activities with Float = 0 are **CRITICAL**:
- **A → B → E → G** (all have Float = 0)
- Also: **A → C → D → G** (check: 3+4+3+5=15 ≠ 19 → Not critical!)
- Wait: A→B→D→G = 3+5+3+5=16 ≠ 19
- A→B→E→G = 3+5+6+5 = **19 ✓ Critical Path!**

**Critical Path: A → B → E → G (Duration = 19 weeks)**

Activity F has Float = 2 weeks (can be delayed up to 2 weeks without delaying project).

---

## 🔵 TYPES OF FLOAT

| Float Type | Definition | Formula |
|-----------|------------|---------|
| **Total Float** | Max delay without delaying project | LT(j) - ET(i) - Duration |
| **Free Float** | Delay without affecting immediate successor | ET(j) - ET(i) - Duration |
| **Independent Float** | Delay independent of predecessors and successors | ET(j) - LT(i) - Duration (if ≥ 0) |

**For most MBA exams, Total Float is sufficient.**

---

## 🔵 PERT — THREE TIME ESTIMATES

PERT handles **uncertainty** in activity durations using three time estimates:

| Estimate | Symbol | Definition |
|---------|--------|-----------|
| **Optimistic Time** | to | Shortest possible duration (if everything goes perfectly) |
| **Most Likely Time** | tm | Most probable duration (modal estimate) |
| **Pessimistic Time** | tp | Longest duration (if things go wrong) |

### PERT Formulas:

**Expected Time:**
```
te = (to + 4tm + tp) / 6
```
(Weighted average — most likely gets 4× weight)

**Variance:**
```
σ² = [(tp - to) / 6]²
```
(Variance of activity duration)

**Standard Deviation:**
```
σ = (tp - to) / 6
```

---

## 🔵 PERT PROBABILITY CALCULATIONS ⭐

**Project Duration Mean:**
```
μ_project = Sum of te of all critical activities
```

**Project Duration Variance:**
```
σ²_project = Sum of σ² of all critical activities
```

**Project Duration Standard Deviation:**
```
σ_project = √(σ²_project)
```

**Probability Calculation:**
Using normal distribution:
```
Z = (D - μ_project) / σ_project

Where D = desired completion date
```
Then look up Z in standard normal table to find probability.

---

### PERT Worked Example:

**Critical path activities with estimates:**

| Activity | to | tm | tp | te | σ² |
|----------|----|----|----|----|-----|
| A | 2 | 3 | 4 | (2+12+4)/6=3 | [(4-2)/6]² = 0.11 |
| B | 3 | 5 | 7 | (3+20+7)/6=5 | [(7-3)/6]² = 0.44 |
| E | 4 | 6 | 8 | (4+24+8)/6=6 | [(8-4)/6]² = 0.44 |
| G | 3 | 5 | 7 | (3+20+7)/6=5 | [(7-3)/6]² = 0.44 |

**Project Mean Duration:**
```
μ = 3 + 5 + 6 + 5 = 19 weeks
```

**Project Variance:**
```
σ² = 0.11 + 0.44 + 0.44 + 0.44 = 1.43
σ = √1.43 = 1.20 weeks
```

**Q: What is the probability of completing the project in 21 weeks?**
```
Z = (21 - 19) / 1.20 = 2/1.20 = 1.67
P(Z ≤ 1.67) = 0.9525 (from normal table)
Probability of completing in 21 weeks = 95.25%
```

**Q: What is the probability of completing in 18 weeks?**
```
Z = (18-19)/1.20 = -0.83
P(Z ≤ -0.83) = 1 - P(Z ≤ 0.83) = 1 - 0.7967 = 0.2033
Probability = 20.33%
```

---

## 🔵 PROJECT CRASHING (Time-Cost Trade-off)

### What is Crashing?
Reducing an activity's duration by investing more resources (more workers, overtime, better equipment) — at a higher cost.

**Key Concepts:**

| Term | Definition |
|------|-----------|
| **Normal Duration** | Planned duration at standard cost |
| **Crash Duration** | Minimum possible duration with maximum resources |
| **Normal Cost** | Cost at normal duration |
| **Crash Cost** | Cost at crash duration (higher) |
| **Cost Slope** | Rate of increase in cost per unit time reduction |

**Cost Slope Formula:**
```
Cost Slope = (Crash Cost - Normal Cost) / (Normal Duration - Crash Duration)
             [₹ per week saved]
```

### Crashing Procedure:
1. Calculate cost slope for all activities
2. **Crash the critical activity with LOWEST cost slope first** (cheapest to speed up)
3. Reduce duration of that activity (but only until: another path becomes critical, OR activity is fully crashed)
4. Update critical path; recalculate project duration
5. Repeat until target duration reached or all critical activities fully crashed

**India Example:**
Mumbai Metro Line 3 was behind schedule. L&T (contractor) crashed by:
- Adding night shifts (overtime cost ↑)
- Increasing tunneling equipment (equipment cost ↑)
- Deploying additional engineers
Crashing increased cost but reduced delays and penalty clauses (avoiding delay costs worth more than crashing cost).

---

## 🔵 CPM vs PERT — SUMMARY

| Feature | CPM | PERT |
|---------|-----|------|
| Activity time | One estimate | Three estimates (to, tm, tp) |
| Formula | None needed | te = (to+4tm+tp)/6 |
| Probabilistic analysis | No | Yes (Z-score, normal distribution) |
| Critical Path | Yes | Yes |
| Crashing | Yes (focus) | Less common |
| Best for | Construction, engineering | R&D, uncertain projects |

---

## 🔴 EXAM-READY CONTENT

### Exam Template for PERT/CPM:
```
Step 1: Draw network diagram (list activities and precedences)
Step 2: Forward pass → Calculate ET for all events
Step 3: Backward pass → Calculate LT for all events
Step 4: Calculate Float = LT(j) - ET(i) - Duration
Step 5: Identify Critical Path (Float = 0)
Step 6: State project duration
Step 7 (PERT only): Calculate te and σ² for each activity
Step 8 (PERT only): Calculate μ and σ for project
Step 9 (PERT only): Use Z = (D-μ)/σ for probability
```

---

### KEY TERMS FLASHCARD

| Term | One-Line Definition |
|------|-------------------|
| CPM | Single time estimate; deterministic; focuses on time-cost trade-off |
| PERT | Three time estimates; probabilistic; focuses on schedule risk |
| Critical Path | Longest path; zero float; determines project duration |
| Float/Slack | Extra time an activity can be delayed without delaying project |
| ET (Earliest Time) | Earliest an event can occur (forward pass) |
| LT (Latest Time) | Latest an event can occur without delaying project (backward pass) |
| te | Expected PERT time = (to + 4tm + tp)/6 |
| σ² | PERT variance = [(tp-to)/6]² |
| Crashing | Reducing activity duration by adding resources (at extra cost) |
| Cost Slope | Extra cost per unit time saved by crashing |
| Dummy Activity | Zero-duration arrow to show dependency in AOA networks |

---

*Chapter 5 Complete | DMO | MBA 2nd Semester, DU SOL*
