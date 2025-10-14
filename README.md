# 🧪 A/B Test in Food Products

This project analyzes user behavior data from a **food delivery company** to evaluate the impact of a design change in the app’s **product display and navigation**.  
Using **A/B testing and statistical analysis**, the study determines whether the modification increased user engagement or conversion.

---

## 🎯 Objective

To identify whether the **interface update** (font and layout change) led to a **significant improvement** in user behavior metrics such as:
- Number of events per user
- Conversion rate through key screens (product view → cart → checkout)
- Retention and session activity

---

## 📂 Dataset Description

The dataset contains **event logs** for users divided into two groups:
- **Group A** – Control group (original design)  
- **Group B** – Experimental group (new design)

Each record includes:
- `user_id` — Unique user identifier  
- `event_name` — Type of event (ProductPage, CartScreenAppear, PaymentScreenSuccessful, etc.)  
- `event_timestamp` — Time of occurrence  
- `experiment_group` — A or B  

---

## 🔍 Analysis Workflow

1. **Data Cleaning & Preparation**
   - Removed duplicates and invalid timestamps
   - Filtered the experiment period
   - Grouped users by experiment group

2. **Exploratory Data Analysis (EDA)**
   - Analyzed event frequency and flow between screens
   - Calculated conversion funnels for both groups
   - Visualized transitions using bar and funnel charts

3. **Statistical Testing**
   - Performed **A/B hypothesis tests** using proportions z-tests
   - Evaluated significance levels (`α = 0.05` and `α = 0.1`)
   - Applied **Bonferroni correction** to adjust for multiple comparisons

---

## 📊 Key Findings

- **No statistically significant differences** were found between groups A and B for main metrics.  
- With α = 0.05, all p-values ≥ 0.08 — the results are **not significant**.  
- Even with Bonferroni correction (`α_adj ≈ 0.0033`), no meaningful differences appear.  
- The visual redesign **did not affect user engagement** across event sequences.

✅ **Conclusion:** The font and layout change did **not impact user behavior**, so maintaining the current version is statistically justified.

---

## 🧠 Insights & Recommendations

- Continue monitoring behavioral data over longer periods before making further UI updates.  
- Focus future experiments on **pricing or product placement**, which may yield higher behavioral variance.  
- Introduce **segmented A/B tests** (e.g., by region or device) to capture micro-level effects.

---

## 🛠️ Tools & Technologies

- **Python 3.10+**
- **pandas** — Data handling  
- **numpy** — Calculations and aggregations  
- **matplotlib** — Data visualization  
- **scipy** — Statistical hypothesis testing  
- **statsmodels** — Confidence intervals & proportion tests  
- **jupyter notebook** — Interactive analysis environment

---

## ▶️ How to Run the Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your_username>/<your_repo>.git
   cd <your_repo>
