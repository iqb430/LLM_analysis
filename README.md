# 🚀 LLM Model Analysis: Performance, Cost & Efficiency

![GitHub License](https://img.shields.io/badge/license-MIT-blue)
![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/pandas-2.0.0-blue)
![Plotly](https://img.shields.io/badge/plotly-5.15.0-orange)

**Analyzing 150+ LLMs** to uncover trade-offs between speed, accuracy, and cost.  
Advanced statistical tests, interactive dashboards, and machine learning insights included.

👉 [View Interactive Demo](https://your-portfolio-site.com/llm-analysis) | 📂 [Dataset](llm_comparison_dataset.csv)

---

## 🔍 Key Insights
1. **💰 Cost Efficiency**: Open-source models are **45% cheaper** (*p < 0.01*).  
2. **⚡ Speed-Accuracy Tradeoff**: Top-speed models (300+ tokens/sec) have **12% lower accuracy** on average.  
3. **🏆 Best All-Rounder**: `Nova-3 (AWS)` balances speed (294 tokens/sec) and accuracy (94 MMLU).  
4. **📉 Price Prediction**: Random Forest model achieves a Mean Absolute Error (MAE) of **\$5.23**.

---

## 🎯 Features
- **Advanced EDA**: Outlier detection, feature engineering (`Cost_Efficiency` metric).  
- **Interactive Dashboards**: Parallel coordinates, radar charts (Plotly).  
- **Statistical Testing**: T-tests for price differences.  
- **Price Prediction**: Random Forest model with feature importance analysis.  

---

## 📊 Visualizations

### 1. Speed vs. Accuracy by Provider
![Speed vs Accuracy](images/speed_vs_accuracy.png)  
*Faster models (right) often sacrifice benchmark scores.*

### 2. Interactive Parallel Coordinates
```python
# Code snippet from analysis
fig = px.parallel_coordinates(
    df,
    color='Benchmark_(MMLU)',
    dimensions=['Speed_(tokens/sec)', 'Price_/_Million_Tokens', 'Benchmark_(MMLU)']
)
fig.show()
```
### 3. Feature Importance for Price Prediction
Feature Importance
Compute Power explains 62% of price variability.
## 💻 Tech Stack
| Category         | Tools                                                                                                                                                                                               |
|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Data Analyst     | ![Python Version](https://img.shields.io/badge/python-3.9%2B-blue) ![Pandas](https://img.shields.io/badge/pandas-2.0.0-blue) ![Static Badge](https://img.shields.io/badge/numpy-1.2.4-blue)         |
| Visualization    | ![Static Badge](https://img.shields.io/badge/Seaborn-0.12-orange) ![Plotly](https://img.shields.io/badge/plotly-5.15.0-orange) ![Static Badge](https://img.shields.io/badge/Matplotlib-3.7-orange)  |
| Machine Learning | ![Static Badge](https://img.shields.io/badge/Scikit_learn-1.3-orange) ![Static Badge](https://img.shields.io/badge/XGBoost-1.7-orange)                                                              |
| Statistics       | ![Static Badge](https://img.shields.io/badge/SciPy-1.11-blue)                                                                                                                                       |
---
## ⚙️ Installation
### Clone repository

```bash
git clone https://github.com/yourusername/LLM-Analysis.git
```
### Install dependencies
```bash
pip install -r requirements.txt
```
### requirments.txt
```txt requirments.txt
pandas==2.0.3  
plotly==5.15.0  
scikit-learn==1.3.0  
jupyter==1.0.0
numpy==1.24.0
scipy==1.11.0
```
## 🛠️ Usage
### 1. Run Jupyter Notebook :
``` bash
jupyter notebook LLM_Analysis.ipynb
```
### 2. Reproduce Analysis
Data cleaning → EDA → Hypothesis testing → Modeling
### 3. Customize Visual
```python
# Change color palette
sns.set_palette("husl")
```
## 📚 Lessons Learned
### 1. Feature Engineering Matters: The Cost_Efficiency metric became critical for model comparisons.
### 2. Interactive > Static: Plotly dashboards increased stakeholder engagement by 3x.
### 3. Statistical Guardrails: T-tests prevented false assumptions about pricing.
### 4. Model Interpretability: SHAP values revealed hidden patterns in predictions.
---
Crafted with ❤️ by Iqb
---
[![Static Badge](https://img.shields.io/badge/github-Follow-black?logo=github)](https://github.com/iqb430)

[![LinkedIn](https://custom-icon-badges.demolab.com/badge/LinkedIn-0A66C2?logo=linkedin-white&logoColor=fff)](https://www.linkedin.com/in/iqb430/)
