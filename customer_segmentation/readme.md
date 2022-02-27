# About The Analysis
Utilize customer segmentation analysis to group a company's customers according to similar characteristics.<br>
Segmenting customers is crucial for maximizing each customer's value and optimizing marketing campaigns.

## Project
### Data
https://www.kaggle.com/blastchar/telco-customer-churn

### Description
The dataset includes some of the main attributes associated with each client, such as basic demographic information, customer account information, and consumption details. A total of 19 features are included. By analyzing this information, we are able to predict whether or not the company will lose customers or what customers will remain loyal to the company. Proactively forecasting enables companies to take prompt action to retain customers.

### Python Packages
* pandas
* numpy
* matplotlib
* seaborn
* sklearn
* xgboost
* catboost

```sh
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns

import warnings
warnings.filterwarnings('ignore') # Never print matching warnings

# Feature Selection
from sklearn.feature_selection import SelectKBest, chi2

# Logistic Regression
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score, confusion_matrix,precision_score,recall_score,roc_auc_score,f1_score,plot_confusion_matrix,plot_roc_curve,roc_curve
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.svm import SVC
from sklearn.neighbors import KNeighborsClassifier
from sklearn.ensemble import RandomForestClassifier
from xgboost import XGBClassifier
from catboost import CatBoostClassifier

# Clustering
from sklearn.preprocessing import MinMaxScaler
from sklearn.cluster import KMeans
from sklearn.metrics import silhouette_score
from sklearn.decomposition import PCA
```

### Outputs
The **Feature Selection** function was used to identify the six factors that had the greatest influence on the results. In order to better predict customer behavior, two methods were employed. <br><br>
In this study, multiple **Logistic Regression** models were used to predict the outcome of the event (whether or not it would churn). Consider the situation where multiple models suggested churn, but client status remained active. In this case, the customer was at risk of churn, and the company should take steps to retain them. <br><br>
Another solution would be to classify customers based on **Cluster Analysis**. This process was carried out to determine which group had the greatest percentage of churning clients, and then to target the active clients in that group.
