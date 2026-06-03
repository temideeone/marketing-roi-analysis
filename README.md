# Simple Linear Regression – Marketing ROI Analysis

### Project Overview
This project analyzes a historical marketing dataset using Python to construct a Simple Linear Regression model. By utilizing Ordinary Least Squares (OLS) estimation, the analysis evaluates expenditures across multiple advertising mediums (TV, Radio, Social Media) to determine their impact on sales performance. The final objective is to identify the channel with the most dominant Return on Investment (ROI) and provide a data-driven capital allocation strategy for corporate stakeholders.

---

### Core Project Goals
* **Data Exploration:** Conduct Exploratory Data Analysis (EDA) to evaluate correlations between marketing streams.
* **Model Selection:** Isolate the independent vehicle exhibiting the highest direct alignment with corporate Sales.
* **Statistical Modeling:** Fit an OLS regression model and extract descriptive parameters.
* **Assumption Validation:** Verify model safety parameters via diagnostic plots (Linearity, Normality, and Homoscedasticity).
* **Strategic Consulting:** Translate mathematical coefficients into clear, actionable budget advice for management.

---

### Environment Setup & Installation
To set up your local environment and reproduce this analysis, ensure you have Python installed, clone this repository, and install the required data science libraries:

```bash
# Clone the repository to your local system
git clone https://github.com

# Navigate into the project folder
cd marketing-roi-analysis

# Install the required dependencies using pip
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
```

---

### Key Analytical Findings & Model Diagnostics

Our exploratory matrix confirmed that **TV Advertising** shares the strongest linear correlation with overall corporate Sales revenue. Using TV spend as our sole independent feature, the OLS regression model produced the following high-confidence metrics:

* **Model Explanatory Power ($R^2 = 0.999$):** The regression model accounts for **99.9%** of all historical sales variations, proving extreme predictive stability.
* **The ROI Multiplier ($\beta_{TV} = 3.5615$):** For every single dollar ($1.00) invested in TV advertising, corporate revenue increases by an estimated **3.5615 units**.
* **Statistical Significance ($p < 0.001$):** The p-value for the TV independent variable is `0.000`, confirming a highly reliable relationship with zero probability of accidental correlation.
* **Durbin-Watson Parameter (`1.998`):** Positioned directly next to the ideal value of `2.0`, confirming complete independence of errors and zero sequencing bias.
* **Residual Balance Check (Jarque-Bera $p = 0.985$):** Confirms that our prediction errors are normally distributed and completely symmetrical.

---

### Strategic Business Recommendation
1. **Capital Consolidation:** Immediately freeze budget expansion across underperforming channels (Radio and Social Media) and redirect those capital reserves into the TV advertising pipeline.
2. **Predictive Budgeting:** Implement the model equation $\text{Sales} = 3.5615 \times (\text{TV Spend}) - 0.1325$ into rolling quarterly forecasts to project unit volumes based on scheduled media purchases.
