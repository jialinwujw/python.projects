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

### Outputs
The **Feature Selection** function was used to identify the six factors that had the greatest influence on the results. In order to better predict customer behavior, two methods were employed. <br><br>
In this study, multiple **Logistic Regression** models were used to predict the outcome of the event (whether or not it would churn). Consider the situation where multiple models suggested churn, but client status remained active. In this case, the customer was at risk of churn, and the company should take steps to retain them. <br><br>
Another solution would be to classify customers based on **Cluster Analysis**. This process was carried out to determine which group had the greatest percentage of churning clients, and then to target the active clients in that group.
