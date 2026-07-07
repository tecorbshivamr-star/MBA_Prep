# 🖥️ LESSON 4: COMPUTER-BASED INFORMATION SYSTEMS
### MBA MIS Revision Notes | Exam-Ready

---

> [!IMPORTANT]
> **Top Exam Topics:** Distinguish all 6 IS types (OAS→TPS→MIS→DSS→GDSS→EIS), Expert Systems, and EUC. Comparison tables = full marks. One of the most important chapters in MIS!

---

## 🎯 LEARNING OBJECTIVES

After this chapter, you should be able to:
- Explain and distinguish all **Computer-Based IS types**
- Describe **OAS, TPS, MIS, DSS, GDSS, EIS** with examples
- Understand **AI and Expert Systems**
- Define **End-User Computing (EUC)** and its types, advantages, and significance

---

## 1. 📖 INTRODUCTION

### The IS Pyramid:

```
                    ┌───────────┐
                    │    EIS    │  ← Top Management (Strategic)
                    └─────┬─────┘
               ┌──────────┴──────────┐
               │   DSS / GDSS / AI   │  ← Middle/Senior Mgmt (Semi-structured)
               └──────────┬──────────┘
          ┌───────────────┴───────────────┐
          │              MIS              │  ← Middle Management (Tactical)
          └───────────────┬───────────────┘
     ┌─────────────────────┴─────────────────────┐
     │                    TPS                    │  ← Operational Level (Structured)
     └─────────────────────┬─────────────────────┘
┌─────────────────────────────────────────────────────┐
│                       OAS                          │  ← All Levels (Support)
└────────────────────────────────────────────────────-┘
```

> Each system serves a **different level of management** and handles **different types of problems**.

> **Master Mnemonic for all types: "OTM-DGE-AI"**
> - **O**AS — Office Automation System
> - **T**PS — Transaction Processing System
> - **M**IS — Management Information System
> - **D**SS — Decision Support System
> - **G**DSS — Group Decision Support System
> - **E**IS — Executive Information System
> - **AI** — Artificial Intelligence & Expert Systems

---

## 2. 📋 OFFICE AUTOMATION SYSTEM (OAS)

### Definition:
> **OAS** is a computer-based system that **automates routine office tasks** such as word processing, communication, scheduling, and document management to improve the productivity of office workers.

### Purpose:
- Replace manual paperwork with digital tools
- Speed up communication and document handling
- Improve productivity of clerical and professional staff

### Components / Tools of OAS:

> **Mnemonic: "DWES-CV"**
> - **D**ocument Management (Word Processing)
> - **W**orkflow Management
> - **E**lectronic Communication (Email, Messaging)
> - **S**cheduling / Calendar Management
> - **C**onferencing (Video, Audio)
> - **V**oice Processing (Voicemail, Speech recognition)

| OAS Tool | Description | Real Example |
|----------|-------------|-------------|
| **Word Processing** | Create, edit, format documents digitally | MS Word, Google Docs |
| **Spreadsheets** | Numerical data analysis and calculations | MS Excel, Google Sheets |
| **Email** | Electronic communication | Outlook, Gmail |
| **Presentation** | Create slide-based presentations | PowerPoint, Google Slides |
| **Scheduling** | Calendar and meeting management | Google Calendar, Outlook Calendar |
| **Video Conferencing** | Online meetings | Zoom, Microsoft Teams, Google Meet |
| **Document Management** | Store, organize, retrieve digital documents | SharePoint, Google Drive |
| **Desktop Publishing** | Professional layout and design | Adobe InDesign, Canva |

### Advantages of OAS:
- Reduces paperwork and physical storage needs
- Faster communication across locations
- Improves collaboration (multiple users edit same document)
- Cost savings (less printing, postage, travel)

### Real-Life Example:
> **Infosys** uses OAS tools (MS Teams, SharePoint, Outlook) to manage communication and documents across 3 lakh+ employees in 50+ countries — without a single physical file.

