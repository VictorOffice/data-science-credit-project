# 🌍 World Bank Economic Data Analysis and GDP Prediction  

**Author:** Victor Alberto Barrios Masso  
**Project:** Udacity Data Scientist Nanodegree  

---

## 🧭 Motivation  

The goal of this project is to explore **World Bank open data (2000–2020)** to identify the key factors driving **GDP per capita** across countries and regions, and to build a **machine learning model** capable of predicting it.  

By connecting **economic interpretation** with **quantitative modeling**, the project demonstrates how open, reproducible data can help explain global development patterns and forecast economic prosperity.  

---

## 🧰 Libraries Used  

The project was developed in **Python** using the following main libraries:  

- `pandas` – data manipulation and cleaning  
- `numpy` – numerical operations and array handling  
- `matplotlib` and `seaborn` – visualization and plotting  
- `scikit-learn` – machine learning (modeling and evaluation)  
- `wbgapi` – access to the World Bank API  
- `joblib` – model persistence and serialization  

All dependencies are listed in the `requirements.txt` file.  

---

## 📂 Project Structure  

data-science-credit-project/
│
├── data/ # Raw and processed datasets
│ ├── world_bank_data.csv
│ └── processed_data.csv
│
├── notebooks/ # Main analysis notebook
│ └── world_bank_gdp_analysis.ipynb
│
├── reports/ # Figures generated from the analysis
│ ├── corr_heatmap.png
│ ├── regional_gdp.png
│ └── feature_importance.png
│
├── models/ # Trained model (optional)
│ └── rf_gdp_model.pkl
│
├── src/ # Additional Python scripts (if used)
│
├── README.md # Project documentation
├── requirements.txt # Required Python packages
└── LICENSE (optional)

---


---

## 📊 Summary of Results  

- **Data Source:** World Bank Databank (2000–2020)  
- **Target Variable:** GDP per capita (current USD)  
- **Model Used:** Random Forest Regressor  

### Key Findings  
- The **most influential features** are:  
  - Life expectancy  
  - Energy use per capita  
  - Population size  
- **Correlations:** education, employment, and energy access strongly correlate with higher income, while extreme inflation or large populations tend to lower per-capita GDP.  
- **Regional Trends:** North America and Europe show sustained growth; Sub-Saharan Africa remains significantly below the world average.  

### Model Performance  
- **R²:** 0.99  
- **RMSE:** ≈ $2,055 USD  
- The model generalizes well across countries and years, with some outliers in resource-dependent and small-island economies.  

---

## 💡 Insights and Interpretation  

The model’s top features align with core development economics theory:  

- **Life expectancy** captures health, education, and institutional quality — the human capital component.  
- **Energy use per capita** reflects industrialization and infrastructure development.  
- **Population** influences the denominator effect — higher populations dilute per-capita output.  

Machine learning complemented traditional analysis by quantifying these relationships and detecting **nonlinear effects**, such as the diminishing impact of trade openness beyond a certain level.  

---

## 🎯 Model Accuracy  

The Random Forest model achieved an **R² of 0.99** and an **RMSE of around $2,055**, showing strong predictive accuracy.  
The **Predicted vs Actual plot** displayed a near-perfect diagonal, confirming robust performance.  

While such accuracy indicates the model captures the structure of the data well, it also highlights that economic indicators are deeply interrelated — not purely independent.  

---

## 🔮 Predictive Scenario  

To illustrate model behavior:  

If a country increases **life expectancy by 5 years** and **energy use per capita by 10%**, the model predicts a GDP per capita increase of roughly **15%**.  
By contrast, a similar increase in **trade openness** without improvements in health or infrastructure yields a smaller gain (~5%).  

This demonstrates that **investing in human and physical capital** has a larger and more sustainable impact on income growth than short-term trade changes.  

---

## ⚠️ Limitations  

- Reporting quality and frequency vary among countries.  
- The model predicts **correlations**, not **causal effects**.  
- Structural shocks (wars, pandemics, policy changes) may alter model performance.  

---

## 🚀 Next Steps  

- Add **composite indicators** such as human capital or governance quality.  
- Apply **SHAP** analysis for interpretability at the country level.  
- Extend the model to **forecasting** with time-series features.  
- Deploy an **interactive dashboard** for exploration and scenario testing.  

---

## 🙏 Acknowledgments  

This project was completed as part of the **Udacity Data Scientist Nanodegree**.  
All data were retrieved from the **World Bank Databank** using the `wbgapi` Python library.  

Special thanks to **Udacity mentors and reviewers** for guidance on reproducibility, feature selection, and model evaluation.  

---

## 🔗 References  

- **World Bank Databank:** [https://data.worldbank.org](https://data.worldbank.org)  
- **Udacity Data Scientist Nanodegree:** [https://www.udacity.com](https://www.udacity.com)  
- **Medium Article:** [Predicting GDP per Capita with World Bank Open Data](https://medium.com/@victoralberto.barriosmasso/predicting-gdp-per-capita-with-world-bank-open-data-a-practical-data-science-project-1a80175bc2ec)

---

## 📎 Hashtags  

#DataScience #MachineLearning #GDPPrediction #EconomicGrowth #WorldBankData

