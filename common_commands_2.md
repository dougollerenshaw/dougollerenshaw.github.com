# Common Python/Jupyter commands
## Doug Ollerenshaw
d.ollerenshaw@gmail.com

Below is a collection of common Python/Jupyter commands that I find myself continually searching for. I’m putting them here so I can have an easy single reference

## Standard Imports
```pythton
import numpy as np
import pandas as pd
import os
import matplotlib.pyplot as plt

%matplotlib notebook
```

## Make Jupyter full screen width
```python
from IPython.core.display import display, HTML
display(HTML("<style>.container { width:100% !important; }</style>"))
```

## Force Jupyter to automatically reload modules when source code is changed

```python
%load_ext autoreload
%autoreload 2
```

## Control Pandas display properties

```python
import pandas as pd
pd.set_option('display.max_rows', 500)
pd.set_option('display.max_columns', 500)
pd.set_option('display.width', 1000)
```

## Make conda environments visible in Jupyter dropdown menu

```python
conda activate myenv
pip install ipykernel
python -m ipykernel install --user --name myenv
```

## Upload to pypi

```python
python setup.py sdist
twine upload dist/*
```
