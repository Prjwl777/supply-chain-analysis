
# Case Study on Demand Forecasting and Wastage Prediction  

## Overview  
This repository contains the code and analysis for a case study conducted by **R Lalrinmawii and Prajwal Singh** from **Christ (Deemed to be University), Pune, Lavasa**. The study explores the application of machine learning techniques to optimize inventory management in a grocery store chain specializing in perishable goods.  

Key areas of focus include:  
- **Demand Forecasting**: Utilizing time series models to predict sales trends.  
- **Wastage Prediction**: Modeling stock wastage patterns to reduce losses.  
- **Anomaly Detection**: Identifying unusual stock levels for proactive inventory control.  
- **Impact Analysis**: Examining the relationship between temperature and sales.  

## Abstract  
The case study demonstrates how machine learning models can address critical challenges in managing perishable goods. Through demand forecasting using ARIMA, anomaly detection with Isolation Forest, and wastage prediction using logistic regression, the study provides actionable insights for inventory optimization.  

While ARIMA effectively forecasts demand trends for high-value customers, the wastage prediction model achieved high accuracy, raising concerns about overfitting. Temperature analysis revealed minimal correlation with sales, suggesting other influencing factors. Recommendations include refining predictive models, incorporating additional data features, and exploring advanced techniques to improve performance.  

## Table of Contents  
1. [Datasets](#datasets)  
2. [Methodology](#methodology)  
3. [Key Findings](#key-findings)  
4. [Usage](#usage)  
5. [Dependencies](#dependencies)  
6. [References](#references)  

---

## Datasets  
The analysis leverages three primary datasets:  
1. **Sales Data**: Includes timestamps, product details, quantities sold, and customer information.  
2. **Stock Level Data**: Contains stock percentages and timestamps for each product.  
3. **Temperature Data**: Consists of sensor-based temperature readings with timestamps.  

Preprocessing steps addressed missing values, standardized formats, and ensured coherence between datasets.  

---

## Methodology  
The case study followed a systematic approach:  

### 1. **Data Preprocessing**  
- Timestamps were standardized using `pd.to_datetime()`.  
- Missing values were handled, and data was cleaned for accuracy.  

### 2. **Exploratory Data Analysis (EDA)**  
- Time series plots revealed seasonal sales patterns.  
- Histograms highlighted inventory balance issues.  
- Correlation analysis explored the influence of temperature on sales.  

### 3. **Modeling and Evaluation**  
- **ARIMA** for demand forecasting.  
- **Isolation Forest** for anomaly detection in stock levels.  
- **Logistic Regression** for stock wastage prediction.  

---

## Key Findings  

### 1. Demand Forecasting  
- **ARIMA** captured sales trends effectively for high-value customers.  
- Variations in demand were analyzed across customer types and payment methods.  
- Insights revealed fluctuations based on customer behavior and external factors.  

### 2. Impact of Temperature on Sales  
- Minimal correlation was observed between temperature and sales.  
- Polynomial regression and heatmap analysis reinforced these findings.  

### 3. Anomaly Detection  
- **Isolation Forest** identified anomalies at extreme stock levels (0% and 100%).  
- Insights enabled better inventory control and reduced risks of overstocking or stockouts.  

### 4. Stock Wastage Prediction  
- Logistic regression achieved high accuracy but raised concerns about overfitting.  
- Analysis revealed that fruits and vegetables had the highest wastage, followed by other perishable items.  

---

## Usage  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/yourusername/demand-forecasting-wastage-prediction.git  
   cd demand-forecasting-wastage-prediction  
   ```  

2. Install dependencies (see [Dependencies](#dependencies)).  

3. Run preprocessing and modeling scripts:  
   ```bash  
   python preprocess_data.py  
   python model_training.py  
   ```  

4. Visualize results:  
   - Visualizations include time series plots, scatter plots, and heatmaps.  
   - Check the `visualizations/` folder for generated figures.  

---

## Dependencies  
Install the required Python packages using:  
```bash  
pip install -r requirements.txt  
```  

Key libraries used:  
- `pandas` for data manipulation.  
- `numpy` for numerical computations.  
- `matplotlib` and `seaborn` for data visualization.  
- `statsmodels` for time series modeling (ARIMA).  
- `scikit-learn` for machine learning models (Isolation Forest, Logistic Regression).  

---

## References  
1. Hyndman, R. J., & Athanasopoulos, G. (2018). *Forecasting: Principles and Practice.* OTexts.  
2. Liu, F. T., Ting, K. M., & Zhou, Z. H. (2008). *Isolation forest.* *2008 Eighth IEEE International Conference on Data Mining.*  
3. Hosmer, D. W., Lemeshow, S., & Sturdivant, R. X. (2013). *Applied Logistic Regression.* John Wiley & Sons.  
4. Aggarwal, C. C. (2017). *Outlier Analysis.* Springer.  

---

## Contribution  
Contributions are welcome! Please fork the repository and create a pull request for enhancements or bug fixes.  

For questions, feel free to open an issue or contact the authors.  

---

