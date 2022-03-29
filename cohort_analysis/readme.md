# About The Analysis
Utilize cohort analysis to evaluate customer behavior throughout the customer lifecycle and uncover issues that are not readily apparent by using overall metrics (e.g., revenue, number of users), especially when marketing methods and activities are constantly changing.<br>
It will allow companies to take informed and timely decisions regarding churn reduction and revenue enhancement.

## Project
### Data
https://archive.ics.uci.edu/ml/datasets/Online+Retail+II

### Descirption
The database contains all transactional information collected from an online store in the United Kingdom from 2010 through 2011. A large portion of the company's customers is wholesalers.<br>
Cohort analysis for retention provides companies with information on how many customers remain active in the following days, weeks, or months. The cohort is based on the month in which a customer purchased his or her first product.

### Python Package
* pandas
* numpy
* matplotlib
* seaborn

```sh
import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns

from operator import attrgetter

import warnings
warnings.filterwarnings('ignore')
```

### Outputs
**Cohort Analysis of Retention Rate**
<br><br>
The quality of the customers acquired in December 2010 is superior to that of those acquired in subsequent months. In the month following their initial purchase, 38% of this group of customers repurchased products. This group of customers is also much more likely to repurchase in subsequent months than new customers in other months. Furthermore, 50% of these customers placed orders after 11 months.
<br><br>
**Cohort Analysis of Average Order Value**
<br><br>
In terms of AOV, the December 2010 customer's AOV stands out as well. AOVs for repurchases from new customers in August 2011 are also favorable. In general, the AOV is low for the second month's transactions, but it increases later.
