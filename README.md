Bitebi9 Python Library
===============

Python Library for Bitebi9's API


Requirements
============
* Tested in Python 2.7
* requests lib. (http://docs.python-requests.org/en/latest/)

Examples
========
Print Last Hours Worth of OHLC
```python
from Bitebi9 import Bitebi9
from pprint import pprint
import time

c = Bitebi9("", "")
ohlc = c.market_ohlc(132, start=0, stop=time.time(), interval="minute", limit=60)
pprint(ohlc)
```


List Currencies
```python
from Bitebi9 import Bitebi9
from pprint import pprint

c = Bitebi9("", "")
currencies = c.currencies()
pprint(currencies)
```


