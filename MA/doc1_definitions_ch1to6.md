# 📖 DOC 1: Exam Definitions + Analogies — Part 1 (Ch 1–6)
### Management Accounting | DU SOL MBA Sem 2

---

## CH 1: Cost Concepts

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Management Accounting** | Process of identifying, measuring, analyzing and communicating financial info to help managers plan, control and make decisions | BugZero CEO's monthly dashboard showing cost per project, team efficiency, profit — all for internal decisions only |
| **Cost** | The amount sacrificed/spent to acquire a product or service | ₹40,000 spent by BugZero on tools + engineer time to complete one testing contract |
| **Direct Cost** | Cost that can be directly and specifically traced to a particular product or job | QA engineer's salary when assigned 100% to one client project |
| **Indirect Cost (Overhead)** | Cost that cannot be directly traced to one product; shared across multiple products | Office electricity bill — shared by all BugZero teams, not one project |
| **Fixed Cost** | Cost that remains CONSTANT regardless of the level of output | BugZero's office rent ₹1L/month — same whether 1 or 100 projects run |
| **Variable Cost** | Cost that changes proportionately with the level of output | Cloud server usage fee — more tests run = more cost |
| **Semi-Variable Cost** | Cost that has BOTH a fixed component and a variable component | BugZero's internet: ₹2,000 fixed base + ₹500 per extra 10GB |
| **Sunk Cost** | A past cost already incurred that CANNOT be recovered, regardless of future decisions | ₹3L spent on a faulty testing tool — ignore this when deciding whether to keep using it |
| **Opportunity Cost** | The value of the BEST alternative foregone when a decision is made | BugZero choosing to test Module A means they CAN'T test Module B — value of B = opportunity cost |
| **Marginal Cost** | The additional cost of producing ONE extra unit of output | Cost of running one extra automated test case in BugZero's CI/CD pipeline |
| **Differential Cost** | The DIFFERENCE in total cost between two alternative decisions | Manual testing costs ₹1L; Automation costs ₹60K → Differential = ₹40K |
| **Relevant Cost** | A future cost that CHANGES with the decision being made — include in analysis | New variable costs when deciding to accept a new contract |
| **Irrelevant Cost** | A cost that does NOT change with the decision — EXCLUDE from analysis | Sunk costs, unavoidable fixed costs |
| **Normal Cost** | Cost incurred under normal, efficient operating conditions — included in product cost | BugZero QA team working 8 hrs/day at standard efficiency |
| **Abnormal Cost** | Cost arising from abnormal/avoidable circumstances — charged to P&L, NOT product | Extra cost due to server crash forcing re-testing of entire module |
| **Product Cost** | Cost attached to the product and carried in inventory (Material, Labour, Factory OH) | BugZero: cost of testing tools + engineer hours assigned to a specific project |
| **Period Cost** | Cost charged to the period it occurs, not attached to product (Admin, Selling costs) | BugZero CEO's salary — charged monthly regardless of how many projects run |

---

