# Bike Sharing Assignment

## **Problem Statement**

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands <br>

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

**Business Goal**:

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Recommendations](#recommendations)
- [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**Issues to Address:**

1. **Revenue Decline:** BoomBikes faces substantial revenue declines due to the ongoing pandemic, necessitating a strategic solution.
2. **Market Sustainability:** The company struggles to sustain itself in the current market scenario, demanding a mindful business plan.
3. **Post-Lockdown Strategy:** BoomBikes aims to accelerate revenue post-lockdown, requiring an understanding of post-quarantine bike demand.

**Objectives:**
The objectives include predicting significant variables influencing American market shared bike demand, determining the crucial predictors, developing a model to understand demand variations, facilitating adaptive business strategies, and exploring demand dynamics for effective decision-making. This case study aims to achieve this goal by building a multivariate linear regression model using the provided [dataset](./day.csv).

The primary objective is to identify the key variables that significantly influence the prediction of shared bike demand and assess how effectively these variables describe the patterns in bike demands.

## Conclusions

- The equation of the best fit line is given by:
  **_cnt_** = 0.2429 + (0.2397× **_Year_**) − (0.0851× **_Holiday Indicator_**)+(0.4612 × **_Temperature_**)−(0.1687× **_Windspeed_**)−(0.0767 × **_July Indicator_**)+(0.0468 × **_September Indicator_**)−(0.1064 × **_Spring Indicator_**)+(0.0351 × **_Winter Indicator_**)−(0.0677 × **_Mist/Cloudy Indicator_**)

- Bike demand is influenced by features such as **yr**, **holiday**, **temp**, **windspeed**, **July**, **September**, **Spring**, **Winter**, and **Mist/Cloudy**.
- Three key feature variables, **temp**, and **yr** exhibit the highest coefficient values, indicating their significant impact.

## Recommendations

- **Leverage High-Impact Features:** Focus on features such as **temp**, and **yr** as they exhibit the highest coefficient values, indicating significant impact on bike demand.

- **Seasonal Strategies:** Develop targeted marketing and pricing strategies for different seasons, particularly emphasizing promotions during **Spring** and **Winter**.

- **Optimize Operational Planning:** Adjust bike availability and distribution based on the significant features identified, optimizing resources for peak demand periods.

- **Weather-Sensitive Promotions:** Implement weather-specific promotions or incentives to encourage bike usage during favorable weather conditions, addressing the impact of **temp* and **windspeed**.

- **New Market Insights:** Use the developed model to gain insights into demand dynamics in the American market, informing business strategies and positioning BoomBikes competitively.

- **Continuous Monitoring and Adaptation:** Regularly update the model with new data and adapt strategies based on evolving market conditions to ensure sustained revenue growth.

## Technologies Used and imported

- calendar
- numpy 
- pandas 
- matplotlib.pyplot 
- seaborn 
- train_test_split from sklearn.model_selection
- MinMaxScaler from sklearn.preprocessing 
- RFE from sklearn.feature_selection
- LinearRegression from sklearn.linear_model 
- statsmodels.api 
- variance_inflation_factor from statsmodels.stats.outliers_influence
- r2_score from sklearn.metrics

## Contact

Created by [@Kartikey Kunal](https://github.com/kunal-kartik919)
