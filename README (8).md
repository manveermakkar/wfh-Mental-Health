# 🏠 The Work-From-Home Shift: Impact of Remote Work on Mental Health

> **Did Remote Work Change People's Eating, Activity, and Mental Health?**

A quantitative research project submitted for the course **Quantitative Methods for Social Sciences (QMSS)**, Department of HSS.

---

## 👥 Team

| Name | Student ID |
|---|---|
| Manveer Makkar | 2401030128 |
| Prakhar Agnihotri | 2401030129 |
| Rajan Palta | 2401030383 |
| Prajwal Pratap Singh | 2401030371 |
| Ronith Singh | 2401030143 |

**Submitted to:** Dr. Amandeep Kaur  
**Date:** 27 April 2026

---

## 📌 Project Overview

The COVID-19 pandemic triggered one of the most rapid and large-scale transformations in global work culture. Millions of employees transitioned overnight from office environments to remote work. This project quantitatively examines how that shift affected physical activity, stress levels, sleep quality, and work-life balance across remote, hybrid, and onsite workers.

Using a dataset of **5,000 employees** across 7 industries and multiple geographies, we apply Chi-Square tests and One-Way ANOVA to test four core hypotheses about the relationship between work location and health/wellbeing outcomes.

---

## 🔬 Research Questions

1. Is there a significant association between work location and **physical activity frequency**?
2. Does **stress level** differ significantly across remote, hybrid, and onsite workers?
3. Is **sleep quality** significantly associated with the type of work arrangement?
4. Do **work-life balance ratings** differ significantly across work location groups?

---

## 📐 Hypotheses

| Hypothesis | Statement | Statistical Test |
|---|---|---|
| **H1** | Daily physical activity is significantly lower in WFH workers compared to their office-going days | Chi-Square Test |
| **H2** | Home-cooked meal frequency / lifestyle behaviour (proxied by activity) is significantly higher during WFH | Chi-Square Test |
| **H3** | Stress levels are significantly associated with work location type | Chi-Square Test |
| **H4** | Work-life balance scores differ significantly across WFH, Hybrid, and full office arrangements | One-Way ANOVA |

---

## 📂 Repository Structure

```
wfh-mental-health/
│
├── README.md                                          # This file
├── qmssProject_final.ipynb                            # Jupyter Notebook (full analysis)
├── Impact_of_Remote_Work_on_Mental_Health.csv         # Dataset (5,000 records, 20 variables)
├── QMSS_Report_WFH_Mental_Health.docx                 # Full project report (Word)
│
├── figures/                                           # Generated charts (auto-saved by notebook)
│   ├── fig3_1_sample_dist.png
│   ├── fig3_2_activity_bar.png
│   ├── fig3_3_stress_bar.png
│   ├── fig3_4_sleep_bar.png
│   ├── fig3_5_wlb_boxplot.png
│   └── fig3_6_hours_boxplot.png
│
└── requirements.txt                                   # Python dependencies
```

---

## 📊 Dataset

**Source:** [Impact of Remote Work on Mental Health](https://www.kaggle.com/datasets/waqi786/remote-work-and-mental-health) — publicly available secondary survey dataset on Kaggle.

| Parameter | Detail |
|---|---|
| Total Records | 5,000 |
| Records after Cleaning | 3,371 |
| Work Location Groups | Remote (n=1,171) · Hybrid (n=1,113) · Onsite (n=1,087) |
| Industries | Healthcare, IT, Education, Finance, Consulting, Manufacturing, Retail |

### Key Variables

| Variable | Type | Values |
|---|---|---|
| `Work_Location` | Categorical (Nominal) | Remote, Hybrid, Onsite |
| `Physical_Activity` | Categorical (Ordinal) | Daily, Weekly |
| `Stress_Level` | Categorical (Ordinal) | Low, Medium, High |
| `Sleep_Quality` | Categorical (Ordinal) | Good, Average, Poor |
| `Work_Life_Balance_Rating` | Numeric (1–5 scale) | 1 (Low) → 5 (High) |
| `Mental_Health_Condition` | Categorical | Anxiety, Depression, Burnout, None |
| `Hours_Worked_Per_Week` | Continuous | 20–60 hours |
| `Age`, `Gender`, `Job_Role`, `Industry`, `Region` | Demographic | Various |

---

## 🛠️ Methods

All statistical analyses were performed in **Python** inside a Jupyter Notebook, using manually implemented calculations (no black-box wrappers) to demonstrate step-by-step workings.

| Method | Applied To |
|---|---|
| **Chi-Square Test of Independence** (manual) | H1: Physical Activity vs Work Location |
| **Chi-Square Test of Independence** (manual) | H3: Stress Level vs Work Location |
| **Chi-Square Test of Independence** (manual) | Sleep Quality vs Work Location |
| **One-Way ANOVA** (manual) | H4: Work-Life Balance Rating across groups |
| Descriptive statistics & visualisations | All variables |

---

## ⚙️ Setup & Running the Notebook

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/wfh-mental-health.git
cd wfh-mental-health

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook qmssProject_final.ipynb
```

### Run All Cells

Open the notebook and run all cells top-to-bottom (`Kernel → Restart & Run All`). Charts will be saved automatically to the working directory.

---

## 📈 Key Findings (Summary)

- **Physical Activity (H1):** Remote workers showed a significantly different distribution of physical activity frequency compared to onsite workers (χ² test, p < 0.05).
- **Stress Levels (H3):** Stress level distribution was found to be significantly associated with work location type.
- **Sleep Quality:** Sleep quality also showed a statistically significant association with work arrangement type.
- **Work-Life Balance (H4):** One-Way ANOVA revealed no statistically significant difference in mean WLB ratings across the three groups — suggesting WLB is perceived similarly regardless of work location.

> See the full report (`QMSS_Report_WFH_Mental_Health.docx`) or the notebook for step-by-step statistical workings and visualisations.

---

## 📋 References

- Dataset: [Kaggle – Remote Work and Mental Health](https://www.kaggle.com/datasets/waqi786/remote-work-and-mental-health)
- Python libraries: `pandas`, `numpy`, `matplotlib`, `scipy`

---

## 📜 License

This project is submitted as academic coursework and is shared for educational purposes only.  
Dataset is publicly available under its original Kaggle license.
