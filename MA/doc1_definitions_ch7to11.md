# 📖 DOC 1: Exam Definitions + Analogies — Part 2 (Ch 7–11)
### Management Accounting | DU SOL MBA Sem 2

---

## CH 7: Budgets & Budgetary Control

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Budget** | A formal, quantitative statement prepared IN ADVANCE for a specific future period expressing management's plans in financial or physical terms | BugZero's annual plan: "We will earn ₹50L, spend ₹40L, profit ₹10L" — written before the year starts |
| **Budgetary Control** | A management system where budgets are prepared, actual results are compared against budgets, variances are identified, and corrective action is taken | BugZero reviews every month: planned ₹4L revenue vs actual ₹3.5L → finds reason and fixes it |
| **Principal Budget Factor** | The factor that limits an organization's activities and around which all other budgets must be built first | BugZero has only 10 QA engineers → max 20 projects/month → sales budget must not exceed this |
| **Fixed Budget** | A budget prepared for ONE level of activity only that does NOT adjust when actual output differs from planned | BugZero budgets for 100 projects; actual = 80 → direct comparison is unfair and misleading |
| **Flexible Budget** | A budget that ADJUSTS variable costs to the actual level of activity achieved, giving a fair comparison | BugZero's flexible budget for 80 projects = Fixed ₹5L + Variable ₹40K×80 = ₹37L (fair comparison) |
| **Zero-Based Budgeting (ZBB)** | A budgeting method where every expense must be justified from ZERO each period — no automatic carry-forward from previous year | BugZero must justify EVERY tool: "Do we still need this Selenium license? This Jira plan?" — not just +10% last year |
| **Sales Budget** | A budget showing expected revenue from sales — the STARTING POINT for all other budgets | BugZero projects 20 contracts × ₹1L = ₹20L monthly sales — all other budgets flow from this |
| **Production Budget** | A budget showing the number of units that must be produced to meet sales targets and desired closing stock levels | BugZero needs 20 projects delivered but wants 5 in pipeline → produce 25 (20 + 5 closing − 0 opening) |
| **Cash Budget** | A budget showing expected CASH inflows and outflows period by period to reveal potential cash surpluses or deficits | BugZero sees in February's cash budget: ₹2L shortfall → arranges overdraft facility in January itself |
| **Master Budget** | The SUMMARY budget combining all functional budgets into a Budgeted P&L, Balance Sheet and Cash Flow Statement | BugZero's complete annual financial picture — one document showing all numbers together |

---

## CH 8: Cost Management

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Cost Management** | A strategic, long-term approach to understanding and optimizing costs to create value and achieve organizational goals | BugZero deciding to invest in automation (higher upfront cost) to save ₹5L/year in manual testing |
| **Cost Control** | The process of monitoring actual costs against pre-set budgets/standards and taking corrective action when costs exceed targets | BugZero's finance team flagging when monthly tool costs cross ₹2L budget and investigating |
| **Cost Reduction** | A PERMANENT lowering of costs through improved methods, better technology or elimination of waste WITHOUT sacrificing quality | BugZero switching from paid Jira to free GitLab Issues — saves ₹30K/year permanently |
| **Activity-Based Costing (ABC)** | A costing method that assigns overhead costs to products based on the ACTIVITIES they consume and the cost drivers of those activities | Instead of spreading all BugZero overhead equally, ABC traces: "Product A used 5 setups → charge 5×₹2,000 setup cost" |
| **Cost Pool** | A group of overhead costs related to ONE specific activity | BugZero's "Test Environment Setup" pool = all costs related to setting up test environments |
| **Cost Driver** | The factor that CAUSES the cost of an activity to increase or decrease | For BugZero's setup activity, cost driver = NUMBER OF SETUPS (more setups = more setup cost) |
| **Theory of Constraints (TOC)** | A management philosophy stating that every system has at least one BOTTLENECK limiting its output; success comes from identifying and managing that bottleneck | BugZero's only Senior QA reviews all projects → everyone waits → this is the bottleneck! |
| **Throughput** | In Throughput Accounting, Throughput = Sales Revenue MINUS Direct Material Cost ONLY (not labour, not overhead) | BugZero sells contract for ₹1L, spends ₹20K on direct tools → Throughput = ₹80K |
| **Target Costing** | A market-driven costing approach where Target Cost = Market Price − Desired Profit. The product must be designed/engineered to meet this target | Market charges ₹80K for security testing. BugZero wants 25% profit = ₹20K. Target Cost = ₹60K — must deliver within this |
| **Value Chain Analysis** | Porter's framework identifying all primary and support activities that create value for the customer, used to find cost reduction and value-adding opportunities | BugZero maps: Get requirements → Test → Report → Support. Finds "report writing" takes too long — reduce cost here |
| **Life Cycle Costing** | Tracking and managing the TOTAL cost of a product across its entire life from R&D to disposal — not just manufacturing/delivery cost | BugZero's automation tool: ₹5L R&D + ₹15L build + ₹5L maintenance + ₹50K disposal = ₹25.5L true total cost |
| **Just-in-Time (JIT)** | A production philosophy: produce the right product, at the right time, in the right quantity — eliminating all waste, especially excess inventory | BugZero uses AWS cloud: spins servers UP when project starts, shuts DOWN when done — no idle servers running 24/7 |
| **Backflush Costing** | A simplified costing system used with JIT where costs are recorded only at COMPLETION of production — bypassing traditional WIP tracking | BugZero records testing costs only when final report is delivered to client, not at each testing stage |

