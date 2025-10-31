# Forecasting Food Safety Incidents

This repository provides access to a collection of **historical global food safety incident datasets**, encompassing both **recalls** and **border rejections**, curated from the **FOODAKAI** platform.  
The data support applied research in **food risk prediction**, **time-series forecasting**, and **data-driven food safety management**.

---

## Agroknow Dataset Description

The repository includes **eight datasets**, each corresponding to a distinct food product or ingredient:  
**almonds, cereals, chicken, cinnamon, cocoa, sesame seeds, shrimps,** and **strawberries**.

Each dataset is provided in **CSV format** and includes records of individual incidents reported globally.  
Each observation refers to a unique **product–hazard event**, as announced by food safety authorities.

Researchers may adapt the datasets according to the scope of their analysis:

- **Ingredient-level forecasting:** use the full dataset without filtering by hazard or origin.  
- **Hazard-specific forecasting:** filter by a specific hazard or hazard category.  
- **Origin-specific forecasting:** filter by country of origin.  
- Data are available at **daily granularity**, which can be aggregated to **weekly, monthly, or quarterly** intervals.  
  Aggregation at the **monthly level** is generally recommended for enhanced model robustness and interpretability.

---

## Dataset Structure

| Column | Description |
|---------|--------------|
| **Incident Type** | Type of reported incident (*border rejection* or *alert*). |
| **Specific Hazards** | Specific hazards associated with each incident. |
| **Hazard Subcategory** | Hierarchical hazard categorization, aligned with the **FOODAKAI Ontology**. |
| **Origins** | Country associated with the reported incident. |
| **Date** | Official date of the incident announcement. |

---

## Methodological Recommendations

When developing forecasting models using these datasets, the following practices are advised:

- Employ **monthly-level aggregation**, which tends to yield more stable and interpretable forecasts.  
- Integrate **external explanatory variables** (e.g., trade volumes, price indices, laboratory testing data, weather indicators) to enhance predictive accuracy.  
- Select **forecasting or regression algorithms** that exhibit robustness to noise, given the inherent variability in incident reporting.  
- Apply **feature engineering** techniques to capture temporal dynamics such as trends, seasonality, and lagged effects.  
- Evaluate model performance using established error metrics, including:  
  - **MAE** – Mean Absolute Error  
  - **MSE** – Mean Squared Error  
  - **RMSE** – Root Mean Squared Error  
  - **SMAPE** – Symmetric Mean Absolute Percentage Error  

---

## Citation

If you use these datasets in academic work, please cite **Agroknow** and the **FOODAKAI platform** as the original data providers.

---

## License and Data Usage

These datasets are provided for **research and educational purposes only**.  
For commercial applications or redistribution, please contact **Agroknow** for licensing and usage permissions.
