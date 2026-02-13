# A/B Testing Automation Framework & Portfolio Analysis

This repository contains a comprehensive A/B testing analysis for an e-commerce platform. The project involves developing an **Automated Statistical Framework** in Python to analyze 5 different feature experiments accurately and efficiently.

## 🚀 Key Framework Features
In this project, I built an `ABTestAnalyzer` class with the following automated logic:
* **SRM (Sample Ratio Mismatch) Check**: Ensures sample distribution between Control and Treatment is valid and unbiased.
* **Automated Normality Test**: Utilizes **Shapiro-Wilk** to detect data distribution.
* **Smart Statistical Selection**: Automatically switches between **T-Test** (for normal data) and **Mann-Whitney U** (for non-normal/skewed data).
* **Multiple Testing Correction**: Applies the **Holm-Bonferroni** method to control the Family-wise Error Rate.
* **Relative Lift & Confidence Intervals**: Calculates business impact and uncertainty.

---

## 📊 Experiment Results Summary

| ID | Feature Experiment | Primary Metric | Statistical Result | Business Decision |
| :--- | :--- | :--- | :--- | :--- |
| **01** | Navigation Menu | Revenue & ATC | ❌ Significant Drop | **Roll-back** |
| **02** | Novelty Products | Category Revenue | ✅ Significant Lift | **Deploy** |
| **03** | Premium Slider | Avg. Product Price | ✅ Significant Lift | **Deploy** |
| **04** | PDP Layout | Conversion Rate | ➖ Neutral | **Discard** |
| **05** | Search Engine | Add to Cart | ⚠️ Partial Success | **Iterate** |

---

## 🛠️ Tech Stack
* **Python 3.11**
* **Pandas & NumPy**: Data manipulation.
* **SciPy**: Statistical testing (`stats.shapiro`, `stats.mannwhitneyu`).
* **Statsmodels**: Proportion tests and p-value corrections.
* **Jupyter Notebook**: Analysis workflow documentation.

---

## 💡 Key Business Insights
1. **Quality over Quantity (Exp 03)**: The *Slider Recommendation* feature proved effective as an **Upselling** tool. While it didn't increase total clicks, it significantly boosted the **Average Product Price**.
2. **Navigation Friction (Exp 01)**: The change to a *Dropdown Menu* harmed user experience, leading to a **10.33% drop** in Add to Cart rates. The quick decision to roll back saved significant potential revenue.

---

## 📬 Contact
**Albert Kurnia Himawan**
* **Email**: albertk.himawan@gmail.com
* **LinkedIn**: Albert Kurnia (https://www.linkedin.com/in/albert-kurnia-58585685/)
