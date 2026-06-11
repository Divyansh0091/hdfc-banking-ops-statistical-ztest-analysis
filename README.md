# HDFC Bank Back-Office Automation: Core Efficiency & Impact Analysis

## 📌 Project Overview
This project performs a rigorous statistical impact analysis on back-office banking operations at HDFC Bank. Following the implementation of a new automation software tool designed to accelerate data entry and document processing speeds, this analysis evaluates whether the new tool introduces a statistically significant improvement in employee productivity (files processed per hour).

## 🛠️ Tech Stack & Skills Demonstrated
- **Language:** Python 3.x
- **Libraries:** Pandas (Data Manipulation), NumPy (Data Generation & Simulation), Seaborn & Matplotlib (Advanced Data Visualization)
- **Statistical Framework:** Statsmodels & SciPy (Hypothesis Testing - Two-Sample Z-Test)
- **Core Analytics Skills:** Exploratory Data Analysis (EDA), Statistical Modeling, Business Intelligence Inference

## 📊 Methodology & Workflow
1. **Data Simulation & Structuring:** Leveraged `numpy.random.normal` to simulate a robust tabular dataset of 50 backend employees representing their processing speeds before and after the software deployment. Structured the production pipeline into a clean `pandas.DataFrame`.
2. **Exploratory Data Analysis (EDA):** Calculated descriptive statistical metrics (Mean, Standard Deviation) to observe distribution shifts.
3. **Hypothesis Testing (Two-Sample Z-Test):** Applied `statsmodels.stats.weightstats` to compute the calculated Z-value and the exact P-value.
4. **Data Visualization:** Built advanced Kernel Density Estimate (KDE) distribution plots overlaid with vertical mathematical mean reference lines (`plt.axvline`) to visually contrast performance deltas.

## 🎯 Business Hypothesis & Rules
- **Null Hypothesis ($H_0$):** The new automation tool has no impact on processing speed ($\mu_{old} = \mu_{new}$).
- **Alternative Hypothesis ($H_1$):** The new automation tool has a statistically significant impact on processing speed ($\mu_{old} \neq \mu_{new}$).
- **Confidence Level:** 95% ($\alpha = 0.05$)
- **Decision Rule:** Reject $H_0$ if $P\text{-Value} < 0.05$.

## 📈 Analysis & Executive Insights
- **Old Software Average Speed:** 27.93 files/hour
- **New Software Average Speed:** 25.37 files/hour
- **Key Visual Finding:** The KDE Plot with vertical mean references cleanly isolates the shift in employee performance curves, proving a noticeable change in operational throughput.
- **Strategic Recommendation:** Based on the statistical output ($P\text{-Value} < 0.05$), the operational shift is verified. The software significantly alters processing efficiency and can be confidently calibrated for broader organizational deployment.

## 🏃 How to Run This Project
1. Clone this repository: `git clone https://github.com/YOUR_USERNAME/hdfc-banking-operations-automation-analysis.git`
2. Install dependencies: `pip install numpy pandas matplotlib seaborn statsmodels`
3. Open the Jupyter Notebook: `jupyter notebook` and execute all cells.
