# 📐 LESSON 6: SAMPLE SIZE DETERMINATION & DATA PREPARATION
### MBA Marketing Research | Exam Revision Notes

---

> [!IMPORTANT]
> **Top Exam Topics:** Sample Size formula (know it!), Steps in Data Preparation, Types of Sampling Errors vs Non-Sampling Errors. Mix of numerical + theory — be ready for both!

---

## 🎯 LEARNING OBJECTIVES

After this chapter, you should be able to:
- Determine the appropriate **sample size** using formulas and rules
- Understand **data coding** and how raw responses become usable data
- Explain the **data preparation process** step by step
- Describe **tabulation and graphical analysis** methods
- Distinguish between **Sampling Errors and Non-Sampling Errors**

---

## 1. 📖 INTRODUCTION

### The Data Journey:
```
Research Problem
      ↓
Design Questionnaire → Determine Sample Size
      ↓
Field Data Collection
      ↓
DATA PREPARATION (This Chapter!)
      ↓
Analysis & Interpretation
      ↓
Report & Recommendations
```

> This chapter bridges **collection and analysis** — raw data from 500 questionnaires is useless unless it's properly prepared, coded, and organized.

---

## 2. 📏 SAMPLE SIZE DETERMINATION

### The Core Question: **"How many respondents do I need?"**

Sample size depends on:

> **Mnemonic: "PPVC-AB"**
> - **P**recision required (margin of error — e)
> - **P**opulation size (N) — matters less than you think!
> - **V**ariability (standard deviation — σ or p)
> - **C**onfidence level (z-score)
> - **A**vailable budget
> - **B**ig or small population (finite correction)

---

### 📊 METHODS OF DETERMINING SAMPLE SIZE

#### Method 1: 📐 Statistical / Formula-Based Approach

**For Estimating a PROPORTION (Categorical Data — Yes/No responses):**

> **Formula:**
> ```
> n = (z² × p × q) / e²
> ```
> Where:
> - **n** = required sample size
> - **z** = z-value for desired confidence level
> - **p** = estimated proportion of attribute in population
> - **q** = 1 – p
> - **e** = acceptable margin of error (precision)

**Z-values to memorize:**
| Confidence Level | Z-value |
|-----------------|---------|
| 90% | 1.645 |
| **95%** | **1.96** ← Most used! |
| 99% | 2.576 |

**Worked Example:**
> A researcher wants to estimate the proportion of consumers who prefer Brand A.
> - Confidence Level = 95% → z = 1.96
> - Expected proportion p = 0.5 (maximum variability, conservative estimate)
> - Margin of error e = 5% = 0.05
>
> **n = (1.96² × 0.5 × 0.5) / (0.05²)**
> n = (3.8416 × 0.25) / 0.0025
> n = 0.9604 / 0.0025
> **n = 384.16 ≈ 385 respondents**

> [!TIP]
> **Golden Rule:** When p is unknown, always use **p = 0.5** (gives maximum/most conservative sample size)
> **n = 384 is the magic number for 95% confidence, 5% error, p=0.5**

---

**For Estimating a MEAN (Continuous Data):**

> **Formula:**
> ```
> n = (z × σ / e)²
> ```
> Where:
> - **σ** = population standard deviation
> - **e** = acceptable error in units
> - **z** = z-value for confidence level

**Example:**
> Researcher wants to estimate average monthly spending on food.
> - σ = ₹500 (from pilot study)
> - e = ₹50 (acceptable error)
> - 95% confidence → z = 1.96
>
> n = (1.96 × 500 / 50)²
> n = (19.6)²
> **n = 384.16 ≈ 385**

---

**Finite Population Correction (FPC):**
> When population is **small and known**, apply correction:
> ```
> n' = n × N / (n + N - 1)
> ```
> - n' = adjusted (smaller) sample size
> - N = population size
> - n = originally calculated sample size

**When to apply FPC:** When n > 5% of N (sample is more than 5% of population)

---

#### Method 2: 💰 Budgetary / Cost-Based Approach

> Sample size = **Total available budget / Cost per respondent**

**Example:**
> Total budget = ₹1,00,000; Cost per interview = ₹500
> Sample size = 1,00,000 / 500 = **200 respondents**

- Simple but may give scientifically inadequate sample
- Used when budget is the binding constraint

---

#### Method 3: 📏 Rules of Thumb / Conventional Standards

