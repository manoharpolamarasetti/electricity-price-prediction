# electricity-price-prediction
Forecasting UK electricity prices and analysing renewable energy impact using machine learning (2009–2023)
# 🔋 UK Electricity Price Prediction (2009–2023)

This project forecasts electricity prices in the UK using machine learning and analyses the effect of renewable energy sources on price volatility.

📘 **Thesis Title**: Predicting Electricity Prices and Quantifying Dependence on Renewable Energies  
📅 Duration: Jan 2024 – June 2024  
🎓 MSc Data Science – University of Aberdeen

---

## 🧠 Problem Statement
The increasing share of intermittent renewable sources like wind and solar introduces significant unpredictability in UK electricity prices. This project develops predictive models to forecast prices and analyses the impact of renewables.

---

## 🧰 Tools & Technologies
- **Languages**: Python
- **Libraries**: Pandas, Scikit-learn, Matplotlib, Seaborn
- **Dashboards**: Tableau (EDA visualisations)
- **Models**:
  - Linear Regression
  - Random Forest
  - Gradient Boosting Regressor

---

## 📊 Data Sources
- National Grid ESO: [Generation Mix](https://www.nationalgrideso.com/data-portal/historic-generation-mix)
- Ofgem & Elexon: Settlement prices and demand
- Date Range: Jan 2009 – Dec 2023
- Granularity: 30-minute settlement periods

---

## 🧪 Models & Evaluation

| Model                | R² (Best) | MAE (Min) | Notes                         |
|---------------------|-----------|-----------|-------------------------------|
| Linear Regression    | 0.26      | 14.3      | Struggled with non-linearity |
| Random Forest        | 0.61      | 10.7      | Strong performance (2019)     |
| Gradient Boosting    | 0.34      | 9.1       | Best overall seasonal fit     |

---

## 🔍 Key Insights
- **Wind & Solar** prices show an inverse relation with market prices.
- **Biomass** gained importance post-2017 due to policy changes.
- Models perform differently across **seasons and years**, emphasising the dynamic nature of the market.

---

## 📁 Project Structure
- `data/`: Descriptions of datasets used
- `notebooks/`: All modelling notebooks (Jupyter)
- `scripts/`: Data preprocessing and utility functions
- `visuals/`: Model charts, feature importance, heatmaps
- `thesis/`: Final dissertation PDF

---

## 🖼️ Sample Visuals

### Feature Importance – Random Forest
![feature_importance](visuals/feature_importance.png)

### Actual vs Predicted Prices (Gradient Boosting)
![model_results](visuals/model_results.png)

---

## 📜 Thesis
Download the full thesis PDF [here](thesis/Manohar_Polamarasetti_Thesis.pdf)

---

## 👤 Author
**Manohar Babu Polamarasetti**  
📍 Aberdeen, UK  
📫 [Email](mailto:polamarasettimanohar@gmail.com) • [GitHub](https://github.com/manoharpolamarasetti)
