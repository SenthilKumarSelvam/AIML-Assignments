# Bike Sharing Assignment
> Predicting Demand for Shared Bikes Using Multiple Linear Regression as per the given problem statement and business goal.
# Table of Contents
* [General Info](#General-information)
* [Technologies Used](#Technologies-used)
* [Overview of Jupyter project](#Project-File-Overview)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information:
This project involves developing a linear regression model using Python to predict and understand the demand for shared bikes offered by BoomBikes, a US-based bike-sharing provider. The project is centered around analyzing various factors that influence bike demand to assist BoomBikes in making informed business decisions post-COVID-19.

Using Python, the project involves data exploration, preprocessing, and the development of a multiple linear regression model. The model is designed to identify significant variables that impact bike demand, providing BoomBikes with actionable insights to tailor their services to market needs. The ultimate goal is to help the company make data-driven decisions to not only survive but thrive in the competitive bike-sharing market as it emerges from the pandemic's shadow.

## Background:
BoomBikes, like many other businesses, has suffered considerable revenue losses due to the COVID-19 pandemic. As lockdown restrictions begin to ease and the economy starts to recover, BoomBikes is eager to reposition itself in the market by understanding the dynamics of bike demand. 

Bike-sharing systems typically allow users to borrow bikes from one location and return them to another, often through a computerized docking system. To prepare for the anticipated changes in demand patterns, BoomBikes needs insights into what drives the demand for shared bikes.

## Business probem that trying to solve:

## Business Goal: 
The primary business challenge for BoomBikes is to identify and understand the factors that significantly influence the demand for shared bikes in the post-pandemic market. This understanding is crucial for developing strategies that can help the company recover and grow its revenue. The goal is to pinpoint which variables are most predictive of bike demand and how they interact with each other to influence customer behavior.

## The Project Solution:
My project is focused on addressing the primary business challenge for BoomBikes: identifying and understanding the factors that significantly influence the demand for shared bikes in the post-pandemic market. This understanding is crucial for developing strategies that can help the company recover and grow its revenue. The goal of the project is to pinpoint which variables are most predictive of bike demand and to understand how these variables interact with each other to influence customer behavior. By achieving this, the project aims to provide BoomBikes with actionable insights that will enable them to adapt their business strategies, optimize operations, and ultimately regain market share in a competitive landscape.

## Dataset Used
The dataset at the core of this project includes daily records of bike demand in various American cities, coupled with data on influencing factors such as weather conditions, seasonal trends, and social behaviors. By leveraging this data, the project aims to build a robust linear regression model that can predict bike demand based on these independent variables. 
.
This model will enable BoomBikes to:
        Forecast future bike demand based on identified trends and factors.
        Adapt their business strategies to align with predicted demand.
        Enhance operational efficiency by optimizing bike availability across locations.

## Technologies Used: 
## Python: 
Primary language for data analysis and model development.
## Jupyter Notebook (Version 4.0.11): 
Provides an interactive environment for coding and documentation.
## NumPy (version 1.26.4): 
Handles numerical computations and array operations.
## Pandas (version 2.2.2): 
Manages data manipulation and analysis tasks.
## Matplotlib & Seaborn (version 0.13.2): 
Creates visualizations for data exploration.
## Statsmodels (version 0.14.2): 
Performs statistical modeling and regression analysis.
## Scikit-learn (version 1.4.2): 
Builds and evaluates the linear regression model.
## SciPy (version 1.13.1): 
Conducts residual analysis and statistical tests.

## Project file-Overview
## Data Understanding:
## ABOUT DATASET
Column = 16 Variables and Rows = 730 as variable data.
## ABOUT DATASET VARIABLES 
instant, dteday, season, yr, mnth, holiday, weekday, workingday, weathersit, temp, atemp, hum, windspeed, casual, registered, cnt

Out of that 7 are Catagorical variables: season, yr, mnth, holiday, weekday, workingday, weathersit 

Out of that 7 are Numerical variables: temp, atemp, hum, windspeed, casual, registered, cnt 

Out of that 2 are non-value added variables: instant, dteday 

## ABOUT PAIRPLOT Understanding:
temp vs. atemp:

Observation: The variables temp and atemp appear to be the most correlated.

Reference: This correlation is evident in both the scatter plot located in row 1, column 2 and its mirror plot in row 2, column 1.

Understanding: Highly correlated.

registered vs. cnt:

Observation: The variables registered and cnt are highly correlated.

Reference: This is visible in the plots located in row 6, column 7 and row 7, column 6.

Understanding: Highly correlated.

casual vs. cnt:

Observation: A notable correlation exists between casual and cnt.

Reference: This is observed in the scatter plots found in row 5, column 7 and row 7, column 5.

Understanding: Correlated.

casual vs. registered:

Observation: There is a visible correlation between casual and registered.

Reference: This can be seen in the plots in row 5, column 6 and row 6, column 5.

Understanding: Correlated.ding**: correlated correlated with total counts.

## ABOUT HEATMAP Understanding:
temp vs. atemp:

Correlation Coefficient: 0.99

Understanding: These variables are almost perfectly corr.temp`.

registered vs. cnt:

Correlation Coefficient: 0.95

UnderstThese variables areThere is a very strong positive c,and cnt, indicating that the number of registered users is a major contributor to the tot (cnt) of users.

casual vs. cnt:

Correlation Coefficient: 0.67

UndThese variables are: There is a moderately strong positiualandcnt`, meaning that casual users also contribute significantly to the total count, though not as much as registered users.

temp vs. cnt:

Correlation Coefficient: 0.63

These variables areding*: There is a moderate po, temp and cnt, indicating that higher temperatures generally lead to an increase in the total number of users.

casual vs. registered:

Correlation Coefficient: 0.39

These variables arestanding**: There is a weak to moderansualandregistered`, which may suggest that days with more casual users tend to have more registered users as well, but the relationship is not as strong.

workingday vs. casual:

Correlation Coefficient: -0.52These variables arenderstanding**: There is a mod workingday and casual, indicating that there are fewer ca.e on weekends or holidays.

temp vs. season:

Correlation Coefficient: These variables are Understanding: There ion between temp and season, which is expected as temperature varies significantly with seasons.

hum vs. weathersit:

**Correlation CoefficientThese variables are - **Understandid weathersit (weather situation), suggesting that worse weather conditions tend to be more humid.

## General Insights:

## High Correlations: temp vs. atemp, registered vs. cnt, and temp vs. season show the strongest positive correlations, indicating closely related variables.

## Moderate Correlations: casual vs. cnt and hum vs. weathersit show moderate correlations, providing insights into user behavior patterns and weather influence.

## Negative Correlations: The correlation between workingday and casual is negative, indicating that ronmental factors on bike-sharing usage.


## Conclusions

## Observation and Conclusion of Model 1 

OLS Regression Results Summary

Model Fit:

R-squared: 0.847 (84.7% of variance in cnt explained)

Adjusted R-squared: 0.843 (Good fit, adjusted for predictors)

F-statistic: 195.7 (Model is statistically significant, p < 0.0001)

Key Predictors:

temp: 0.5277 (Positive effect on cnt)

hum: -0.1611 (Negative effect on cnt)

windspeed: -0.1809 (Negative effect on cnt)

season_spring: -0.0555 (Decrease in cnt compared to base season)

season_winter: 0.0992 (Increase in cnt compared to base season)

Residuals: Not perfectly normal (Omnibus and Jarque-Bera tests significant)

Condition Number: 25.2 (Mild multicollinearity)

VIF Results Summary

High VIF Values (VIF > 10): Indicate severe multicollinearity. Consider removing or combining these features.

hum - 32.10

temp - 18.99

Moderate VIF Values (5 ≤ VIF < 10): Indicate some multicollinearity. Review their impact but might be manageable.

workingday - 5.28

windspeed - 4.91

weekday_Sat - 4.91

season_spring - 4.80

weekday_Sun - 4.76

Low VIF Values (VIF < 5): Indicate low multicollinearity and are generally safe to include in the model.

season_winter - 3.69

season_summer - 3.04

weathersit_mist - 2.31

yr - 2.09

mnth_Jul - 1.60

mnth_Sep - 1.38

weathersit_snow - 1.25

## The model is effective but may need refinement due to some issues with residual normality.

## Observation and Conclusion of Model 2

OLS Regression Results Summary

Model Fit:

R-squared: 0.843 (84.3% of variance in cnt explained)

Adjusted R-squared: 0.839 (Good fit, adjusted for predictors)

F-statistic: 204.4 (Model is statistically significant, p < 0.0001)
Key Predictors:


temp: 0.5304 (Positive effect on cnt)

hum: -0.1697 (Negative effect on cnt)

windspeed: -0.1834 (Negative effect on cnt)

season_spring: -0.0564 (Decrease in cnt compared to base season)

season_winter: 0.0972 (Increase in cnt compared to base season)

weathersit_mist: -0.0532 (Decrease in cnt under misty conditions)

weathersit_snow: -0.2381 (Significant decrease in cnt under snowy conditions)

Residuals: Not perfectly normal (Omnibus and Jarque-Bera tests significant)

Condition Number: 19.6 (Indicating mild multicollinearity)

VIF Results Summary

High VIF Values (VIF > 10): Indicate severe multicollinearity. Consider removing or combining these features.

hum - 28.03

temp - 16.06

Moderate VIF Values (5 ≤ VIF < 10): Indicate some multicollinearity. Review their impact but might be manageable.

windspeed - 4.67

season_spring - 4.03

Low VIF Values (VIF < 5): Indicate low multicollinearity and are generally safe to include in the model.

season_winter - 3.35

season_summer - 2.79

weathersit_mist - 2.28

yr - 2.08

mnth_Jul - 1.58

mnth_Sep - 1.39

weathersit_snow - 1.24

weekday_Sat - 1.19

holiday - 1.05

## Model 2 demonstrates a strong fit, but there are concerns with multicollinearity, particularly for `hum` and `temp`.

## Observation and Conclusion of Model 3

OLS Regression Results Summary

Model Fit:

R-squared: 0.836 (83.6% of variance in cnt explained)

Adjusted R-squared: 0.832 (Good fit, adjusted for predictors)

F-statistic: 211.6 (Model is statistically significant, p < 0.0001)

Key Predictors:

temp: 0.4924 (Positive effect on cnt)

windspeed: -0.1500 (Negative effect on cnt)

season_spring: -0.0670 (Decrease in cnt compared to base season)

season_winter: 0.0816 (Increase in cnt compared to base season)

weathersit_mist: -0.0803 (Decrease in cnt under misty conditions)

weathersit_snow: -0.2846 (Significant decrease in cnt under snowy conditions)

Residuals: Not perfectly normal (Omnibus and Jarque-Bera tests significant)

Condition Number: 17.4 (Indicating low multicollinearity)

VIF Results Summary

Moderate VIF Values (5 ≤ VIF < 10): Indicate some multicollinearity. Review their impact but might be manageable.

temp - 5.12

Low VIF Values (VIF < 5): Indicate low multicollinearity and are generally safe to include in the model.

windspeed - 4.62

season_summer - 2.23

season_spring - 2.10

yr - 2.07

season_winter - 1.79

mnth_Jul - 1.58

weathersit_mist - 1.55

mnth_Sep - 1.34

weekday_Sat - 1.19

weathersit_snow - 1.08

holiday - 1.05

## Model 3 is robust with low multicollinearity, but the normality of residuals remains a concern.

## Observation and Conclusion of Model 4

OLS Regression Results Summary

Model Fit:

R-squared: 0.833 (83.3% of variance in cnt explained)

Adjusted R-squared: 0.829 (Good fit, adjusted for predictors)

F-statistic: 226.1 (Model is statistically significant, p < 0.0001)

Key Predictors:

temp: 0.4509 (Positive effect on cnt)

windspeed: -0.1415 (Negative effect on cnt)

season_spring: -0.1124 (Significant decrease in cnt compared to base season)

season_winter: 0.0445 (Increase in cnt compared to base season)

weathersit_mist: -0.0797 (Decrease in cnt under misty conditions)

weathersit_snow: -0.2859 (Significant decrease in cnt under snowy conditions)

Residuals: Not perfectly normal (Omnibus and Jarque-Bera tests significant)

Condition Number: 14.1 (Indicating low multicollinearity)

VIF Results Summary

Moderate VIF Values (5 ≤ VIF < 10): Indicate some multicollinearity. Review their impact but might be manageable.

None

Low VIF Values (VIF < 5): Indicate low multicollinearity and are generally safe to include in the model.

temp - 4.64

windspeed - 4.03

yr - 2.06

season_spring - 1.66

weathersit_mist - 1.52

season_winter - 1.40

mnth_Jul - 1.35

mnth_Sep - 1.20

weekday_Sat - 1.19

weathersit_snow - 1.08

holiday - 1.05

## Model 4 has a good fit with low multicollinearity but shows issues with residual normality.

## Observation and Conclusion of Model 5

OLS Regression Results Summary

Model Fit:

R-squared: 0.832 (83.2% of variance in cnt explained)

Adjusted R-squared: 0.829 (Good fit, adjusted for predictors)

F-statistic: 247.5 (Model is statistically significant, p < 0.0001)

Key Predictors:

temp: 0.4498 (Positive effect on cnt)

windspeed: -0.1395 (Negative effect on cnt)

season_spring: -0.1123 (Decrease in cnt compared to base season)

season_winter: 0.0449 (Increase in cnt compared to base season)

weathersit_mist: -0.0796 (Decrease in cnt under misty conditions)

weathersit_snow: -0.2855 (Significant decrease in cnt under snowy conditions)

Residuals: Not perfectly normal (Omnibus and Jarque-Bera tests significant)

Condition Number: 14.0 (Indicating low multicollinearity)

VIF Results Summary

Moderate VIF Values (5 ≤ VIF < 10): Indicate some multicollinearity. Review their impact but might be manageable.

None

Low VIF Values (VIF < 5): Indicate low multicollinearity and are generally safe to include in the model.

temp - 4.61

windspeed - 4.00

yr - 2.06

season_spring - 1.64

weathersit_mist - 1.52

season_winter - 1.39

mnth_Jul - 1.35

mnth_Sep - 1.20

weathersit_snow - 1.08

holiday - 1.04

## Model 5 is the VIFs and p-values both are within an acceptable range. So we go ahead and make our predictions using this model only.


## Conclusions from Q-Q Plot

Normality Check: Residuals are generally close to normal, as most points align with the red line.
.
Central Alignment: Residuals near the center are well-distributed.

Tail Deviation: Residuals in the tails deviate from the line, indicating potential outliers or non-normality.

Conclusion: Residuals are approximately normal with slight issues at the extremes.

## Final Conclusion:

We can see that the equation of our best fitted line is:

cnt = 0.2531 + 0.2342 * yr - 0.0980 * holiday + 0.4498 * temp - 0.1395 * windspeed - 0.1123 * season_spring + 0.0449 * season_winter - 0.0729 * mnth_Jul + 0.0573 * mnth_Sep - 0.0796 * weathersit_mist - 0.2855 * weathersit_sow

        Model Performance Metrics	Train Set	Test Set
0	R-Squared Value	                0.83200	        0.7940
1	Adjusted R-Squared Value	0.82900	        0.7829
2	RMSE	                        0.09183	         0.1082

## From the derived model, the following predictors are statistically significant. Therefore, the company should consider these predictor variables while preparing the bike rental strategy:

yr

holiday

temp

windspeed

season_spring

season_winter

mnth_Jul

mnth_Sep

weathersit_mist

weathersit_snow