Common industry standards:

| Study Type | Recommended Sample Size |
|-----------|------------------------|
| Exploratory Research | 15 – 30 |
| Focus Group (per group) | 6 – 12 |
| Test Markets | 200+ per market |
| National Consumer Survey | 1,000 – 2,000 |
| Advertising Pre-test | 150 – 300 per ad |
| Product Concept Test | 200 – 300 |
| Pricing Research | 300 – 500 |

---

#### Method 4: 📊 Based on Number of Sub-groups

> **Rule:** n ≥ **100 per major sub-group** (gender, region, age bracket)

**Example:**
> Survey of 4 regions × 2 genders = 8 sub-groups
> Minimum sample = 8 × 100 = **800 respondents**

---

### ⚖️ Effect of Sample Size on Precision

```
Larger Sample → Lower Sampling Error → Higher Precision
BUT:
Beyond ~1,500, gains become marginal (law of diminishing returns)
```

| Sample Size | Approx. Margin of Error (at 95% confidence) |
|------------|---------------------------------------------|
| 100 | ±10% |
| 200 | ±7% |
| 400 | ±5% |
| 600 | ±4% |
| 1,000 | ±3% |
| 2,500 | ±2% |

---

## 3. 💻 DATA CODING

> **Definition:** Data Coding is the process of **assigning numerical codes or symbols** to each response category so that data can be entered into a computer for analysis.

### Why Code?
- Computers process **numbers**, not words
- Converts "Yes/No/Maybe" → 1/2/3
- Enables statistical analysis in SPSS, Excel, SAS

---

### Types of Coding:

#### A. Pre-Coding (Before Data Collection)
- Codes are assigned **during questionnaire design**
- Closed-ended questions are pre-coded
- **Example:** Already printed on questionnaire:
  ```
  Gender:  Male [1]  Female [2]  Other [3]
  ```

#### B. Post-Coding (After Data Collection)
- For **open-ended questions** where responses weren't pre-specified
- Researcher reads all responses → **creates categories** → assigns codes
- Example:
  ```
  Q: "Why do you prefer Zomato?" (open-ended)
  After collection, responses coded as:
  1 = Speed/Delivery time
  2 = Price/Offers/Discounts
  3 = App interface/Ease of use
  4 = Restaurant variety
  5 = Other
  ```

### Coding Book / Codebook:
> A **document that lists all variables, their codes, and what each code means**

| Variable | Question | Code | Meaning |
|----------|---------|------|---------|
| Q1 | Gender | 1 | Male |
| Q1 | Gender | 2 | Female |
| Q2 | Age | 1 | Below 25 |
| Q2 | Age | 2 | 25–35 |
| Q5 | Satisfaction | 1–5 | 1=Very Dissatisfied, 5=Very Satisfied |

### Coding Rules:
1. Codes must be **mutually exclusive** (one response = one code)
2. Codes must be **exhaustive** (every possible answer has a code)
3. Use **numeric codes** whenever possible
4. Have an **"Other" or "Not Applicable"** category
5. Missing values should be coded distinctly (e.g., 99 = No response)

---

## 4. 🛠️ DATA PREPARATION

> **Definition:** Data Preparation is the process of **converting raw collected data into a clean, organized, analysis-ready dataset**.

### Steps in Data Preparation:

> **Mnemonic: "ECTCA"** — *"Each Chapter Takes Careful Attention"*
> - **E**diting
> - **C**oding
> - **T**ranscription / Data Entry
> - **C**leaning
> - **A**nalysis-ready file creation

---

### Step 1: 🔵 EDITING

> Checking all questionnaires/responses for **completeness, consistency, and legibility** before coding.

**Two types of editing:**

#### Field Editing (Done by Field Supervisor immediately after collection):
- Check for **legibility** — can responses be read?
- Check for **completeness** — all questions answered?
- Check for **consistency** — do answers logically match?
- Return to respondent if needed (while memory is fresh)

#### Office Editing (Done at central office):
- More thorough review of all questionnaires
- Decide what to do with **problematic questionnaires**

**Decisions during editing:**

| Problem | Action |
|---------|--------|
| **Incomplete questionnaire** | Return to field if possible; else partial use |
| **Inconsistent answers** | Mark as invalid; don't use those responses |
| **Illegible responses** | Assign a missing value code |
| **All same answers (straight lining)** | Suspect respondent — discard questionnaire |
| **Logic errors** (e.g., age=15, married=yes with 3 kids) | Flag as suspect |

