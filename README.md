# GoogleSheets_Cancer_issue

# 🧬 Cancer Survival Analysis – Google Sheets Case Study

**By:** Patcharin Perngkam  
**Tools:** Google Sheets | Pivot Tables | Charts  
**Dataset:** Fictional cancer patient data (17,686 records)

---

## 📌 Project Overview

This project explores a dataset of cancer patients with the goal of identifying patterns in:

- **Survival time**
- **Cancer recurrence**
- **Demographic trends**

All analysis was done in **Google Sheets**, showcasing what's possible using pivot tables, charts, and formulas for real-world health data.

---

## 🎯 Objectives

1. Understand how survival time varies across treatments, tumor size, and cancer stage.
2. Analyze recurrence patterns across demographics and genetic markers.
3. Visualize distributions and breakdowns using pivot tables and charts.

---

## 🧼 Step 1: Data Cleaning

- Loaded the dataset (`.csv`) into Google Sheets.
- Verified correct formatting for numeric columns like `Age`, `TumorSize`, and `SurvivalMonths`.
- Removed blank or non-numeric cells for accurate charting.
- Renamed columns for clarity.

---

## 📊 Step 2: Demographic Breakdown

### ✅ Cancer Type by Gender

Used a pivot table to count patients per gender by cancer type, then visualized with a horizontal bar chart.

- Pivot table: `CancerType` vs `Gender`

  ![Cancer Type by Gender](/images/Cancer_Gender.png)

- Chart: Bar chart

  ![Cancer Type by Gender](/images/CancerType_by_Gender.png)

  > 🔍 **Insight:** Prostate cancer appeared exclusively in male patients, while breast and skin cancer were more evenly distributed.

---

### ✅ Cancer Type by Region

Visualized the number of patients per cancer type by hospital region.

- Pivot table: `CancerType` vs `hospital region`

  ![Hospital Region Chart](/images/Hospital_Region.png)

- Chart: Column chart

  ![Hospital Region Chart](/images/CancerType%20by%20Hospital%20Region.png)

> 🔍 **Insight:** Skin and lung cancer were among the most common in every region, but slight variations existed regionally.

---

### ✅ Average Age & BMI by Cancer Type

Calculated average age and BMI using pivot tables.

- Pivot table: `CancerType` vs `Age and BMI`

  ![Average Age and BMI](/images/Average_Age_BMI.png)

- Chart: Bar chart

  ![Average Age and BMI](/images/Average%20Age%20or%20BMI%20per%20CancerType.png)

  > 🔍 **Insight:** Patients across all cancer types had a similar average age (around 53–54 years) and BMI (~29).

---

## 📈 Step 3: Survival Analysis

### ✅ Tumor Size vs Survival Time

CreatedHistogram of Survival Time using
`TumorSize` and `SurvivalMonths`.

- Chart: `TumorSize` and `SurvivalMonths`

  ![Tumor Size vs Survival](/images/TumorSize%20vs%20SurvivalMonths.png)

  > 📉 **Result:**  
  > Equation: `y = 0.0261x + 60.2`  
  > R² = 0.0  
  > **Interpretation:** No strong correlation was found between tumor size and survival time.

---

## 🔁 Step 4: Recurrence Patterns

### ✅ Recurrence by Cancer Type

- Pivot table: `Recurrence by Cancer Type`

  ![Recurrence by Cance Type](/images/Recurrence_Type.png)

- Chart: Column chart

  ![Recurrence by Cance Type](/images/Recurrence%20by%20Cancer%20Type.png)

> 🔍 **Insight:** Recurrence was fairly balanced across cancer types.

### ✅ Recurrence by Stage

- Pivot table: `Recurrence by Stage`

  ![Recurrence by Stage](/images/Recurrence_Stage.png)

- Chart: Stacked bar chart

  ![Recurrence by Stage](/images/Recurrence%20by%20Stage.png)

> 🔍 **Insight:** Patients with Stage III or IV cancers had a higher recurrence count — consistent with real-world expectations.

### ✅ Recurrence by Smoking Status

- Pivot table: `Recurrence by Smoking Status`

  ![Recurrence by Smoking Status](/images/Recurrence_Smoking.png)

- Chart: Pie chart

  ![Recurrence by Smoking Status](/images/Recurrence%20by%20Smoking%20Status.png)

  > 🔍 **Insight:** Former smokers had slightly higher recurrence than current or non-smokers, though all groups were close.

### ✅ Recurrence by Genetic Marker

- Pivot table: `Recurrence by Genetic Marker`

  ![Recurrence by Genetic Market](/images/Recurrence_Genetic.png)

- Chart: Bar chart

  ![Recurrence by Genetic Market](/images/Recurrence%20by%20Genetic%20Marker.png)

  > 🔍 **Insight:** The KRAS genetic marker showed the highest number of recurrences, potentially signaling a biological link.

---

## ✅ Final Summary & Key Learnings

- Cancer stage has a clearer link to recurrence and survival than tumor size.
- Demographic insights (age, gender, BMI) helped reveal population patterns.
- Google Sheets can be a surprisingly powerful data tool — pivot tables, scatter plots, histograms, and formulas made it possible to extract real insights without any code.

---

## 📎 Files Included

| File               | Description                      |
| ------------------ | -------------------------------- |
| `cancer issue.csv` | Raw dataset                      |
| `README.md`        | This documentation               |
| `/images`          | Screenshots of charts and tables |

---

> 💡 This was my first data case study using only Google Sheets. I'm proud of how much insight I could extract without writing any code — and I’m excited to build even more!

