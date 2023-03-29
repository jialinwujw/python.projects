# About The Analysis
Utilize market basket analysis to identify customer purchase patterns to increase sales. 
<br>
Its primary objective is to identify products and categories that are more likely to be purchased together.

## Project
### Data
https://www.kaggle.com/sulmansarwar/transactions-from-a-bakery

### Description
This dataset includes the transaction date, the transaction ID, and the items purchased. A single transaction ID may be associated with more than one observation since a single transaction can buy multiple items. Using these data, we can determine which items are most frequently purchased together, thus determining which basket sells the most. Companies can then utilize this information to offer attractive bundles with incentive pricing. Therefore, they will be able to increase sales and average order values.

### Python Packages
* pandas
* numpy
* matplotlib
* seaborn

```sh
import pandas as pd
import numpy as np
import warnings
warnings.filterwarnings('ignore')

import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns

from mlxtend.frequent_patterns import apriori, association_rules
```

### Outputs
**Support**
- Antecedent/Consequent Support refers to the default popularity of an item and can be calculated by finding number of transactions containing a particular item divided by total number of transactions. Suppose we want to find support for item A: Support(A) = Transactions Containing A / Total Transactions
- Support measures the proportion of transactions that contain both items in a rule. A high support value indicates that the items in the rule are frequently purchased together.


**Confidence**
- Confidence refers to the likelihood that an Consequent item is also bought if Antecedent item is bought. It can be calculated by finding the number of transactions where Antecedent and Consequent are bought together, divided by total number of transactions where Antecedent is bought.
- Confidence (Antecedent -> Consequent) = Transactions Containing both Antecedent and Consequent / Transactions Containing Antecedent
- A high confidence value indicates that when the Antecedent item(s) are purchased, the likelihood of also purchasing the Consequent item(s) is high.

**Lift**
- Lift measures the degree of association between the Antecedent and Consequent items, relative to what would be expected if the items were purchased independently. In other words, Lift (Antecedent -> Consequent) refers to the increase in the ratio of sale of Consequent item(s) when Antecedent item(s) is sold.
- Lift (Antecedent -> Consequent) = Confidence (Antecedent -> Consequent) / Support (Consequent)
- The likelihood of buying Antecedent item(s) and Consequent item(s) together is Lift (Antecedent -> Consequent) times more than the likelihood of just buying Consequent item(s).
- A Lift of 1 means there is no association between Antecedent and Consequent items. Lift of greater than 1 means products Antecedent item(s) and Consequent item(s) are more likely to be bought together. Finally, Lift of less than 1 refers to the case where two products are unlikely to be bought together.