---

## 3. 💳 TRANSACTION PROCESSING SYSTEM (TPS)

### Definition:
> **TPS** is a computerized IS that **records, processes, and stores day-to-day business transactions** in a fast, accurate, and reliable manner.

> A "transaction" = any business event that generates or changes data: a sale, a payment, an order, a deposit.

### Characteristics of TPS:

> **Mnemonic: "RAPID"**
> - **R**apid processing (high speed)
> - **A**ccuracy — zero tolerance for errors
> - **P**re-defined processing (structured, routine tasks)
> - **I**ntegrity — data consistency must be maintained
> - **D**ependability — must work 24/7 without failure

### Two Modes of TPS Processing:

| Mode | Description | When Used | Example |
|------|-------------|-----------|---------|
| **Batch Processing** | Transactions collected and processed together at scheduled intervals | When real-time not critical | Payroll processed at month-end; utility bills generated nightly |
| **Real-Time (OLTP)** | Each transaction processed immediately as it occurs | When instant update needed | ATM withdrawal, UPI payment, online ticket booking |

### Examples of TPS in Action:

| Industry | TPS Application |
|----------|----------------|
| **Banking** | ATM transactions, fund transfers, loan payments |
| **Retail** | Point-of-sale (POS) billing systems at D-Mart, Reliance |
| **Airlines** | Booking, check-in, seat allocation (IRCTC, IndiGo) |
| **E-commerce** | Order placement, payment, inventory update (Amazon, Flipkart) |
| **HR** | Payroll processing, attendance tracking |
| **Telecom** | Call billing, recharge, data usage tracking (Jio, Airtel) |

