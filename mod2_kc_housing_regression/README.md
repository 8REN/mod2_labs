# Buy and Selling Homes in King County

  
  ## mulitple regression on King County Housing Dataset
  
  
 Author: Brennan Mathis
 
 The contents of this repository contain a detailed analysis of the provided King County Washington dataset. (kc_house_data.csv)
 
 ### Problem:
 
 Does the size of the home affect price? (such as bedrooms, square foot living)
 Does the distance from the nearest major city affect price?
 Does the age of the home affect the grade/condition of the home, therefore affecting price? Historic homes?
 What variables affect price overall, and use to predict price
 
### Libraries
from geopy.distance import geodesic
from geopy import Point
import numpy as np 
import pandas as pd 
import seaborn as sns 
import matplotlib.pyplot as plt
import scipy.stats as stats
import statsmodels.api as sm
import statsmodels.formula.api as smf
import statsmodels.stats.api as sms
from statsmodels.formula.api import ols
from statsmodels.stats import diagnostic
from sklearn.feature_selection import RFE
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
from sklearn.model_selection import cross_val_score
from sklearn import svm
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score
from sklearn.model_selection import KFold

## Simple Linear Regression perfomed on individual variables

## Multiple Regression performed on :
### 'price', 'bedrooms', 'bathrooms', 'condition', 'grade', 'age', 'sqm_living', 'sqm_living15', 'sqm_lot',  and 'distance_seattle'
### 'price', 'condition', 'grade', 'age'

 ![age/gradeboxplot](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_age_grade_boxplot.png)
 
 ![age/pricescatter](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_ageprice_scatter.png)
 
 ![violinplot1](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_bedvsprice_violin.png)
 
 ![violinplot2](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_gradevsprice_violin.png)
 
 ![lot/pricekde](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_lotsizeprice_kde.png)
 
![lot/pricekde](https://github.com/br3nnan8/mod2_kc_housing_regression/blob/master/visualizations/kc_renovatedvsnonrenovated_kde.png)
 
 To expand on this project, I would like to assess scaling the continuous data and providing more weight to certain variables in the model. Additional regressions with polynomials as well.
 
 
