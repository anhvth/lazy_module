LazyModule
================

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

## Install

``` sh
pip install --upgrade pip && pip install lazy_module
#or
pip install git+https://github.com/anhvth/lazy_module
```

## How to use

``` python
import time
```

``` python
start = time.time()
import pandas as pd
print('Import time:', time.time()-start)
```

    Import time: 0.30898594856262207

## Lazy import

``` python
from lazy_module.core import *
start = time.time()
pd = LazyModule('pandas')
print('Import time:', time.time()-start)
# Ipython tabcomplition should work normally
```

    Import time: 5.507469177246094e-05

## Issue

-   Class import is not suported yet, assertion error will occor at
    runtime when the object is being called