### Key Features:
- Handles **large volumes** of simple, structured transactions
- Provides **audit trail** — complete record of all transactions
- Forms the **data foundation** for all higher-level IS (MIS, DSS, EIS)
- Must be **ACID compliant**:
  - **A**tomicity (all or nothing)
  - **C**onsistency (data remains valid)
  - **I**solation (concurrent transactions don't interfere)
  - **D**urability (committed transactions are permanent)

### Real-Life Example:
> When you pay via UPI on Zomato — the TPS: verifies your bank balance → deducts amount → credits Zomato's account → updates order status → generates transaction ID — all in under 2 seconds!

---

## 4. 📊 MANAGEMENT INFORMATION SYSTEM (MIS)

### Definition:
> **MIS** is an IS that **collects data from TPS, processes it, and provides structured, periodic reports** to middle-level managers to support planning, control, and decision making.

### Key Characteristics:

> **Mnemonic: "SPIRO"**
> - **S**tructured reports (pre-defined formats)
> - **P**eriodic (daily, weekly, monthly)
> - **I**nternal focus (company data)
> - **R**outine decisions (not novel problems)
> - **O**perational/Tactical management level

### How MIS Works:
```
TPS Data (raw transactions)
      ↓
MIS processes + summarizes
      ↓
Reports to Middle Managers
(Weekly sales report, Monthly inventory report, etc.)
```

### Types of MIS Reports:

| Report Type | Description | Example |
|-------------|-------------|---------|
| **Scheduled/Periodic** | Generated at fixed intervals | Monthly sales report every 1st of the month |
| **Exception Report** | Triggered only when something unusual occurs | Alert when inventory falls below minimum level |
| **Demand/Ad-hoc Report** | Generated on request | Manager asks: "What were Q3 sales in South India?" |
| **Summary Report** | Aggregated data in condensed form | Total sales by product category for the year |
| **Comparative Report** | Compares current vs past or vs budget | Actual sales vs target sales |

### Real-Life Example:
> **Big Bazaar's** MIS generates weekly reports showing: which product categories are selling fast, which stores are underperforming, what's the stock level across all outlets — helping regional managers take corrective actions.

### MIS vs TPS:

| Feature | TPS | MIS |
|---------|-----|-----|
| **Focus** | Recording transactions | Reporting and summarizing |
| **User** | Operational staff | Middle managers |
| **Data** | Detailed, real-time | Summarized, periodic |
| **Output** | Transaction records | Management reports |
| **Decision type** | Structured, routine | Semi-structured |

---

## 5. 🧠 DECISION SUPPORT SYSTEM (DSS)

### Definition:
> **DSS** is an interactive, computer-based IS that **supports semi-structured and unstructured managerial decisions** by combining data, analytical models, and user-friendly interfaces.

### Key Difference from MIS:
> MIS gives you **reports** (what happened). DSS helps you **analyze** (what should I do about it?).

### Characteristics of DSS:

> **Mnemonic: "FIAMI"**
> - **F**lexible — adapts to user's changing needs
> - **I**nteractive — user controls the analysis
> - **A**nalytical models — uses statistical/mathematical tools
> - **M**ultiple scenarios — "what-if" analysis capability
> - **I**ntegrates data from multiple sources

### Components of DSS:

| Component | Description |
|-----------|-------------|
| **Database** | Internal + external data (TPS data, market data, government data) |
| **Model Base** | Statistical, financial, and optimization models |
| **User Interface** | Easy-to-use screens, dashboards, query tools |
| **Model Management** | Software that manages and runs analytical models |

### Types of DSS:

| Type | Description | Example |
|------|-------------|---------|
| **Model-driven DSS** | Uses mathematical/statistical models | Financial forecasting model for Tata Motors |
| **Data-driven DSS** | Analyzes large databases | Flipkart's sales analysis by region/product |
| **Communication-driven DSS** | Supports group collaboration | Video conferencing + shared analysis tools |
| **Document-driven DSS** | Manages and retrieves documents | Legal research tools, policy document retrieval |
| **Knowledge-driven DSS** | Uses rules and expertise | Medical diagnosis suggestion systems |

### Real-Life Examples:
- **Airlines (IndiGo):** DSS models optimal ticket pricing based on demand, time-to-departure, competitor prices — revenue management
- **HDFC Bank:** DSS helps credit managers decide whether to approve large business loans by modeling risk factors
- **Swiggy:** DSS models optimal delivery partner allocation based on location, traffic, order volume

### MIS vs DSS:

| Feature | MIS | DSS |
|---------|-----|-----|
| **Purpose** | Report what happened | Help decide what to do |
| **Interaction** | Low (pre-set reports) | High (user drives analysis) |
| **Decision type** | Structured | Semi-structured / Unstructured |
| **Flexibility** | Low | High |
| **Output** | Fixed format reports | Customized analysis, models |
| **User** | Middle managers | Senior managers, analysts |

---

## 6. 👥 GROUP DECISION SUPPORT SYSTEM (GDSS)

### Definition:
> **GDSS** is a computer-based IS that **supports collective decision making by groups** — providing tools for communication, idea sharing, voting, and consensus building among multiple participants.

### Why GDSS?
> Many important business decisions are made by **committees or teams** (not individuals). GDSS enables efficient, structured group collaboration — especially when members are in different locations.

### Features of GDSS:

> **Mnemonic: "AVCE"**
> - **A**nonymity — members can share ideas without attribution (reduces politics/fear)
> - **V**oting/Ranking tools — structured way to reach consensus
> - **C**ollaboration tools — shared whiteboards, document editing
> - **E**lectronic brainstorming — simultaneous idea generation

### Components of GDSS:

| Component | Description |
|-----------|-------------|
| **Electronic Brainstorming** | Multiple members type ideas simultaneously — all see all ideas |
| **Idea Organizer** | Groups, categorizes, and ranks ideas generated |
| **Voting Tools** | Electronic voting to rank options or reach consensus |
| **Policy Formation** | Tools to draft and refine policy/decision statements |
| **Group Dictionary** | Common glossary to ensure everyone uses same terms |

### Advantages of GDSS:
1. **Anonymity** reduces groupthink and political pressure
2. **Simultaneous input** — all members contribute at same time (faster than sequential speaking)
3. **Automatic documentation** — all ideas captured digitally
4. **Better participation** — even shy members contribute freely
5. **Geographically dispersed** teams can collaborate effectively

### Disadvantages of GDSS:
1. Loss of **non-verbal cues** (body language, tone)
2. **Technology resistance** among some members
3. **Anonymity** can be misused for irresponsible comments
4. **Initial setup cost** is high
5. Too much focus on process may miss creative breakthroughs

### Real-Life Example:
> A multinational company's board meeting with members in Mumbai, London, and New York uses GDSS tools (like Mentimeter, MS Teams + voting features) to evaluate 5 acquisition targets and reach a consensus decision.

### DSS vs GDSS:

| Feature | DSS | GDSS |
|---------|-----|------|
| **Users** | Individual decision maker | Group of decision makers |
| **Focus** | Analysis and modeling | Collaboration and consensus |
| **Key Feature** | What-if analysis | Electronic brainstorming, voting |
| **Anonymity** | Not applicable | Key feature |

---

## 7. 👔 EXECUTIVE INFORMATION SYSTEM (EIS)

### Definition:
> **EIS** (also called **ESS — Executive Support System**) is an IS designed specifically for **top-level executives** to access strategic information in a **highly summarized, visual, and easy-to-use format**.

### Why Executives Need a Special IS?
- Executives deal with **unstructured, strategic decisions**
- They need **big picture data** — not detailed transaction records
- They are often **not technical** — need very simple interfaces
- They need data from **both internal and external sources**

### Characteristics of EIS:

> **Mnemonic: "DEALS"**
> - **D**rill-down capability (zoom in for detail)
> - **E**asy-to-use interface (touchscreen, graphical)
> - **A**ggregate summary level view
> - **L**ive / real-time data
> - **S**trategic external data (competitor info, market trends)

### Features of EIS:

| Feature | Description |
|---------|-------------|
| **Dashboard** | Visual overview of key KPIs (Key Performance Indicators) |
| **Drill-Down** | Start from summary, click to see details progressively |
| **Exception Highlighting** | Alerts when KPIs deviate from targets (red/yellow/green indicators) |
| **Ad-hoc Queries** | Executives can ask questions without IT help |
| **External Data** | Integrates competitor data, stock prices, news feeds |
| **Mobile Access** | Available on tablets, smartphones for executives on the move |

### Real-Life Example:
> **Mukesh Ambani's** executive dashboard at Reliance shows: Real-time revenue across all divisions (Jio, Retail, Refining), market share vs competitors, stock price, global oil prices — all on one screen. Drill-down to see which Jio circle is underperforming.

### EIS vs MIS vs DSS:

| Feature | MIS | DSS | EIS |
|---------|-----|-----|-----|
| **User** | Middle managers | Analysts/Managers | Top executives (CEO, CFO) |
| **Decision type** | Structured/routine | Semi-structured | Unstructured/strategic |
| **Data** | Internal, summarized | Internal + external | Highly aggregated + external |
| **Interaction** | Low | High | Very easy (graphical) |
| **Output** | Periodic reports | Models, scenarios | Dashboards, KPIs |
| **Time horizon** | Short/medium | Medium | Long-term (strategic) |

---

## 8. 🤖 ARTIFICIAL INTELLIGENCE & EXPERT SYSTEMS

### Artificial Intelligence (AI):

> **Definition:** AI is the simulation of **human intelligence processes by computer systems** — including learning, reasoning, problem solving, and decision making.

### Types of AI in Business:

| AI Type | Description | Example |
|---------|-------------|---------|
| **Machine Learning** | System learns from data and improves automatically | Netflix recommendation engine learns your preferences |
| **Natural Language Processing (NLP)** | Computers understand and generate human language | Google Assistant, ChatGPT, Alexa |
| **Computer Vision** | Computers interpret images/video | Ola's driver selfie verification system |
| **Robotics / RPA** | Physical or software robots automating tasks | Amazon warehouse robots, RPA in banking |
| **Predictive Analytics** | AI predicts future outcomes | Flipkart predicts demand for products before festivals |

---

### Expert Systems (ES):

> **Definition:** An **Expert System** is a computer program that **emulates the decision-making ability of a human expert** in a specific domain using a knowledge base and inference engine.

> Also called: **Knowledge-Based Systems**

### Components of Expert System:

> **Mnemonic: "KIRU"**
> - **K**nowledge Base — repository of expert knowledge (facts + rules)
> - **I**nference Engine — the "reasoning" component (applies rules to facts)
> - **R**ule Base — IF-THEN rules representing expert logic
> - **U**ser Interface — how users interact with the system

```
User Question
      ↓
User Interface
      ↓
Inference Engine (applies rules from Rule Base)
      ↓
Knowledge Base (facts + expert rules)
      ↓
Recommendation/Decision
```

### Example of Expert System Rules:
```
IF patient has fever > 38°C
AND patient has cough
AND patient has body ache
THEN diagnose as likely Influenza
AND recommend antiviral medication
```

### Real-Life Expert System Examples:

| Domain | ES Application |
|--------|---------------|
| **Medicine** | MYCIN (diagnoses bacterial infections, recommends antibiotics) |
| **Banking** | Credit scoring — should this loan be approved? |
| **Insurance** | Risk assessment — what premium should be charged? |
| **Engineering** | XCON (configures computer systems for Digital Equipment Corp.) |
| **Legal** | Legal research and case outcome prediction |
| **Agriculture** | Crop disease diagnosis systems for Indian farmers |

### Advantages of Expert Systems:
1. Makes **expert knowledge available** 24/7 (human experts sleep!)
2. **Consistent decisions** — no mood-based variation
3. Can work in **hazardous environments** where humans can't
4. **Trains junior staff** by explaining reasoning
5. **Preserves knowledge** — expert's knowledge doesn't retire

### Disadvantages of Expert Systems:
1. **Narrow scope** — only works within its specific domain
2. **Cannot handle novel situations** not in knowledge base
3. **Expensive and time-consuming** to build (knowledge acquisition problem)
4. **Knowledge base becomes outdated** — needs regular updating
5. **Cannot learn** (unlike AI/ML) — rules must be manually updated

### AI vs Expert Systems:

| Feature | Expert System | AI / Machine Learning |
|---------|--------------|----------------------|
| **Learning** | No — rules manually programmed | Yes — learns from data |
| **Domain** | Narrow, specific domain | Broad, general |
| **Reasoning** | Rule-based (IF-THEN) | Pattern recognition |
| **Transparency** | Explainable (can show which rule used) | Often "black box" |
| **Example** | Medical diagnosis system | Netflix recommendations |

---

## 9. 💻 END-USER COMPUTING (EUC)

### Definition:
> **End-User Computing (EUC)** is the ability of **non-IT professional users (end users)** to directly develop, use, and control their own IS applications — without depending on the IT department.

> EUC emerged because: users knew their own needs best, IT departments had long backlogs, and user-friendly tools became available.

---

### Types of EUC:

> **Mnemonic: "CAPD"**
> - **C**ommand-level users
> - **A**pplication developers (end users)
> - **P**rogrammers (functional)
> - **D**ata users (non-programming)

| Type | Description | Example |
|------|-------------|---------|
| **Non-programming EUC** | Users run pre-built applications, don't write code | Accountant using Tally, HR using HRMS software |
| **Command-level EUC** | Users enter commands/queries to retrieve data | Using SQL queries to pull reports from database |
| **End-User Programming** | Users write simple programs using Excel macros, MATLAB | Finance manager building VBA macros in Excel |
| **Functional Support Personnel** | IT-literate non-IT staff who support other users | A "super-user" in accounts who trains colleagues on SAP |
| **End-User Application Development** | Users build complete applications using low-code/no-code tools | Marketing manager builds CRM tracker in MS Access or Airtable |

---

### Advantages of EUC:

> **Mnemonic: "FRISCO"**
> - **F**aster development — no waiting for IT dept
> - **R**esponsiveness to user needs
> - **I**ndependence from IT dept
> - **S**atisfaction — users get exactly what they need
> - **C**ost reduction — saves IT department resources
> - **O**wnership — users feel ownership of their tools

| Advantage | Description |
|-----------|-------------|
| **Faster Development** | Users build tools quickly without lengthy IT project cycles |
| **Better fit** | Tools match user needs exactly — no misunderstanding between user and IT |
| **Reduced IT backlog** | Simple requests handled by users free IT for complex projects |
| **Increased satisfaction** | Users feel in control of their work tools |
| **Cost effective** | Many small apps built at near-zero IT cost |
| **Innovation** | Users experiment and innovate at grassroots level |

---

### Disadvantages of EUC:

> **Mnemonic: "SQUAD"**
> - **S**ecurity risks — no IT oversight
> - **Q**uality issues — no testing, poor documentation
> - **U**ncontrolled data — multiple versions, inconsistency
> - **A**udit problems — hard to track and verify
> - **D**uplication — multiple users build same tools independently

| Disadvantage | Description |
|-------------|-------------|
| **Security Risk** | Users may not follow security protocols — data breaches |
| **Poor Quality** | No formal testing — bugs, errors in user-built apps |
| **Data Inconsistency** | Different users maintain different versions of same data |
| **Lack of Documentation** | User-built systems have no proper documentation — knowledge lost if user leaves |
| **Redundancy** | Same application built multiple times by different users independently |
| **Shadow IT** | Unauthorized systems created outside IT governance |

---

### Significance of EUC:

1. **Democratizes technology** — puts computing power in users' hands
2. **Bridges gap** between business needs and IT delivery
3. **Accelerates digital transformation** at grassroots level
4. **Enables business agility** — users respond to changes without IT delays
5. **Empowers knowledge workers** to solve their own problems

---

### Benefits of EUC:

| Benefit | Description |
|---------|-------------|
| **Operational** | Daily tasks done faster and more accurately |
| **Managerial** | Managers get instant custom reports without waiting for IT |
| **Strategic** | Organization becomes more data-driven at all levels |
| **IT Department** | Freed from routine requests to focus on strategic systems |
| **Individual** | Employees feel more empowered and productive |

---

## 📊 MASTER COMPARISON TABLE — ALL IS TYPES

| IS Type | Users | Management Level | Decision Type | Key Feature | Example |
|---------|-------|-----------------|--------------|-------------|---------|
| **OAS** | All staff | All levels | Support/Clerical | Automates office work | MS Office, Email, Zoom |
| **TPS** | Operational staff | Operational | Structured, routine | Fast transaction recording | ATM, POS, UPI payments |
| **MIS** | Middle managers | Tactical | Semi-structured | Periodic summary reports | Weekly sales report |
| **DSS** | Analysts/Managers | Middle/Senior | Semi-structured | "What-if" modeling | Pricing model, loan analysis |
| **GDSS** | Groups/Committees | All senior levels | Semi/Unstructured | Anonymous group voting | Board meeting decision tool |
| **EIS** | Top executives | Strategic | Unstructured | Visual dashboards, drill-down | CEO KPI dashboard |
| **AI/ES** | Domain experts + users | All levels | Structured/Expert | Inference engine, learning | Fraud detection, diagnosis |
| **EUC** | Non-IT end users | All levels | Any | User-built applications | Excel macros, Power BI reports |

---

## 🧠 MASTER MNEMONIC SHEET — LESSON 4

| Topic | Mnemonic | Full Form |
|-------|----------|-----------|
| All IS types | **OTM-DGE-AI** | OAS, TPS, MIS, DSS, GDSS, EIS, AI |
| OAS tools | **DWES-CV** | Document, Workflow, Email, Scheduling, Conferencing, Voice |
| TPS characteristics | **RAPID** | Rapid, Accurate, Pre-defined, Integrity, Dependable |
| MIS report types | **SPIRO** | Scheduled, Periodic, Internal, Routine, Operational |
| DSS features | **FIAMI** | Flexible, Interactive, Analytical, Multiple scenarios, Integrates data |
| GDSS features | **AVCE** | Anonymity, Voting, Collaboration, E-brainstorming |
| EIS features | **DEALS** | Drill-down, Easy interface, Aggregate, Live data, Strategic external |
| Expert System components | **KIRU** | Knowledge base, Inference engine, Rule base, User interface |
| EUC types | **CAPD** | Command, Application dev, Programmer, Data user |
| EUC advantages | **FRISCO** | Faster, Responsive, Independent, Satisfied, Cost, Ownership |
| EUC disadvantages | **SQUAD** | Security, Quality, Uncontrolled, Audit, Duplication |

---

## ⚡ QUICK REVISION FLASHCARDS

**Q: What is OAS? Give 3 examples of OAS tools.**
A: Office Automation System — automates routine office tasks. Examples: MS Word, Email, Zoom.

**Q: What are the two processing modes of TPS?**
A: Batch Processing (periodic, grouped) and Real-Time/OLTP (immediate, one at a time).

**Q: What does ACID stand for in TPS?**
A: Atomicity, Consistency, Isolation, Durability.

**Q: Key difference between MIS and DSS?**
A: MIS gives periodic structured reports (what happened). DSS supports interactive "what-if" analysis (what should I do).

**Q: What is the key feature of GDSS over DSS?**
A: GDSS supports GROUP decision making with anonymity, simultaneous brainstorming, and electronic voting.

**Q: What are the two main components of an Expert System?**
A: Knowledge Base (facts + rules) and Inference Engine (applies rules to reach conclusions).

**Q: What is EUC?**
A: End-User Computing — non-IT professionals directly developing and using their own IS applications.

**Q: What is "Shadow IT"?**
A: Unauthorized systems/apps created by users outside IT department control — a risk of EUC.

**Q: EIS vs MIS — key difference?**
A: EIS is for top executives — strategic, highly summarized, visual dashboards, external data. MIS is for middle managers — periodic tactical reports from internal data.

**Q: What is the "knowledge acquisition problem" in Expert Systems?**
A: The difficulty of extracting and encoding expert knowledge into the system — experts often can't articulate all their knowledge explicitly.

---

## 📌 EXAM PATTERN LIKELY QUESTIONS

| Type | Question |
|------|---------|
| **Long (10 marks)** | Explain the different types of Computer-Based Information Systems with examples |
| **Long (10 marks)** | What is DSS? How does it differ from MIS and EIS? |
| **Short (5 marks)** | What is TPS? What are its characteristics? |
| **Short (5 marks)** | Explain Expert Systems with components and examples |
| **Short (5 marks)** | What is End-User Computing? What are its advantages and disadvantages? |
| **Short (5 marks)** | What is GDSS? How does it differ from DSS? |
| **Short (5 marks)** | What is an EIS? What features make it suitable for executives? |
| **Compare** | Draw a comparison table of OAS, TPS, MIS, DSS, EIS |
| **Definition** | Define: Inference Engine, OLTP, Batch Processing, Shadow IT, Drill-down |
| **Short** | What is the significance of End-User Computing in modern organizations? |

---

> [!NOTE]
> **Lesson 4 ke Top 3 Must-Know:**
> 1. **Master Comparison Table (OAS→EIS)** — 6 IS types ek table mein — ye 10-marker ka perfect answer hai
> 2. **Expert System = Knowledge Base + Inference Engine** — KIRU mnemonic yaad rakh, aur ek example zaroor do
> 3. **EUC — FRISCO advantages aur SQUAD disadvantages** — clean list = easy marks!
>
> **Aage bhej bhai! 🔥💪**
