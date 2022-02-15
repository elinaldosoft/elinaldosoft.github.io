---
layout: post
title:  "Parse string datetime to object datetime"
date:   2022-02-15 11:01:00 -0300
categories: python
comments: true
---

### Parse string datetime to object datetime

```
from datetime import datetime

string = '20/09/2021 14:36:31'

dt = datetime.strptime(string, "%d/%m/%Y %H:%M:%S")

datetime.datetime(2021, 9, 20, 14, 36, 31)

type(dt)
datetime.datetime

dt.year
dt.day
dt.month
dt.hour
dt.minute
dt.second
```

