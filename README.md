# Business Goal
Estimate the Unit Sales of Walmart retail goods to support their strategic development, make tactical decisions, and manage their demand and supply planning processes in order to avoid customer service issues and high inventory costs.



# Analysis Plan
<img width="817" alt="截圖 2023-03-01 上午11 42 27" src="https://user-images.githubusercontent.com/102202557/222219640-27c68d7d-46c3-4242-9ebb-4c6688d61c37.png">

### Implemetn feature engineering
1. Sales related features, like lag sales for different time period, and rolling sales for different time period. This type of features reflect trend component. 
2. Price related features, like max, min standard deviation of prices for that product. 
3. Calendar related features. Different weekdays like Monday, Tuesday, Wednesday; different month like January, February and so on and so forth.

### Model Training
We will implement LightGBM via Python, and use different models for different weeks and 10 different models for different stores, so we will have 4 weeks* 10 stores = 40 models in total.

# Result
We successfully forescast sales of 28 days with less than 0.6 WRMSSE (Weighted Root Mean Squared Scaled Error).
