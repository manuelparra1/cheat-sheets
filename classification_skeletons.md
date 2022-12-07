## Top Imports
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