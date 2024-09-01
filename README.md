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
ABOUT DATASET
Column = 16 Variables and Rows = 730 as variable data.
ABOUT DATASET VARIABLES
instant, dteday, season, yr, mnth, holiday, weekday, workingday, weathersit, temp, atemp, hum, windspeed, casual, registered, cnt
Out of that 7 are Catagorical variables: season, yr, mnth, holiday, weekday, workingday, weathersit 
Out of that 7 are Numerical variables: temp, atemp, hum, windspeed, casual, registered, cnt 
Out of that 2 are non-value added variables: instant, dteday 

ABOUT PAIRPLOT Understanding


## Conclusions