---

### Step 2: 🔵 CODING

*(Already covered in detail in Section 3)*

- Assign numeric codes to all responses
- Create Codebook
- Handle missing values systematically

---

### Step 3: 🔵 TRANSCRIPTION / DATA ENTRY

> Entering the coded data into the **computer** (SPSS, Excel, SAS dataset)

**Methods:**
- **Manual data entry** — Operator types codes into spreadsheet
- **Optical Mark Reader (OMR)** — Machine reads marked bubbles (like exams!)
- **CAPI/CATI** — Computer-assisted interviewing enters data automatically
- **Online surveys** — Data auto-captured in real-time (Google Forms → Sheets)

**Double Entry Verification:**
> Same data entered **twice** by two different operators → compare → find discrepancies → correct
> Used for high-stakes research to minimize entry errors

---

### Step 4: 🔵 DATA CLEANING

> The process of **detecting and correcting errors and inconsistencies** in the dataset.

**Types of errors caught during cleaning:**

| Error Type | Example | Solution |
|-----------|---------|---------|
| **Out-of-range values** | Age = 200, Rating = 8 (on 1-5 scale) | Flag and correct |
| **Impossible combinations** | Male + Pregnant = Yes | Flag as error |
| **Missing values** | Blank cells | Code as missing (e.g., 99) or impute |
| **Duplicate entries** | Same respondent entered twice | Remove duplicate |
| **Logical inconsistencies** | Non-user rating product | Investigate |

**Methods of handling missing data:**
1. **Listwise deletion** — Remove entire row with any missing value
2. **Pairwise deletion** — Use available data for each analysis
3. **Mean substitution** — Replace missing with variable mean
4. **Multiple Imputation** — Advanced statistical method to estimate missing values

---

### Step 5: 🔵 ANALYSIS-READY FILE

- All variables properly labelled
- Codebook finalized
- Missing values documented
- Dataset saved in appropriate format (SPSS .sav, Excel .xlsx, CSV)
- Ready for statistical analysis!

---

## 5. 📊 TABULATION AND GRAPHICAL ANALYSIS

### TABULATION

> **Definition:** Tabulation is the **orderly arrangement of data in rows and columns (tables)** to summarize and organize findings.

**Types of Tabulation:**

#### 1. Simple / One-Way Tabulation (Frequency Distribution)
- Shows **distribution of ONE variable** at a time
- Most basic form of data summary

**Example:**
| Gender | Frequency | Percentage |
|--------|-----------|------------|
| Male | 220 | 44% |
| Female | 280 | 56% |
| **Total** | **500** | **100%** |

#### 2. Cross Tabulation (Contingency Table / Two-Way Table)
- Shows relationship between **TWO or more variables simultaneously**
- Most widely used analytical tool in MR!
- Basis for **Chi-Square test** of association

**Example:**
| | Prefers Pepsi | Prefers Coke | Total |
|-|--------------|--------------|-------|
| **Male** | 140 | 80 | 220 |
| **Female** | 100 | 180 | 280 |
| **Total** | 240 | 260 | 500 |

> This tells us: Males prefer Pepsi (64%), Females prefer Coke (64%) — a clear gender difference!

**Key Concepts in Cross-Tabulation:**
- **Row Variable** — Variable listed in rows
- **Column Variable** — Variable listed in columns
- **Cell** — Intersection of row and column
- **Marginal Totals** — Row totals, column totals
- **Cell Percentages** — Row %, Column %, Total %

---

### GRAPHICAL ANALYSIS

> **Definition:** Visual representation of data using charts and diagrams to make patterns and trends immediately visible.

**Types of Graphs and When to Use:**

> **Mnemonic: "BLOPS-PH"**
> - **B**ar Chart
> - **L**ine Chart
> - **O**give (Cumulative Frequency)
> - **P**ie Chart
> - **S**catter Plot
> - **P**ictogram
> - **H**istogram

