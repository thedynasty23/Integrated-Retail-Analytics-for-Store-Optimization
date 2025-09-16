# 🏬 Integrated Retail Analytics for Store Optimization  

##### **👨‍💻 Contribution** – RAJVANSH  

## 📖 Project Summary  
This project demonstrates the transformative out of advanced machine learning in optimizing retail operations. Using **⚡ XGBoost**, a powerful gradient boosting algorithm, the system leverages multi-source data — including store attributes, economic indicators, promotions, and sales history — to deliver **granular sales forecasting, anomaly detection, customer segmentation, and market basket analysis**.  

**🔎 Forecasting Performance:**  
- 🎯 **Overall MAE:** 1357.57  
- 📉 **Overall RMSE:** 3018.71  
- ✅ Best-performing store–department pairs achieved **RMSE ≈ 0.000062**, indicating near-perfect prediction in some cases.  
- ⚠️ Challenging segments (e.g., **Store 39, Dept 3**) reached **RMSE ≈ 42,008**, suggesting room for localized model tuning.  

---

## ❓ Problem Statement  
Retailers face challenges in **demand forecasting, inventory optimization, workforce allocation, and promotional planning**. This project addresses those by integrating ML-driven forecasting and business analytics to generate **actionable strategies**.  

---

## 🔍 1. Know Your Data  
- 📂 Imported and merged datasets: `sales data-set.csv`, `features data set.csv`, `stores data-set.csv`.  
- 🔎 Performed dataset overview, missing values analysis, duplicates check, and feature summaries.  
- 📝 Generated a **Retail Dataset Analysis Report** to document input/output variables and missing value percentages.  

---

## 📊 2. Understanding Your Variables  
- 📚 Comprehensive variable descriptions across datasets (Sales, Features, Stores).  
- 🏬 Defined business context for each variable (e.g., `Weekly_Sales`, `IsHoliday`, `Store_Type`).  
- 🧭 Established quick reference rules for downstream modeling.  

---

## 🛠️ 3. Data Wrangling  
- 🔗 Merged multi-source datasets into a unified dataframe.  
- 🧹 Cleaned and standardized categorical variables.  
- 🚦 Applied strategies for handling missing values and anomalies.  

---

## 🚨 4. Anomaly Detection  
Applied three complementary techniques to flag irregular sales patterns:  
- 💡 **STL decomposition** for trend-seasonality breakdown.  
- ⚙️ **SPC (Statistical Process Control)** to identify control-limit breaches.  
- 🌲 **Isolation Forest** for outlier detection.  
- 🤝 Combined consensus approach to finalize anomaly points.  

---

## 📈 5. Data Visualization & Storytelling  
Created multiple visualizations to understand relationships:  
- 📊 Weekly sales, temperature, fuel price, CPI distributions.  
- 📈 Overall sales trends and seasonal effects.  
- 🎉 Holiday vs non-holiday comparison.  
- 🏬 Store type/size vs weekly sales.  
- 🏷️ Department-level variability.  
- 🔥 Correlation heatmap for feature relationships.  

---

## 🛒 6. Market Basket Analysis  
- 📌 Identified product associations to inform cross-selling.  
- 🎯 Generated rules to guide promotions and bundled offers.  

---

## 🧩 7. Feature Engineering  
- 🔁 Lagged features & 📈 rolling statistics for time-series modeling.  
- 🔗 Interaction terms (e.g., Store_Type × IsHoliday).  
- 🏬 Store-level and store-department-level aggregations.  
- 🚦 Anomaly handling and categorical encoding.  

---

## 🧮 8. Feature Selection  
- 📉 Variance threshold filtering to drop low-information features.  
- 🌲 Feature importance ranking with RandomForestRegressor.  

---

## 👥 9. Customer Segmentation  
- 🛠️ Applied **KMeans clustering** with diagnostics to segment stores/departments.  
- 🧑‍🤝‍🧑 Segmentation insights support tailored marketing and inventory strategies.  

---

## 🎯 10. Personalized Marketing & Inventory Strategy  
Linked segmentation results with markdown strategies to optimize promotions and reduce overstock/stockout risk.  

---

## 🧾 11. Strategy Generation Logic  
Codified rules that integrate segmentation, anomaly flags, and forecast results into actionable recommendations.  

---

## 🤖 12. Demand Forecasting  
- Implemented **XGBoost Regressor** as the core model.  
- 🔧 Tuned hyperparameters (`learning_rate=0.1, max_depth=4, n_estimators=200`, etc.) via GridSearch.  
- 🐞 Debugged flat predictions using lag/rolling features and early stopping.  

**📊 Results:**  
- ✅ Top groups: near-perfect predictions with **MAE/RMSE ≈ 0.000062**.  
- ❌ Worst groups: **Store 39, Dept 3** with **RMSE ≈ 42,008**.  
- 🎯 **Overall performance:** MAE = 1357.57, RMSE = 3018.71.  

---

## 🏁 Conclusion  
The project highlights:  
- 📦 **Inventory optimization** via accurate weekly forecasts.  
- 👥 **Workforce & promotion planning** enabled by demand spikes prediction.  
- 🏬 **Localized strategies** tailored by store–department segmentation.  
- 🚀 Integrated anomaly detection, segmentation, and basket analysis enhance overall decision-making.  

---

## ⚙️ Technical Requirements  
- 🐍 Python 3.8+  
- 📓 Jupyter Notebook / Google Colab  
- 📚 Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `statsmodels`  

---

## ▶️ Usage and Replication  
1. Clone the repo:  
   ```bash
   git clone https://github.com/thedynasty23/Integrated-Retail-Analytics-for-Store-Optimization.git
   cd Integrated-Retail-Analytics-for-Store-Optimization
