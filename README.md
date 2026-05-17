# 🧠 Teen Mental Health — Exploratory Data Analysis

> Uncovering behavioral patterns associated with depression risk in 1,200 adolescents through data-driven analysis.

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Kaggle](https://img.shields.io/badge/Kaggle-View%20Notebook-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## 📌 Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on a structured dataset of 1,200 teenagers aged 13–19, examining how daily behavioral habits — sleep, screen time, stress, and anxiety — relate to depression risk.

The analysis goes beyond visualization by incorporating **statistical hypothesis testing** to validate each finding, making the conclusions evidence-based rather than observational.

---

## 🔍 Key Findings

| Finding | Detail |
|---|---|
| 😟 **Stress & Anxiety** | +58% and +55% higher in depressed teens — strongest separators |
| 📱 **Social Media Usage** | Depressed teens average 6.7 hrs/day vs 4.5 hrs for non-depressed (+50%) |
| 😴 **Sleep Deprivation** | Depressed teens sleep only 4.8 hrs/night vs 6.5 hrs (−27%) |
| 🚫 **Platform Type** | Instagram vs TikTok shows **no significant difference** (Chi-Square p = 0.80) |
| ⚖️ **Class Imbalance** | 97.4% non-depressed vs 2.6% depressed — must be addressed before modeling |

---

## 📁 Repository Structure

```
teen-mental-health-eda/
│
├── Teen_Mental_Health.ipynb    # Main analysis notebook
├── Teen_Mental_Health_Dataset.csv  # Dataset
├── README.md                   # This file
└── requirements.txt            # Python dependencies
```

---

## 📊 Analysis Structure

The notebook is organized into 15 sections:

1. **Introduction** — Background, objectives, and key findings summary
2. **Dataset Overview** — Shape, data types, and descriptive statistics
3. **Dataset Type Identification** — Structured tabular classification
4. **Data Cleaning** — Null checks, duplicates, formatting, outlier detection
5. **Univariate Analysis** — Distribution of numerical and categorical features
6. **Bivariate Analysis** — Violin plot, KDE, stacked bar chart vs depression label
7. **Multivariate Analysis** — Pairplot, groupby mean comparison, bar chart
8. **Correlation Analysis** — Heatmap and ranked correlation with depression label
9. **Target Variable Analysis** — Class distribution and imbalance severity
10. **Feature Engineering** — `high_screen_time`, `sleep_category` with visualizations
11. **Outlier Detection** — Scatter plot, distribution plot, IQR method
12. **Class Imbalance Handling** — Recommended techniques (SMOTE, class weighting)
13. **Statistical Testing** — Pearson correlation, Independent T-test, Chi-Square test
14. **Final Insights & Business Understanding** — Stakeholder recommendations
15. **Conclusion** — Summary, limitations, and next steps

---

## 🧪 Statistical Testing

| Test | Variable | Result |
|---|---|---|
| Pearson Correlation | All numerical features | sleep, social media, stress, anxiety → significant (p < 0.05) |
| Independent T-Test | sleep_hours | Depressed teens sleep 1.73 hrs less (p < 0.0001) |
| Chi-Square Test | platform_usage | No association with depression (p = 0.7966) |

---

## ⚙️ Requirements

```bash
pip install pandas numpy matplotlib seaborn scipy
```

Or install all dependencies at once:

```bash
pip install -r requirements.txt
```

**requirements.txt:**
```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scipy>=1.9.0
```

---

## 🚀 How to Run

**Clone the repository:**
```bash
git clone https://github.com/your-username/teen-mental-health-eda.git
cd teen-mental-health-eda
```

**Launch the notebook:**
```bash
jupyter notebook Teen_Mental_Health.ipynb
```

Or open directly on **[Kaggle](#)** *(add your Kaggle link here)*.

---

## 🔗 Behavioral Risk Chain

```
Excessive social media usage
        ↓
Reduced sleep duration
        ↓
Elevated stress & anxiety
        ↓
Higher depression risk
```

Early intervention at any single point — especially sleep — may help prevent the full chain from developing.

---

## ⚠️ Limitations

- All correlations are weak (r < 0.2) — findings are directional, not conclusive
- External factors (family environment, trauma, socioeconomic status) are not captured
- Depression label is behavioral, not a clinical diagnosis
- Small minority class (n = 31) limits statistical power for minority-group findings

---

## 🔮 Next Steps

- [ ] Apply **SMOTE** or class weighting to handle imbalance
- [ ] Build a binary classification model (Logistic Regression / Random Forest / XGBoost)
- [ ] Evaluate using **Recall** and **F1-Score** as primary metrics
- [ ] Apply **SHAP values** for feature importance interpretability

---

## 👤 Author

**[Your Name]**
- Kaggle: [@your-kaggle-username](#)
- LinkedIn: [your-linkedin](#)
- GitHub: [@your-github-username](#)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

*Teen depression is not caused by one habit alone — it emerges from compounding behavioral imbalances. This analysis demonstrates that data-driven approaches can surface meaningful patterns to support earlier, more targeted mental health interventions.*
