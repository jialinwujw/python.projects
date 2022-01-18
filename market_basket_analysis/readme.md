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

import matplotlib.pyplot as plt
%matplotlib inline
import seaborn as sns
```

### Outputs
* **Product Sales**
  - The pandas.DataFrame.groupby function is used to count the total sales of each product, leading to the conclusion that *coffee* has the highest sales, followed by *bread*. 
* **Purchase Patterns**
  - By encoding, identify the basket of each transaction and then calculate the sales for each basket. This indicates an outstanding performance by *bread & coffee* basket.
