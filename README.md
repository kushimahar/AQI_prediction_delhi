# AQI Prediction
## Introduction
The Air Quality Index (AQI) stands as a pivotal metric that gauges the quality of air, serving as a critical indicator of environmental health and public welfare. In India, particularly during festive seasons, such as Diwali, a notable surge in pollution levels has been witnessed, significantly impacting air quality. The confluence of various factors, including increased vehicular emissions, crop residue burning, and fireworks during celebrations, escalates the pollution levels, exacerbating the already pressing issue of air pollution[3].

This project delves into the crucial task of predicting AQI during the festive seasons in Delhi, India. Focusing on the period from November to January, encompassing celebrations like Diwali, the study aims to comprehend and forecast the patterns of air quality fluctuations, particularly emphasizing the three primary monitoring stations in Delhi: Anand Vihar, Punjabi Bagh, and Mundka[3]. These locations have consistently recorded some of the highest AQI levels during these festive periods.

## Data Collection
The data for this analysis was sourced meticulously from the Central Pollution Control Board's official portal [1][2], spanning across three successive years: 2020-2021, 2021-2022, and 2022-2023. The datasets extracted cover the critical months of November to January, encapsulating the festive periods renowned for their heightened pollution levels.

The chosen datasets encompass diverse parameters, including PM2.5, PM10, NO2, SO2, NH3, CO, Ozone, and AQI, crucial in evaluating air quality. Specifically targeting these periods enabled a comprehensive analysis of the AQI trends during these festival-laden months.

## AQI Calculation and Prediction
Now that our dataset for the three cities is clean, we perform the following machine learning models on them to analyse and predict the AQI for future:
1. Linear Regression
2. Support Vector Regression
3. Random Forest
4. XG Boost

The class distribution is checked and balanced using SMOTE.
### SMOTE (Synthetic Minority Over-sampling Technique):
It is a resampling technique that addresses class imbalance by generating synthetic samples from the minority class, thereby balancing the distribution of classes in the dataset. It works by creating synthetic instances along the line segments joining k minority class nearest neighbors, effectively increasing the representation of the minority class without duplicating existing instances.

## Results and Findings:
Overall, the predicted AQI values seem to be decreasing over time. This suggests that the air quality in these areas is generally improving over the specified period.
Anand Vihar, Punjabi Bagh, and Mundka show varying trends over time.
Anand Vihar's AQI values consistently decrease, indicating better air quality compared to Punjabi Bagh and Mundka.
Punjabi Bagh and Mundka exhibit a fluctuating pattern, indicating less stable air quality compared to Anand Vihar.
### Maximum AQI:
Anand Vihar: 397 Very Poor
Punjabi Bhag: 468 Very Poor
Mundka: 504 Severe

## Conclusion:
This project addressed the challenge of imbalanced datasets through the application of SMOTE, enhancing the model's ability to learn from underrepresented data. By implementing XGBoost, Random Forest, Support Vector Regression, and Linear Regression models, we identified XGBoost as the optimal choice due to its lowest RMSE and highest R^2 value. This model not only showcased superior performance but also highlighted the importance of proper handling of imbalanced data. Through SMOTE, we effectively balanced the dataset, enabling more accurate predictions and emphasizing the significance of addressing class imbalance in machine learning applications
The variability in AQI values between the areas indicates a need for more precise air quality monitoring and data-driven policies to maintain air quality standards.

## Reference
1. Central Pollution Control Board (CPCB) /CCR [http://app.cpcbccr.com/ccr/]
2. Data Contributions are acknowledged to (as given on CPCB), DPCC, Haryana State, RSPCB, SAFAR, UPPCB
3. Delhi, NCR Air Pollution LIVE Updates: Delhi air severe due to construction, agricultural waste, says expert, by mint [https://www.livemint.com/news/india/delhi-air-pollution-live-updates-aqi-severe-thick-smog-ncr-air-quality-mumbai-worsen-schools-closed-11698973435338.html]
​
