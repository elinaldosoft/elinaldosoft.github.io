---
layout: post
title:  "Parsing strings into datetime"
date:   2022-02-15 11:01:00 -0300
categories: python
comments: true
---

### In this example I will show how to parsing strings into datetime

The main method is `datetime.strptime(date_string, format)`

### The formats
The format list supported by python [strftime.org](https://strftime.org/){:target="_blank"}.
- https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes

### Tip to memorize
- *str*-*p*-*time*
    - str = string
    - p = parser
    - time = datetime

```
from datetime import datetime

string = '20/09/2021 14:36:31'

dt = datetime.strptime(string, "%d/%m/%Y %H:%M:%S")

datetime.datetime(2021, 9, 20, 14, 36, 31)

type(dt)
datetime.datetime
```

### Full reference
- [https://docs.python.org/3/library/datetime.html#datetime.datetime.strptime](https://docs.python.org/3/library/datetime.html#datetime.datetime.strptime){:target="_blank"}

### Useful properties
```
datetime.year
datetime.day
datetime.month
datetime.hour
datetime.minute
datetime.second
datetime.microsecond
```