# OCD Treatment Analytics for Pharma Product Strategy  
An Excel-based clinical analytics project exploring OCD severity patterns, comorbidities, demographics, and medication class performance to support product & medical strategy decisions.


## 1. Project Overview  
This project demonstrates the core competencies of a Product Analyst or Medical Affairs Analyst by translating complex, real-world style clinical data (N=60) into actionable, evidence-based insights for therapeutic strategy, market segmentation, and clinical decision support within the biopharma industry.The analysis provides critical intelligence necessary for building data-driven business cases, optimizing product roadmaps, and prioritizing Real-World Evidence (RWE) generation across the product lifecycle.

Core Analytical ObjectivesThe analysis utilizes the Yale-Brown Obsessive Compulsive Scale (Y-BOCS) and patient metadata to:

- Segment Severity: Uncover patterns in symptom severity ({Y-BOCS}) across key demographic factors (e.g., Age Group, Sex). 
- Comorbidity Impact: Quantify the influence of co-morbid Depression and Anxiety on overall disease severity and treatment response rates.  
- High-Risk Phenotypes: Identify and prioritize specific Obsession-Compulsion combinations that drive the highest functional impairment.
- TrTreatment Efficacy: Compare mean treatment outcomes across various medication classes, including SSRI Monotherapy vs. Augmentation.  
- Prognostic Factors: Assess the predictive role of Disease Duration (time from symptom onset) on subsequent treatment success and failure.
  
Analysis Tool: Microsoft Excel (PivotTables, Calculated Fields, and Visual Dashboards) — Demonstrating proficiency in rapid data-to-insight generation before scaling to platform/engineering solutions.
---

## 2. Dataset Summary  

**Core Attributes**
Each record includes essential data for clinical modeling:
- Demographics: Age and Gender
- Disease Profile: Symptom Duration
- Obsession/Compulsion Type, and the presence of Depression/Anxiety Comorbidities
- Treatment: Primary Medication Class (SSRI, SNRI, Benzodiazepine, None)
- Severity Metric: Raw {Y-BOCS} Scores (Obsessions & Compulsions)
  
**Derived fields:**  
- **Total OCD Severity** = Average of obsession + compulsion score  
- **Age group** (Under 30, 30–50, Over 50)  
- **Duration band** (0–5 yrs, 5–10 yrs, >10 yrs)

---

## 3. Analytics & Visual Insights  

Each visualization is paired with a clear interpretation written from a pharma-analytics perspective.

---

### 3.1 OCD Severity by Gender  
**Insight:**  
Female patients exhibit a significantly higher overall disease burden, with their average Total OCD Severity ($\mathbf{46.31}$ $\text{Y-BOCS}$) approximately $25\%$ higher than male patients ($\mathbf{36.92}$ $\text{Y-BOCS}$). This difference is primarily driven by Compulsion Severity (Females: $22.28$ vs. Males: $15.96$). This justifies segmenting patient support programs and educational outreach to specifically target and measure compulsion reduction in the female patient population.

**Visualization:**  
![](dataset/gender_severity.png)

---

### 3.2 OCD Severity by Age Group  
**Insight:**  
Patients under 30 demonstrate the highest average severity.  
This indicates earlier-stage, more disruptive illness, representing a key segment for early-intervention therapies and long-term treatment planning.

**Visualization:**  
![](dataset/agegroup_severity.png)

---

### 3.3 OCD Severity by Depression Comorbidity  
**Insight:**  
Patients without depression show *higher* OCD scores.  
This suggests their OCD symptoms may be more primary rather than secondary to mood disorders — potentially affecting how treatment is prioritized.

**Visualization:**  
![](dataset/depression_severity.png)

---

### 3.4 OCD Severity by Anxiety Comorbidity  
**Insight:**  
Anxiety comorbidity correlates with significantly higher compulsion severity.  
This implies anxiety may intensify compulsive behaviors — a valuable insight for combination-therapy research or clinical messaging.

