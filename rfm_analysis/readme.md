# About The Analysis
Utilize RFM analysis to assess the value of customers and their ability to create value. Customers' value can be determined by looking at three indicators: their recent purchasing behavior, their overall purchasing frequency, and the amount of money they spend.


## Project
### Data
https://www.kaggle.com/datasets/kyanyoga/sample-sales-data

### Descirption
This database contains transactional information pertaining to sales, orders, customers, and shipping. To perform RFM analysis, only four metrics were extracted: Customer Name, Order Number, Order Date, and Sales.

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

import warnings
warnings.filterwarnings('ignore')
```

### Outputs
Customer Segmentation based on RFM Score (R, F, M Tier Concentration)

| Segmentation | RFM Score |
| ------------- |:-------------:|
| Soulmate | 111 |
| Lover | 222 |
| Potential Lover | 223 |
| New Passion | 13X, 23X |
| About to Dump You | 334 |
| Ex Lover | 411 |
| Departed | 43X, 44X |

The code file outlines the specific marketing strategies for each segmentation. 
<br><br>
*Take **Soulmate** segment as an example. They are the most valuable customers who purchased the most recently, buy the most frequently, and spend the highest money. The priority should be paid to this group of customers and the satisfaction of these customers should be improved in order to increase customer retention. VIP services and personalized services can be provided to enhance the user experience.*