## CH 2: Material, Labour & Overhead

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Material Control** | A system to ensure the right material is available at the right time, in the right quantity, at minimum cost, preventing waste and theft | BugZero ensuring USB testing dongles are always available without over-ordering |
| **Reorder Level** | The stock level at which a fresh purchase order MUST be placed to avoid stock-out | BugZero places a new dongle order when stock hits 200 units |
| **Minimum Level** | The LOWEST level stock should fall to — a safety buffer against stock-out | BugZero never lets dongles fall below 95 units |
| **Maximum Level** | The HIGHEST stock level — prevents over-investment in inventory | BugZero never holds more than 460 dongles |
| **Danger Level** | Stock level below which production WILL STOP — emergency territory | Below 35 dongles = testing projects come to a halt! |
| **EOQ** | The order quantity that minimizes TOTAL inventory cost by balancing ordering cost and carrying cost | BugZero finds ordering 775 dongles at a time costs the least overall |
| **ABC Analysis** | Classification of inventory into A (high value, 10% items, 70% cost), B (medium), C (low value, 70% items, 5% cost) for differential control | BugZero's test servers = A (monitor daily); USB hubs = B; pens = C |
| **Time Rate** | A wage system where workers are paid based on TIME worked, regardless of output | QA engineer gets ₹200/hour whether testing is fast or slow |
| **Piece Rate** | A wage system where workers are paid based on OUTPUT produced, regardless of time | QA gets ₹10 for every test case written |
| **Taylor's Differential Piece Rate** | A two-rate piece system: efficient workers (≥ standard) get 120% rate; inefficient workers (< standard) get 80% rate | Standard = 100 tests/day. Worker does 120 → paid at 120% rate. Worker does 80 → paid at 80% rate |
| **Halsey Plan** | Incentive plan where worker gets time wages PLUS 50% of time saved as bonus | BugZero QA finishes 10-hour task in 6 hours → gets base pay + 50% of 4 saved hours as bonus |
| **Rowan Plan** | Incentive plan where bonus is a PROPORTION of time saved to standard time, applied to basic wages | Same scenario → bonus = (4÷10) × basic wages = 40% of basic wages as bonus |
| **Labour Turnover** | The rate at which employees leave and need to be replaced in an organization | 3 of BugZero's 10 QA engineers quit this year → 30% turnover rate |
| **Idle Time** | Time for which workers are PAID but NO productive work is done | BugZero QAs waiting 2 hours for client to provide access credentials — paid but not working |
| **Overhead** | All INDIRECT costs — Indirect Material + Indirect Labour + Indirect Expenses | BugZero's office rent, admin salaries, electricity — not traceable to one project |
| **OAR (Overhead Absorption Rate)** | Pre-determined rate used to charge overhead costs to individual products/jobs | BugZero charges ₹20 overhead per machine hour to each project |
| **Over-absorption** | Overhead ABSORBED exceeds actual overhead incurred — excess credited to P&L | BugZero absorbed ₹1,10,000 overhead but actual was only ₹1,05,000 → ₹5,000 over-absorbed |
| **Under-absorption** | Overhead ABSORBED is less than actual overhead — shortfall debited to P&L | BugZero absorbed ₹1,10,000 but actual was ₹1,15,000 → ₹5,000 under-absorbed |

---

## CH 3: Job, Batch & Contract Costing

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Job Costing** | A costing method where costs are collected separately for each unique job done to customer's specific requirements | BugZero tracking every hour, tool and expense specifically for a security testing job for one fintech client |
| **Batch Costing** | A form of job costing where a GROUP of identical units is costed together; cost per unit = total batch cost ÷ number of units | BugZero producing 100 identical test report templates — ₹50,000 batch cost ÷ 100 = ₹500 each |
| **Contract Costing** | Costing method for large, long-term (1+ year) contracts carried out at the CLIENT'S site | BugZero wins a ₹1Cr, 2-year contract to build automated testing for State Bank — all work at bank's premises |
| **Work Certified** | The value of work completed and officially certified/approved by an architect or engineer | Bank's project manager certifies ₹12L worth of BugZero's testing platform is complete |
| **Work Uncertified (WIP)** | Work physically completed but NOT yet certified — shown as WIP at COST on balance sheet | BugZero completed ₹50K of additional features not yet verified by client |
| **Retention Money** | A % of Work Certified that the client HOLDS BACK and pays only on full contract completion | Client holds 10% of ₹12L = ₹1.2L until BugZero finishes the entire 2-year contract |
| **Escalation Clause** | A contract provision allowing price revision if material/labour costs increase beyond a specified limit | BugZero's contract allows price increase if cloud costs rise by more than 15% |
| **Notional Profit** | Estimated profit earned on work done to date = Work Certified − Cost of Work Certified | BugZero certified ₹12L, cost was ₹8.3L → Notional Profit = ₹3.7L |

---

## CH 4: Process Costing

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Process Costing** | A costing method for continuous, mass production where identical units pass through multiple stages and cost is averaged across all output | BugZero's 3-stage testing pipeline: Unit Test → Integration → UAT. Each stage costs are tracked separately |
| **Normal Loss** | The expected, pre-estimated, unavoidable loss that occurs in normal production conditions — its cost is ABSORBED by good output | BugZero expects 10% of code builds to fail QA — this is normal and built into pricing |
| **Abnormal Loss** | Loss that EXCEEDS the normal expected level — caused by avoidable factors — CHARGED TO P&L as a loss | BugZero expects 10% failure but 18% failed this month → extra 8% = Abnormal Loss, charged to P&L |
| **Abnormal Gain** | When ACTUAL loss is LESS than normal loss — better than expected output — CREDITED TO P&L | BugZero expected 10% failure but only 6% failed → 4% Abnormal Gain — credited to P&L as a saving |
| **Equivalent Units (EU)** | WIP units converted into equivalent fully-complete units based on their % of completion | 100 WIP units that are 60% complete = 60 Equivalent Units (as if 60 units fully done) |
| **Joint Products** | Two or more products of SIGNIFICANT commercial value produced simultaneously from the same raw material up to the split-off point | BugZero's test run produces both a Security Report (₹30K value) and a Performance Report (₹20K value) — both significant |
| **By-Products** | A product of MINOR value produced incidentally alongside the main product | When BugZero documents tests, leftover data analysis can be sold cheaply as a basic report — minor value |
| **Split-off Point** | The point in the production process where joint products SEPARATE and can be individually identified | BugZero's testing process at the point where security testing separates from performance testing |

