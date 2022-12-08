## _Top Imports_
```python
	
import numpy as np
import seaborn as sns
import scipy.stats as stats
import pandas as pd
import matplotlib.pyplot as plt
from pydataset import data

# pip install ipython
from IPython.display import display, Latex

#pip install quantum-random
import qrandom

import os
import env as env
import acquire as acq
	
```
### Avoid `Unnamed: 0` Column

#### Importing CSV
```python
pd.read_csv('file.csv',index_col=0)
```
#### Saving CSV
```python
pd.to_csv('file.csv,index=False)
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
## Drop Null Value
```python
	df.dropna()
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

## Display Latex
```python
	if p < alpha:
    display(Latex((f"Failed to reject $H_{0}$")))
```