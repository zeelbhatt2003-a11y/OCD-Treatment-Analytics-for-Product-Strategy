![OCD Analytics Banner](dataset/ocd_banner.png)

# OCD Treatment Analytics for Pharma Product Strategy  
An Excel-based clinical analytics project exploring OCD severity patterns, comorbidities, demographics, and medication class performance to support product & medical strategy decisions.


## Table of Contents  
1. [Project Overview](#1-project-overview)  
2. [Dataset Summary](#2-dataset-summary)  
3. [Key Insights](#3-analytics--visual-insights)  
4. [Visualizations](#3-analytics--visual-insights)  
5. [Strategic Recommendations](#4-strategic-insights-for-biopharma-product--medical-teams)  
6. [Limitations & Next Steps](#limitations--next-steps)  
7. [Repository Files](#5-repository-files)  


## 1. Project Overview  
This project demonstrates the capabilities of a **Health Data Analyst/Product Analyst** by translating real-world style clinical data (N = 60) into high-impact insights supporting:

- Therapeutic strategy  
- Market segmentation  
- Evidence generation  
- Clinical communication  
- Treatment optimization  

The analysis uses **Excel (PivotTables, calculated fields, dashboards)** to model:

### Core Analytical Objectives  
- **Severity Segmentation:** Identify patterns in Y-BOCS severity across demographics  
- **Comorbidity Impact:** Understand how Depression/Anxiety influence symptom burden  
- **High-Risk Phenotypes:** Detect severe Obsession–Compulsion clusters  
- **Treatment Performance:** Compare symptom severity across medication classes  
- **Prognostic Factors:** Analyze disease duration and long-term severity trends  

This reflects real analytical workflows used in Pharma, Medical Affairs, RWE, and Product Strategy.


## 2. Dataset Summary  

### **Core Attributes Collected**
- **Demographics:** Age, Gender  
- **Disease Profile:** Symptom duration  
- **Comorbidities:** Depression, Anxiety  
- **Clinical Variables:** Obsession type, Compulsion type  
- **Treatment:** Primary medication class  
- **Severity Metrics:** Y-BOCS Obsessions & Compulsions  

### **Derived Fields**
- **Total OCD Severity** = Mean of Obsession + Compulsion score  
- **Age Groups:** Under 30 · 30–50 · Over 50  
- **Duration Bands:** 0–5 yrs · 5–10 yrs · >10 yrs  


# 3. Analytics & Visual Insights  

Each visualization includes both an **observation** and a **strategic interpretation**.


## 3.1 OCD Severity by Gender  
**Insight:**  
Female patients show slightly higher severity levels.

**Interpretation:**  
May reflect stronger emotional, ruminative symptom profiles — helpful for tailoring patient support programs.

**Visualization:**  
![](dataset/gender_severity.png)


## 3.2 OCD Severity by Age Group  
**Insight:**  
Patients **under 30** show the **highest severity**.

**Interpretation:**  
Indicates early-onset, high-burden illness → key target group for **early intervention therapies**.

**Visualization:**  
![](dataset/agegroup_severity.png)


## 3.3 Severity by Depression Comorbidity  
**Insight:**  
Surprisingly, patients **without depression** show slightly higher OCD severity.

**Interpretation:**  
OCD may be more primary and independent of mood symptoms — affects clinical prioritization.

**Visualization:**  
![](dataset/depression_severity.png)


## 3.4 Severity by Anxiety Comorbidity  
**Insight:**  
Anxiety comorbidity significantly increases **compulsion severity**.

**Interpretation:**  
Anxiety may intensify compulsive behavior → supports combination therapy messaging.

**Visualization:**  
![](dataset/anxiety_severity.png)


## 3.5 Obsession–Compulsion Severity Heatmap  
**High-Severity Clusters Identified:**
- Religious → Praying  
- Harm-Related → Checking  
- Symmetry → Checking  

**Interpretation:**  
These define **high-burden phenotypes** — ideal for precision medicine, clinical trial enrichment, and targeted CBT programs.

**Visualization:**  
![](dataset/obsession_compulsion_heatmap.png)


## 3.6 Medication Class × Anxiety Status  
**Insight:**  
Patients receiving **no medication** show the **highest severity**.

**Interpretation:**  
Indicates major unmet need and treatment gaps.

**Visualization:**  
![](dataset/meds_anxiety.png)


## 3.7 Medication Class × Disease Duration  
**Insight:**  
Severity increases with disease duration across all medication classes.

**Interpretation:**  
Supports long-term disease progression modeling; SSRIs show most stable long-term patterns.

**Visualization:**  
![](dataset/meds_duration.png)


# 4. Strategic Insights for Biopharma Product & Medical Teams  


## 4.1 High-Value Unmet-Need Segments  
- **Untreated, high-severity patients**  
- **Long-duration, partial-response patients**  
- **Early severe onset (<30 yrs)** — ideal for early-intervention campaigns  


## 4.2 Medication Class Performance  
- **SSRIs:** Most stable long-term control  
- **SNRIs:** Highly variable → requires targeted RWE  
- **Benzodiazepines:** Associated with high severity → treatment-resistant signal  


## 4.3 Behavioral Phenotype Clusters  
Heatmap-driven phenotypes support:
- Precision segmentation  
- RWE prioritization  
- Advanced therapy messaging  


## 4.4 Opportunities for Intervention  
- Digital therapeutics for high compulsion severity  
- Combined therapy strategies for comorbidity-linked severity  
- Early intervention for high-burden young adults  


# Limitations & Next Steps  

### Limitations  
- Sample size = 60  
- Medication adherence not measured  
- Limited comorbidity categories  

### Next Steps  
- Build regression models to predict severity  
- Expand dataset to 500+ patients  
- Develop automated Excel dashboards  


# 5. Repository Files  

| File | Description |
|------|-------------|
| `ocd_analytics.xlsx` | Primary patient dataset |
| `dataset/*.png` | Visualizations exported from Excel |
| `README.md` | Full project report |


**Project by Zeel Bhatt**  
**zeelbhatt2003@gmail.com**

