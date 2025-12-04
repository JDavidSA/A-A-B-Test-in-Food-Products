<!-- MAIN TITLE -->
<h1 align="center">🧪 A/B Test in Food Products</h1>

<p align="center">
  Analysis of user behavior for a food delivery company to evaluate the impact of a visual design update in the app’s product display and navigation.<br>
  Using A/B testing and statistical methods, this project determines whether the interface change improved engagement or conversion.
</p>

---

## 🧭 1. Introduction

Food delivery apps rely heavily on interface clarity to drive conversions across the product browsing → cart → checkout flow.  
This project evaluates whether a **UI redesign** specifically changes to font style and layout positively affected user behavior.

Through A/B testing and statistical hypothesis validation, the study identifies whether users exposed to the new design behaved differently from those viewing the original version.

---

## 🎯 2. Project Objective

The primary goal is to determine whether the visual update resulted in measurable behavioral improvements, including:

- Increase in **events per user**
- Higher **conversion** across key screens (Product → Cart → Checkout)
- Improved **session activity** or retention patterns

The analysis ensures decisions about design rollouts are backed by statistical evidence.

---

## 🧪 3. What Was Done

### ✔ Data Cleaning & Preparation
- Removal of duplicated user events  
- Filtering of event logs to include only the experiment window  
- Validation of timestamps and standardization of user flow sequences  
- Segmentation of users into **control (A)** and **experiment (B)** groups  

### ✔ Exploratory Data Analysis (EDA)
- Computation of event frequency per user and per experiment group  
- Funnel analysis for key screens: Product Page → Cart → Checkout  
- Bar charts, funnel graphs, and event flow inspection to detect behavioral differences  

### ✔ Statistical Testing
- **Two-Proportion Z-Tests** for conversion comparisons  
- Evaluation under significance levels **α = 0.05** and **α = 0.1**  
- Application of **Bonferroni correction** for multiple hypothesis testing  
- Determination of whether observed differences are meaningful or attributable to chance  

---

## 🛠️ 4. Tools & Technologies Used

- **Python 3.10+**  
- **Pandas** — Data manipulation  
- **NumPy** — Aggregations & vectorized computation  
- **Matplotlib** — Data visualization  
- **SciPy** — Hypothesis testing  
- **Statsmodels** — Statistical modeling and confidence intervals  
- **Jupyter Notebook**

---

## 📊 5. Key Results

### ✔ Statistical Outcomes
- No significant differences were found between Groups A and B across major conversion and engagement metrics.  
- All p-values were **≥ 0.08**, meaning the differences are not statistically significant at α = 0.05.  
- Under Bonferroni correction (`α_adj ≈ 0.0033`), the findings remain non-significant.  

### ✔ Behavioral Interpretation
- The redesign **did not influence user conversion**, event activity, or overall navigation.  
- User flows and drop-off points were nearly identical between groups.  

---

## 📌 6. Conclusion

The A/B test results show that the UI update focused on font and layout changes **did not produce any measurable improvement** in user behavior.  
Both groups (A and B) displayed nearly identical engagement patterns, funnel progression, and conversion rates, with all p-values ≥ 0.08, confirming that the differences are **not statistically significant**.

### 🔍 Interpretation

Because the redesign was purely visual, it did not modify how users interacted with the product flow. In food delivery apps, meaningful behavioral changes typically come from structural or functional updates rather than cosmetic ones.

### ✔ Final Conclusion

Keeping the existing UI is statistically justified.  
Future experiments should focus on changes with higher behavioral impact such as product placement, pricing visibility, or interaction flow adjustments rather than minor visual styling updates.