| Graph Type | Best For | Data Type | Example |
|-----------|---------|-----------|---------|
| **Bar Chart** | Comparing categories | Nominal, Ordinal | Brand preference by region |
| **Pie Chart** | Showing parts of a whole (%) | Nominal | Market share breakdown |
| **Line Chart** | Showing trends over time | Interval, Ratio | Sales trend 2019–2024 |
| **Histogram** | Distribution of continuous data | Interval, Ratio | Age distribution of customers |
| **Scatter Plot** | Relationship between two variables | Interval, Ratio | Price vs Sales volume |
| **Ogive** | Cumulative frequency distribution | Interval, Ratio | "Less than" / "More than" curves |
| **Pictogram** | Simple visual display | Nominal | Icons representing product quantities |

**Rules for Good Graphical Display:**
1. **Title** — Clear, descriptive title
2. **Labels** — All axes labelled with units
3. **Scale** — Consistent, appropriate scale (don't truncate to mislead!)
4. **Legend** — Explain all symbols/colours
5. **Source** — Cite data source
6. **Simplicity** — One key message per chart

---

## 6. ⚠️ SAMPLING ERRORS

### What is Sampling Error?

> **Sampling Error** = The difference between the **sample statistic** and the true **population parameter** — arising purely because we studied a sample instead of the entire population.

```
Sampling Error = Sample Statistic − True Population Parameter
```

**Even a perfectly designed study will have SOME sampling error** — it's inevitable when using a sample.

---

### TWO MAJOR TYPES OF ERRORS:

```
Total Research Error
├── A. SAMPLING ERRORS (Random Error)
│   ├── Random Sampling Error
│   └── Systematic Sampling Error (Bias)
└── B. NON-SAMPLING ERRORS (Non-Random Error)
    ├── Researcher/Administration Errors
    ├── Respondent Errors
    └── Data Processing Errors
```

---

### A. SAMPLING ERRORS

#### 1. Random Sampling Error
- Occurs due to **chance** in the selection process
- **Cannot be eliminated** but can be **reduced** by increasing sample size
- Affects **precision** — how close estimate is to true value
- **Sampling Distribution** and **Standard Error** quantify this

#### 2. Systematic Sampling Error (Sampling Bias)
- Consistent, **directional error** from flawed sampling design
- NOT reduced by increasing sample size
- **Can be eliminated** by fixing the design

**Sources of Systematic Bias:**
- **Frame bias** — sampling frame doesn't match population
- **Selection bias** — non-random selection of units
- **Non-response bias** — non-respondents differ from respondents

---

### B. NON-SAMPLING ERRORS

> **Definition:** Errors that arise from **sources other than the sampling process** — in questionnaire design, field execution, data entry, or respondent behaviour.

> [!IMPORTANT]
> Non-sampling errors can occur in a CENSUS too! They're NOT eliminated by studying everyone.

**Three Sub-Categories:**

#### 1. 👨‍💼 Researcher / Administrative Errors

> **Mnemonic: "FIQPS"**
> - **F**rame error — wrong sampling frame used
> - **I**nterviewer error — leading questions, wrong recording
> - **Q**uestionnaire error — poor wording, ambiguous questions, leading questions
> - **P**rocessing error — data entry mistakes, coding errors
> - **S**election error — interviewers choosing easy respondents (not random)

| Error | Description | Example |
|-------|------------|---------|
| **Surrogate Information Error** | Wrong information measured | Asking purchase intention instead of actual purchase |
| **Measurement Error** | Scale doesn't measure what intended | Using a happiness scale for brand loyalty |
| **Interviewer Error** | Interviewer influences responses | Nodding when respondent says "yes" |
| **Recording Error** | Wrong option marked | Respondent says "Agree" but "Strongly Agree" is checked |
| **Questionnaire Error** | Ambiguous/leading questions | "Don't you agree Maggi is the best noodle brand?" |

#### 2. 🧑 Respondent Errors

| Error | Description | Example |
|-------|------------|---------|
| **Inability Error** | Respondent genuinely doesn't know | "How often did you shop in 2019?" |
| **Unwillingness Error** | Respondent refuses to answer honestly | Income questions, embarrassing habits |
| **Social Desirability Bias** | Answer to look good/acceptable | Overstating income, charity donations |
| **Acquiescence Bias** | Tendency to always agree | Saying "Yes" to every statement |
| **Prestige Bias** | Exaggerating status | "Yes, I drink imported wine" (rarely) |

#### 3. 🖥️ Data Processing Errors

| Error | Description |
|-------|------------|
| **Transcription Error** | Wrong code entered (4 instead of 3) |
| **Editing Error** | Wrong judgment during editing |
| **Coding Error** | Response wrongly categorized |
| **Analysis Error** | Wrong statistical test applied |

---

### SAMPLING vs NON-SAMPLING ERRORS — MASTER COMPARISON

| Feature | Sampling Error | Non-Sampling Error |
|---------|---------------|-------------------|
| **Source** | Sample vs population gap | Design, execution, processing |
| **Occurs in Census?** | No (no sampling done) | YES — census also has this |
| **Direction** | Random (varies) | Can be systematic |
| **Reduced by?** | Increasing sample size | Better design, training, process |
| **Can be calculated?** | Yes (statistical formula) | Difficult to quantify |
| **Types** | Random, Systematic bias | Researcher, Respondent, Processing |

---

## 🧠 MASTER MNEMONIC SHEET — LESSON 6

| Topic | Mnemonic | Full Form |
|-------|----------|-----------|
| Sample Size Factors | **PPVC-AB** | Precision, Population, Variability, Confidence, Available budget, Big/small pop |
| Data Preparation Steps | **ECTCA** | Editing, Coding, Transcription, Cleaning, Analysis-ready |
| Graph Types | **BLOPS-PH** | Bar, Line, Ogive, Pie, Scatter, Pictogram, Histogram |
| Researcher Errors | **FIQPS** | Frame, Interviewer, Questionnaire, Processing, Selection |
| Key z-values | **1.645 / 1.96 / 2.576** | 90% / 95% / 99% confidence |
| Magic sample number | **384 / 385** | n for 95% confidence, 5% error, p=0.5 |

---

## ⚡ QUICK REVISION FLASHCARDS

**Q: Formula for sample size (proportion)?**
A: n = (z² × p × q) / e²

**Q: What sample size gives 95% confidence, 5% error with p=0.5?**
A: **n = 385** (the magic number in MR!)

**Q: What z-value corresponds to 95% confidence?**
A: **z = 1.96**

**Q: What is Finite Population Correction?**
A: n' = nN/(n+N-1); used when sample is >5% of population to reduce sample size needed

**Q: What is the difference between editing and cleaning?**
A: Editing = checking questionnaires for completeness/consistency BEFORE coding; Cleaning = detecting/correcting errors in the dataset AFTER data entry

**Q: What is a Cross Tabulation?**
A: A table showing simultaneous distribution of two or more variables; basis for Chi-Square test

**Q: Can Non-Sampling errors occur in a census?**
A: YES! Non-sampling errors (interviewer bias, respondent bias, data entry errors) occur even when studying the entire population

**Q: What is Acquiescence Bias?**
A: Respondent's tendency to agree with statements regardless of content ("yes bias")

**Q: What is Double Data Entry?**
A: Entering same data twice by two operators, then comparing to catch transcription errors

**Q: What is Social Desirability Bias?**
A: Respondents answer in socially acceptable/impressive way rather than truthfully

---

## 📌 EXAM PATTERN LIKELY QUESTIONS

| Type | Question |
|------|---------|
| Numerical | A researcher wants 95% confidence with 5% error. If p=0.5, what is the sample size? |
| Long | Explain the steps in Data Preparation for Marketing Research |
| Short | What is Data Coding? Explain pre-coding and post-coding with examples |
| Short | Distinguish between Sampling Errors and Non-Sampling Errors |
| Short | What is Cross Tabulation? Why is it important in MR? |
| Short | What are Respondent Errors? Explain with examples |
| Short | What are the different types of graphs used in Marketing Research? |
| Long | What factors influence the determination of sample size? |
| Short | What is Finite Population Correction? When is it applied? |
| Definition | Define: Codebook, Field Editing, Social Desirability Bias, Acquiescence Bias |

---

> [!NOTE]
> **Bhai, Lesson 6 ke Top 3 Must-Know:**
> 1. **Sample size formula** — n = z²pq/e² — ek numerical zaroor aayega! z=1.96 aur p=0.5 yaad rakh → answer = 384/385
> 2. **ECTCA** — Data preparation ke 5 steps — editing, coding, transcription, cleaning, analysis file
> 3. **Sampling vs Non-Sampling Error** — ye wala distinction examiners ka favourite hai — Census mein bhi non-sampling error hota hai!
>
> **6 chapters done! Teri preparation solid ja rahi hai bhai! 🔥💪 Aur chapters bhej!**