**Visualization:**  
![](dataset/anxiety_severity.png)

---

### 3.5 Obsession–Compulsion Severity Heatmap  
**Insight:**  
This heatmap identifies high-severity pairings such as:  
- **Religious + Praying**  
- **Harm-related + Checking**  
- **Symmetry + Checking**  

These clusters highlight the most clinically burdensome behavior patterns and help identify patients needing intensified therapy.

**Visualization:**  
![](dataset/obsession_compulsion_heatmap.png)

---

### 3.6 Medication Class × Anxiety Status  
**Insight:**  
Among medication classes, patients on **“None”** showed the highest severity — indicating unmet treatment needs.  
For medicated patients, benzodiazepine users showed relatively high severity, suggesting partial response or inappropriate monotherapy.

**Visualization:**  
![](dataset/meds_anxiety.png)

---

### 3.7 Medication Class × Disease Duration  
**Insight:**  
Severity tends to increase with longer disease duration for all medication classes.  
SSRI users show the most stable pattern across duration groups, supporting SSRIs as the most consistent long-term therapy.

**Visualization:**  
![](dataset/meds_duration.png)

---

## 4. Strategic Insights for Biopharma Product & Medical Teams

The analysis of the N=60 patient cohort provides actionable, evidence-based direction for product strategy, market segmentation, and clinical communication.

### 1. Clear Unmet-Need Segments
* **High-Acuity/Untreated:** Focus on patients with high baseline severity (e.g., Obsession Y-BOCS up to 31.2) who are currently on **No Medication** but possess **Anxiety Comorbidity**. This defines an immediate, high-value segment for **treatment initiation campaigns**.
* **Long-Duration & Refractory:** Patients with **Disease Duration >10 years** often show partial response. This segment requires **therapeutic augmentation** or switching strategies to overcome chronic symptom plateaus.
* **Early, Severe Onset:** The **Under 30 age group** shows peak **Obsession Severity** (24.81), necessitating **early, aggressive intervention** programs focused on disrupting acute obsessional thought patterns.

### 2. Medication Class Performance & Clinical Guidance
* **SSRI Stability:** SSRIs demonstrate the most **consistent long-term symptom control** in chronic users, confirming their role as the gold-standard baseline therapy.
* **SNRI Heterogeneity:** Performance varies significantly by comorbidity profile, signaling a need for **targeted RWE** to define its optimal placement in the treatment algorithm.
* **Benzodiazepine Correlation:** Use correlates with **higher overall severity**, flagging a potential **treatment-resistant subgroup** or the need for **clinician education** on its appropriate adjunctive vs. monotherapy use.

### 3. Behavioral Phenotype Clusters
* **Precision Targeting:** The Obsession–Compulsion Heatmap identifies maximum-severity clusters (e.g., Religious Obsession + Checking, Obsession Y-BOCS = 32.5). These severe phenotypes are ideal for **Precision Medicine Segmentation** and **advanced therapy trials** to prove efficacy in the most burdensome patient subsets.

### 4. Opportunities for Targeted Interventions
* **Digital/Behavioral Therapy:** Target solutions toward patient segments with high **Compulsion severity** (e.g., 30–50 age group) to manage entrenched, high-impact rituals.
* **Clinical Messaging:** Focus on the impact of **Comorbidity-Linked Severity** (Anxiety/Depression) to encourage clinicians toward comprehensive, multi-modal treatment planning.
* **Early Intervention:** Implement programs targeting young adults to reduce the long-term functional impairment caused by severe symptom onset.

---

## 5. Repository Files

This project utilizes the following data files:

* `ocd_analytics.xlsx - Sheet1.csv`: **Primary Patient Data.** Contains raw demographics, clinical variables, and Y-BOCS scores.
* `ocd_analytics.xlsx - Sheet3.csv`: **PivotTable Source Data.** Contains aggregated summary tables used for all statistical insights and visualizations.
