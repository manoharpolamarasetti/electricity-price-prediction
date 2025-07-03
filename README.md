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

## 📁 Dataset

One of the datasets used in this project is too large to host on GitHub, so it's stored on Google Drive.

📥 [Download Full Dataset ][(https://drive.google.com/uc?export=download&id=YOUR_FILE_ID)](https://drive.google.com/file/d/11szPrOgtDp6iQFmiLUzZe-ZRZuavrws3/view?usp=sharing)

> ⚠️ You may need to right-click the link and choose "Save link as…" if Google Drive blocks previewing due to file size.

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


### 🔹 Actual vs Predicted Prices (Gradient Boosting – January 2016)
*Model trained from 2009 to 2015 and tested on January 2016 (First 200 samples)*

![Gradient Boosting - Jan 2016](electricity-price-prediction/visuals/Gradient%20boosting%20trained%20from%202009%20to%202015%20and%20tested%20January%202016(first%20200%20samples).png)

- The model captures overall trends but underpredicts sharp spikes.
- Common limitation in tree-based regressors for volatile time series.

---

### 🔹 Feature Importance (Random Forest – January 2019)
*Model trained from 2014 to 2018 and tested on January 2019*

![Random Forest Feature Importance - Jan 2019](electricity-price-prediction/visuals/Random%20Forest%20feature%20importance%20(trained%20from%202014%20to%202018%20and%20predicted%20January%202019)Figure%2018%20Random%20Forest%20f.png)

- **Top contributor:** `STORAGE`
- Other important features: `HYDRO`, `BIOMASS`, `RENEWABLE`, `GENERATION`
- Shows how energy source variability influences electricity price forecasts.


---

---

## 📜 Thesis

📄 ## 📜 Thesis

📄 [View Thesis (PDF)](electricity-price-prediction/thesis/thesis.pdf)

This thesis outlines the methodology, machine learning models, and insights developed while forecasting UK electricity prices and analyzing the impact of renewable energy sources from 2009–2023.




---

## 👤 Author
**Manohar Babu Polamarasetti**  
📍 Aberdeen, UK  
📫 [Email](mailto:polamarasettimanohar@gmail.com) • [GitHub](https://github.com/manoharpolamarasetti)
