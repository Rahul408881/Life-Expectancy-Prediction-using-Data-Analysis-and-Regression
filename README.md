# 🌍 Life Expectancy Prediction Using Machine Learning



This project explores the prediction of **life expectancy** across 193 countries (2000–2015) using  
statistical and machine learning models. The work focuses on data preprocessing, regression  
techniques, and model evaluation to identify the most effective approach for predicting global  
health outcomes.

<img width="1536" height="1024" alt="led" src="https://github.com/user-attachments/assets/737e5813-a3e3-47ad-bbf6-70860fd13e75" />



## 📂 Repository Structure  
- `life_expectancy_analysis.Rmd` → R Markdown file with narrative, plots, and analysis.  
- `Report.pdf` → Final report with methodology, results, and discussions.  

---

## 🧪 Methodology
- **Data Source**: WHO Global Health Observatory & UN datasets (193 countries, 2000–2015).  
- **Preprocessing**:  
  - Null value removal & imputation.  
  - Outlier detection (Boxplots, Z-score, IQR).  
  - Correlation & multicollinearity checks.  
- **Models Tested**:  
  - Linear Regression  
  - Ridge Regression  
  - Lasso Regression  
  - Elastic Net Regression  

---

## 📊 Results
| Model              | MAE   | RMSE  | R² (Adj) |
|--------------------|-------|-------|----------|
| Linear Regression  | 1.40  | 2.29  | 0.745    |
| Lasso Regression   | 1.60  | 2.29  | ~0.74    |
| Ridge Regression   | 5.00  | 7.07  | Lower    |
| **Elastic Net**    | **0.50** | **0.71** | **0.82** |

- **Elastic Net Regression** emerged as the best model, achieving the lowest MAE and RMSE:contentReference[oaicite:1]{index=1}.  
- Key influential predictors: **Adult Mortality, Infant Deaths, Schooling, HIV/AIDS, Healthcare Expenditure, BMI, Polio/Diphtheria Immunization**.  

---

## 🖼️ Visualizations
Example plots generated in the `.Rmd` notebook:  
- 📈 Correlation heatmap of health and economic indicators.  
- 📊 Boxplots for outlier detection across mortality and immunization variables.  
- 📉 Residual & QQ plots for regression diagnostics.  
- 🔍 Model comparison charts (MAE/RMSE across models).  
