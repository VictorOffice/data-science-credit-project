# World Bank Economic Data Analysis & GDP per Capita Prediction

## Motivation
Analyze World Bank indicators (2000–2020) to understand the main drivers of GDP per capita and build a simple predictive model for stakeholder decision-making and scenario planning.

## Business Questions
1. Which indicators are most correlated with GDP per capita?
2. How has GDP per capita evolved across regions (2000–2020)?
3. Can we predict GDP per capita using a simple ML model?

## Data
- Source: World Bank (2000–2020), fetched via `wbgapi`.
- Grain: country–year panel.
- Target: GDP per capita (current USD).

## Libraries Used
- pandas, numpy, matplotlib, seaborn  
- scikit-learn, joblib  
- wbgapi  
> Full pinned versions in `requirements.txt`.

## Repository Structure
- `notebooks/world_bank_gdp_analysis.ipynb` — Full CRISP-DM workflow (EDA → Preparation → Modeling → Evaluation → Scenario). Includes functions with docstrings and comments.
- `requirements.txt` — Python dependencies.
- `.gitignore` — excludes cache/temporary/large artifacts.
- `data/` — local-only cache/exports (not tracked).
- `reports/` — optional HTML/PDF exports (not tracked).
- `models/` — optional saved models (`.joblib`, not tracked).

## How to Run
```bash
cd data-science-credit-project
python -V
# (optional) activate your venv
pip install -r requirements.txt
jupyter notebook
# Open notebooks/world_bank_gdp_analysis.ipynb
# Kernel → Restart & Run All