---

## CH 9: Performance Measurement — BSC

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Balanced Scorecard (BSC)** | A strategic performance framework by Kaplan & Norton (1992) that measures performance from FOUR perspectives: Financial, Customer, Internal Process, and Learning & Growth | BugZero's monthly KPI board: Profit (Financial) + Client Satisfaction (Customer) + Bug Rate (Internal) + Training Hours (Learning) |
| **Financial Perspective** | BSC dimension measuring how the company looks to SHAREHOLDERS — profitability, revenue growth, ROI | BugZero: 25% profit margin, 30% revenue growth year-on-year |
| **Customer Perspective** | BSC dimension measuring how CUSTOMERS perceive the company — satisfaction, retention, market share | BugZero: 4.5/5 satisfaction score, 70% repeat client rate |
| **Internal Process Perspective** | BSC dimension measuring what the company must EXCEL AT internally — quality, efficiency, innovation | BugZero: Bug escape rate < 3%, test cycle time 2 days, 60% automation coverage |
| **Learning & Growth Perspective** | BSC dimension measuring the company's ability to IMPROVE and BUILD CAPABILITIES — training, skills, technology | BugZero: 3 certifications per engineer per year, 85% employee retention |
| **Performance Drivers** | LEAD indicators — factors that DRIVE future performance results; they predict what results will come | BugZero training hours today → engineer skills tomorrow → better quality next month → higher client satisfaction next quarter |
| **Performance Measures** | LAG indicators — measure PAST outcomes; tell what has already happened | BugZero's client satisfaction score this month = result of past 3 months of work |
| **Return on Investment (ROI)** | Financial performance measure: Net Profit ÷ Capital Employed × 100. Shows what % return is earned on money invested | BugZero earns ₹6L profit on ₹30L investment → ROI = 20% — means ₹20 earned per ₹100 invested |
| **Residual Income (RI)** | Net Profit MINUS the minimum required return on capital. Positive RI = value created; Negative RI = value destroyed | BugZero profit ₹6L, required return = 15% of ₹30L = ₹4.5L → RI = ₹1.5L (creating value above minimum!) |

---

## CH 10: Inventory Management

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Inventory Management** | The systematic process of ordering, storing, using and replenishing a company's inventory to ensure smooth operations while minimizing total inventory costs | BugZero ensuring USB dongles, server RAM and licenses are always available without overstocking |
| **Ordering Cost** | Cost incurred EACH TIME a purchase order is placed, regardless of order size (admin, inspection, freight per order) | BugZero: every time they order dongles, they spend ₹500 on paperwork and delivery — regardless of how many |
| **Carrying Cost** | Cost of HOLDING inventory over time (warehouse, insurance, capital tied up, obsolescence risk) | BugZero storing 1,000 spare dongles costs ₹2/unit/year in storage and insurance |
| **Stock-out Cost** | Cost incurred when inventory RUNS OUT and demand cannot be met (lost sales, emergency purchases, production downtime) | BugZero runs out of test servers → project halts → client penalizes ₹50K for delay |
| **VED Analysis** | Classification of inventory by CRITICALITY: Vital (operations stop without it), Essential (severely hampered), Desirable (useful but not critical) | Selenium license = Vital; Postman = Essential; Adobe Acrobat for reports = Desirable |
| **FSN Analysis** | Classification of inventory by MOVEMENT RATE: Fast-moving (consumed quickly), Slow-moving (low usage), Non-moving (dead stock) | USB-C cables = Fast; ethernet switches = Slow; old CD-ROM drives = Non-moving (dispose!) |
| **HML Analysis** | Classification by UNIT PRICE: High value items, Medium value items, Low value items — controls purchasing authority | High: Server (requires CEO approval); Medium: Laptop (manager approval); Low: USB cable (team lead approval) |
| **SDE Analysis** | Classification by AVAILABILITY: Scarce (hard to get — high safety stock), Difficult (takes time), Easy (readily available — minimal stock) | Specialized testing chip = Scarce (keep 6-month stock); specific RAM = Difficult; USB cables = Easy |
| **GOLF Analysis** | Classification by SOURCE: Government supply, Ordinary market, Local supplier, Foreign import | Foreign-sourced testing equipment = F (needs 3-month lead time planning) |
| **FIFO** | First In First Out: Oldest stock issued FIRST. Closing stock valued at LATEST prices. In rising prices → highest profit | BugZero issues first-purchased dongles first. Stock on hand = recently bought (costlier) ones |
| **LIFO** | Last In First Out: Newest stock issued FIRST. Closing stock at OLDEST prices. In rising prices → lowest profit. NOT accepted under Ind AS | BugZero issues latest batch first. Old (cheaper) stock remains, understating balance sheet |
| **Weighted Average Price** | Issues valued at AVERAGE cost. WAP recalculated each time new receipt arrives = Total Value ÷ Total Units | After each dongle purchase, BugZero recalculates average price and issues at that rate |

