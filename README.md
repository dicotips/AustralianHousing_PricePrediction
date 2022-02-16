# Australian Housing Price Prediction - Advanced Regression

## Table of Contents

* [Introduction](#Introduction)
* [Methods Used](#Method-Used)
* [Download and Setup](#Download-and-Setup)
* [Problem Statement](#Problem-Statement)
* [Business Goal](#Business-Goal)
* [Data Preparation](#Data-Preparation)
* [Model Building and Evaluation](#Model-Building-and-Evaluation)
* [Conclusions](#Conclusions)

## Introduction 

In this programming assignment I built regression models to predict the Australian Housing Price market.

This repository contains the following files required by the assignment:

* Jupyter Notebook file with the Data Preparation and Model Building to predict the housing price in the Australian Market.
* PDF File with answers to the Subjective Questions.

### Methods Used
* Data Preparation
* Model Building

### Technologies
* Python
* Pandas
* Numpy
* Seaborn & matplotlib
* Statsmodels
* SkitLearn
* Jupyter Notebooks

## Download and Setup
### Prerequisites

This project needs Anaconda installed in the computer.

For more details about the instalation, go to:  https://docs.anaconda.com/anaconda/install/index.html
### How to Run

You can download the source code cloning this repository using Git:

1. Open your favorite Terminal app (Unix, Linux or Macos), such as Terminal, Command, Console, iTerm2, so on.

2. Clone the repository

```
git clone https://github.com/dicotips/AustralianHousing_PricePrediction.git
```

3. Open the ** *.ipynb** notebook file in Anaconda.

```
jupyter notebook AdvancedRegressionAssignment.ipynb
```

## Problem Statement

**Source:** UpGrad Assignment description

*A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.*

*The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.*

*The company wants to know:*

* Which variables are significant in predicting the price of a house, and
* How well those variables describe the price of a house.

*Also, determine the optimal value of lambda for ridge and lasso regression.*

### Business Goal

*You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.*

---

### Data Preparation:

1. Data Clearning and Missing Data Analysis.
2. Outlier Analysis & Treatment.
3. Deriving Categorical Columns.
4. Univariate Analysis.
5. Bivariate Analysis.
6. Multivariate Analysis.

### Model Building & Evaluation

1. Training and Test data split.
2. Feature Scaling - StandardScaler.
3. Feature Engineering & Selection using RFE and Variance Inflation factor.
4. Model preperation using OLS & Linear Regression.
5. Regularization Ridge & Lasso Regression Model.
6. Residual Analysis.
7. Model Evaluation & Assessment.
8. Prediction.
9. Final Conclusion & Analysis.

### Conclusions

R2_Score for Lasso regresion is slightly better than the others. All the models have similar R2_score.

#### Ridge Regression
* **Optimal Lambda Value:** 10
* **R2 Score Train:** 0.92
* **R2 Test Score:**  0.89
* **RMSE Test:**      0.13

#### Lasso Regression
* **Optimal Lambda Value:** 0.0002
* **R2 Score Train:**  0.93
* **R2 Test Score:**   0.89
* **RMSE Test:**       0.13

#### Most Significant Variables are:
* MSZoning
* Neighborhood
* GrLivArea
* Exterior1st