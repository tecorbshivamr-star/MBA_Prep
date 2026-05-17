# 📗 MR CHAPTER 6: Sample Size & Data Preparation
### Subject: Marketing Research | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

In Chapter 5, we learned *how* to pick people. 
Now, we must ask: ***How many* people do we need to pick?** (Sample Size).
- Do we need to survey 100 people? 1,000 people? 100,000 people? 
- If you survey too few, your data is mathematically useless. If you survey too many, you waste millions of rupees. There is an exact mathematical formula to find the perfect number (usually around 384 people for a national survey!).

Once you get those 384 surveys back, they are messy. People skipped questions, people checked the wrong boxes, people drew smiley faces on the paper. 
**Data Preparation** is the tedious process of cleaning this messy paper data and converting it into neat numbers on an Excel spreadsheet so a computer can analyze it.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. Sampling Error vs Non-Sampling Error
- **Sampling Error:** The natural mathematical error that happens because you only tested a *drop* of blood, not the whole body. *How to fix it?* Increase the sample size.
- **Non-Sampling Error:** Human stupidity. The interviewer lied and filled out the forms himself. The data-entry guy typed "100" instead of "10". The survey question was confusing. *How to fix it?* Better training. (Note: Increasing sample size does NOT fix this; it just makes it worse!).

### 2. Determining Sample Size (n)
You need three things to use the statistical formula:
1. **Confidence Level (Z):** How certain do you want to be? Usually 95% (which gives a Z-score of 1.96).
2. **Acceptable Error (E):** Are you okay with being ±5% wrong?
3. **Variance/Standard Deviation (σ):** How diverse is the population? (If everyone is identical, you only need to survey 1 person!).

### 3. Data Preparation Steps
1. **Editing:** Throwing out incomplete or obviously fake surveys.
2. **Coding:** Turning words into numbers. (Male = 1, Female = 2).
3. **Data Entry:** Typing it into SPSS or Excel.
4. **Data Cleaning:** Running a computer check to find impossible answers (e.g., someone entered their age as 350 years old).

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. What is the difference between Sampling Error and Non-Sampling Error? Briefly describe the steps involved in the Data Preparation process before statistical analysis can begin. (15 Marks)

**1. Sampling Error vs. Non-Sampling Error:**

| Feature | Sampling Error | Non-Sampling Error |
| :--- | :--- | :--- |
| **Definition** | The error that occurs because the specific sample selected is an imperfect representation of the target population. | All other errors that occur during the research process (design, collection, entry, analysis). |
| **Cause** | Natural statistical variation (chance). | Human error, bias, poor questionnaire design, non-response, data entry mistakes. |
| **Effect of Sample Size** | **Decreases** mathematically as sample size increases. | Tends to **Increase** as sample size increases (because managing a massive survey team leads to more human mistakes). |
| **Controllability** | Can be precisely calculated and quantified using statistics (e.g., ±3% margin of error). | Extremely difficult to quantify; can ruin the entire study without the researcher realizing it. |

**2. The Data Preparation Process:**
Raw data collected from the field cannot be immediately analyzed. It must pass through a rigorous, sequential data preparation process to ensure integrity.

*   **Step 1: Questionnaire Checking / Validation:**
    Upon return from the field, researchers check if the questionnaires are complete and legible. If a field worker's batch shows identical patterns (indicating fraud/cheating), the entire batch is discarded.
*   **Step 2: Editing:**
    A thorough review of the responses to identify and correct illogical, inconsistent, or incomplete answers. 
    *   *Example:* If a respondent claims their age is 15 but lists their occupation as 'Surgeon', the editor must decide whether to discard the questionnaire or treat the response as 'Missing Data'.
*   **Step 3: Coding:**
    Assigning numerical values to responses so they can be read by statistical software (like SPSS).
    *   *Closed-ended questions:* Simple mapping (e.g., Yes = 1, No = 2).
    *   *Open-ended questions:* Highly complex. The researcher must read hundreds of text answers, group them into common themes, and assign a code to each theme.
*   **Step 4: Transcription / Data Entry:**
    The physical act of transferring the coded data from paper questionnaires into a computer database (Excel/SPSS). (Less relevant today with online surveys like Qualtrics, which automate this step).
*   **Step 5: Data Cleaning & Missing Value Treatment:**
    Running preliminary descriptive statistics (like frequency distributions) to find "outliers" or impossible codes (e.g., a '7' in a column that should only contain 1s and 2s). 
    *   *Missing Data:* The researcher must decide how to handle blanks (e.g., Casewise deletion, replacing with the mean, or using statistical imputation).

**Conclusion:**
In marketing research, the axiom "Garbage In, Garbage Out" applies perfectly. Sophisticated statistical analysis cannot salvage poorly prepared, error-ridden data. Rigorous data preparation is the bedrock of valid research findings.
