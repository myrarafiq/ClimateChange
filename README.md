# 🌍 Who's to Blame for Climate Change?

**Project Type**: Climate Change Prediction & Modeling with R

In 1896, Swedish scientist Svante Arrhenius predicted that atmospheric CO₂ levels could alter Earth's temperature. Over a century later, climate change is an urgent global issue. Countries meet annually at COP summits to set CO₂ reduction targets — but how do we know what's fair, and who should reduce the most?

This project explores which factors most strongly predict a country's CO₂ emissions. We use data from the **World Bank**, train predictive models (including regression and neural networks), and forecast future emissions for 2020 to offer insights on what drives emissions and how they might be reduced.

---

## 📦 Dataset

**Source**: [The World Bank](https://databank.worldbank.org/source/world-development-indicators)  
**Scope**: Socio-economic and environmental indicators for countries over multiple years  
**Target Variable**: `co2_emission` (metric tons per capita)

**Predictors include**:
- GDP, population, trade, employment sectors  
- Land use, urbanization, life expectancy  
- Imports/exports, energy-related economic activity  

Full variable descriptions are available in the dataset file.

---

## 🧪 Project Roadmap

### Part 1: EDA
- Visualized key features and explored relationships with CO₂ emissions  
- Identified population, GDP, trade, and industrial activity as strong predictors  

### Part 2: Baseline Model
- Created a simple **mean model** as a baseline  
- RMSE used to evaluate model performance  

### Part 3: Regression Models
- Trained multiple linear regression models  
- Explored variable combinations and multicollinearity  
- Best model (excluding `country` to avoid overfitting) had an RMSE of **2.3**

### Part 4: Neural Networks
- Scaled predictors between 0–1  
- Built and tested multiple neural networks  
- Compared to regression performance — regression outperformed NN in this case  

### Part 5: Evaluation & Insights
- Used best model to predict **2020** emissions  
- RMSE increased slightly to **2.5**, likely due to COVID-19 disruptions  
- Key predictors included:
  - `population`
  - `gdp`
  - `life_expectancy`
  - `service_employment_per`
  - `trade_gdp_per`

---

## 📊 Key Takeaways

- **Economic and demographic factors** are the strongest predictors of CO₂ emissions  
- Countries with large populations and industrial GDP tend to emit more  
- Models show promise for forward-looking **policy forecasting**  
- 2020 predictions matched real data well, validating model performance  

---

## ⚠️ Limitations

- Each year treated as an **independent observation** — doesn't capture time trends  
- No policy or energy source data included — can't assess causation or mitigation  
- Correlation ≠ causation: we identified patterns, not drivers  

---