---

## CH 5: Marginal Costing & Decision Making

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Marginal Costing** | A costing technique where ONLY variable costs are charged to products. Fixed costs are treated as period costs and written off entirely to P&L in the period they occur | BugZero charges only cloud costs + engineer time (variable) to each project. Office rent (fixed) goes directly to P&L |
| **Contribution** | The amount by which sales revenue EXCEEDS variable cost — contributing first to fixed costs, then to profit | BugZero earns ₹1L per contract, spends ₹40K variable costs → ₹60K contribution (covers rent, then profit) |
| **P/V Ratio** | The percentage of each rupee of sales that represents contribution. Shows how profitable a product is relative to its sales | BugZero P/V = 60% means every ₹1 of revenue gives ₹0.60 contribution toward fixed costs and profit |
| **Break-Even Point (BEP)** | The level of sales at which total revenue EQUALS total cost — neither profit nor loss is made | BugZero needs 5 contracts/month to exactly cover rent + salaries. The 6th contract onwards = profit |
| **Margin of Safety (MOS)** | The amount by which actual sales EXCEED break-even sales. Shows how much sales can fall before a loss occurs | BugZero does 8 contracts, BEP is 5 → MOS = 3 contracts. Sales can drop by 3 before they lose money |
| **Absorption Costing** | A costing method where BOTH fixed AND variable costs are charged to products. Fixed overhead is absorbed into product cost | Traditional method: BugZero would include office rent as part of each project's cost |
| **Limiting Factor / Key Factor** | The scarce resource that constrains an organization's activity and limits its output | BugZero only has 200 QA engineer hours — they can't take unlimited projects |

---

## CH 6: Standard Costing & Variance Analysis

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Standard Cost** | A pre-determined, estimated cost set BEFORE production begins, representing the expected cost under efficient operating conditions | BugZero estimates each testing project SHOULD take 40 hrs at ₹500/hr = ₹20,000 standard cost |
| **Standard Costing** | A system where standard costs are set in advance, actual costs are recorded, variances are calculated, and corrective action is taken | BugZero planned ₹20K per project but actually spent ₹24K — investigate why using variance analysis |
| **Variance** | The DIFFERENCE between standard (planned) cost and actual cost — used to measure performance and control costs | BugZero variance = ₹24,000 actual − ₹20,000 standard = ₹4,000 Adverse |
| **Favourable Variance (F)** | When actual cost is LESS than standard cost (or actual revenue is MORE than standard) — a GOOD outcome | BugZero spent ₹18,000 instead of ₹20,000 planned → ₹2,000 Favourable — saved money! |
| **Adverse Variance (A)** | When actual cost is MORE than standard cost (or actual revenue is LESS than standard) — a BAD outcome | BugZero spent ₹24,000 instead of ₹20,000 planned → ₹4,000 Adverse — overspent! |
| **Material Price Variance** | Variance caused by paying a DIFFERENT price per unit of material than the standard price | BugZero planned to pay ₹10/dongle but paid ₹12 — price variance = Adverse |
| **Material Usage Variance** | Variance caused by using MORE or LESS material than the standard quantity for actual output | BugZero planned 500 dongles for 100 projects but used 520 — usage variance = Adverse |
| **Labour Rate Variance** | Variance caused by paying workers at a DIFFERENT rate than the standard wage rate | BugZero planned ₹500/hr for QA but paid ₹520/hr — rate variance = Adverse |
| **Labour Efficiency Variance** | Variance caused by workers taking MORE or LESS time than the standard hours for actual output | BugZero planned 400 hrs for 100 projects but workers took 420 hrs — efficiency variance = Adverse |
| **Ideal Standard** | A standard based on PERFECT efficiency with zero waste, zero idle time — rarely achievable in practice | BugZero's theoretical best: every test perfect first time, no rework, zero errors |
| **Current Standard** | A standard set for current period's expected conditions — MOST PRACTICAL and commonly used | BugZero's realistic target: 95% pass rate, 5% rework expected this quarter |

---
*📅 Doc 1 Part 1 | Ch 1–6 Definitions | Management Accounting | DU SOL MBA Sem 2*