---

## CH 11: Performance Measurement & Evaluation

| Term | Exam Definition | Real-Life Analogy |
|------|----------------|-------------------|
| **Cost Centre** | A responsibility centre where the manager is accountable for COSTS ONLY — no control over revenue | BugZero's IT infrastructure team: judged only on keeping tech costs within ₹1.5L/month budget |
| **Revenue Centre** | A responsibility centre where the manager is accountable for REVENUE ONLY — no control over costs | BugZero's Sales team: judged only on bringing in ₹20L revenue per month |
| **Profit Centre** | A responsibility centre where the manager controls BOTH REVENUE AND COSTS — measured on profit | BugZero's QA Services Division: manager controls pricing AND team costs → measured on division profit |
| **Investment Centre** | A responsibility centre where manager controls Revenue, Costs AND CAPITAL ASSETS — measured by ROI, RI, EVA | BugZero as a whole company: CEO decides all revenue, costs AND how capital is invested |
| **Economic Value Added (EVA)** | True economic profit = NOPAT minus the full cost of ALL capital (debt + equity). Positive EVA = real value created for shareholders | BugZero earned ₹10.5L after tax, but investors expect 12% on ₹80L = ₹9.6L → EVA = ₹0.9L (creating real value!) |
| **NOPAT** | Net Operating Profit After Tax = Operating Profit × (1 − Tax Rate). Excludes financing costs for fair comparison | BugZero operating profit ₹15L, tax 30% → NOPAT = ₹15L × 0.70 = ₹10.5L |
| **WACC** | Weighted Average Cost of Capital = average cost of debt and equity weighted by their proportions. The minimum return investors expect | BugZero: 60% equity at 15% + 40% debt at 8% → WACC = 60%×15% + 40%×8% = 9% + 3.2% = 12.2% |
| **Performance Pyramid** | Lynch & Cross (1991) framework: Corporate vision flows DOWN as objectives; operational results flow UP as measures. External (quality/delivery) vs Internal (cycle time/waste) | BugZero CEO sets "20% profit growth" → flows down to QA team as "reduce rework by 30%" → results flow back up |
| **Building Block Model** | Fitzgerald & Moon (1996) performance framework for SERVICE firms with 3 blocks: 6 Dimensions of performance, 3 Standards for target-setting, 3 Rewards for motivation | BugZero uses all 6 dimensions (quality, flexibility, etc.), sets achievable standards, rewards fairly |
| **6 Dimensions (Building Block)** | Financial Performance, Competitiveness, Quality, Flexibility, Resource Utilization, Innovation — what to MEASURE in service firms | BugZero measures: profit (financial), client wins (competitive), bug rate (quality), response time (flexibility) |
| **3 Standards (Building Block)** | Ownership (managers set own targets), Achievability (stretch but realistic), Equity (fair to all departments) | BugZero QA manager helps SET the 95% pass rate target → more committed to achieving it |
| **3 Rewards (Building Block)** | Clarity (rewards understood), Motivation (rewards drive right behavior), Controllability (rewarded for what they control) | BugZero clearly tells QA team: "Hit <3% bug escape rate → ₹10K bonus" — clear, motivating, within their control |
| **Performance Prism** | Neely et al. (2002) stakeholder-first framework with 5 facets: Stakeholder Satisfaction, Strategies, Processes, Capabilities, Stakeholder Contribution | BugZero asks clients what THEY want first → then builds strategy, processes, capabilities around that |
| **Triple Bottom Line (TBL)** | Elkington (1994) framework: business success measured across Profit (Economic), People (Social), Planet (Environmental) — the 3 Ps | BugZero: Profit = ₹30L | People = gender pay equity + CSR | Planet = renewable energy servers |
| **Transfer Pricing** | The price charged when one DIVISION of a company sells goods or services to another division of the SAME company | BugZero's Tool Development division "sells" automation tools to QA Services division at an agreed internal price |

---
*📅 Doc 1 Part 2 | Ch 7–11 Definitions | Management Accounting | DU SOL MBA Sem 2*
