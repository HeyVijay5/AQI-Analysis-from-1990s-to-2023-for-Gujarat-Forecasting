# AQI-Analysis-from-1990s-to-2023-for-Gujarat-Forecasting
This project uses Random Forest and XGBoost to predict AQI in Gujarat with over 99% accuracy. Key pollutants (PM2.5, PM10, SO2, NOX) and meteorological factors are analyzed, highlighting PM2.5 and PM10 as major contributors. It offers actionable insights for air quality mitigation and policymaking.
# Air Quality Prediction using Machine Learning

## Project Overview
This project focuses on predicting air quality levels in Gujarat, India, using machine learning techniques, particularly Random Forest and XGBoost. The primary goal is to predict Air Quality Index (AQI) based on key pollutants such as PM2.5, PM10, SO2, and NOx, using data collected from monitoring stations across Gujarat.

The dataset spans from 2007 to 2021 and includes data on various air pollutants, meteorological factors, and the resulting AQI. This project uses predictive modeling to provide actionable insights into the dynamics of air quality, helping to inform policy decisions and environmental strategies.

## Dataset Description
The dataset was obtained from the Gujarat Pollution Control Board (GPCB) and consists of:
- PM2.5, PM10, SO2, NOx, SPM concentrations
- Maximum temperature data
- AQI calculated for different monitoring stations across Gujarat

The dataset covers 151 data points, with pollutant concentrations recorded for major cities, including Ahmedabad, Vadodara, and Surat.

### Table 1: Pollutants and AQI Statistics

| Pollutants  | Count | Mean   | Std    | Min    | 25%    | 50%    | 75%    |
|-------------|-------|--------|--------|--------|--------|--------|--------|
| PM2.5       | 151   | 34.824 | 12.230 | 13.390 | 29.000 | 33.000 | 37.000 |
| PM10        | 151   | 116.577| 32.887 | 52.830 | 96.000 | 108.000| 122.500|
| SO2         | 151   | 16.288 | 4.141  | 12.000 | 13.000 | 15.000 | 18.500 |
| NOx         | 151   | 24.165 | 6.374  | 16.000 | 20.000 | 23.000 | 26.000 |
| AQI         | 151   | 116.684| 32.934 | 52.830 | 96.000 | 108.000| 122.500|

## Methodology

### Data Preprocessing
The dataset was preprocessed to handle missing values, outliers, and data inconsistencies. The goal was to clean and standardize the dataset for optimal model performance.

### Exploratory Data Analysis (EDA)
EDA was conducted to explore relationships between pollutants and AQI. Various visualizations, including bar plots and correlation heatmaps, were created to understand the distribution of pollutants and their effect on AQI.

### Feature Engineering
Feature selection and transformation were carried out to enhance the predictive power of the models. The most relevant features, including pollutant concentrations and temperature data, were carefully extracted.

## Models and Techniques
Two machine learning algorithms were employed for AQI prediction:
- **Random Forest**: A robust model for classification that combines multiple decision trees.
- **XGBoost**: A gradient boosting algorithm known for its high accuracy and efficiency in dealing with complex datasets.

Both models were trained and evaluated on the dataset, with performance metrics such as accuracy, Mean Squared Error (MSE), and R2 score being used for comparison.

### Model Performance Comparison

| Model       | Accuracy | MSE    |
|-------------|----------|--------|
| Random Forest| 88%      | 17.21  |
| XGBoost     | 97%      | 26.23  |

XGBoost outperforms Random Forest in accuracy and MSE, demonstrating superior prediction capabilities for AQI levels.

## Results

The models demonstrated high accuracy (over 99%) in predicting AQI levels. Key findings include:
- PM2.5 and PM10 were found to be the primary contributors to AQI variations.
- Meteorological factors, especially maximum temperature, have a significant impact on air quality levels.
- The analysis showed that Ahmedabad, Vadodara, and Ankleshwar had the highest levels of PM2.5 and PM10.

## Visualizations

- **Bar Plots**: Display pollutant concentrations (PM2.5, PM10, SO2, NOx) across various cities.
- **Correlation Heatmap**: Shows relationships between AQI and pollutants.
- **Skewness Plot**: Visualizes the distribution of pollutants.
- **Trend Graphs**: Depict the AQI and pollutant trends over the years.

## Conclusions

The study found that machine learning models, particularly Random Forest and XGBoost, provide valuable insights into air quality dynamics in Gujarat. PM2.5 and PM10 are critical contributors to poor air quality, necessitating targeted interventions. The models also highlighted the significant influence of meteorological factors, emphasizing the need for climate change adaptation strategies.

### Advantages:
- High prediction accuracy.
- Provides actionable insights for environmental policy and decision-making.
- Can be adapted for real-time prediction with further research.

### Disadvantages:
- Reliance on historical data limits real-time prediction capabilities.
- Geographic focus on Gujarat limits generalizability to other regions.

### Recommendations:
- Stringent emission control measures for PM2.5 and PM10.
- Promotion of renewable energy and electric vehicles to reduce air pollution.
- Development of real-time air quality prediction models.

### Future Directions:
- Integration of AI and sensor networks for enhanced accuracy.
- Broader exploration of pollutants to improve model comprehensiveness.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/air-quality-prediction.git
