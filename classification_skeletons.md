## _Top Imports_
```python
	
import numpy as np
import seaborn as sns
import scipy.stats as stats
import pandas as pd
import matplotlib.pyplot as plt
from pydataset import data

import os
import env as env
import acquire as acq
	
```
## _Pandas - Fill Blanks_

```python

iris_df.isna().sum()
df['column'].fillna('killer_filler',inplace=True)

```
## _Pandas - Drop Columns_

```python

to_drop = ['species_id', 'measurement_id']
iris_df.drop(columns=to_drop,inplace=True)

```
## _Data Preparation_
```python
	
	df = clean_data(df)
	
	train_validate, test = train_test_split(df, test_size=.2, random_state=123, stratify=df.survived)
	train, validate = train_test_split(train_validate, 
                                       test_size=.3, 
                                       random_state=123, 
                                       stratify=train_validate.survived)
	return train, validate, test
```