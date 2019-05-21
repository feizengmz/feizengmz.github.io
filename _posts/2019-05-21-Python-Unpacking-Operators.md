---
layout:     post
title:      Python Unpacking Operators
subtitle:   * and **
date:       2019-05-21
author:     Fei
header-img: img/post-bg-universe.jpg
catalog: true
tags:
    - Python
---



I believe most have already seen below 2 operators before.

## \*, \*\*

Yes they can do mathematical operations, like:
```Python
>>> 2*3
6
>>> 2**3
8
```
They are also used to pass in an arbitrary number of arguments to a function.
```
some_func(fargs,*args,**kwargs)
```
The trick we are going to learn today is to use them as **Unpacking Operators**.

```Python
>>> args = [3, 6]
>>> list(range(*args))            # call with arguments unpacked from a list
[3, 4, 5]
```
In above example, a list *args* is **unpacked** into 2 arguments and pass to *range*
