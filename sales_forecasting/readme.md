# About The Analysis
Utilize the sales forecast technique to estimate revenues for a period of time (such as a quarter or year).<br>
With a well-designed sales forecast, companies can devise more effective strategies to counteract risk and mitigate losses.

## Project
### Data
https://www.kaggle.com/manjeetsingh/retaildataset

### Descirption
The dataset consists of sales figures for multiple stores between 2010 and 2012. Furthermore, many other data points that may impact sales are gathered, such as store information, holiday seasons, and social indexes. First, we can determine the effects of various factors on sales through the data analysis model. In decision-making, we thus seek to maximize cost-effectiveness by increasing the weight of important factors and reducing the weight of less important ones. Lastly, we can create a better forecasting model based on historical information and highly relevant data to predict future sales.

### Python Package
* pandas
* numpy
* matplotlib
* seaborn
* sklearn
* statsmodels
* eli5

```sh
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns

# Linear Regression in SKLearn
from sklearn.model_selection import train_test_split 
from sklearn.linear_model import LinearRegression
from sklearn import metrics

# Calculate the Feature Importance
import eli5
from eli5.sklearn import PermutationImportance

# Linear Regression in Statsmodels
import statsmodels.api as sm
from scipy import stats

# Decision Tree
from sklearn.tree import DecisionTreeRegressor
from sklearn import tree

# Random Forest
from sklearn.ensemble import RandomForestRegressor

import warnings
warnings.filterwarnings('ignore')
```

### Outputs
* Linear Regression in SKLearn
* Linear Regression in Statsmodels
* Regression Tree in Decision Tree
* Regression Tree in Random Forest
<br>
Randomly allocated 80% of the data to the training set and 20% to the test set. Utilize the above four methods to model the sales forecasting based on the training set and then compare these models by the test set.
<br>
In sum, compared to linear regression, <strong>regression tree models</strong>, especially <strong>Random Forest</strong>, were better at forecasting sales. Yet, a further test should be performed to ensure that excessive <strong>overfitting</strong> has not occurred.
