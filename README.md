# Forked from https://github.com/pistonly/modwtpy

Added a faster implementation of the base algorithm for only modwt

Potential future work:
- Improve all module in the library
- Submit commit to original repo and pywavelets

# modwtpy
modwt in python

find the detail from the matlab Documentation:
http://www.mathworks.com/help/wavelet/ref/modwt.html,
http://www.mathworks.com/help/wavelet/ref/modwtmra.html,

and the wavelet is imported from pywt:
http://www.pybytes.com/pywavelets/ref/wavelets.html

##Example:
```python
from modwt import modwt, modwtmra
import pandas as pd


gdpdata = pd.DataFrame.from_csv('GDPcomponents.csv')
wt = modwt(gdpdata['govtexp'], 'db2', 5)
wtmra = modwtmra(wt, 'db2')
```
